---
title: Note sulla versione | Guida di Adobe Experience Manager versione 4.1
description: Ultima versione delle guide di Adobe Experience Manager
exl-id: c70b3bbc-3332-4626-bc30-641034f8fd06
source-git-commit: f74126c1eb7bccf0c9464cbe9b1138af5bd4938f
workflow-type: tm+mt
source-wordcount: '3275'
ht-degree: 3%

---

# Rilascio 4.1.x delle guide di Adobe Experience Manager

Queste note sulla versione descrivono le istruzioni di aggiornamento, le nuove funzioni e i miglioramenti introdotti nella versione 4.1.x delle Guide di Adobe Experience Manager (in seguito denominati *Guide AEM*).

## Aggiornamento alla versione più recente

È possibile aggiornare facilmente la versione corrente di AEM Guide alla versione 4.1.2. Prima di procedere con l’aggiornamento alla versione 4.1.2 di AEM Guide, è necessario tenere in considerazione i seguenti punti:
* Se utilizzi le versioni 4.1 o 4.1.x, puoi effettuare direttamente l’aggiornamento alla versione 4.1.2.
* Se utilizzi la versione 4.0.x, devi eseguire l’aggiornamento alla versione 4.1 o 4.1.x prima di eseguire l’aggiornamento alla versione 4.1.2.
* Se utilizzi la versione 3.8.5, devi eseguire l’aggiornamento alla versione 4.0.x prima di eseguire l’aggiornamento alla versione 4.1.
* Se utilizzi una versione precedente alla versione 3.8.5, consulta la sezione sull’aggiornamento nella guida all’installazione specifica per il prodotto.

Per maggiori dettagli, vedi [Istruzioni di aggiornamento](assets/Adobe-Experience-Manager-Guides-Upgrade-Instructions-EN.pdf).

## 4.1.2. | Note sulla versione

## Matrice di compatibilità

In questa sezione viene elencata la matrice di compatibilità per le applicazioni software supportate da AEM versione 4.1.2.

### ADOBE EXPERIENCE MANAGER

**Non UID**
Versione 6.5 Service Pack 13, 12, 11 o 10

**UUID**
Versione 6.5 Service Pack 13, 12, 11 o 10

Per ulteriori dettagli, consulta la sezione Requisiti tecnici nella guida all’installazione e alla configurazione delle guide Adobe Experience Manager .


### FrameMaker e FrameMaker Publishing Server

| Versione | FMPS 2020 | FMPS 2019 | Fm 2020 | Fm 2019 |
| --- | --- | --- | --- | --- |
| 4.1.2 (non UUID) | 2020.2 o superiore* | 2019 | 2020.3 o superiore | 2019.8 (ultimo aggiornamento) |
| 4.1.2 (UUID) | 2020.2 o superiore* | Non compatibile | 2020.4 o superiore | Non compatibile |
|  |  |  |  |

*La linea di base e le condizioni create in AEM sono supportate nelle versioni FMPS a partire dal 2020.2.

### Connettore dell&#39;ossigeno

| Versione | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno | Modifica in Windows Ossigeno | Modifica in Oxygen Mac |
| --- | --- | --- |--- |--- |
| 4.1.2 (non UUID) | 2,0 | 2,0 | 1,6 | 1,6 |
| 4.1.2 (UUID) | 2.7 | 2,7 | 2.3 | 2.3. |
|  |  |  |


## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

* Quando si selezionano tutti i profili di cartella, viene visualizzato un profilo di cartella invisibile (errato). (10393)
* La creazione della linea di base non sceglie la versione più recente, quando il fuso orario dell’utente è diverso da quello del server. (10336)
* La scelta rapida Control+F non apre il modale di ricerca del browser nella console Risorse dopo l’installazione di AEM Guide 4.1. (10339)
* Si verifica un errore di creazione della linea di base per l&#39;argomento che ha il riferimento a una cartella. (10383)
* La scheda Predefiniti di output mostra una schermata vuota a intermittenza e in alcuni casi vengono visualizzati predefiniti non modificabili. (10390)
* La gestione dello spazio chiave sta generando eccezioni ed errori. (10449)

### Problemi noti con la soluzione alternativa

* La linea di base esportata durante la traduzione non viene caricata nella scheda della linea di base dell&#39;editor.

   **Soluzione alternativa**: Utilizzare la scheda baseline del dashboard mappa DITA.

## 4.1. | Note sulla versione

Queste note sulla versione descrivono le istruzioni di aggiornamento, le nuove funzioni e i miglioramenti introdotti nella versione 4.1.x delle Guide di Adobe Experience Manager (in seguito denominati *Guide AEM*).

## Matrice di compatibilità

Questa sezione elenca la matrice di compatibilità per le applicazioni software supportate dalla versione 4.1 di AEM.

### ADOBE EXPERIENCE MANAGER

**Non UID**
Versione 6.5 Service Pack 13, 12, 10 o 11

**UUID**
Versione 6.5 Service Pack 13, 12, 10 o 11

Per ulteriori dettagli, consulta la sezione Requisiti tecnici nella guida all’installazione e alla configurazione delle guide Adobe Experience Manager .




### FrameMaker e FrameMaker Publishing Server

| Versione | FMPS 2020 | FMPS 2019 | Fm 2020 | Fm 2019 |
| --- | --- | --- | --- | --- |
| 4.1 (non UUID) | 2020.2 o superiore* | 2019 | 2020.3 o superiore | 2019.8 (ultimo aggiornamento) |
| 4.1 (UUID) | 2020.2 o superiore* | Non compatibile | 2020.4 o superiore | Non compatibile |
|  |  |  |  |

*La linea di base e le condizioni create in AEM sono supportate nelle versioni FMPS a partire dal 2020.2.

### Connettore dell&#39;ossigeno

| Versione | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno | Modifica in Windows Ossigeno | Modifica in Oxygen Mac |
| --- | --- | --- |--- |--- |
| 4.1 (non UUID) | 2,0 | 2,0 | 1,6 | 1,6 |
| 4.1 (UUID) | 2,7 | 2,7 | 2.3. | 2.3. |
|  |  |  |


## Nuove funzioni e miglioramenti

AEM Guide offre molti miglioramenti e nuove funzioni nella versione 4.1:

### Editor web avanzato

* **Risoluzione dei tasti migliorata**

Un riferimento a una chiave di contenuto DITA inserisce una parte di contenuto da un argomento all’altro. Utilizza una chiave per individuare il contenuto. È necessario risolvere i riferimenti chiave associati a un argomento DITA. La mappa radice selezionata ha la precedenza più alta per risolvere i riferimenti chiave.

![finestra di dialogo delle preferenze utente](assets/user-preferences.png)

Ora i riferimenti chiave vengono risolti in base alla mappa radice impostata nel seguente ordine di priorità:

1. Preferenze utente
2. Pannello Vista mappa
3. Profilo cartella

Per ulteriori dettagli, consulta *Risolvere i riferimenti chiave* nella guida Utilizzo delle guide di Adobe Experience Manager .

* **Aggiungi un pannello personalizzato nel pannello a sinistra**

Ora è possibile aggiungere un pannello personalizzato nel pannello di sinistra dell’Editor Web. Puoi utilizzare un pannello personalizzato per vari scopi, ad esempio per fornire aiuto o eseguire i test per un progetto. Se è stato configurato un pannello personalizzato, questo viene visualizzato anche nell’elenco dei pannelli all’interno della **Impostazioni editor**. Puoi attivare o disattivare l’opzione per visualizzare o nascondere il pannello personalizzato.

* **Possibilità di modificare lo stato del documento degli argomenti in una mappa DITA**

Ora è possibile modificare facilmente lo stato del documento degli argomenti selezionati all&#39;interno di una mappa DITA. È inoltre possibile aprire e modificare le proprietà degli argomenti selezionati in una mappa DITA dalla **Altre opzioni** nella parte inferiore del pannello Visualizza mappa.

![proprietà argomento selezionate](assets/map-view-properties.png)

* **Informazioni sulla versione visualizzate in modalità Anteprima**

L’editor Web consente di gestire le versioni. Ora è anche possibile visualizzare la versione dell&#39;argomento attivo o la mappa DITA nell&#39;angolo in alto a destra della scheda file dell&#39;argomento in modalità Anteprima di un argomento.

![versione di anteprima](assets/preview-version.png)


* **Comportamento di aggiornamento migliorato dell’Editor Web**

I seguenti miglioramenti sono ora disponibili con l’operazione di aggiornamento del browser nell’editor Web:

* Ora è disponibile il supporto per aggiornare il browser mentre si modifica il contenuto nell&#39;editor Web. Se si preme l&#39;icona di aggiornamento del browser quando si aprono per la modifica uno o più file con modifiche non salvate, viene richiesto di salvare i file o annullare l&#39;azione di aggiornamento.

* Anche quando si aggiorna il browser, vengono mantenute le viste del pannello di sinistra e del pannello di destra.

* L’argomento attivo o la mappa DITA viene riaperta nell’area di modifica del contenuto.

* **Creare mappe basate su modelli personalizzati**

Ora è disponibile la potente funzione per creare modelli mappa personalizzati. È possibile utilizzarli per creare mappe DITA insieme ai modelli di argomento e di mappa a cui si fa riferimento nel modello di mappa.

![modelli dita](assets/dita-templates.png)

È inoltre possibile fare riferimento ad altri modelli mappa e modelli argomento dal modello mappa personalizzato. I modelli di mappa a cui si fa riferimento possono fare riferimento a vari modelli di mappa, modelli di argomento, argomenti, mappe, immagini, video e altre risorse.

![creare modelli dita](assets/create-dita-template.png)

Il modello di mappa personalizzato può aiutarti a replicare molto facilmente i modelli di mappa e l&#39;intera struttura di cartelle di riferimento. Questi modelli personalizzati sono particolarmente utili per creare e ricreare più mappe con strutture e riferimenti ricorsivi.

* **Supporto dello schema**
Per &quot;Schematron&quot; si intende un linguaggio di convalida basato su regole utilizzato per definire i test per un file XML. Utilizzando un file Schematron è possibile definire determinate regole e quindi convalidarle per un argomento DITA o una mappa. L’editor web supporta i file Schematron. È possibile importare i file Schematron e modificarli in Web Editor. Il supporto di Schematron nell&#39;editor Web consente di convalidare i file in base a un insieme di regole e di mantenere coerenza e correttezza tra gli argomenti.

![convalida schema](assets/schematron-validate.png)

* **Finestra di dialogo migliorata alla chiusura del file**

AEM Guide chiede di salvare le modifiche e sbloccare i file bloccati quando si tenta di chiudere un file aperto nell&#39;Editor Web. I prompt vengono visualizzati in base al **Chiedi il check-in alla chiusura** e **Chiedi nuova versione alla chiusura** impostazioni configurate dall&#39;amministratore.

In base alla configurazione, è possibile salvare le modifiche e creare una nuova versione del documento. Oppure, puoi anche archiviare il file e salvare le modifiche alla versione corrente.

![File chiuso](assets/file-close-save-changes-unlock.png)

Per ulteriori dettagli, consulta *Scenari di chiusura e salvataggio dei file* nella guida Utilizzo delle guide di Adobe Experience Manager .* Il **Inserisci parola chiave** è stata migliorata la funzione . Ora è più semplice trovare una parola chiave da inserire, in quanto le parole chiave sono elencate in ordine alfabetico. È inoltre possibile cercare parole chiave digitando una stringa di ricerca nella casella Ricerca.

![inserisci parola chiave](assets/insert-keyword.png)

* **Supporto per documenti Markdown**
Markdown è un linguaggio di markup leggero che consente di aggiungere elementi di formattazione a documenti di testo normale. L’editor Web consente di utilizzare documenti Markdown (.md) insieme ai documenti DITA. È possibile creare e visualizzare in anteprima facilmente un documento Markdown nell’editor Web e aggiungerlo nel file di mappa tramite l’editor di mappe DITA.  Per ulteriori dettagli, consulta 
*Creare documenti Markdown dall’editor Web* nella guida Utilizzo delle guide di Adobe Experience Manager .

![markdown di supporto](assets/create-markdown-dita-topic.png)

* **Possibilità di configurare una visualizzazione tag predefinita**
Se un utente abilita la visualizzazione dei tag dall’editor Web, questa rimane abilitata anche nelle sessioni.  Ciò significa che non è necessario abilitare nuovamente la visualizzazione Tag per accedervi in un secondo momento. L’amministratore può configurare lo stato predefinito per la visualizzazione dei tag nell’editor Web. Il valore predefinito per Visualizzazione tag per una nuova sessione utente è determinato dalla proprietà tagsView nel file ui_config.json .

* Ora i file nella vista archivio vengono caricati in batch. Tutti i file presenti nel file principale o `/content/dam folder` sono elencati. Ma dal livello successivo o dalla cartella secondaria vengono caricati 75 file alla volta. Questo caricamento batch è efficiente e puoi accedere più rapidamente ai file rispetto al caricamento di tutti i file esistenti in una cartella.

![caricare altri file](assets/load-more-files.png)

### Nuovo dashboard della linea di base

AEM versione 4.1 di Guide fornisce la funzione Linea di base integrata all’interno dell’editor web. È ora possibile creare linee di base dall’editor Web e utilizzarle per pubblicare o tradurre argomenti di versioni diverse.

**Nota**: Per il sistema aggiornato, aggiornare **ui_config.json** per Profilo cartella.

Utilizza questa funzione per creare una baseline con una versione specifica degli argomenti disponibili in una data e in un&#39;ora specifiche. Inoltre, ottieni il supporto API per creare o aggiornare una linea di base con un’etichetta definita per una versione di argomenti.

![scheda gestione linea di base](assets/baseline-manage.png)

È possibile cercare i file in base ai nomi dei file o alla posizione del file. Puoi anche filtrare gli argomenti da visualizzare nella finestra di modifica della linea di base e ordinarli in base a colonne specifiche.

![scheda gestione linea di base](assets/baseline-filter.png)

Le prestazioni del processo di creazione della linea di base sono state ulteriormente migliorate. Il processo di creazione delle linee di base è asincrono, pertanto puoi continuare a modificare altri file nell’Editor web durante la creazione della linea di base. Per ulteriori dettagli, consulta *Creare e gestire le linee di base dall’editor web* nella guida Utilizzo delle guide di Adobe Experience Manager .

Nota: La scheda Linea di base nel dashboard della mappa è nascosta per impostazione predefinita. L’amministratore può abilitare la scheda Linea di base nel dashboard della mappa.

* Il parametro della linea di base nelle API da scaricare Map ora utilizza il titolo della linea di base per recuperare il contenuto con le versioni.

### Processo di traduzione migliorato

* **Possibilità di creare un progetto di traduzione dell&#39;ambito**
Se devi creare solo l’ambito di un progetto da tradurre, puoi selezionare 
**Crea un nuovo progetto di traduzione dell&#39;ambito**. Questo non invierà le copie per la traduzione e lo stato di traduzione originale dei file viene mantenuto.

![progetto di traduzione dell&#39;ambito](assets/scoping-translation-project.png)

* La **Lingue** vengono visualizzate le cartelle della lingua insieme ai relativi codici della lingua. Ad esempio, francese (fr) e tedesco (de).

![traduzione linguistica](assets/translation-languages.png)

Per maggiori dettagli sulla traduzione, vedi *Tradurre documenti dall&#39;editor Web* nella guida Utilizzo delle guide di Adobe Experience Manager .


### Pubblicazione ottimizzata

* Puoi anche accedere al **Pubblica dashboard** dalla scheda Outputs (Output) durante la generazione dell&#39;output dal dashboard della mappa. Un elenco di tutte le attività di pubblicazione attive è disponibile nel dashboard di pubblicazione.

![uscite in coda](assets/queued-output.png)

* Dal dashboard mappa è possibile selezionare più file DITAVAL per generare contenuto condizionale. È possibile mantenere l&#39;ordine dei file aggiungendo o eliminando file. Puoi anche passare il cursore del mouse sul nome del file per visualizzare il percorso nell’archivio AEM in cui è memorizzato il file.

* Le linee di base sono state rispettate per i metadati dell&#39;output AEM sito. È inoltre possibile elaborare le proprietà di una versione della linea di base come metadati. Se non viene definita alcuna linea di base, le proprietà della versione più recente vengono elaborate come metadati.

* La **Nome file** e **Argomenti della riga di comando DITA-OT** sono state aggiunte opzioni per i predefiniti di output HTML5, EPUB e Personalizzato. Ora è possibile specificare il nome del file con cui si desidera salvare l&#39;output. È inoltre possibile specificare gli argomenti aggiuntivi da elaborare durante la generazione dell&#39;output.

### Dashboard mappa

Quando si seleziona per scaricare la mappa DITA, la richiesta viene messa in coda e si riceve una notifica una volta che la mappa è pronta per il download. Puoi scegliere di scaricare il file mappa immediatamente o scaricarlo in un secondo momento dal collegamento fornito nella casella in entrata della notifica AEM.

![Download mappa](assets/download-map-prompt.png)

### Altri miglioramenti delle funzioni

* AEM Guide ora supporta Oxygen XML Author versione 24.1.
* Il parametro della linea di base nelle API da scaricare Map ora utilizza il titolo della linea di base per recuperare il contenuto con le versioni.

### Funzione obsoleta

AEM Guide non supporta più la generazione del formato di output DITA per i documenti FrameMaker. Questa opzione DITA è stata rimossa anche dai predefiniti di output del dashboard Mappa.

## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

* Il supporto per l’authoring non è disponibile come alternativa per i riferimenti basati sul percorso del file per la pubblicazione. (8076)
* Il pacchetto DITA Add on impedisce il rilevamento di risorse duplicate DAM. (8417)
* Dopo il check-in di un documento da Oxygen a AEM, il contenuto giapponese nel documento viene sostituito da punti interrogativi (????). (9124)
* L&#39;aggiornamento dei file estratti non funziona sulla registrazione con l&#39;autenticazione Web in Ossigeno. (9179)
* Il file non viene estratto quando viene aperto in Ossigeno. (9192)
* Dopo il check-in di un documento da Oxygen a AEM, il contenuto giapponese nel documento viene sostituito da punti interrogativi (????). (9276)
* Autenticazione Web non funzionante in Ossigeno. (9296)
* Il ricaricamento non riesce in Ossigeno quando i file esistono già in AEM nella stessa posizione. (9328)
* Opzione non disponibile per la sincronizzazione forzata del contenuto tra AEM e il sistema locale. (9439)
* L&#39;ID non viene generato automaticamente per l&#39;elemento aggiunto utilizzando **Inserisci contenuto riutilizzabile** finestra di dialogo dalla barra degli strumenti secondaria. (5826)
* Non viene visualizzata alcuna finestra di dialogo di conferma per il caricamento di un’immagine con lo stesso nome di un file esistente, tramite l’editor. (6011)
* Uno spazio unificatore non disponibile nel pallet di caratteri. (7523)
* L’elenco degli elementi (Alt+Invio) viene visualizzato in grigio nel tema scuro/scuro. (7913)
* La versione non viene aggiornata quando si salva la revisione di un argomento dalla barra degli strumenti del pannello mappa. (8228)
* xref non può essere inserito anche in posizioni valide. (8354)
* L’operazione &quot;getversionlabel&quot; presenta limitazioni e non fornisce le prestazioni previste. (8513)
* Si verificano problemi con la finestra di dialogo di conferma sulla chiusura di un file bloccato o modificato che non è attualmente aperto nell&#39;editor. (8692)
* Si verifica un errore durante l’aggiunta di un utente come amministratore nel profilo della cartella quando l’ID utente è numerico. (8908)
* Il pannello di traduzione è visibile anche all’apertura della mappa DITA nell’Editor mappa. (9053)
* Il codice della lingua non viene visualizzato con la lingua nel pannello Traduzione. (9108)
* Le schede Traduzione e Linea di base sono visibili per un certo periodo di tempo nel dashboard Mappa. (9146)
* Al termine della traduzione, viene creata una versione aggiuntiva per la risorsa tradotta. (9310)
* La traduzione approvata non si integra alla lingua di destinazione quando il codice della lingua di destinazione contiene cinque caratteri come `fr_ca`. (9357)
* Il contenuto tradotto non funziona quando il codice della lingua di destinazione creato viene menzionato come `fr-fr, `, `en-us`. (9527)
* Al caricamento di una mappa DITA che si trova al di fuori della cartella della lingua, viene registrata un&#39;eccezione nel backend.(9543)
* Impossibile creare un file DITA utilizzando il modello DITA personalizzato dall&#39;editor. (7262)
* La mappa DITA si perde quando si pubblica una mappa UUID DITA tramite FMPS. (7278)
* AEM Guide non copia le proprietà non univoche di una risorsa quando questa viene copiata e incollata. (8241)
* Il nome del file della mappa DITA non viene convertito in minuscolo al momento della creazione. (8383)
* La descrizione dell’attività di revisione non viene visualizzata nella notifica e-mail inviata quando viene assegnata una nuova attività di revisione. (8507)
* Scaricare l’API della mappa | Le cartelle temporanee non vengono pulite in caso di errori del processo di download. (8523)
* `columnpreview.jsp` dipende da SP.  (8543)
* I processi di output con stato come &quot;In attesa&quot; o &quot;In esecuzione&quot; non vengono ripuliti nel dashboard di pubblicazione.  (8569)
* Icona predefinita selezionata per generare un rapporto utilizzando il pulsante Genera, anche quando la proprietà dell’icona è definita. (8573)
* I problemi si verificano nel processo di revisione durante l&#39;aggiornamento da 3.8.X a 4.0. (8788)
* Nel pannello Revisione dell&#39;Editor Web, se un nome utente è lungo, le icone da accettare/rifiutare non vengono visualizzate chiaramente. (8793)
* La struttura dei riferimenti si interrompe dopo la rimozione di un argomento e l&#39;esecuzione di un&#39;operazione Sposta. (8804)
* La DTD personalizzata definita dall&#39;utente non ha la precedenza rispetto alla DTD DITA standard incorporata in DITA-OT. (9104)
* La posizione dell’evidenziazione non è corretta nella visualizzazione affiancata. (9305)
* La nota a piè di pagina utilizzata per riferimento non scorre fino alla sezione a piè di pagina nell&#39;output AEM sito. (9061)
* L&#39;ordine delle note a piè di pagina non è corretto nell&#39;output del sito AEM. (9327)
* Le nuove risorse DITA create vengono sempre estratte da un altro utente. (9387)
* L’errore viene sempre connesso alla creazione di nuovo contenuto. (9388)
* La terza schermata nel processo di creazione dell&#39;attività di revisione non mostra l&#39;elenco dei glossari. (4558)
* Riferimenti UUID non corretti assegnati durante il caricamento di più file dal connettore FrameMaker/Oxygen. (8269)
* La notifica e-mail non viene inviata quando un’attività di revisione viene riassegnata nella casella in entrata. (8376)
* Impossibile aggiungere il secondo utente amministratore come primo utente amministratore a una cartella. (8430)
* **Applica etichette** nella scheda Linea di base le etichette non vengono visualizzate nel menu a discesa. (8455)
* Quando si utilizza la pubblicazione della linea di base con l’immagine come rif nell’argomento, l’immagine non viene pubblicata nell’output. (8564)
* La funzione di eliminazione dell&#39;output non riesce se sono presenti numerosi nodi della cronologia di output rimasti. (8568)
* Nel pannello della cronologia delle versioni, la sezione della versione corrente mostra una marca temporale errata e viene modificata dalle informazioni. (8765)
* Linea di base non aggiornata in base all&#39;etichetta definita. (8799)
* L&#39;errore si verifica quando i file la cui cartella padre contiene caratteri speciali nel nome file, vengono aperti in Ossigeno (utilizzando **Modifica in ossigeno** ). (8918)
* Il caricamento di file da Oxygen a AEM non riesce. (9157)
* Se il contenuto viene spostato in un’altra cartella, la mappa di download con baseline non funziona. (9331)
* Oxygen controlla una versione non corretta di un argomento dopo un ripristino di una versione in AEM. (9411)
* La ricerca nel pannello Repository e nella finestra di dialogo Sfoglia topicref blocca lo schermo quando il contenuto è grande. (9432)
* Se l’impostazione **Crea nuova versione per il file caricato** è attivato, viene creata una nuova versione per il ripristino e il salvataggio su qualsiasi nodo bloccato. (9473)
* Le differenze di marca temporale errate vengono visualizzate nell’interfaccia utente di Assets al ripristino della versione di un file. (9480)
* I file vengono estratti automaticamente al ripristino di qualsiasi versione. (9482)
* L’icona Blocca viene visualizzata nella vista archivio anche quando il file viene archiviato dall’editor.  (5756)
* Impossibile aggiungere elementi di sfondo in una libreria utilizzando la visualizzazione Autore dell&#39;editor Web. (7652)
* La modalità Anteprima non supporta `deliveryTarget` attributo di elaborazione condizionale in DITA. (7685)
* All’apertura di un argomento del glossario nell’editor XML, AEM forza il suo salvataggio anche se non è stato modificato. (8105)
* La finestra di dialogo Inserisci riferimenti viene visualizzata quando si aggiungono sottoprogetti a una mappa utilizzando l&#39;interfaccia utente. (8212)
* Riutilizza arresti anomali del pannello dei contenuti durante la ricerca di caratteri speciali `[` o `*` .(8279)
* Durante l&#39;authoring di Glossentry, l&#39;Editor Web mostra il contenuto come Nota. (8384)
* L&#39;editor XML rimuove la nuova riga nel blocco di codice. (8522)
* Se si passa dalla modalità di origine a quella di authoring, l’argomento viene contrassegnato come non più valido e il contenuto deve essere nuovamente salvato.(8524)
* Impossibile chiudere un argomento sbloccato. (8545)
* Non esiste alcuna opzione per scegliere il percorso della Knowledge Base nei predefiniti di pubblicazione basati su articoli. (8636)
* Non sono disponibili attributi per l&#39;aggiunta di un capitolo nella libreria tramite trascinamento dalla vista Preferiti. (8746)
* La finestra di dialogo Inserisci parola chiave non dispone della capacità di ricerca e le parole chiave non sono elencate in ordine ordinato. (9094)
* Se si esegue una ricerca in XML Editor, la pagina viene bloccata. (9452)
* Siti mancanti AEM predefiniti nella scheda Output. (9567)
* Immagini di SVG il cui rendering non viene eseguito correttamente nelle modalità di authoring di XML Editor. (9426)
* La linea di base non viene rispettata durante la pubblicazione tramite salesforce. (8953)
* Non è presente la possibilità di cancellare la rootmap dalle impostazioni delle preferenze utente. (8534)
