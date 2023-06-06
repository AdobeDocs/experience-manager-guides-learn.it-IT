---
title: Migrazione di contenuti da non-UUID a UUID
description: Scopri come migrare contenuti non UUID a UUID
exl-id: 093b380e-9a8b-4e60-aeaa-3458e8c257f2
source-git-commit: 21edbb2f8a49213ea95fac8a957056711219e7e4
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Migrazione di contenuti da non-UUID a UUID {#id226TI0U20XA}

>[!IMPORTANT]
>
> Puoi migrare il contenuto non UUID al server UUID. Per eseguire la migrazione al server UUID è necessario che sia installato un server non UUID con guide AEM versione 4.0.

Per migrare il contenuto non UUID, effettua le seguenti operazioni:

>[!NOTE]
>
> Ogni passaggio è fondamentale e la mancanza di uno dei passaggi può causare errori o danneggiamento dei dati del server. Assicurati di completare tutti i passaggi.

1. Assicurati che **Abilita moduli di avvio dei flussi di lavoro di post-elaborazione** in *com.adobe.fmdita.config.ConfigManager* e **Abilita postelaborazione versione** in *com.adobe.fmdita.postprocess.version.PostProcessVersionObservation* sono attivati.

   ```http
   http://<server name>:<port>/system/console/configMgr/com.adobe.fmdita.config.ConfigManager
   ```

1. Installa la versione UUID della versione principale successiva rispetto alla versione non UUID. Ad esempio, se utilizzi la build 4.0 non UUID, devi installare UUID versione 4.1.

1. Nella scheda Avvio, disabilita i seguenti flussi di lavoro e qualsiasi altro flusso di lavoro che viene eseguito su /content/dam utilizzando i moduli di avvio in `http://localhost:4502/libs/cq/workflow/content/console.html`:

   - **Aggiorna risorsa DAM** workflow
   - **Writeback di metadati DAM** workflow

1. Disattiva **Abilita moduli di avvio dei flussi di lavoro di post-elaborazione** in *com.adobe.fmdita.config.ConfigManager* e disattiva **Abilita postelaborazione versione** in *com.adobe.fmdita.postprocess.version.PostProcessVersionObservation*.

   ```http
   http://<server name>:<port>/system/console/configMgr/com.adobe.fmdita.config.ConfigManager
   ```

1. Aggiungi un logger separato per `com.adobe.fmdita.uuid.upgrade.UuidUpgrade.`

   La risposta del browser è disponibile anche in /content/uuid-upgrade/logs.

1. Esegui la query specificata su una cartella con dati più piccoli con `doReviews=false` prima di eseguirlo su / content/dam: `http://localhost:4502/bin/dxml/uuid_upgrade?root=/content/dam/test&doReviews=false`

   >[!TIP]
   >
   >  È possibile verificare se tutti i file della cartella sono stati aggiornati correttamente e se tutte le funzionalità funzionano solo per tale cartella.

**Parametri per la query:**

    - &quot;root&quot;: cartella principale in cui deve essere eseguito l’aggiornamento \(Utilizza /content/dam per tutto l’archivio.\)
    - &quot;doReviews&quot;: true/false \(Se le recensioni devono essere aggiornate o no. Il valore predefinito è false.\)
    - &quot;doBaselines&quot;: true/false \(se le linee di base devono essere aggiornate o meno. Il valore predefinito è true.\)
    - `processLevel`: -1\(failed without restore\), 0\(failed with restore\), 1\(failed with errors\), 2\(successfully upgrade riuscito\) \(Quando si ritenta lo script dopo un errore, verranno elaborati di nuovo solo i file con &quot;fmUpgradeStatus&quot; &lt;= processLevel, altrimenti verranno ignorati. Il valore predefinito è 1.\)
    - &quot;ignoreImageVersions&quot;: true/false \(Ignora l’elaborazione delle versioni delle immagini. Il valore predefinito è false.\)
    
    >[!NOTA]
    >
    > Possiamo eseguire la migrazione dei contenuti a livello di cartella o del contenuto completo/dam oppure sulla stessa cartella \(eseguire nuovamente la migrazione\).

1. Dopo la migrazione del server, abilitare i flussi di lavoro e la post-elaborazione seguenti per continuare a lavorare sul server:

   - **Aggiorna risorsa DAM** workflow
   - **Metadati DAM** workflow

>[!NOTE]
>
> Se alcuni file non vengono elaborati o sono danneggiati prima della migrazione, rimangono danneggiati anche dopo la migrazione.
