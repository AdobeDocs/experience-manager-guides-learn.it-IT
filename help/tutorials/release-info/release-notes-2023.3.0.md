---
title: Note sulla versione | Guide Adobe Experience Manager as a Cloud Service, versione di marzo 2023
description: Versione più recente delle guide di Adobe Experience Manager as a Cloud Service
source-git-commit: 07709048f560a77b923436d990c831a5f8b907e3
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 2%

---

# Rilascio di marzo delle guide di Adobe Experience Manager as a Cloud Service

## Aggiornamento alla versione più recente

Aggiorna le guide correnti di Adobe Experience Manager as a Cloud Service (in seguito denominate *Guide AEM as a Cloud Service*) eseguendo le seguenti operazioni:
1. Controlla il codice Git dei Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
2. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file dei tuoi Cloud Services Codice Git a 2023.3.242.
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

Questa sezione elenca la matrice di compatibilità per le applicazioni software supportate dalla versione di AEM Guide as a Cloud Service di marzo 2023.

### FrameMaker e FrameMaker Publishing Server

| AEM guide as a Cloud Release | FMPS | FrameMaker |
| --- | --- | --- |
| 2023.03.0 | Non compatibile | 2022 o superiore |
|  |  |  |


### Connettore dell&#39;ossigeno

| AEM guide as a Cloud Release | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno | Modifica in Windows Ossigeno | Modifica in Oxygen Mac |
| --- | --- | --- | --- | --- |
| 2023.03.0 | 2.9-uuid-2 | 2.9-uuid-2 | 2.3 | 2.3 |
|  |  |  |  |


## Nuove funzioni e miglioramenti

AEM guide as a Cloud Service fornisce miglioramenti e nuove funzioni nell’ultima versione:

### Aprire e riprodurre file video o audio nell’Editor Web

AEM Guide ora fornisce la funzione per aprire e riprodurre i file audio o video nell’editor Web. È possibile modificare il volume o la visualizzazione del video. Nel menu di scelta rapida sono disponibili anche le opzioni per **Scarica**, modifica **Velocità di riproduzione** o visualizzazione **Immagine nell&#39;immagine**.

<img src="assets/video-web-editor.png" alt="riprodurre video" width="600">


## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

* Il download del processo PDF non funziona correttamente nell&#39;editor Web. (11496)
* Output JSON | Mappare metadati con valore di proprietà come `"value in spaces and double quotes"` porta a un errore di pubblicazione. (11438)
* L&#39;inserimento di file multimediali audio e video non riesce nel formato YouTube sotto il **Inserisci file multimediali** icona. (11320)
* L&#39;errore di convalida si verifica quando una mappa viene creata utilizzando il modello con un elemento titolo specializzato. (11212)
* PDF nativo | la nota a piè di pagina presente nell’intestazione della tabella porta al testo in grassetto e allineato al centro nel piè di pagina della pagina corrispondente all’interno dell’output di PDF. (10610)
>[!NOTE]
>
>Per riflettere la modifica di Native PDF, elimina la cartella PDF che si trova in /content/dam/dita-templates, quindi esegui l’aggiornamento alla build più recente. (10610)

### Problema noto con la soluzione alternativa

Adobe ha identificato il seguente problema noto per la versione di AEM Guide as a Cloud Service di marzo 2023.

* Gli utenti non possono salvare o creare la versione di una risorsa duplicata.

**Soluzione alternativa**: Prima di apportare modifiche alla risorsa duplicata, rielaborala dall’interfaccia utente di Assets.

