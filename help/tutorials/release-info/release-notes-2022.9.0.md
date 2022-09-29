---
title: Note sulla versione | Guide Adobe Experience Manager as a Cloud Service, versione di settembre 2022
description: Versione più recente delle guide di Adobe Experience Manager as a Cloud Service
source-git-commit: 748a37298849b3fbf6079c19de3cb052dee3a464
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 3%

---

# Versione più recente delle guide di Adobe Experience Manager as a Cloud Service

## Aggiornamento alla versione più recente

Aggiorna le guide correnti di Adobe Experience Manager as a Cloud Service (in seguito denominate *Guide AEM as a Cloud Service*) eseguendo le seguenti operazioni:
1. Controlla il codice Git dei Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
2. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file dei tuoi Cloud Services Codice Git a 2022.9.178.
3. Conferma le modifiche ed esegui la pipeline dei Cloud Services per eseguire l’aggiornamento all’ultima versione di AEM Guide as a Cloud Service.

## Passaggi per indicizzare il contenuto esistente

Esegui i seguenti passaggi per l’indicizzazione del contenuto esistente e utilizza il nuovo testo trova e sostituisci a livello di mappa:
* Esegui una richiesta POST al server (con autenticazione corretta) - `http://<server:port>/bin/guides/map-find/indexin`.
(Facoltativo: Puoi trasmettere percorsi specifici delle mappe per indicizzarle, per impostazione predefinita tutte le mappe saranno indicizzate || Esempio :   `https://<Server:port>/bin/guides/map-find/indexing?paths=<map_path_in_repository>`)
* L’API restituirà un jobId. Per controllare lo stato del processo, puoi inviare una richiesta di GET con ID processo allo stesso punto finale - `http://<server:port>/bin/guides/map-find/indexing?jobId={jobId}`
(Ad esempio: `http://<_localhost:8080_>/bin/guides/map-find/indexing?jobId=2022/9/15/7/27/7dfa1271-981e-4617-b5a4-c18379f11c42_678)`
* Una volta completato il processo, la richiesta di GET di cui sopra risponderà con successo e menzionerà se eventuali mappe non sono riuscite. Le mappe indicizzate correttamente possono essere confermate dai log del server.


## Matrice di compatibilità

In questa sezione viene elencata la matrice di compatibilità per le applicazioni software supportate dalla versione di AEM Guide as a Cloud Service di settembre 2022.

### FrameMaker e FrameMaker Publishing Server

| FMPS | FrameMaker |
| --- | --- |
| Non compatibile | Aggiornamento 4 e superiore del 2020 |
|  |  |

*La linea di base e le condizioni create in AEM sono supportate nelle versioni FMPS a partire dal 2020.2.

### Connettore dell&#39;ossigeno

| AEM guide as a Cloud Release | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno | Modifica in Windows Ossigeno | Modifica in Oxygen Mac |
| --- | --- | --- | --- | --- |
| 2022.9.0 | 2.7.13 | 2.7.13 | 2.3 | 2.3. |
|  |  |  |  |


## Nuove funzioni e miglioramenti

AEM Guide as a Cloud Service offre molti miglioramenti e nuove funzioni nell’ultima versione:


### Creare una linea di base dinamica basata sulle etichette

AEM Guide offre la funzione di creare linee di base dinamiche basate su etichette. Se si genera una baseline, si scarica una baseline o si crea un progetto di traduzione utilizzando una baseline, i file vengono selezionati in modo dinamico in base alle etichette aggiornate. Questa funzione è utile in quanto non è necessario modificare la linea di base durante l’aggiornamento delle etichette.
Puoi anche esportare lo snapshot della baseline come CSV.

![Creare linee di base](assets/dynamic-baseline.png)

### Trova e sostituisci il testo a livello di mappa

È ora possibile cercare i file all’interno di una mappa che contengono testo specifico. Il testo cercato viene evidenziato nei file. È inoltre possibile sostituire la parola o la frase cercata con un&#39;altra parola o frase all&#39;interno dei file.
Seleziona la **Sostituisci** per sostituire l&#39;occorrenza corrente e la **Sostituisci tutto nel file** per sostituire tutte le occorrenze nel file selezionato.

![Trova sostituisci nella mappa](assets/map-find-replace.png)

Per impostazione predefinita, le opzioni **File di estrazione prima della sostituzione** e **Crea nuova versione dopo la sostituzione** sono selezionati, in modo che un file venga estratto prima di sostituire il testo e venga creata una nuova versione dopo la sostituzione del testo.

### Visualizza la differenza di versione per i file Out of Sync dal dashboard di traduzione

Ora puoi scegliere di tradurre il **Non sincronizzato** in base alle modifiche apportate tra le due versioni di un argomento.\
![Dashboard di traduzione](assets/translation-version-diff.png)
Dal dashboard di traduzione è possibile vedere facilmente le differenze tra l’ultima versione tradotta e la versione corrente del file selezionato.

![finestra di dialogo della differenza della versione](assets/version-diff.png)

In base alle differenze, puoi decidere se tradurre o meno un argomento.

### Interfaccia utente metadati disponibile per i predefiniti di PDF

È possibile impostare i metadati dal predefinito di output di una mappa DITA. È possibile impostare i metadati Titolo, Autore, Oggetto e Parole chiave. Questi metadati vengono mappati sui metadati nelle Proprietà file del PDF di output.
Questi metadati sostituiscono i metadati definiti a livello di libro. È possibile definire i metadati in modo specifico in ogni predefinito di output e trasmetterli al PDF di output.

![Metadati in predefinito](assets/preset-metadata.png)


## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

* Editor web | Quando si spostano elementi all’interno di un argomento, gli ID assegnati sugli elementi vengono sovrascritti dagli ID assegnati automaticamente. (7895)
* Tracciare le modifiche | Il contenuto viene perso quando un nuovo elemento viene inserito utilizzando la chiave Invio. (10246)
* Non viene creata una sottomappa riferita alla mappa principale nei modelli dita. (10231)
* Editor XML | Copia e incolla non funziona in modalità di authoring. (10309)
* Non vengono deselezionate più etichette di versione una volta selezionate. (9561)
* La navigazione automatica al percorso nella finestra di dialogo di navigazione del sito non funziona come file browse. (9920)
* Il pannello Struttura non visualizza il contenuto quando viene attivato da **Autore** a **Origine** modalità. (10319)
* Il confronto in un nuovo argomento creato utilizzando un contenuto nel modello di argomento non funziona. L’ID hash copiato non viene aggiornato nella copia del contenuto. (9890)
* Editor web | Nessun caricatore esistente durante la creazione di una mappa dal modello di mappa. (9891)
* Nuovo editor mappa | Il testo in grassetto o corsivo aggiunto nel titolo della mappa non viene mantenuto se si passa da **Autore** al **Layout** visualizza. (10218)
* Nuovo editor mappa | Le condizioni applicate a qualsiasi riferimento non possono essere rimosse dalla vista Layout. (10213)
* Nuovo editor mappa | L’applicazione dei riferimenti alle condizioni non funziona nella vista Layout come nella vista Autore. (10198)
* Nuovo editor mappa | Sposta a sinistra dal menu di scelta rapida rimuove il riferimento se non può essere spostato a sinistra. (10219)
* Nuovo editor mappa |L’icona non viene visualizzata correttamente per i riferimenti contenuti in una mappa creata con la vista Layout. (10197)
* Pannello Repository | Fai clic con il pulsante destro del mouse nel pannello dell’archivio per visualizzare un errore dell’applicazione. (10123)
* Trova e sostituisci | La modalità scura non è leggibile per i risultati della ricerca nell’editor web. (9978)
* Traduzione | I metadati e i tag non vengono propagati alle copie tradotte. (4696)
* Il contenuto da incollare (ctrl+c/ctrl+v) genera un errore in modalità di authoring. (10304)
* Modello PDF | L’aggiunta di immagini di sfondo a qualsiasi layout di pagina visualizza l’assoluto del percorso immagine e le immagini non vengono visualizzate nel PDF di output. (10297)
* PDF nativo | Il titolo del capitolo e l’intestazione del capitolo non funzionano nella pubblicazione di PDF. (9947)
* PDF nativo | `xref` per un concetto non viene risolto correttamente per un argomento DITA specifico. (10229)
* PDF nativo | Impossibile visualizzare il testo della didascalia per una tabella nell’output di PDF generato. (9827)
* PDF nativo | I riferimenti nelle appendici non vengono visualizzati come appendici nell’output di PDF. (10182)
* PDF nativo | L’attributo Frame di una tabella non viene propagato al HTML temporaneo (come classe). (10353)
* PDF nativo | i file HTML temp aggiungono le classi colsep e rowsep a td e il valore anche se il loro valore è 0 nel DITA di origine. (10352)
* PDF nativo | I metadati per i criteri aggiunti nel layout di pagina non vengono rispettati. (10377)
* PDF nativo | La generazione di PDF non riesce per contenuti specifici. (9927)
* PDF nativo | Il contenuto tramite conkeyref non viene visualizzato nell’output di PDF. (9836)
* PDF nativo | I riferimenti chiave per Keydefs con immagini o collegamenti esterni non sono stati risolti. (10063)
* La visualizzazione dell&#39;autore per una mappa non visualizza il testo segnaposto per la tabella e la classifica. (10330)
* Quando creiamo una nuova baseline, il filtro della baseline già selezionato non viene applicato. (9954)
* File video mancante dalla linea di base se il nome della cartella principale ha un carattere spazio. (10031)
* La creazione della linea di base non sceglie la versione più recente quando il fuso orario dell’utente è diverso da quello del server. (10190)
* La scelta rapida Ctrl + F non apre il modale di ricerca del browser nella console Risorse dopo l’installazione AEM Guide 4.1 in AEM 6.5.12. (10189)


## Problemi noti

Adobe ha identificato i seguenti problemi noti per la versione di AEM Guide as a Cloud Service a settembre 2022.


* La linea di base dinamica non è integrata con la pubblicazione di knowledge base.

* Traduzione | L’icona di differenza della versione viene visualizzata per il contenuto sorgente a causa di eventuali modifiche nel contenuto di destinazione.
