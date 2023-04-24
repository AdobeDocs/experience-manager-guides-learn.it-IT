---
title: Note sulla versione | Guide Adobe Experience Manager as a Cloud Service, versione di maggio 2022
description: Rilascio di maggio delle guide di Adobe Experience Manager as a Cloud Service
exl-id: 7928a300-5ec9-492c-b9be-02b6f87638c6
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '1874'
ht-degree: 4%

---

# Rilascio di maggio delle guide di Adobe Experience Manager as a Cloud Service

## Aggiornamento alla versione di maggio

Aggiorna le guide correnti di Adobe Experience Manager as a Cloud Service (in seguito denominate *Guide AEM as a Cloud Service*) eseguendo le seguenti operazioni:
1. Controlla il codice Git dei Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
1. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file dei tuoi Cloud Services Codice Git a 2022.5.144.
1. Conferma le modifiche ed esegui la pipeline dei Cloud Services per eseguire l’aggiornamento alla versione di maggio di AEM Guide as a Cloud Service.

## Matrice di compatibilità

Questa sezione elenca la matrice di compatibilità per le applicazioni software supportate dalla versione di AEM Guide as a Cloud Service di maggio 2022.

### FrameMaker e FrameMaker Publishing Server

| FMPS | FrameMaker |
| --- | --- |
| Non compatibile | Aggiornamento 4 e superiore del 2020 |
|  |  |

*La linea di base e le condizioni create in AEM sono supportate nelle versioni FMPS a partire dal 2020.2.

### Connettore dell&#39;ossigeno

| AEM guide as a Cloud Release | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno |
| --- | --- | --- |
| 2022.5.0 | 2.6.9 | 2.6.9 |
|  |  |  |


## Nuove funzioni e miglioramenti

AEM guide as a Cloud Service offre numerosi miglioramenti e nuove funzioni nella versione di maggio:

### Editor web avanzato

* **Creare mappe basate su modelli personalizzati**

Ora è disponibile la potente funzione per creare modelli mappa personalizzati. È possibile utilizzarli per creare mappe DITA insieme ai modelli di argomento e di mappa a cui si fa riferimento nel modello di mappa.

![modelli dita](assets/dita-templates.png)

È inoltre possibile fare riferimento ad altri modelli mappa e modelli argomento dal modello mappa personalizzato. I modelli di mappa a cui si fa riferimento possono fare riferimento a vari modelli di mappa, modelli di argomento, argomenti, mappe, immagini, video e altre risorse.

![creare modelli dita](assets/create-dita-template.png)

Il modello di mappa personalizzato può aiutarti a replicare molto facilmente i modelli di mappa e l&#39;intera struttura di cartelle di riferimento. Questi modelli personalizzati sono particolarmente utili per creare e ricreare più mappe con strutture e riferimenti ricorsivi.

* La **Inserisci parola chiave** è stata migliorata la funzione . Ora è più semplice trovare una parola chiave da inserire, in quanto le parole chiave sono elencate in ordine alfabetico. È inoltre possibile cercare parole chiave digitando una stringa di ricerca nella casella Ricerca.

![inserisci parola chiave](assets/insert-keyword.png)

* Ora i file nella vista archivio vengono caricati in batch. Vengono caricati 75 file alla volta. Questo caricamento batch è efficiente e puoi accedere più rapidamente ai file rispetto al caricamento di tutti i file esistenti in una cartella.

![caricare altri file](assets/load-more-files.png)

* È possibile eseguire il rendering delle immagini SVG che includono dati incorporati o collegamenti in tutte le schermate dell’editor XML, incluse, tra l’altro, le visualizzazioni Anteprima e Autore.

* L&#39;XSD/DTD predefinito può essere aggiornato alla versione più recente

### Processo di traduzione migliorato

* **Possibilità di creare un progetto di traduzione dell&#39;ambito**
Se devi creare solo l’ambito di un progetto da tradurre, puoi selezionare 
**Crea un nuovo progetto di traduzione dell&#39;ambito**. Questo non invierà le copie per la traduzione e lo stato di traduzione originale dei file viene mantenuto.

![progetto di traduzione dell&#39;ambito](assets/scoping-translation-project.png)

* Se si rifiuta la traduzione per uno o più argomenti di un processo di traduzione, lo stato di traduzione in corso di tutti gli argomenti rifiutati ritorna al loro stato originale.

* La **Lingue** vengono visualizzate le cartelle della lingua insieme ai relativi codici della lingua. Ad esempio, francese (fr) e tedesco (de).

* La funzione di traduzione ora supporta anche il codice della lingua, che include sia il paese che la lingua. Ad esempio, `fr-fr`, `en-us`.

![traduzione linguistica](assets/translation-languages.png)

* Al caricamento di una mappa DITA al di fuori della cartella della lingua, non viene registrata alcuna eccezione nel backend.

Per maggiori dettagli sulla traduzione, vedi *Tradurre documenti dall&#39;editor Web* in Utilizzo delle guide di Adobe Experience Manager as a Cloud Service.


### Pubblicazione ottimizzata

* Puoi anche accedere al **Pubblica dashboard** dalla scheda Outputs (Output) durante la generazione dell&#39;output dal dashboard della mappa. Un elenco di tutte le attività di pubblicazione attive è disponibile nel dashboard di pubblicazione.

![uscite in coda](assets/queued-output.png)

* Dal dashboard mappa è possibile selezionare più file DITAVAL per generare contenuto condizionale. È possibile mantenere l&#39;ordine dei file aggiungendo o eliminando file. Puoi anche passare il cursore del mouse sul nome del file per visualizzare il percorso nell’archivio AEM in cui è memorizzato il file.

* **Funzione obsoleta**
AEM as a Cloud Service non supporta più la generazione del formato di output DITA per i documenti FrameMaker. Questa opzione DITA è stata rimossa anche dai predefiniti di output del dashboard Mappa.

### Miglioramento della pubblicazione basata su articoli

XML Editor consente di mappare più di una categoria di prodotto su un articolo durante la pubblicazione su un profilo Salesforce.

### Altri miglioramenti delle funzioni

* La modalità Anteprima supporta anche `deliveryTarget` attributo di elaborazione condizionale in DITA. È disponibile come opzione nel filtro a discesa insieme a **pubblico**, **piattaforma**, **prodotto**, prop, **altri prop**.
* È stata fornita l&#39;opzione per la sincronizzazione forzata tra il server AEM di Oxygen e il sistema locale.

## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

* Nel pannello di revisione dell&#39;editor Web, l&#39;utente non è in grado di rispondere ai commenti di revisione. (9667)
* L&#39;applicazione viene lasciata vuota quando si fa clic su una cartella vuota dopo l&#39;aggiornamento tramite il menu Opzioni. (9639)
* Viene creata una nuova versione quando **Salva e chiudi** il file archiviato. (9638)
* Il pulsante Chiudi non viene visualizzato quando **Salva come nuova versione** la casella di controllo è abilitata. (9637)
* Il PDF corretto non viene pubblicato se viene pubblicato per la prima volta tramite un PDF separato per ciascun capitolo e quindi un singolo file PDF (l’opzione Crea file PDF separati non è selezionata). (9632)
* La dashboard della mappa genera problemi di metadati per gli utenti non amministratori. (9620)
* Una volta creata una linea di base, lo stato viene impostato su non riuscito nell&#39;interfaccia utente (la chiamata di stato get non riesce) se il server dispone di più di 10000 file. (9608)
* L’archiviazione di dati di grandi dimensioni nelle proprietà causa un errore di pubblicazione in quanto il flusso di lavoro di pubblicazione suddiviso non riesce. (9586)
* Lo stato Filtri attributi condizionali non viene mantenuto quando si passa da Anteprima a Origine e si torna alla modalità Anteprima. (9553)
* Il nome della mappa segnaletica viene lasciato vuoto nella vista Archivio nel caso in cui non venga fornito alcun nome tramite la `mainbooktitle` tag . (9538)
* Errore HTTP 400 durante l&#39;apertura di un file caricato utilizzando Oxygen. (9535)
* I predefiniti di una mappa precedentemente aperta rimangono visibili nella scheda Output quando si apre una mappa senza predefiniti definiti. (9523)
* La funzionalità di ricerca per Tag e Attributi non funziona nel pannello Struttura. (9506)
* La raccolta appena creata non è visibile finché il browser non viene aggiornato il browser. (9505)
* Le etichette Attributi condizionali (non i valori) vengono visualizzate in modalità sorgente quando si aggiungono tutte le condizioni tramite l’opzione &quot;Aggiungi tutte le proprietà&quot;. (9501)
* I file vengono estratti automaticamente al ripristino di qualsiasi versione. (9482)
* Le differenze di marca temporale errate vengono visualizzate nell’interfaccia utente di Assets al ripristino della versione di un file. (9480)
* Durante l&#39;inserimento di elementi nell&#39;elemento topicref della mappa DITA vengono aggiunti più elementi dai risultati della ricerca. (9474)
* Se l’impostazione **Crea nuova versione per il file caricato** è attivato, viene creata una nuova versione per il ripristino e il salvataggio su qualsiasi nodo bloccato. (9473)
* Il testo visualizzato di Riferimento chiave e Riferimento chiave di contenuto non viene mantenuto quando si modifica l’URL del collegamento, se il testo di visualizzazione non viene aggiunto durante la definizione del riferimento chiave. (9458)
* In Cronologia versioni, il numero di versione e l&#39;etichetta non vengono visualizzati per la versione corrente. (9446)
* L’editor si blocca quando alcuni file di contenuto vengono aperti nell’editor. (9443)
* La ricerca nel pannello Repository e nella finestra di dialogo Sfoglia topicref blocca lo schermo quando il contenuto è grande. (9432)
* I metadati passati all&#39;output AEM sito non rispettano la linea di base del contenuto. (9416)
* Oxygen controlla una versione non corretta di un argomento dopo un ripristino di una versione in AEM. (9411)
* La baseline non riuscita disabilita la modifica nella scheda Predefinito del dashboard della mappa. (9403)
* L’errore viene sempre connesso alla creazione di nuovo contenuto. (9388)
* Le nuove risorse DITA create vengono sempre estratte da un altro utente. (9387)
* L&#39;elemento Rinomina non funziona correttamente durante la conversione di topicref in glossref. (9380)
* L&#39;etichetta della versione non viene visualizzata come menu a discesa in **Salva come nuova versione** finestra di dialogo. (9379)
* Le condizioni non vengono applicate al passaggio tra diverse versioni da **Mostra differenze** a discesa. (9366)
* Si verificano più problemi durante l’utilizzo dei filtri di anteprima. (9365)
* Impossibile inserire risorse non DITA e DITAVAL in topicref. (9363)
* La traduzione approvata non si integra alla lingua di destinazione quando il codice della lingua di destinazione contiene cinque caratteri come `fr_ca`. (9357)
* Impossibile cercare i file utilizzando **Trova file nella cartella** dal **Altre opzioni** e l’app non risponde. (9337)
* La finestra di dialogo Sfoglia si blocca se sono presenti numerose chiavi. (9332)
* I file DITAVAL non funzionano durante la pubblicazione basata su articoli. (9330)
* L&#39;ordine delle note a piè di pagina non è corretto nell&#39;output del sito AEM. (9327)
* La ricerca non viene eseguita automaticamente quando viene modificato il percorso selezionato. (9323)
* Al termine della traduzione, viene creata una versione aggiuntiva per la risorsa tradotta. (9310)
* Impossibile eliminare gli utenti amministratore nel profilo della cartella. (9306)
* La mappa principale aggiornata da Riferimento chiave di contenuto non viene impostata finché la pagina non viene aggiornata. (9302)
* Autenticazione Web non funzionante in Ossigeno. (9296)
* I collegamenti web con caratteri codificati non funzionano correttamente. (9227)
* Il file non viene estratto quando viene aperto in Ossigeno. (9217)
* L&#39;aggiornamento dei file estratti non funziona sulla registrazione con l&#39;autenticazione Web in Ossigeno. (9179)
* Le schede Traduzione e Linea di base sono visibili per un certo periodo di tempo nel dashboard Mappa. (9146)
* Problemi di esperienza o di funzionalità si verificano durante il ricaricamento del profilo cartella. (9103)
* L’eliminazione dell’editor di layout di pagina non lo chiude dal pannello centrale nella vista Creazione. (9087)
* L&#39;errore di convalida si verifica nell&#39;Editor Web quando si rimuove un&#39;immagine e quindi si salva la nuova versione del documento. (8985)
* Impossibile visualizzare tutte le `glossrefs` nel pannello Glossario (contenuto specifico). (8886)
* `xref` senza testo non viene visualizzato nell&#39;output di pubblicazione basato su articoli. (8764)
* I riferimenti si interrompono quando si spostano immagini o file multimediali che hanno uno spazio nei nomi dei file. (8624)
* Interruzione dei riferimenti nella scelta `Select All` e lo spostamento dei file multimediali o del contenuto DITA in un&#39;altra cartella. (8622)
* I processi di output con stato come &quot;In attesa&quot; o &quot;In esecuzione&quot; non vengono ripuliti nel dashboard di pubblicazione.  (8569)
* La funzione di eliminazione dell&#39;output non riesce se sono presenti numerosi nodi della cronologia di output rimasti. (8568)
* Il pacchetto DITA Add on impedisce il rilevamento di risorse duplicate DAM. (8417)
* Pulsante Crea attività di revisione abilitato per i file non DITA. (8401)
* La finestra di dialogo Inserisci riferimenti viene visualizzata quando si aggiungono sottoprogetti a una mappa utilizzando l&#39;interfaccia utente. (8212)
* Spazio imprevisto trovato in ogni vuoto `entry` quando l&#39;attributo outputclass viene aggiunto a `tgroup` elemento. (7532)
* Il pannello Archivio non visualizza le icone di blocco dei file estratti o estratti non appena l’azione è completata. (5817)
* L’icona Blocca viene visualizzata nella vista archivio anche quando il file viene archiviato dall’editor.  (5756)
* Siti mancanti AEM predefiniti nella scheda Output. (9567)
* L&#39;editor XML si blocca quando si tenta di modificare alcuni file DITA. (9537)
* Se si esegue una ricerca in XML Editor, la pagina viene bloccata. (9452)
* Se il contenuto viene spostato in un’altra cartella, la mappa di download con baseline non funziona. (9331)
* Il ricaricamento non riesce in Ossigeno quando i file esistono già in AEM nella stessa posizione. (9328)
* La posizione dell’evidenziazione non è corretta nella visualizzazione affiancata. (9305)
* Dopo il check-in di un documento da Oxygen a AEM, il contenuto giapponese nel documento viene sostituito da punti interrogativi (????). (9276)
* Il caricamento di file da Oxygen a AEM non riesce. (9157)
* La notifica e-mail non viene inviata quando un’attività di revisione viene riassegnata nella casella in entrata. (8376)

## Problemi noti

All’apertura dell’editor viene visualizzata una pagina vuota a intermittenza.
