---
title: Note sulla versione | Adobe Experience Manager Guides as a Cloud Service, versione di aprile 2023
description: Ultima versione di Adobe Experience Manager Guides as a Cloud Service
exl-id: 3b09f0b3-cfa4-422d-91b7-733ab1c1896c
source-git-commit: cf612da41f79b0bf9da4c4d7454a0e3c86af7a4c
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 2%

---

# Versione di aprile di Adobe Experience Manager Guides as a Cloud Service

## Effettua l’aggiornamento alla versione più recente

Aggiorna le guide Adobe Experience Manager as a Cloud Service correnti (in seguito denominate *Guide AEM as a Cloud Service*) eseguendo i seguenti passaggi:

1. Consulta il codice Git del Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
2. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file del codice Git dei tuoi Cloud Services in 2023.4.249.
3. Apporta le modifiche ed esegui la pipeline dei Cloud Services per l’aggiornamento all’ultima versione as a Cloud Service delle guide AEM.

## Passaggi per indicizzare il contenuto esistente (solo se utilizzi una versione precedente alla versione di settembre di AEM Guides as a Cloud Service)

Per indicizzare il contenuto esistente e utilizzare il nuovo testo di ricerca e sostituzione a livello di mappa, effettua le seguenti operazioni:

* Eseguire una richiesta POST al server (con l’autenticazione corretta) - `http://<server:port>/bin/guides/map-find/indexing`.
(Facoltativo: Puoi trasmettere percorsi specifici delle mappe per indicizzarle; per impostazione predefinita, tutte le mappe saranno indicizzate || Esempio: `https://<Server:port>/bin/guides/map-find/indexing?paths=<map_path_in_repository>`)

* L’API restituirà un jobId. Per verificare lo stato del processo, puoi inviare una richiesta di GET con ID processo allo stesso endpoint: `http://<server:port>/bin/guides/map-find/indexing?jobId={jobId}`
(Ad esempio: http://&lt;
_localhost:8080_>/bin/guides/map-find/indexing?jobId=2022/9/15/7/27/7dfa1271-981e-4617-b5a4-c18379f11c42_678)

* Una volta completato il processo, la richiesta di GET di cui sopra risponderà con successo e menzionerà se eventuali mappe non sono riuscite. Le mappe indicizzate correttamente possono essere confermate dai registri del server.

## Matrice di compatibilità

In questa sezione è elencata la matrice di compatibilità per le applicazioni software supportate dalla versione di aprile 2023 delle guide AEM as a Cloud Service.

### Server di pubblicazione FrameMaker e FrameMaker

| Versione di AEM Guides as a Cloud | FMPS | FrameMaker |
| --- | --- | --- |
| 2023.04.0 | Non compatibile | 2022 o versione successiva |
|  |  |  |


### Connettore ossigeno

| Versione di AEM Guides as a Cloud | Finestre del connettore dell&#39;ossigeno | Connettore di ossigeno Mac | Modifica in finestre a ossigeno | Modifica in Oxygen Mac |
| --- | --- | --- | --- | --- |
| 2023.04.0 | 2,9-uuid-2 | 2,9-uuid-2 | 2.3 | 2.3 |
|  |  |  |  |


## Nuove funzioni e miglioramenti

AEM Guides as a Cloud Service offre miglioramenti e nuove funzioni nell’ultima versione:

### Supporto avanzato dei metadati nella pubblicazione PDF

Le guide AEM ora forniscono supporto avanzato per i metadati mappati sui metadati nell’output PDF. Le opzioni relative ai metadati includono informazioni sul documento e sul relativo contenuto, ad esempio il nome dell&#39;autore, il titolo del documento, le parole chiave, le informazioni sul copyright e altri campi dati.

<img src="assets/pdf-metadata.png" alt=" metadati pdf nativi">

Potete importare un file XMP e le guide AEM possono scegliere le informazioni dal file. Puoi anche fornire i nomi e i valori dei metadati utilizzando il menu a discesa. Puoi anche aggiungere metadati personalizzati digitando direttamente nel campo del nome.


### Pannello Visualizzazione Struttura migliorata

Le guide AEM forniscono un pannello migliorato Visualizzazione struttura in cui è possibile ottenere la visualizzazione gerarchica degli elementi utilizzati nel documento.

<img src="assets/select-element-content-outline-view_cs.png" alt=" metadati pdf nativi">

La vista Struttura offre i seguenti miglioramenti:

* Il menu a discesa Opzioni vista (View Options) viene visualizzato sopra il pannello Visualizzazione struttura (Outline View). Se un elemento ha un ID, un attributo e un testo, puoi selezionarli dal menu a discesa per visualizzarli insieme all’elemento. Gli attributi che possono essere visualizzati nel pannello Visualizzazione struttura sono determinati dalle impostazioni Attributi di visualizzazione configurate dall&#39;amministratore all&#39;interno del **Impostazioni editor**.

* Utilizzando la funzione di ricerca, puoi cercare un elemento in base al suo nome, ID, testo o valore dell’attributo.


### Pubblicazione basata su microservizi per guide AEM as a Cloud Service

AEM Guides as a Cloud Service fornisce la funzione di eseguire carichi di lavoro di pubblicazione di grandi dimensioni in concomitanza con la pubblicazione basata su microservizi e di sfruttare la piattaforma senza server Adobe I/O Runtime leader del settore.

Nella versione di aprile è ora possibile eseguire più richieste di pubblicazione simultaneamente e generare output di PDF in blocco in modo molto efficiente utilizzando la pubblicazione di PDF nativi basata su microservizi.
Per ulteriori dettagli, consulta [Configurare una nuova pubblicazione basata su microservizi per le guide AEM as a Cloud Service](../knowledge-base/publishing/configure-microservices.md).


## Problemi risolti

Di seguito sono elencati i bug risolti in varie aree:

* Native PDF | La pubblicazione di contenuti con una classe di output con parentesi() comporta un blocco della pubblicazione. (11596)
* Il problema si verifica quando si sposta (trascina e rilascia) al posto di una voce di elenco esistente con l’opzione Rileva modifiche attivata. (11570)
* Si verifica un problema quando si sposta (trascina e rilascia) come nuova voce di elenco con l’opzione Rileva modifiche attivata. (11569)
* Il rientro o il rientro degli elementi dell&#39;elenco non funziona come previsto con l&#39;opzione Rileva modifiche attivata. (11568)
* L&#39;aggiunta di contenuto su una riga con Revisioni attivate e quindi la disattivazione di Revisioni non ne determina la disattivazione. (11567)
* Difficoltà nel trascinare una voce di elenco, il testo viene spostato al posto della voce di elenco. (11566)
* La revisione completata non si apre in modalità di sola lettura. (11387)
* Il problema si verifica nella ricerca del sito AEM (non funziona oltre i nodi di 2-3 livelli). (11352)
* Durante l’authoring nell’elemento visualizzato in verde (Rileva modifiche), il nuovo contenuto viene visualizzato come revisione anche se la modifica della traccia è disabilitata. (7021)

### Problema noto con la soluzione alternativa

L’Adobe ha identificato il seguente problema noto per la versione as a Cloud Service di aprile 2023 delle guide AEM.

* Native PDF | I vecchi metadati vengono compilati solo dopo l’apertura esplicita del predefinito di output.
