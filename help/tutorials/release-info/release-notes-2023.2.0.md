---
title: Note sulla versione | Adobe Experience Manager Guides as a Cloud Service, versione di febbraio 2023
description: Versione di febbraio di Adobe Experience Manager Guides as a Cloud Service
exl-id: c639b136-11ed-4a8b-a595-4bb5da879747
source-git-commit: ee520ab86ea41df7556a1f40d7bfc5e3617b34ae
workflow-type: tm+mt
source-wordcount: '2178'
ht-degree: 2%

---

# Versione di febbraio di Adobe Experience Manager Guides as a Cloud Service

## Effettua l’aggiornamento alla versione di febbraio

Aggiorna le guide Adobe Experience Manager as a Cloud Service correnti (in seguito denominate *Guide AEM as a Cloud Service*) eseguendo i seguenti passaggi:
1. Consulta il codice Git del Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
2. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file del codice Git dei tuoi Cloud Services in 2023.2.235.
3. Apporta le modifiche ed esegui la pipeline dei Cloud Services per l’aggiornamento alla versione di febbraio dell’as a Cloud Service AEM Guides.

## Passaggi per indicizzare il contenuto esistente (solo se utilizzi una versione precedente alla versione di settembre di AEM Guides as a Cloud Service)

Effettua le seguenti operazioni per indicizzare il contenuto esistente e utilizzare il nuovo testo Trova e sostituisci a livello di mappa:

* Eseguire una richiesta POST al server (con l’autenticazione corretta) - `http://<server:port>/bin/guides/map-find/indexing`.
(Facoltativo: Puoi trasmettere percorsi specifici delle mappe per indicizzarle; per impostazione predefinita, tutte le mappe saranno indicizzate || Esempio: `https://<Server:port>/bin/guides/map-find/indexing?paths=<map_path_in_repository>`)

* L’API restituirà un jobId. Per verificare lo stato del processo, puoi inviare una richiesta di GET con ID processo allo stesso endpoint: `http://<server:port>/bin/guides/map-find/indexing?jobId={jobId}`
(Ad esempio: http://&lt;
_localhost:8080_>/bin/guides/map-find/indexing?jobId=2022/9/15/7/27/7dfa1271-981e-4617-b5a4-c18379f11c42_678)

* Una volta completato il processo, la richiesta di GET di cui sopra risponderà con successo e menzionerà se eventuali mappe non sono riuscite. Le mappe indicizzate correttamente possono essere confermate dai registri del server.

## Matrice di compatibilità

In questa sezione è elencata la matrice di compatibilità per le applicazioni software supportate dalla versione di febbraio 2023 delle guide AEM as a Cloud Service.

### Server di pubblicazione FrameMaker e FrameMaker

| Versione di AEM Guides as a Cloud | FMPS | FrameMaker |
| --- | --- | --- |
| 2023.02.0 | Non compatibile | 2022 o versione successiva |
|  |  |  |

*Le condizioni di base e quelle create nell’AEM sono supportate nelle versioni di FMPS a partire dal 2020.2.

### Connettore ossigeno

| Versione di AEM Guides as a Cloud | Finestre del connettore dell&#39;ossigeno | Connettore di ossigeno Mac | Modifica in finestre a ossigeno | Modifica in Oxygen Mac |
| --- | --- | --- | --- | --- |
| 2023.02.0 | 2,8-uuid-8 | 2,8-uuid-8 | 2.3 | 2.3 |
|  |  |  |  |


## Nuove funzioni e miglioramenti

AEM Guides as a Cloud Service fornisce miglioramenti e nuove funzioni nella versione di febbraio:

### Generare rapporti dall’editor web

Le guide AEM sono dotate di una funzione nell’editor web che consente di verificare la completezza complessiva dei documenti tecnici e di generare report per essi.
È possibile visualizzare l&#39;elenco degli argomenti, gestire i metadati e visualizzare gli elementi multimediali utilizzati in tutti i riferimenti per la mappa corrente dalla
**Rapporti** nell&#39;editor Web.

**Genera la vista Elenco argomenti**

È possibile generare l&#39;Elenco argomenti che fornisce informazioni dettagliate sugli argomenti, ad esempio il tipo di riferimento, lo stato del documento e l&#39;autore. È inoltre possibile generare il file CSV per scaricare lo snapshot corrente degli argomenti nella mappa DITA.

**Gestione dei metadati e modifica dello stato del documento**

È possibile applicare tag a un singolo argomento oppure utilizzare la funzione di assegnazione tag in blocco per applicare più tag a più argomenti, a una mappa DITA o a una mappa secondaria. È inoltre possibile modificare lo stato del documento di tutti gli argomenti selezionati al successivo possibile stato comune del documento.

<img src="assets/web-editor-metadata-panel.png" alt="gestire i metadati" width="600">

**Generare il rapporto Multimedia**

È possibile generare il report multimediale che contiene informazioni dettagliate sul file multimediale utilizzato nei riferimenti all&#39;interno della mappa corrente. È possibile filtrare e ordinare i file multimediali elencati nel report.
È inoltre possibile generare il file CSV per scaricare l&#39;istantanea corrente dei file multimediali utilizzati nella mappa DITA.

<img src="assets/web-editor-reports-multimedia.png" alt="report multimediale" width="600">

### UX rinnovata per la funzionalità di revisione

Ora le guide AEM forniscono un’interfaccia utente migliorata che consente di rivedere gli argomenti condivisi per la revisione. Nell’esperienza più recente, la funzionalità di revisione presenta i seguenti miglioramenti:

* Interfaccia utente aggiornata
* Pannello Condizioni che consente di evidenziare il contenuto in base alle condizioni disponibili nell’argomento
* Ogni commento nel pannello dei commenti è collegato al testo corrispondente nell&#39;argomento corrente. Consente di identificare il testo commentato.
* I commenti vengono visualizzati nell&#39;ordine del testo commentato nel documento.
* Il nome dell&#39;attività di revisione viene visualizzato nel flusso di lavoro di revisione.
* Selezionare la rootmap per l&#39;attività di revisione utilizzata per risolvere tutti i riferimenti chiave e i termini del glossario utilizzati nel contenuto della revisione.
* Barra degli strumenti contestuale che consente di evidenziare o barrare rapidamente il testo
* Menu Opzioni per modificare o eliminare i commenti
* Per i commenti obsoleti, è possibile accedere alla visualizzazione affiancata che consente di confrontare la versione precedente dell&#39;argomento con la versione di revisione corrente.
* Quando si utilizzano i filtri, i commenti nel pannello di destra vengono filtrati in base alla selezione e il numero di commenti nel pannello di sinistra viene aggiornato di conseguenza.


   <img alt="attività di revisione" src="assets/comment-pop-up-panel.png" width="600">



### Miglioramenti alla traduzione

Sono ora disponibili miglioramenti più semplici nel dashboard di traduzione che consentono di tradurre facilmente i documenti dall’editor web.

**Passa l’etichetta della versione alla versione di destinazione**

Le guide AEM consentono di passare l&#39;etichetta del file di origine al file di destinazione. Questo consente di identificare facilmente la versione sorgente del file tradotto.

<img alt="etichette di traduzione" src="assets/translation-pass-source-label.png" width="600">

Ad esempio, se disponi di alcuni file sorgente a cui è applicata l’etichetta di versione Release 1.0, puoi anche trasmettere l’etichetta di origine (Release 1.0) al file tradotto.

**Forza sincronizzazione per risorse non sincronizzate**

Se apporti modifiche ad alcune risorse, le guide AEM le contrassegna come non sincronizzate. Puoi tradurre nuovamente le risorse modificate o scegliere di ignorare lo stato Non sincronizzato. Ad esempio, se hai apportato alcune modifiche minori che non richiedono alcuna traduzione, puoi contrassegnarle come In sincronia.

<img src="assets/translation-version-diff.png" alt="bacheca di traduzione" width="600">

**Visualizza progetti di traduzione in corso per un argomento o una mappa**

Alcuni dei riferimenti nel dashboard di traduzione potrebbero essere in corso. Ora AEM Guides fornisce una funzione per aiutarti a visualizzare l’elenco di tutti i progetti di traduzione in corso (insieme alla lingua di destinazione) che contengono il riferimento selezionato.


### Genera output in vari formati dall’editor web

Ora è possibile generare facilmente l&#39;output per gli argomenti o la mappa DITA dall&#39;Editor Web. Puoi configurare vari predefiniti di output come Sito AEM, PDF, HTML5, JSON (un formato di output headless) e output personalizzato. Puoi quindi utilizzarli per generare i rispettivi output.

È possibile definire gli attributi negli argomenti DITA e quindi utilizzare il predefinito di condizione per applicare una condizione durante la pubblicazione dell&#39;output. È inoltre possibile utilizzare la funzione di pubblicazione della linea di base per pubblicare selettivamente una versione specifica della mappa o dell&#39;argomento DITA.


### Trova e sostituisci il testo a livello di mappa

Le guide AEM consentono di cercare all&#39;interno di una mappa file contenenti testo specifico. Il testo cercato viene evidenziato nei file. Ora è anche possibile sostituire la parola o la frase cercata con un&#39;altra parola o frase all&#39;interno di tutti i file. Puoi selezionare **Sostituisci tutto** a destra nella parte superiore dell’elenco per sostituire tutte le occorrenze del termine cercato in tutti i file.

<img src="assets/map-find-replace.png" alt="mappa trova sostituisci" width="600">

### Eliminare e duplicare i file dal pannello dell’archivio

Ora è possibile creare facilmente un duplicato o una copia di un file da **Opzioni** del file selezionato nel pannello del repository. Per impostazione predefinita, il file viene creato con un suffisso (come `filename_1.extension`).

<img src="assets/options-menu-repo-view-file-level.png" alt="menu opzioni file " width="500">


### Altri miglioramenti dell’editor web

* Nelle guide AEM è possibile eseguire alcune operazioni comuni per immagini e file multimediali utilizzando il menu di scelta rapida. Ora puoi anche individuare l’immagine o il supporto selezionato nell’archivio o visualizzare l’anteprima del file nell’interfaccia utente di Assets.

* Il nome del profilo cartella corrente viene visualizzato come etichetta per l&#39;icona Preferenze utente nella barra degli strumenti principale. Questo ti aiuta a identificare il profilo di cartella su cui stai lavorando.

* Quando apri una mappa nella vista mappa, il titolo della mappa corrente viene visualizzato al centro della barra degli strumenti principale. Questa funzione è utile per comunicare agli utenti quale mappa è attualmente aperta.


### Titolo da visualizzare al posto di UUID nell’editor di ossigeno

Ora AEM Guides consente di scegliere **Usa titolo nell’editor e nel gestore delle mappe** nelle impostazioni. Se si seleziona questa opzione, il titolo del file viene visualizzato nella scheda del file quando viene aperto nell&#39;Editor o in Gestione mappe DITA. Se non selezioni questa opzione, nella scheda del file viene visualizzato l’UUID del file.

### Pubblicazione basata su microservizi per guide AEM as a Cloud Service

Il nuovo microservizio di pubblicazione consente di eseguire contemporaneamente carichi di lavoro di pubblicazione di grandi dimensioni su guide AEM as a Cloud Service e di sfruttare la piattaforma senza server Adobe I/O Runtime leader del settore.

Per ogni richiesta di pubblicazione, le guide AEM as a Cloud Service eseguono un contenitore separato che viene ridimensionato orizzontalmente in base alle richieste dell’utente. In questo modo è possibile eseguire più richieste di pubblicazione e ottenere prestazioni migliori.

Per ulteriori dettagli, consulta [Configurare una nuova pubblicazione basata su microservizi per le guide AEM as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-guides-learn/tutorials/knowledge-base/publishing/configure-microservices.md).

### Native PDF | Aggiungi un segnalibro personalizzato nell’output di PDF

Ora puoi aggiungere un segnalibro personalizzato a un particolare contenuto nell’output PDF finale per facilitarne la navigazione. Questa opzione viene aggiunta al sommario creato dai titoli di argomento o di sezione nella mappa DITA.

### Native PDF | Applicare uno stile personalizzato alle voci del sommario e al contenuto dell’argomento

Le guide AEM consentono di applicare uno stile personalizzato alle voci del sommario o a un particolare argomento nell’output di PDF. È ad esempio possibile modificare il colore del testo nel sommario e nel titolo dell&#39;argomento. È inoltre possibile applicare stili all&#39;intero contenuto dell&#39;argomento.


### Native PDF | Personalizza lo stile del marcatore pagina nel componente Nota a piè di pagina

Ora è possibile applicare uno stile al marcatore di pagina nelle note a piè di pagina. Ad esempio, è possibile aggiungere parentesi quadre o modificarne il colore. Questi stili consentono agli utenti di identificare facilmente gli indicatori di pagina nel documento.

### Native PDF | Barra delle modifiche per indicare gli argomenti modificati nel sommario

Le guide AEM ora consentono di identificare rapidamente gli argomenti modificati nel sommario dell’output PDF.  Viene visualizzata una barra di modifica a sinistra degli argomenti modificati nel sommario. Puoi fare clic sull’argomento nel sommario e visualizzare le modifiche dettagliate.

<img src="assets/change-marker-toc.png" alt="Modifica marcatore nel sommario " width="500">

## Problemi risolti

Di seguito sono elencati i bug risolti in varie aree:

### Authoring  

* Le modifiche nell’HTML dell’editor web causano problemi con `<dl>` e `<dlentry>`. (11024)
* Alcuni attributi non vengono trattati come condizionali e causano problemi. (10895)
* Tre o più livelli nidificati `<indexterm>` non sono nidificati nell’esportazione nativa di PDF. (10799)
* Il contenuto scompare nel corpo di un’attività quando si passa dalla vista Creazione alla vista Origine. (10735)
* I commenti di revisione non vengono inseriti correttamente in un&#39;attività di revisione. (10625)
* **Annulla** o **Ripeti** non funziona correttamente su alcuni file. (10373)
* I metadati personalizzati non vengono mantenuti durante l’azione di copia e incolla. (10367)
* L&#39;opzione Annulla nell&#39;editor XML consente di portare l&#39;utente nella parte superiore della pagina. (10091)
* Le proprietà del nodo vengono rimosse dopo l’operazione di copia e incolla di una risorsa. (10053)
* mimeType è codificato per la creazione e l’aggiornamento di risorse DITA. (8979)
* Il nome dell’autore della versione nella Cronologia versioni è &quot;fmdita-serviceuser&quot; per i file caricati tramite l’interfaccia utente di Assets. (8910)
* I frammenti di contenuto non possono essere copiati e incollati quando AEM Guides è installato in Cloud. (11315)
* Il browser (Editor Web) non è in grado di caricare contenuti con uno schema personalizzato. (11211)

### Gestione

* Copiare una risorsa mappa DITA (dall’interfaccia utente di Asset ) causa l’esistenza di linee di base errate nella risorsa copiata. (11218)
* Non viene visualizzato alcun messaggio di avvertenza al caricamento di un file che supera il limite consentito dall’AEM (2 GB per impostazione predefinita). (10817)
* Web Editor-Baseline | Il comportamento della colonna Più recente nel dashboard della nuova linea di base all&#39;interno dell&#39;editor Web è diverso. (10808)
* Traduzione | Il processo di traduzione non viene avviato perché /libs/fmdita/i18n/ja.json non è valido. (10543)
* Traduzione | Si verifica un errore in un progetto di traduzione dell’ambito creato dal dashboard di traduzione (Traduzione umana). (10526)
* Traduzione | La post-elaborazione è bloccata per l’intera cartella della lingua le cui risorse sono presenti in un progetto di traduzione attivo. (10332)
* Se la versione viene modificata e salvata nell’editor della linea di base, per qualsiasi risorsa vengono visualizzati più pop-up. (10399)
* La perdita di sessione si verifica alle `com.day.cq.search.impl.builder.QueryBuilderImpl.createResourceResolver(QueryBuilderImpl.java:210)`. (10279)

### Pubblicazione

* La rigenerazione dell&#39;argomento non funziona per alcuni scenari. (10635)
* Publishlistener non visualizza i dati richiesti nei registri di informazioni e contiene anche alcuni registri di posta indesiderata.( 10567)
* Native PDF | Quando si crea un predefinito di output con l’opzione &quot;Aggiungi al profilo cartella&quot;, la generazione di PDF non riesce e viene generata un’eccezione Null Pointer. (10950)
* Native PDF | Si verificano problemi durante la rotazione dell’intestazione della tabella. (10555)
* Native PDF | Nidificato `<indexterm>` non sono nidificati nell’esportazione nativa di PDF. (10521)
* Native PDF | Il topicref nidificato nelle appendici viene trasformato in h1 nella HTML temporanea. (10454)
* La pubblicazione della linea di base non riesce per PDF generato con FrameMaker Publishing Server 2020. (10551)
* Native PDF | Aggiunta `xref` a un’immagine non esegue il rendering dell’immagine sul PDF generato. (11346)
* Native PDF | Il tag immagine aggiunge l’attributo display-inline a tutte le immagini. (10653)
* Native PDF | I commenti bozza sono nascosti per impostazione predefinita nell&#39;output generato. (10560)
* Native PDF | navtitle non è onorato per topichead. (10509)
