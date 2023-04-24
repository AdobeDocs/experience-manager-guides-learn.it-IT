---
title: Configurare la nuova pubblicazione basata su microservizi per le guide AEM as a Cloud Service
description: Scopri come configurare la nuova pubblicazione basata su microservizi per le guide AEM.
exl-id: 92e3091d-6337-4dc6-9609-12b1503684cd
source-git-commit: 95c89acd02b798d42c817b52f6f8e0710a0abb76
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 0%

---

# Configurare la nuova pubblicazione basata su microservizi per le guide AEM as a Cloud Service

Il nuovo microservizio di pubblicazione consente agli utenti di eseguire carichi di lavoro di pubblicazione di grandi dimensioni contemporaneamente su AEM Guide as a Cloud Service e di sfruttare la piattaforma Adobe I/O Runtime senza server leader del settore.

Per ogni richiesta di pubblicazione AEM Guide as a Cloud Service esegue un contenitore separato che viene ridimensionato in orizzontale in base alle richieste dell’utente. In questo modo gli utenti possono eseguire più richieste di pubblicazione e ottenere prestazioni migliori rispetto ai server di AEM on-premise di grandi dimensioni.

>[!NOTE]
>
> Attualmente la pubblicazione basata su microservizi in AEM Guide supporta solo l’output di PDF tramite la pubblicazione di PDF nativi o tramite DITA-OT. Nelle prossime versioni verrà aggiunto il supporto per la pubblicazione basata su microservizi per più tipi di output.

Poiché il nuovo servizio di pubblicazione cloud è protetto dall’autenticazione basata su JWT di Adobe IMS, i clienti devono seguire i passaggi seguenti per integrare i propri ambienti con i flussi di lavoro di autenticazione basati su token sicuri di Adobe e iniziare a utilizzare la nuova soluzione di pubblicazione scalabile basata su cloud.


## Creare configurazioni IMS nella console Adobe Developer

**Ruolo necessario per creare le confuzioni**: Amministratore di sistema

Per creare configurazioni IMS nella console Adobe Developer, effettua le seguenti operazioni:

1. Apri Console per sviluppatori: `https://developer.adobe.com/console`.

1. Passa a **Progetti** scheda dall&#39;alto.

   <img src="assets/projects-tab.png" alt="scheda progetti" width="500">

1. Per creare un nuovo progetto vuoto, seleziona **Progetto vuoto** dal **Crea nuovo progetto** a discesa.

   <img src="assets/create-new-project.png" alt="crea nuovo progetto" width="500">

1. Seleziona **API** dal **Aggiungi a progetto** menu a discesa per aggiungere l&#39;API di gestione IO al progetto.

   <img src="assets/add-project.png" alt="aggiungi progetto" width="300">

   <img src="assets/io-management-api.png" alt="gestione dell'io" width="500">

1. Crea una nuova coppia di chiavi pubblica/privata durante l’aggiunta dell’API. Questo scaricherà automaticamente la chiave privata sul tuo sistema.

   <img src="assets/generate-key-pair.png" alt="genera coppia di chiavi" width="500">

1. Salva l’API configurata.

   <img src="assets/save-api.png" alt="salva api" width="600">

1. Torna a **Progetti** e fai clic su **Panoramica del progetto** a sinistra.

   <img src="assets/project-overview.png" alt="panoramica del progetto" width="500">

1. Fai clic su **Scarica** pulsante nella parte superiore per scaricare il servizio JSON.

   <img src="assets/download-json.png" alt="scaricare json" width="500">

Ora hai configurato i dettagli di autenticazione JWT e hai scaricato anche la chiave privata e i dettagli del servizio JSON. Mantieni questi due file a portata di mano in quanto questi file sono richiesti nella sezione successiva.

### Aggiungere la configurazione IMS all’ambiente

Per aggiungere la configurazione IMS all’ambiente, effettua le seguenti operazioni:

1. Apri experience manager, quindi seleziona il programma che contiene l&#39;ambiente da configurare.
1. Passa a **Ambienti** scheda .
1. Fai clic sul nome dell’ambiente da configurare. Consente di passare alla pagina Informazioni ambiente .
1. Passa a **Configurazione** scheda .
1. Carica la chiave privata e il progetto JSON come mostrato nella schermata sottostante. Assicurati di usare gli stessi nomi e configurazioni come evidenziato di seguito.

   <img src="assets/ims-config-environment.png" alt="configurazioni ims" width="500">

>[!NOTE]
>
> Devi aprire, copiare e incollare il contenuto del file JSON della chiave privata e dei dettagli del servizio nella colonna del valore del pannello Configurazione , come mostrato nella schermata precedente.

Dopo aver aggiunto la configurazione IMS all’ambiente, esegui le seguenti operazioni per collegare queste proprietà con AEM Guide utilizzando OSGi:

1. Nel codice del progetto Git di cloud manager, aggiungi i due file seguenti (per il contenuto del file, consulta [Appendice](#appendix)).

   * `com.adobe.aem.guides.eventing.ImsConfiguratorService.cfg.json`
   * `com.adobe.fmdita.publishworkflow.PublishWorkflowConfigurationService.xml`
1. Assicurati che i file appena aggiunti siano coperti dal tuo `filter.xml`.
1. Conferma e invia le modifiche Git.
1. Esegui la pipeline per applicare le modifiche all’ambiente.

Al termine della procedura, dovresti essere in grado di utilizzare la nuova pubblicazione cloud basata su microservizi.

## Appendice {#appendix}

**File**:
`com.adobe.aem.guides.eventing.ImsConfiguratorService.cfg.json`

**Contenuto**:

```
{
  "service.account.details": "$[secret:SERVICE_ACCOUNT_DETAILS]",
  "private.key": "$[secret:PRIVATE_KEY]"
}
```

**File**: `com.adobe.fmdita.publishworkflow.PublishWorkflowConfigurationService.xml`

**Contenuto**:
* `dxml.use.publish.microservice`: Passa per abilitare la pubblicazione PDF basata su microservizi utilizzando DITA-OT
* `dxml.use.publish.microservice.native.pdf`: Passa a per abilitare la pubblicazione nativa PDF basata su microservizi

```
<?xml version="1.0" encoding="UTF-8"?>
<jcr:root xmlns:jcr="http://www.jcp.org/jcr/1.0" xmlns:sling="http://sling.apache.org/jcr/sling/1.0"
          jcr:primaryType="sling:OsgiConfig"
          dxml.publish.microservice.url="https://adobeioruntime.net/api/v1/web/543112-guidespublisher/default/publishercaller.json"
          dxml.use.publish.microservice="{Boolean}true"
          dxml.use.publish.microservice.native.pdf="{Boolean}true"
/>
```
