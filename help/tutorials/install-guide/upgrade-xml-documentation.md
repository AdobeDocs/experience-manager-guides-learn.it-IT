---
title: Aggiornare le guide di Adobe Experience Manager
description: Scopri come aggiornare le guide di Adobe Experience Manager
source-git-commit: 414ee8ae3b12bb40054ddbe9e1a008ebc6058f89
workflow-type: tm+mt
source-wordcount: '2750'
ht-degree: 1%

---


# Aggiornare le guide di Adobe Experience Manager {#id224MBE0M0XA}

>[!NOTE]
>
> Segui le istruzioni di aggiornamento specifiche per la versione con licenza del tuo prodotto.

È possibile aggiornare la versione corrente delle guide AEM alla versione 4.2.1
- Se utilizzi le versioni 4.1, 4.1.x o 4.2, puoi eseguire direttamente l’aggiornamento alla versione 4.2.1.
- Se utilizzi la versione 4.0, devi effettuare l’aggiornamento alla versione 4.2 prima di passare alla versione 4.2.1.
- Se utilizzi la versione 3.8.5, devi effettuare l’aggiornamento alla versione 4.0 prima di passare alla versione 4.2.
- Se utilizzi una versione precedente alla 3.8.5, consulta la sezione Aggiornamento delle guide AEM nella guida all’installazione specifica per il prodotto.

>[!NOTE]
>
> È necessario installare il service pack per l’AEM prima di aggiornare la versione delle guide AEM.

Per ulteriori informazioni, consulta le procedure seguenti:

- [Aggiornamento da 3.8.5 a versione 4.0](#id2256DK003E1)
- [Aggiornamento alla versione 4.2](#id22A3F500SXA)
- [Aggiornamento alla versione 4.2.1](#upgrade-version-4-2-1)


>[!IMPORTANT]
>
> Prima di iniziare l&#39;aggiornamento, eseguire un backup completo del sistema per evitare la perdita di dati.

## Aggiornamento dalla versione 3.8.5 alla versione 4.0 {#id2256DK003E1}

Se utilizzi le guide AEM versione 3.8.5, puoi effettuare l’aggiornamento alla versione 4.0 delle guide AEM. Con la funzione di aggiornamento, non è necessario disinstallare la versione precedente delle guide AEM.

Prima di eseguire il processo è necessario completare alcune attività. Le seguenti sottosezioni ti guideranno attraverso i prerequisiti, la generazione di rapporti e il processo di migrazione. Inoltre, dopo aver installato le guide AEM versione 4.0, è possibile personalizzare varie configurazioni, in base alle impostazioni del cliente.

>[!NOTE]
>
> Questo processo di aggiornamento è applicabile solo dalla versione 3.8.5 alla versione 4.0. Per il processo di aggiornamento dalla versione 3.4 o successiva alla versione 3.8.5, fare riferimento al *Aggiornamento delle guide AEM* nella guida all&#39;installazione specifica del prodotto disponibile nella [Pagina Archiviazione della Guida](https://helpx.adobe.com/xml-documentation-for-experience-manager/archive.html).

****Prerequisiti****

Prima di avviare il processo di aggiornamento delle Guide AEM, accertati di disporre di:

1. Importazione dei commenti di revisione negli argomenti aperti per la revisione.
1. Chiuse tutte le recensioni attive.
1. Ha chiuso tutte le attività di traduzione.
1. Disinstalla eventuali hotfix di AEM Guides installati nella versione precedente \(principale o patch\) delle guide AEM.

**Prima di installare la versione 4.0**

Prima di installare la versione 4.0, effettuare le seguenti operazioni:

1. A questo punto verificare che la versione delle guide AEM sia la 3.8.5.
1. Scarica il pacchetto dello script di aggiornamento. Per eseguire questa operazione, cercare &quot;Pacchetto di aggiornamento alla soluzione XML Documentation 4.0&quot; in [Portale di distribuzione software Adobe](https://experience.adobe.com/#/downloads/content/software-distribution/it/aem.html) che scaricherà un file zip.
1. Carica questo pacchetto in AEM tramite Gestione pacchetti e installa il pacchetto.
1. Una volta installato il pacchetto di aggiornamento, esegui i seguenti script specificati nello stesso ordine e segui le istruzioni fornite:

**Verifica l’API di compatibilità per l’aggiornamento**

Questa API è progettata per valutare lo stato corrente del sistema e segnalare se l’aggiornamento è possibile o meno. Per eseguire questo script, attiva il seguente endpoint specificato:

| Punto finale | /bin/dxml/upgrade/3xto4x/report |
| --- | --- |
| Tipo di richiesta | **GET** Puoi utilizzare un browser web per accedere all’istanza AEM come amministratore. |
| Risposta prevista | - Nel caso in cui tutti i nodi richiesti possano essere spostati, riceverai un controllo superato. <br>- Se nella posizione di destinazione è presente un nodo, viene visualizzato un errore rilevante. Pulisci l’archivio \(elimina nodo /var/dxml\) e reinstalla il pacchetto di aggiornamento, quindi attiva di nuovo questo endpoint. <br>**Nota:** Questo non è un errore comune in quanto la posizione di destinazione non è stata utilizzata in precedenza dalle guide AEM 3.x. <br> - Se questo script non riesce, non procedere e segnalalo al team di successo del cliente. |

**API di migrazione dati di sistema**

Questa API è progettata per migrare i dati di sistema come indicato nella **Mappatura della migrazione** sezione.

1. Non eseguire questo script se l’API Verifica compatibilità aggiornamento non riesce \(non procedere\).
1. Una volta che l’API di verifica compatibilità dell’aggiornamento restituisce il risultato positivo, puoi eseguire lo script di aggiornamento.

| Punto finale | /bin/dxml/upgrade/3xto4x |
| --- | --- |
| Tipo di richiesta | **POST** Questo script è una richiesta POST, quindi deve essere eseguito tramite agenti come Postman. |
| Risposta prevista | - Una volta completata la migrazione, è possibile installare la soluzione XML Documentation versione 4.0.<br>- In caso di errori, ripristina l’ultimo punto di controllo e condividi i registri degli errori con l’output API al team di successo del cliente. |

**Mappatura della migrazione**: l’API di cui sopra migra tutti i dati nella posizione di origine alla posizione di destinazione.

| Sorgente | Destinazione |
|------|------|
| /content/fmdita | /var/dxml |
| /content/dxml | /var/dxml |
| /etc/fmdita | /libs/fmdita |

## Installa versione 4.0 {#id23598G006XA}

1. Installa la versione 4.0 solo se i passaggi di aggiornamento hanno avuto esito positivo.
1. Scarica il pacchetto di versione 4.0 da [Portale di distribuzione software Adobe](https://experience.adobe.com/#/downloads/content/software-distribution/it/aem.html):

   - Se si utilizza una versione UUID del software, cercare &quot;4.0 UUID Release for XML Documentation solution for AEM 6.5&quot;.
   - Se si utilizza una versione del software non UUID, cercare &quot;4.0 Non-UUID Release for XML Documentation solution for AEM 6.5&quot;.
Carica il pacchetto nell&#39;istanza del server AEM esistente utilizzando Gestione pacchetti CRX e installalo.

   >[!NOTE]
   >
   > Attendere l&#39;avvio di tutti i componenti di sistema.

1. Cancella la cache del browser dopo l’installazione del pacchetto.
1. Se un dispatcher è configurato nell’istanza di AEM Author, effettua le seguenti operazioni:
   - Assicurati che nelle regole del dispatcher vengano gestiti i seguenti elementi:
   - Il pattern URL /home/users/\*/preferences è inserito nella whitelist.
   - Il modello URL /libs/cq/security/userinfo.json non è memorizzato nella cache.
1. Cancella cache del dispatcher \(per cancellare qualsiasi `clientlibs` memorizzato in cache\).

## Aggiornamento alla versione 4.2 {#id22A3F500SXA}

L’aggiornamento alla versione 4.2 dipende dalla versione corrente delle guide AEM.

Se utilizzi le versioni 4.0, 4.1 o 4.1.x, puoi eseguire direttamente l’aggiornamento alla versione 4.2.

****Prerequisiti****

Prima di avviare il processo di aggiornamento delle Guide AEM 4.2, assicurati di disporre di:

1. Aggiornato alle guide AEM versione 4.0, 4.1 o 4.1.x.
1. Ha chiuso tutte le attività di traduzione.
1. Il livello di registro è stato modificato in **INFO** per `com.adobe.fmdita.translationservices.TranslationMapUpgradeScript` e aggiungi questi registri in un nuovo file di registro, ad esempio, `logs/translation_upgrade.log.`

>[!NOTE]
>
> Chiudere tutte le recensioni attive. Se le attività di revisione non vengono chiuse durante l’aggiornamento alla versione 4.2, le precedenti attività di revisione in corso continuano a coinvolgere gli utenti nelle pagine di revisione precedenti e le attività di revisione create dopo l’aggiornamento visualizzano gli ultimi aggiornamenti della funzionalità.

## Installare la versione 4.2 {#id2245IK0E0EV}

1. Scarica il pacchetto di versione 4.2 da [Portale di distribuzione software Adobe](https://experience.adobe.com/#/downloads/content/software-distribution/it/aem.html).
1. Installa la versione 4.2 del pacchetto.
1. Dopo aver completato l’installazione del pacchetto, attendi i seguenti messaggi\(s\) nei registri:

   `Completed the post deployment setup script`

   Il messaggio sopra riportato indica che tutti i passaggi dell&#39;installazione sono stati completati.

   Se riscontri uno dei seguenti prefissi ERROR, segnalali al team di successo del cliente:

   - Errore nello script di installazione post-distribuzione
   - Eccezione durante il porting del MAP di traduzione
   - Impossibile trasferire la mappa di traduzione dalla versione 1 alla versione 2 per la proprietà
1. Aggiornamento del plug-in del connettore ossigeno rilasciato con la versione 4.2 (se necessario).
1. Cancella la cache del browser dopo l’installazione del pacchetto.
1. Continua ad aggiornare le personalizzazioni come descritto nella sezione successiva.

## Dopo aver installato la versione 4.2 {#id2326F02004K}

>[!IMPORTANT]
>
> Il modello Hi-tech non viene visualizzato sul server aggiornato. Per includere il modello hi-tech sul server è possibile copiarlo: Fonte: /libs/fmdita/pdf/Hi-Tech Destinazione: /content/dam/dita-templates/pdf

Dopo aver installato le guide AEM, è possibile unire le varie configurazioni applicabili dalla versione appena installata alla configurazione.

>[!NOTE]
>
> Il modello dam-update-asset può essere personalizzato. Pertanto, se sono state apportate personalizzazioni, è necessario sincronizzare le personalizzazioni e le guide AEM nella copia di lavoro del modello.

1. **Flusso di lavoro Aggiorna risorsa DAM \(Modifiche post-elaborazione\):**

1. Apri URL:

   ```http
   http://localhost:4502/libs/cq/workflow/admin/console/content/models.html
   ```

1. Seleziona **Flusso di lavoro Aggiorna risorsa DAM**.
1. Fai clic su **Modifica**.
1. Se il **Iniziatore post-elaborazione DXML** è presente, assicurati che le personalizzazioni siano sincronizzate.
1. Se il **Iniziatore post-elaborazione DXML** il componente è assente, esegui i seguenti passaggi per inserirlo:

1. Clic **Inserisci componente** \(Responsabile della guida AEM per la post-elaborazione come fase finale del processo\).
1. Configurare **Passaggio del processo** con i dettagli seguenti:

   **Scheda Comune**

   **Titolo:** Iniziatore post-elaborazione DXML

   **Descrizione**: passaggio dell’iniziatore di post-elaborazione DXML che attiverà un processo sling per la post-elaborazione DXML della risorsa modificata/creata

   **Scheda Processo**

   - Seleziona **Iniziatore post-elaborazione DXML** dal **Processo** elenco a discesa

   - Seleziona **Avanzamento gestore**

   - Seleziona **Fine**

1. Clic **Sincronizza** in alto a destra dopo aver completato le modifiche. Riceverai una notifica di esito positivo.

   >[!NOTE]
   >
   > Aggiorna e verifica che le modifiche personalizzate e il passaggio di post-elaborazione delle guide AEM siano presenti nel modello di flusso di lavoro finale.

1. Una volta **Flusso di lavoro Aggiorna risorsa DAM**&#x200B;è convalidato, controlla le configurazioni di avvio corrispondenti. Per farlo, vai all’interfaccia del flusso di lavoro AEM e apri i moduli di avvio.

   ```http
   http://localhost:4502/libs/cq/workflow/content/console.html
   ```

   Trova e apporta le modifiche \(se necessario\) ai seguenti due moduli di avvio \(che dovrebbe essere attivo\) corrispondenti a **Flusso di lavoro Aggiorna risorsa DAM**:

1. Modulo di avvio per &quot;*Nodo creato*&quot; per **Flusso di lavoro Aggiorna risorsa DAM**- per condizione `"jcr:content/jcr:mimeType!=video"`, il valore &quot;Globbing&quot; deve essere:

   ```json
   /content/dam(/((?!/subassets|/translation_output).)*/)renditions/original
   ```

   - &#39;excludeList&#39; deve avere `"event-user-data:changedByWorkflowProcess"`.
   - Modulo di avvio per &quot;*Nodo modificato*&quot; per **Flusso di lavoro Aggiorna risorsa DAM -** per la condizione &quot;`jcr:content/jcr:mimeType!=video`&quot;,
   - 
      - il valore &#39;Globbing&#39; deve essere:

   ```json
   `"/content/dam(/((?!/subassets|/translation_output).)*/)renditions/original"`
   ```

   - &#39;excludeList&#39; deve avere `"event-user-data:changedByWorkflowProcess"`.
1. Al termine dell’aggiornamento, accertati che le personalizzazioni/sovrapposizioni siano convalidate e aggiornate in modo che corrispondano al nuovo codice dell’applicazione. Di seguito sono riportati alcuni esempi:
   - Tutti i componenti sovrapposti da/libs/fmditaor/libssdevono essere confrontati con il nuovo codice del prodotto e gli aggiornamenti devono essere eseguiti in file sovrapposti in/apps.
   - Tutte le categorie clientlib utilizzate dal prodotto, devono essere riviste per eventuali modifiche. Eventuali configurazioni sostituite \(esempi di seguito\) devono essere confrontate con quelle più recenti in modo da ottenere le funzioni più recenti:
   - elementmapping.xml
   - ui\_config.json\(potrebbe essere stato impostato in profili cartella\)
   - modificato `com.adobe.fmdita.config.ConfigManager`
   - Verifica se uno qualsiasi dei codici personalizzati utilizzava percorsi precedenti \(come indicato nella [Mappatura della migrazione](#id2244LE040XA) section\) - devono essere aggiornati ai nuovi percorsi in modo che anche le personalizzazioni funzionino come previsto.
1. Scopri le nuove configurazioni introdotte nella versione corrente \(seleziona [Note sulla versione](../release-info/release-notes-4.2.md)\) e verificare se sono interessate eventuali funzionalità, quindi adottare le misure appropriate. Un esempio potrebbe essere quello di utilizzare &quot;Gestione migliorata dei file e delle versioni&quot; introdotta nella versione 4.0, per la quale è necessario abilitare una configurazione.

## Passaggi per indicizzare il contenuto esistente per utilizzare la nuova funzione Trova e sostituisci:

Effettua le seguenti operazioni per indicizzare il contenuto esistente e utilizzare il nuovo testo Trova e sostituisci a livello di mappa:

- Esegui una richiesta POST al server \(con autenticazione corretta\) - `http://<server:port\>/bin/guides/map-find/indexing`. \(Facoltativo: È possibile passare percorsi specifici delle mappe per indicizzarle. Per impostazione predefinita, tutte le mappe saranno indicizzate \|\| Ad esempio: `https://<Server:port\>/bin/guides/map-find/indexing?paths=<map\_path\_in\_repository\>`\)

- L’API restituirà un jobId. Per verificare lo stato del processo, puoi inviare una richiesta di GET con ID processo allo stesso endpoint: `http://<server:port\>/bin/guides/map-find/indexing?jobId=\{jobId\}`\(Ad esempio: `http://localhost:8080/bin/guides/map-find/indexing?jobId=2022/9/15/7/27/7dfa1271-981e-4617-b5a4-c18379f11c42`\)

- Una volta completato il processo, la richiesta di GET di cui sopra risponderà con successo e menzionerà se eventuali mappe non sono riuscite. Le mappe indicizzate correttamente possono essere confermate dai registri del server.

## Aggiornamento alla versione 4.2.1 {#upgrade-version-4-2-1}

L’aggiornamento alla versione 4.2.1 dipende dalla versione corrente delle guide AEM.

Se utilizzi le versioni 4.1 o 4.1.x o 4.2, puoi eseguire direttamente l’aggiornamento alla versione 4.2.1.

>[!NOTE]
>
>La post-elaborazione e l’indicizzazione potrebbero richiedere alcune ore. Si consiglia di avviare il processo di aggiornamento durante le ore non di punta.

****Prerequisiti****

Prima di avviare il processo di aggiornamento delle Guide AEM 4.2.1, assicurati di disporre di:

1. Aggiornato alle guide AEM versione 4.1, 4.1.x o 4.2.
1. Ha chiuso tutte le attività di traduzione.
1. Il livello di registro è stato modificato in **INFO** per `com.adobe.fmdita.translationservices.TranslationMapUpgradeScript` e aggiungi questi registri in un nuovo file di registro, ad esempio, `logs/translation_upgrade.log.`

>[!NOTE]
>
> Chiudere tutte le recensioni attive. Se le attività di revisione non vengono chiuse durante l’aggiornamento alla versione 4.2, le precedenti attività di revisione in corso continuano a coinvolgere gli utenti nelle pagine di revisione precedenti e le attività di revisione create dopo l’aggiornamento visualizzano gli ultimi aggiornamenti della funzionalità.

## Installare la versione 4.2.1

1. Scarica il pacchetto di versione 4.2.1 da [Portale di distribuzione software Adobe](https://experience.adobe.com/#/downloads/content/software-distribution/it/aem.html).
1. Installa la versione 4.2.1 del pacchetto.
1. Puoi scegliere di premere il trigger per avviare il processo di aggiornamento della mappa di traduzione. Per ulteriori informazioni, consulta [Abilitare l’attivazione dello script tramite un servlet](#enable-trigger-serverlet).


1. Dopo aver completato l’installazione del pacchetto, attendi i seguenti messaggi\(s\) nei registri:

   `Completed the post deployment setup script`

   Il messaggio sopra riportato indica che tutti i passaggi dell&#39;installazione sono stati completati.

   Se riscontri uno dei seguenti prefissi ERROR, segnalali al team di successo del cliente:

   - Errore nello script di installazione post-distribuzione
   - Eccezione durante il porting del MAP di traduzione
   - Impossibile trasferire la mappa di traduzione dalla versione 1 alla versione 2 per la proprietà
1. Aggiornamento del plug-in del connettore ossigeno rilasciato con la versione 4.2 (se necessario).
1. Cancella la cache del browser dopo l’installazione del pacchetto.
1. Continua ad aggiornare le personalizzazioni come descritto nella sezione successiva.

### Abilitare l’attivazione dello script tramite un servlet{#enable-trigger-serverlet}

POST:

```
http://localhost:4503/bin/guides/script/start?jobType=translation-map-upgrade
```

Risposta:

```
{
"msg": "Job is successfully submitted and lock node is created for future reference",
"lockNodePath": "/var/dxml/executor-locks/translation-map-upgrade/1683190032886",
"status": "SCHEDULED"
}
```

Nella risposta precedente JSON, la chiave `lockNodePath` contiene il percorso del nodo creato nell’archivio che punta al processo inviato. Verrà eliminato automaticamente una volta completato il processo; fino ad allora, puoi fare riferimento a questo nodo per lo stato corrente del processo.

Registro di esempio: di seguito è riportato un esempio di registri che verranno visualizzati nel file di registro dopo l’attivazione dello script.

```
04.05.2023 14:17:12.876 *INFO* [[0:0:0:0:0:0:0:1] [1683190032736] POST /bin/guides/script/start HTTP/1.1] com.adobe.dxml.common.executor.RunnableSynchronizedOTS Acquiring lock for job : translation-map-upgrade
04.05.2023 14:17:12.897 *INFO* [pool-59-thread-1] com.adobe.fmdita.xmltranslation.ots.TranslationMapUpgradeOTS Starting the thread to upgrade translation map from V1 to V2
04.05.2023 14:17:12.899 *INFO* [pool-59-thread-1] com.adobe.dxml.common.executor.RunnableSynchronizedOTS Initiating lock for node : /var/dxml/executor-locks/translation-map-upgrade/1683190032886
04.05.2023 14:17:12.901 *INFO* [pool-59-thread-1] com.adobe.fmdita.translationservices.TranslationMapUpgradeScript Starting porting of translation map from V1 to V2
04.05.2023 14:17:12.904 *INFO* [pool-59-thread-1] com.adobe.fmdita.translationservices.TranslationMapUpgradeScript Memory increase is of : 764 kB
04.05.2023 14:17:12.906 *INFO* [pool-59-thread-1] com.adobe.fmdita.translationservices.TranslationMapUpgradeScript Completed porting of translation map from V1 to V2
04.05.2023 14:17:12.907 *INFO* [pool-59-thread-1] com.adobe.dxml.common.executor.RunnableSynchronizedOTS Releasing lock for node : /var/dxml/executor-locks/translation-map-upgrade/1683190032886
04.05.2023 14:17:12.909 *INFO* [pool-59-thread-1] com.adobe.fmdita.xmltranslation.ots.TranslationMapUpgradeOTS Completed the thread to upgrade translation map from V1 to V2
```

Cerca `com.adobe.fmdita.translationservices.TranslationMapUpgradeScript Completed porting of translation map from V1 to V2` e `com.adobe.fmdita.xmltranslation.ots.TranslationMapUpgradeOTS Completed the thread to upgrade translation map from V1 to V2` prima di procedere ai passaggi successivi.



## Dopo aver installato la versione 4.2.1

>[!IMPORTANT]
>
> Il modello Hi-tech non viene visualizzato sul server aggiornato. Per includere il modello hi-tech sul server è possibile copiarlo: Fonte: /libs/fmdita/pdf/Hi-Tech Destinazione: /content/dam/dita-templates/pdf

Dopo aver installato le guide AEM, è possibile unire le varie configurazioni applicabili dalla versione appena installata alla configurazione.

>[!NOTE]
>
> Il modello dam-update-asset può essere personalizzato. Pertanto, se sono state apportate personalizzazioni, è necessario sincronizzare le personalizzazioni e le guide AEM nella copia di lavoro del modello.

1. **Flusso di lavoro Aggiorna risorsa DAM \(Modifiche post-elaborazione\):**

1. Apri URL:

   ```http
   http://localhost:4502/libs/cq/workflow/admin/console/content/models.html
   ```

1. Seleziona **Flusso di lavoro Aggiorna risorsa DAM**.
1. Fai clic su **Modifica**.
1. Se il **Iniziatore post-elaborazione DXML** è presente, assicurati che le personalizzazioni siano sincronizzate.
1. Se il **Iniziatore post-elaborazione DXML** il componente è assente, esegui i seguenti passaggi per inserirlo:

1. Clic **Inserisci componente** \(Responsabile della guida AEM per la post-elaborazione come fase finale del processo\).
1. Configurare **Passaggio del processo** con i dettagli seguenti:

   **Scheda Comune**

   **Titolo:** Iniziatore post-elaborazione DXML

   **Descrizione**: passaggio dell’iniziatore di post-elaborazione DXML che attiverà un processo sling per la post-elaborazione DXML della risorsa modificata/creata

   **Scheda Processo**

   - Seleziona **Iniziatore post-elaborazione DXML** dal **Processo** elenco a discesa

   - Seleziona **Avanzamento gestore**

   - Seleziona **Fine**

1. Clic **Sincronizza** in alto a destra dopo aver completato le modifiche. Riceverai una notifica di esito positivo.

   >[!NOTE]
   >
   > Aggiorna e verifica che le modifiche personalizzate e il passaggio di post-elaborazione delle guide AEM siano presenti nel modello di flusso di lavoro finale.

1. Una volta **Flusso di lavoro Aggiorna risorsa DAM**&#x200B;è convalidato, controlla le configurazioni di avvio corrispondenti. Per farlo, vai all’interfaccia del flusso di lavoro AEM e apri i moduli di avvio.

   ```http
   http://localhost:4502/libs/cq/workflow/content/console.html
   ```

   Trova e apporta le modifiche \(se necessario\) ai seguenti due moduli di avvio \(che dovrebbe essere attivo\) corrispondenti a **Flusso di lavoro Aggiorna risorsa DAM**:

1. Modulo di avvio per &quot;*Nodo creato*&quot; per **Flusso di lavoro Aggiorna risorsa DAM**- per condizione `"jcr:content/jcr:mimeType!=video"`, il valore &quot;Globbing&quot; deve essere:

   ```json
   /content/dam(/((?!/subassets|/translation_output).)*/)renditions/original
   ```

   - &#39;excludeList&#39; deve avere `"event-user-data:changedByWorkflowProcess"`.
   - Modulo di avvio per &quot;*Nodo modificato*&quot; per **Flusso di lavoro Aggiorna risorsa DAM -** per la condizione &quot;`jcr:content/jcr:mimeType!=video`&quot;, il valore &#39;Globbing&#39; deve essere:

   ```json
   `"/content/dam(/((?!/subassets|/translation_output).)*/)renditions/original"`
   ```

   - `excludeList` dovrebbe avere `"event-user-data:changedByWorkflowProcess"`.


1. Al termine dell’aggiornamento, accertati che le personalizzazioni/sovrapposizioni siano convalidate e aggiornate in modo che corrispondano al nuovo codice dell’applicazione. Di seguito sono riportati alcuni esempi:
   - Tutti i componenti sovrapposti da/libs/fmditaor/libssdevono essere confrontati con il nuovo codice del prodotto e gli aggiornamenti devono essere eseguiti in file sovrapposti in/apps.
   - Tutte le categorie clientlib utilizzate dal prodotto, devono essere riviste per eventuali modifiche. Eventuali configurazioni sostituite \(esempi di seguito\) devono essere confrontate con quelle più recenti in modo da ottenere le funzioni più recenti:
   - elementmapping.xml
   - ui\_config.json\(potrebbe essere stato impostato in profili cartella\)
   - modificato `com.adobe.fmdita.config.ConfigManager`
   - Verifica se uno qualsiasi dei codici personalizzati utilizzava percorsi precedenti \(come indicato nella [Mappatura della migrazione](#id2244LE040XA) section\) - devono essere aggiornati ai nuovi percorsi in modo che anche le personalizzazioni funzionino come previsto.
1. Scopri le nuove configurazioni introdotte nella versione corrente \(seleziona [Note sulla versione](../release-info/release-notes-4.2.1.md)\) e verificare se sono interessate eventuali funzionalità, quindi adottare le misure appropriate. Un esempio potrebbe essere quello di utilizzare &quot;Gestione migliorata dei file e delle versioni&quot; introdotta nella versione 4.0, per la quale è necessario abilitare una configurazione.

## Passaggi per indicizzare il contenuto esistente per utilizzare la nuova funzione Trova e sostituisci:

Effettua le seguenti operazioni per indicizzare il contenuto esistente e utilizzare il nuovo testo Trova e sostituisci a livello di mappa:

- Assicurati che `damAssetLucene` indicizzazione completata. Può richiedere alcune ore, a seconda della quantità di dati presenti sul server. Puoi confermare che la reindicizzazione è stata completata verificando che il campo di reindicizzazione sia impostato su false in
   `http://<server:port>/oak:index/damAssetLucene`.  Inoltre, se hai aggiunto delle personalizzazioni in `damAssetLucene`, potrebbe essere necessario riapplicarli.

- Esegui una richiesta POST al server \(con autenticazione corretta\) - `http://<server:port\>/bin/guides/map-find/indexing`. (Facoltativo: Puoi trasmettere percorsi specifici delle mappe per indicizzarle; per impostazione predefinita, tutte le mappe saranno indicizzate \|\| Ad esempio: `https://<Server:port\>/bin/guides/map-find/indexing?paths=<map\_path\_in\_repository\>`)

- È inoltre possibile passare una cartella principale per indicizzare le mappe DITA di una cartella specifica (e delle relative sottocartelle). Ad esempio, `http://<server:port\>/bin/guides/map-find/indexing?root=/content/dam/test`. Si noti che se vengono passati sia il parametro paths che il parametro root, viene considerato solo il parametro paths.

- L’API restituirà un jobId. Per verificare lo stato del processo, puoi inviare una richiesta di GET con ID processo allo stesso endpoint: `http://<server:port\>/bin/guides/map-find/indexing?jobId=\{jobId\}`\(Ad esempio: `http://localhost:8080/bin/guides/map-find/indexing?jobId=2022/9/15/7/27/7dfa1271-981e-4617-b5a4-c18379f11c42`\)


- Una volta completato il processo, la richiesta di GET di cui sopra risponderà con successo e menzionerà se eventuali mappe non sono riuscite. Le mappe indicizzate correttamente possono essere confermate dai registri del server.

**Argomento padre:**[ Scarica e installa](download-install.md)
