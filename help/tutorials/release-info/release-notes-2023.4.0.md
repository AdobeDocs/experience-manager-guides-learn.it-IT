---
title: Note sulla versione | Guide Adobe Experience Manager as a Cloud Service, versione di aprile 2023
description: Versione più recente delle guide di Adobe Experience Manager as a Cloud Service
source-git-commit: 77b118655ad8e37e00b0371497e4a2578ddd276e
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 2%

---

# Rilascio di aprile delle guide di Adobe Experience Manager as a Cloud Service

## Aggiornamento alla versione più recente

Aggiorna le guide correnti di Adobe Experience Manager as a Cloud Service (in seguito denominate *Guide AEM as a Cloud Service*) eseguendo le seguenti operazioni:

1. Controlla il codice Git dei Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
2. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file dei tuoi Cloud Services Codice Git a 2023.4.249.
3. Conferma le modifiche ed esegui la pipeline dei Cloud Services per eseguire l’aggiornamento all’ultima versione di AEM Guide as a Cloud Service.

## Passaggi per indicizzare il contenuto esistente (solo se disponi di una versione precedente al rilascio di settembre delle AEM guide as a Cloud Service)

Esegui i seguenti passaggi per indicizzare il contenuto esistente e utilizzare il nuovo testo trova e sostituisci a livello di mappa:

* Esegui una richiesta POST al server (con autenticazione corretta) - `http://<server:port>/bin/guides/map-find/indexing`.
(Facoltativo: Puoi trasmettere percorsi specifici delle mappe per indicizzarle, per impostazione predefinita tutte le mappe saranno indicizzate || Esempio : `https://<Server:port>/bin/guides/map-find/indexing?paths=<map_path_in_repository>`)

* L’API restituirà un jobId. Per controllare lo stato del processo, puoi inviare una richiesta di GET con ID processo allo stesso punto finale - `http://<server:port>/bin/guides/map-find/indexing?jobId={jobId}`
(Ad esempio: http://&lt;
_localhost:8080_>/bin/guides/map-find/indexing?jobId=2022/9/15/7/27/7dfa1271-981e-4617-b5a4-c18379f11c42_678)

* Una volta completato il processo, la richiesta di GET di cui sopra risponderà con successo e menzionerà se eventuali mappe non sono riuscite. Le mappe indicizzate correttamente possono essere confermate dai log del server.

## Matrice di compatibilità

In questa sezione viene elencata la matrice di compatibilità per le applicazioni software supportate dalla versione di AEM Guide as a Cloud Service di aprile 2023.

### FrameMaker e FrameMaker Publishing Server

| AEM guide as a Cloud Release | FMPS | FrameMaker |
| --- | --- | --- |
| 2023.04.0 | Non compatibile | 2022 o superiore |
|  |  |  |


### Connettore dell&#39;ossigeno

| AEM guide as a Cloud Release | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno | Modifica in Windows Ossigeno | Modifica in Oxygen Mac |
| --- | --- | --- | --- | --- |
| 2023.04.0 | 2.9-uuid-2 | 2.9-uuid-2 | 2.3 | 2.3 |
|  |  |  |  |


## Nuove funzioni e miglioramenti

AEM guide as a Cloud Service fornisce miglioramenti e nuove funzioni nell’ultima versione:

### Supporto avanzato dei metadati nella pubblicazione in PDF

AEM Guide ora fornisce supporto avanzato per i metadati mappati ai metadati nell’output di PDF. Le opzioni relative ai metadati includono informazioni sul documento e sul relativo contenuto, ad esempio il nome dell’autore, il titolo del documento, le parole chiave, le informazioni sul copyright e altri campi di dati.

<img src="assets/pdf-metadata.png" alt=" metadati pdf nativi">

È possibile importare un file XMP e AEM Guide può scegliere le informazioni dal file. È inoltre possibile fornire i nomi e i valori dei metadati utilizzando il menu a discesa . Puoi anche aggiungere metadati personalizzati digitando direttamente nel campo name.


### Pannello Vista struttura avanzato

AEM guide fornisce un pannello Visualizzazione struttura improvvisato in cui viene visualizzata la visualizzazione gerarchica degli elementi utilizzati nel documento.

<img src="assets/select-element-content-outline-view_cs.png" alt=" metadati pdf nativi">

La vista Struttura offre i seguenti miglioramenti:

* Il menu a discesa Opzioni vista viene visualizzato nella parte superiore del pannello Visualizzazione struttura. Se un elemento ha un ID, un attributo e un testo, puoi selezionarli dal menu a discesa per visualizzarli insieme all’elemento. Gli attributi che possono essere visualizzati nel pannello Visualizzazione struttura sono determinati dalle impostazioni Attributi di visualizzazione configurate dall&#39;amministratore all&#39;interno della **Impostazioni editor**.

* Utilizzando la funzione di ricerca, puoi cercare un elemento in base al nome, all’ID, al testo o al valore dell’attributo.


### Pubblicazione basata su microservizi per AEM guide as a Cloud Service

AEM Guide as a Cloud Service offre la funzione di eseguire carichi di lavoro di pubblicazione di grandi dimensioni in contemporanea con la pubblicazione basata su microservizi e di sfruttare la piattaforma Adobe I/O Runtime senza server leader del settore.

Nella versione di aprile è ora possibile eseguire più richieste di pubblicazione contemporaneamente e generare output in massa di PDF in modo molto efficiente utilizzando la pubblicazione nativa di PDF basata su microservizi.
Per ulteriori dettagli, consulta [Configurare la nuova pubblicazione basata su microservizi per le guide AEM as a Cloud Service](../knowledge-base/publishing/configure-microservices.md).


## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

* PDF nativo | La pubblicazione di contenuti con una classe di output con parentesi graffe() determina un blocco della pubblicazione. (11596)
* Il problema si verifica quando si sposta (trascina e rilascia) al posto di una voce dell’elenco esistente con l’opzione Rileva modifiche in. (11570)
* Il problema si verifica quando si sposta (trascina e rilascia) una nuova voce di elenco con la funzione di tracciamento delle modifiche. (11569)
* Le voci di elenco rientro o rientro non funzionano come previsto con la funzione di tracciamento delle modifiche. (11568)
* L’aggiunta di contenuto su una riga con l’opzione Track Changes (Modifica rilevamento) attivata e la disattivazione di Track Changes (Rileva modifiche) non la disattiva in realtà. (11567)
* Difficoltà nel trascinamento e nel rilascio di un elemento dell’elenco, il testo viene spostato al posto dell’elemento dell’elenco. (11566)
* La revisione completata non si apre in modalità di sola lettura. (11387)
* Il problema si verifica nella ricerca AEM sito (non funziona oltre i nodi di livello 2-3). (11352)
* Durante l’authoring nell’elemento visualizzato in verde (Rileva modifiche), il nuovo contenuto viene visualizzato come cambiamento di tracciamento anche se la modifica di traccia è disabilitata. (7021)

### Problema noto con la soluzione alternativa

Adobe ha identificato il seguente problema noto per la versione di AEM Guide as a Cloud Service nell’aprile 2023.

* PDF nativo | I vecchi metadati non vengono compilati finché il predefinito di output non viene aperto in modo esplicito.

