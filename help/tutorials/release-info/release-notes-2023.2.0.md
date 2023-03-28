---
title: Note sulla versione | Guide Adobe Experience Manager as a Cloud Service, versione di febbraio 2023
description: Versione di febbraio delle guide di Adobe Experience Manager as a Cloud Service
exl-id: c639b136-11ed-4a8b-a595-4bb5da879747
source-git-commit: ee520ab86ea41df7556a1f40d7bfc5e3617b34ae
workflow-type: tm+mt
source-wordcount: '2178'
ht-degree: 2%

---

# Versione di febbraio delle guide di Adobe Experience Manager as a Cloud Service

## Aggiornamento alla versione di febbraio

Aggiorna le guide correnti di Adobe Experience Manager as a Cloud Service (in seguito denominate *Guide AEM as a Cloud Service*) eseguendo le seguenti operazioni:
1. Controlla il codice Git dei Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
2. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file dei tuoi Cloud Services Codice Git a 2023.2.235.
3. Conferma le modifiche ed esegui la pipeline dei Cloud Services per eseguire l’aggiornamento alla versione di febbraio di AEM Guide as a Cloud Service.

## Passaggi per indicizzare il contenuto esistente (solo se disponi di una versione precedente al rilascio di settembre delle AEM guide as a Cloud Service)

Esegui i seguenti passaggi per l’indicizzazione del contenuto esistente e utilizza il nuovo testo trova e sostituisci a livello di mappa:

* Esegui una richiesta POST al server (con autenticazione corretta) - `http://<server:port>/bin/guides/map-find/indexing`.
(Facoltativo: Puoi trasmettere percorsi specifici delle mappe per indicizzarle, per impostazione predefinita tutte le mappe saranno indicizzate || Esempio : `https://<Server:port>/bin/guides/map-find/indexing?paths=<map_path_in_repository>`)

* L’API restituirà un jobId. Per controllare lo stato del processo, puoi inviare una richiesta di GET con ID processo allo stesso punto finale - `http://<server:port>/bin/guides/map-find/indexing?jobId={jobId}`
(Ad esempio: http://&lt;
_localhost:8080_>/bin/guides/map-find/indexing?jobId=2022/9/15/7/27/7dfa1271-981e-4617-b5a4-c18379f11c42_678)

* Una volta completato il processo, la richiesta di GET di cui sopra risponderà con successo e menzionerà se eventuali mappe non sono riuscite. Le mappe indicizzate correttamente possono essere confermate dai log del server.

## Matrice di compatibilità

In questa sezione viene elencata la matrice di compatibilità per le applicazioni software supportate da AEM Guide as a Cloud Service versione di febbraio 2023.

### FrameMaker e FrameMaker Publishing Server

| AEM guide as a Cloud Release | FMPS | FrameMaker |
| --- | --- | --- |
| 2023.02.0 | Non compatibile | 2022 o superiore |
|  |  |  |

*La linea di base e le condizioni create in AEM sono supportate nelle versioni FMPS a partire dal 2020.2.

### Connettore dell&#39;ossigeno

| AEM guide as a Cloud Release | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno | Modifica in Windows Ossigeno | Modifica in Oxygen Mac |
| --- | --- | --- | --- | --- |
| 2023.02.0 | 2.8-uuid-8 | 2.8-uuid-8 | 2.3 | 2.3 |
|  |  |  |  |


## Nuove funzioni e miglioramenti

AEM Guide as a Cloud Service fornisce miglioramenti e nuove funzioni nella versione di febbraio:

### Generare report dall&#39;editor Web

AEM Guide include una funzione nell’editor Web che consente di controllare la completezza complessiva dei documenti tecnici e di generare report per essi.
È possibile visualizzare l&#39;elenco degli argomenti, gestire i metadati e visualizzare i file multimediali utilizzati in tutti i riferimenti per la mappa corrente dal
**Rapporti** nell&#39;editor Web.

**Genera la vista Elenco argomenti**

È possibile generare l&#39;elenco argomenti che fornisce informazioni dettagliate sugli argomenti, ad esempio il tipo di riferimento, lo stato del documento e l&#39;autore. È inoltre possibile generare il CSV per scaricare lo snapshot corrente degli argomenti nella mappa DITA.

**Gestione dei metadati e modifica dello stato del documento**

È possibile applicare tag su un singolo argomento o utilizzare la funzione di assegnazione tag in blocco per applicare più tag su più argomenti, una mappa DITA o una mappa secondaria. È inoltre possibile modificare lo stato del documento di tutti gli argomenti selezionati al successivo stato comune del documento.

<img src="assets/web-editor-metadata-panel.png" alt="gestire i metadati" width="600">

**Genera il report Multimedia**

Puoi generare il rapporto multimediale che contiene informazioni dettagliate sui contenuti multimediali utilizzati nei tuoi riferimenti all&#39;interno della mappa corrente. Puoi filtrare e ordinare i file multimediali elencati nel rapporto.
È inoltre possibile generare il CSV per scaricare lo snapshot corrente dei file multimediali utilizzati nella mappa DITA.

<img src="assets/web-editor-reports-multimedia.png" alt="rapporto multimediale" width="600">

### UX rivista per la funzionalità di revisione

Ora AEM guide fornisce un UX migliorato che ti aiuta a rivedere gli argomenti condivisi per la revisione. Nell’esperienza più recente, la funzionalità di revisione presenta i seguenti miglioramenti:

* Interfaccia utente aggiornata
* Pannello Condizioni che consente di evidenziare il contenuto in base alle condizioni disponibili nell’argomento
* Ogni commento nel pannello dei commenti è collegato al testo corrispondente nell&#39;argomento corrente. Consente di identificare il testo con commenti.
* I commenti vengono visualizzati nell&#39;ordine del testo del commento nel documento.
* Il nome dell’attività di revisione viene visualizzato nel flusso di lavoro di revisione.
* Selezionare la rootmap per l&#39;attività di revisione utilizzata per risolvere tutti i riferimenti chiave e i termini del glossario utilizzati nel contenuto della revisione.
* Barra degli strumenti contestuale che consente di evidenziare o barrare rapidamente il testo
* Menu delle opzioni per modificare o eliminare i commenti personalizzati
* Per i commenti obsoleti, è possibile accedere a una visualizzazione affiancata che consente di confrontare la versione precedente dell’argomento con la versione di revisione corrente.
* Quando si utilizzano i filtri, i commenti nel pannello di destra vengono filtrati in base alla selezione e il numero di commenti nel pannello di sinistra viene aggiornato di conseguenza.


   <img alt="compito di revisione" src="assets/comment-pop-up-panel.png" width="600">



### Miglioramenti alla traduzione

Ora è possibile migliorare la traduzione dei documenti dall’Editor Web in modo più semplice e intuitivo nel dashboard Traduzione.

**Passa l’etichetta della versione alla versione di destinazione**

AEM Guide consente di passare l’etichetta del file di origine al file di destinazione. Questo consente di identificare facilmente la versione di origine del file tradotto.

<img alt="etichette di traduzione" src="assets/translation-pass-source-label.png" width="600">

Ad esempio, se hai alcuni file di origine a cui è stata applicata l’etichetta di versione Release 1.0, puoi anche passare l’etichetta di origine (Release 1.0) al file tradotto.

**Forza la sincronizzazione per le risorse fuori sincronia**

Se apporti modifiche ad alcune risorse, AEM guide le contrassegna come non sincronizzate. È possibile tradurre nuovamente le risorse modificate o scegliere di ignorare lo stato Out of Sync. Ad esempio, se hai apportato alcune modifiche minori che non hanno bisogno di una traduzione, puoi contrassegnarne lo stato come In Sync.

<img src="assets/translation-version-diff.png" alt="commissione di traduzione" width="600">

**Visualizza progetti di traduzione in corso per un argomento o una mappa**

È possibile che alcuni riferimenti nel dashboard di traduzione siano in corso. Ora AEM Guide offre una funzione che consente di visualizzare l’elenco di tutti i progetti di traduzione in corso (insieme alla lingua di destinazione) contenenti il riferimento selezionato.


### Genera output in vari formati dall&#39;editor web

Ora è possibile generare facilmente l&#39;output per gli argomenti o la mappa DITA dall&#39;Editor Web. Puoi configurare vari predefiniti di output come AEM sito, PDF, HTML5, JSON (un formato di output headless) e output personalizzato. Puoi quindi utilizzarli per generare le rispettive uscite.

È possibile definire gli attributi negli argomenti DITA e quindi utilizzare il predefinito per le condizioni per applicare una condizione durante la pubblicazione dell&#39;output. È inoltre possibile utilizzare la funzione di pubblicazione Linea di base per pubblicare in modo selettivo una versione specifica della mappa o dell&#39;argomento DITA.


### Trova e sostituisci il testo a livello di mappa

AEM Guide consente di cercare i file all’interno di una mappa che contengono testo specifico. Il testo cercato viene evidenziato nei file. Ora è anche possibile sostituire la parola o la frase cercata con un&#39;altra parola o frase all&#39;interno di tutti i file. È possibile selezionare **Sostituisci tutto** a destra nella parte superiore dell’elenco per sostituire tutte le occorrenze del termine ricercato in tutti i file.

<img src="assets/map-find-replace.png" alt="trova sostituzione mappa" width="600">

### Eliminare e duplicare i file dal pannello del repository

Ora è possibile creare facilmente un duplicato o una copia di un file dal **Opzioni** del file selezionato nel pannello archivio. Per impostazione predefinita, il file viene creato con un suffisso (come `filename_1.extension`).

<img src="assets/options-menu-repo-view-file-level.png" alt="menu opzioni file " width="500">


### Altri miglioramenti dell’editor web

* In Guide AEM, è possibile eseguire alcune operazioni comuni per immagini e file multimediali utilizzando il menu di scelta rapida. Ora è anche possibile individuare l’immagine o il supporto selezionati nella directory archivio o visualizzare l’anteprima del file nell’interfaccia utente di Assets.

* Il nome del profilo cartella corrente viene visualizzato come etichetta per l’icona Preferenze utente nella barra degli strumenti principale. Questo consente di identificare il profilo della cartella su cui stai lavorando.

* Quando si apre una mappa nella vista mappa, il titolo della mappa corrente viene visualizzato al centro della barra degli strumenti principale. È utile per informare gli utenti della mappa attualmente aperta.


### Visualizza il titolo al posto di UUID nell&#39;Editor di ossigeno

Ora AEM Guide ti consente di scegliere **Usa titolo in Editor e Maps Manager** in Impostazioni. Se si seleziona questa opzione, il titolo del file viene visualizzato nella scheda del file quando viene aperto nell&#39;Editor o nel Gestore mappe DITA. Se non selezioni questa opzione, l’UUID del file viene visualizzato nella scheda del file.

### Pubblicazione basata su microservizi per AEM guide as a Cloud Service

Il nuovo microservizio di pubblicazione consente di eseguire carichi di lavoro di pubblicazione di grandi dimensioni simultaneamente su AEM Guide as a Cloud Service e di sfruttare la piattaforma Adobe I/O Runtime senza server leader del settore.

Per ogni richiesta di pubblicazione AEM Guide as a Cloud Service esegue un contenitore separato che viene ridimensionato in orizzontale in base alle richieste dell’utente. Questo consente di eseguire più richieste di pubblicazione e di ottenere prestazioni migliori.

Per ulteriori dettagli, consulta [Configurare la nuova pubblicazione basata su microservizi per le guide AEM as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-guides-learn/tutorials/knowledge-base/publishing/configure-microservices.md).

### PDF nativo | Aggiungi un segnalibro personalizzato nell’output di PDF

Ora è possibile aggiungere un segnalibro personalizzato su un particolare contenuto nell’output finale di PDF per facilitarne la navigazione. Questo viene aggiunto al sommario creato dai titoli degli argomenti o delle sezioni nella mappa DITA.

### PDF nativo | Applicare uno stile personalizzato alle voci del sommario e al contenuto dell’argomento

AEM Guide fornisce la funzione per applicare lo stile personalizzato alle voci del sommario o a un particolare argomento nell’output di PDF. Ad esempio, puoi modificare il colore del testo nel sommario e il titolo dell’argomento. È inoltre possibile applicare stili all’intero contenuto dell’argomento.


### PDF nativo | Personalizzare lo stile del marcatore pagina nel componente a piè di pagina

Ora è possibile formattare il marcatore pagina nelle note a piè di pagina. Ad esempio, è possibile aggiungere parentesi o modificarne il colore. Questi stili consentono agli utenti di identificare facilmente i marcatori pagina nel documento.

### PDF nativo | Cambia barra per indicare gli argomenti modificati nel Sommario

AEM Guide ora consente di identificare rapidamente gli argomenti modificati nel sommario dell’output di PDF.  Mostra una barra di modifica a sinistra degli argomenti modificati nel sommario. Puoi fare clic sull’argomento nel sommario e visualizzare le modifiche dettagliate.

<img src="assets/change-marker-toc.png" alt="Cambia marcatore nel sommario " width="500">

## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

### Authoring  

* Le modifiche nel codice HTML dell’editor web causano problemi con `<dl>` e `<dlentry>`. (11024)
* Alcuni attributi non vengono trattati come condizionali e causano problemi. (10895)
* Tre livelli o più nidificati `<indexterm>` non sono nidificati nell’esportazione nativa di PDF. (10799)
* Il contenuto scompare nel corpo di un’attività quando si passa dalla visualizzazione Autore alla visualizzazione Origine. (10735)
* I commenti di revisione non sono inseriti in un&#39;attività di revisione. (10625)
* **Annulla** o **Ripeti** non funziona correttamente su alcuni file. (10373)
* I metadati personalizzati non vengono mantenuti quando si esegue un&#39;azione Copia e Incolla. (10367)
* L’opzione Annulla in XML Editor porta l’utente nella parte superiore della pagina. (10091)
* Le proprietà del nodo vengono rimosse dopo l’operazione di copia e incolla di una risorsa. (10053)
* mimeType è codificato per la creazione e l&#39;aggiornamento delle risorse DITA. (8979)
* Il nome del creatore della versione in Cronologia versioni è &quot;fmdita-serviceuser&quot; per i file caricati tramite l’interfaccia utente di Assets. (8910)
* I frammenti di contenuto non possono essere copiati e incollati quando AEM Guide è installato su Cloud. (11315)
* Il browser (Editor web) si blocca durante il caricamento del contenuto con uno schema personalizzato. (11211)

### Gestione

* Copiare una risorsa mappa DITA (dall’interfaccia utente di Assets ) causa la presenza di linee di base errate nella risorsa copiata. (11218)
* Il messaggio di avviso non viene visualizzato al caricamento di un file che supera il limite consentito in AEM (2 GB per impostazione predefinita). (10817)
* Editor web di base | Il comportamento della colonna Più recente è diverso nel nuovo dashboard della linea di base all’interno dell’editor Web. (10808)
* Traduzione | Il lavoro di traduzione non viene avviato a causa di /libs/fmdita/i18n/ja.json non valido. (10543)
* Traduzione | Si verifica un errore in un progetto di traduzione dell’ambito creato dal dashboard di traduzione (traduzione umana). (10526)
* Traduzione | L’elaborazione post è bloccata per l’intera cartella linguistica le cui risorse sono presenti in un progetto di traduzione attivo. (10332)
* Se la versione viene modificata e salvata nell’editor Linea di base, vengono visualizzati più pop-up per qualsiasi risorsa. (10399)
* La perdita di sessione si verifica in `com.day.cq.search.impl.builder.QueryBuilderImpl.createResourceResolver(QueryBuilderImpl.java:210)`. (10279)

### Pubblicazione

* La rigenerazione dell&#39;argomento non funziona in alcuni scenari. (10635)
* Il listener Publishlistener non visualizza i dati richiesti nei log di informazioni e contiene anche alcuni log junk.( 10567)
* PDF nativo | Quando si crea un predefinito di output con l’opzione &quot;Aggiungi al profilo cartella&quot;, la generazione di PDF non riesce e viene generata un’eccezione Null Pointer. (10950)
* PDF nativo | Si verificano problemi durante la rotazione dell’intestazione della tabella. (10555)
* PDF nativo | Nidificato `<indexterm>` non sono nidificati nell’esportazione nativa di PDF. (10521)
* PDF nativo | Il topicref nidificato nelle appendici viene trasformato in h1 nella HTML temporanea. (10454)
* La pubblicazione della linea di base non riesce per PDF generato con FrameMaker Publishing Server 2020. (10551)
* PDF nativo | Aggiunta `xref` in un&#39;immagine non esegue il rendering dell&#39;immagine sul PDF generato. (11346)
* PDF nativo | Il tag immagine aggiunge l’attributo display-inline a tutte le immagini. (10653)
* PDF nativo | I commenti Bozza sono nascosti per impostazione predefinita nell’output generato. (10560)
* PDF nativo | navtitle non è onorato per topichead. (10509)
