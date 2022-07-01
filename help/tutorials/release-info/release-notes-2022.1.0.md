---
title: Note sulla versione per [!DNL AEM Guides], versione di gennaio 2022
description: Rilascio di gennaio [!DNL Adobe Experience Manager Guides] as a Cloud Service
exl-id: b2da77fa-f17c-440b-be59-acaafcd9a57c
source-git-commit: b5e64512956f0a7f33c2021bc431d69239f2a088
workflow-type: tm+mt
source-wordcount: '2429'
ht-degree: 3%

---

# Rilascio di gennaio [!DNL Adobe Experience Manager Guides] as a Cloud Service

## Aggiornamento alla versione di gennaio

Aggiorna il tuo [!DNL Adobe Experience Manager Guides] as a Cloud Service (successivamente indicato come [!DNL AEM Guides] as a Cloud Service) eseguendo le seguenti operazioni:
1. Controlla il codice Git dei Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
2. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file dei tuoi Cloud Services Codice Git a 2022.1.78.
3. Conferma le modifiche ed esegui la pipeline dei Cloud Services per eseguire l’aggiornamento alla versione di gennaio di [!DNL AEM Guides] as a Cloud Service.

## Matrice di compatibilità

In questa sezione viene elencata la matrice di compatibilità per le applicazioni software supportate da [!DNL AEM Guides] Versione as a Cloud Service di gennaio 2022.

### FrameMaker e FrameMaker Publishing Server

| FMPS | FrameMaker |
| --- | --- |
| Non compatibile | Aggiornamento 4 e superiore del 2020 |
|  |  |


### Connettore dell&#39;ossigeno

| [!DNL AEM Guides] Versione cloud | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno | Modifica in Windows Ossigeno | Modifica in Oxygen Mac |
| --- | --- | --- | --- | --- |
| 2022.1.0 | 2.4.0 | 2.4.0 | 2.2 | 2.2. |
|  |  |  |  |  |


## Nuove funzioni e miglioramenti

### Pubblicazione basata su articoli

Con la versione di gennaio, è stata introdotta una funzione di pubblicazione basata su articoli integrata all’interno dell’editor web. Puoi utilizzare la funzione di pubblicazione basata sugli articoli per generare in modo incrementale l’output di uno o più argomenti o pubblicare i contenuti in una piattaforma knowledgebase.

Questa funzione consente agli utenti di creare la mappa DITA in modo additivo e pubblicare gli argomenti come e quando sono pronti. Dopo aver pubblicato la mappa, utilizza la funzione di pubblicazione basata sugli articoli per ottenere una pubblicazione incrementale solo per gli articoli aggiornati.

![Pubblicazione basata su articoli](assets/article-based-publishing.png)

Oltre a AEM, puoi utilizzare questa funzione unica per pubblicare i tuoi articoli su qualsiasi portale della knowledge base come Salesforce. Questa funzione è dotata anche di un modello di contenuto OOTB, basato su AEM componenti core, che consente di creare un archivio dei contenuti tecnici basato sulle conoscenze. La cosa fantastica di questo modello è che è completamente personalizzabile in base alle tue esigenze organizzative e può anche supportare casi d’uso come portali intranet aziendali.
È inoltre possibile filtrare gli articoli in base allo stato del documento e all’ora di modifica.

Questa pubblicazione on-the-go basata su articoli non solo offre un controllo completo sulla pubblicazione dei contenuti, ma riduce anche il tempo complessivo per la pubblicazione dei contenuti aggiornati.
Quando pubblichi gli articoli utilizzando questo modello, può anche trasmettere i metadati alle pagine pubblicate.
Per ulteriori dettagli, consulta *Pubblicazione basata su articoli dall’editor web* nella Guida utente.

### Editor Web migliorato

Sono stati introdotti numerosi miglioramenti e nuove funzioni nell’editor web:

* Il supporto per lo schema oggetto è stato aggiunto anche nell’editor Web. È ora possibile creare e utilizzare lo schema soggetto utilizzando il pannello Schema oggetto. Con l&#39;aggiunta dello schema del soggetto, è ora possibile utilizzare i metadati aziendali e la tassonomia.

![Schema soggetto](assets/subject-scheme-panel.png)

* In questa versione è stato introdotto un nuovo strumento per gestire glossari in blocco. Utilizzando questo strumento, è possibile convertire rapidamente il testo in glossario e glossario in termini in blocco per una mappa selezionata o argomenti aperti.

![Punto attivo globale](assets/glossary-hotspot-tool.png)

* È stata aggiunta la funzionalità di aggiornamento nel pannello Contenuto riutilizzabile , che consente di aggiornare rapidamente il contenuto riutilizzabile nei file di riferimento.
* Il nuovo indicatore della copia di lavoro indica se la copia corrente del file è sincronizzata con la versione salvata o meno.

![Indicatore della versione](assets/version-update-indicator.png)

* Il filtro di ricerca nel pannello Archivio e la finestra di dialogo Sfoglia file è stato migliorato per fornire più opzioni di filtro, che possono essere ulteriormente personalizzate.

![Filtri di ricerca nell’archivio](assets/repository-filter-search.png)

* È ora possibile caricare i file .docx dall&#39;editor Web.

### Autore con FrameMaker

Ora è possibile creare e pubblicare i documenti in FrameMaker. FrameMaker viene fornito con un connettore preconfigurato ad Adobe Experience Manager. In FrameMaker è disponibile un&#39;interfaccia di facile utilizzo che consente di mantenere versioni dei documenti in un ambiente distribuito e collaborativo.

Una volta creato il contenuto, FrameMaker consente di pubblicare i documenti in diversi formati: PDF, HTML5, EPUB e DITA. È inoltre possibile eseguire le varie operazioni di gestione dei file, come il pagamento, il pagamento con dipendenti, il check-in, l&#39;aggiornamento e così via.
Per creare con FrameMaker in [!DNL AEM Guides] Utilizzo as a Cloud Service di FrameMaker versione 2020.4 e successive.

### Nuovo dashboard di traduzione

Nell’Editor Web è stato introdotto un nuovo dashboard di traduzione con le seguenti funzioni:

* Ordinamento, ricerca e filtraggio dell’elenco di argomenti.
* Filtrare il contenuto per tipo di riferimento: riferimenti diretti o indiretti.
* Navigazione semplice per trovare un progetto esistente durante l&#39;avvio di una richiesta di traduzione.
* È stato introdotto un meccanismo di traduzione multilingue per evitare la creazione di più progetti per ogni lingua quando la richiesta di traduzione viene avviata per più lingue.
* È stata introdotta una configurazione per nascondere la scheda di traduzione nel dashboard della mappa. Per impostazione predefinita è visibile. È possibile scegliere di tradurre il contenuto utilizzando il dashboard mappa o l’Editor Web.

![Dashboard di traduzione](assets/translation-from-web-editor.png)

### Pubblicazione migliorata

* Gli autori possono ora trasmettere metadati a livello di mappa e argomento alla pubblicazione DITA-OT. Questa funzione è utile quando i modelli PDF personalizzati sono progettati per utilizzare proprietà di metadati dei file come tag, autore, stato del documento e altro ancora.

![Metadati DITA-OT](assets/custom-meta-data-output-preset.png)

* È stata aggiunta una nuova configurazione per consentire agli utenti di conservare o eliminare le versioni degli argomenti da eliminare quando **Elimina e crea** viene utilizzata nella generazione di output del sito AEM.

### Gestione dei file migliorata

Durante l’utilizzo dei file in AEM Assets è ora possibile vedere i seguenti miglioramenti:
* È stata introdotta una nuova esperienza di caricamento dei file e una nuova finestra di dialogo per la scelta di una strategia di risoluzione dei conflitti.

![Conflitto di caricamento dei file](assets/file-upload-name-conflict.png)

* Possibilità di creare una nuova versione del file caricato con la possibilità di impedire la sovrascrittura di un file estratto.
* Ora è possibile visualizzare un&#39;anteprima delle immagini direttamente dalla vista Cronologia versioni. Inoltre, per i file DITA e non DITA, la cronologia delle versioni mostra separatamente le informazioni sulla versione corrente.

![Miniatura della cronologia delle versioni](assets/version-history-preview-image.png)

* Ogni volta che l&#39;utente crea un file DITA, il nome del file predefinito viene visualizzato in piccolo casing per essere in linea con lo scenario di creazione della cartella AEM nativa.

### Nuova funzione di esportazione dei rapporti

I rapporti sono molto utili per identificare lo stato di salute dei contenuti. [!DNL AEM Guides] In as a Cloud Service sono disponibili vari report per il controllo dei contenuti. Ora non solo puoi visualizzare i rapporti, ma anche esportare i dati del rapporto in un file CSV per visualizzarli e condividerli con il tuo team più grande. I dati dei rapporti possono darvi un&#39;occhiata rapida a qualsiasi collegamento interrotto o immagine mancante.

![Esportazione del rapporto](assets/export-report.png)

### Miglioramento dell&#39;esperienza di aggiornamento di Oxygen DAM

Quando si aggiornano i file da AEM server in Ossigeno, viene visualizzato un messaggio di avviso se nella sessione corrente di Ossigeno sono presenti file non salvati. È possibile scegliere di annullare l&#39;operazione di aggiornamento per salvare tutti i file non salvati. Senza questa funzione, gli utenti perdevano informazioni non salvate nei documenti.


### Altri miglioramenti delle funzioni

* Ora puoi creare una nuova **Progetto Dita** modello **/apps/projects/templates** percorso.
* Scarica ora il valore predefinito **ui_config.json** dai profili della cartella. Può essere utilizzato per unire le modifiche personalizzate rispetto a quelle esistenti **ui_config.json** durante l&#39;aggiornamento.
* Non è necessario cancellare la cache del browser anche quando sono presenti nuove versioni di file JS.

## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

### Editor web

* I conref appaiono di colore rosso anche quando non sono rotti. (8239)
* Il valore per l’attributo condizionale non viene compilato automaticamente se l’opzione Aggiungi tutte le proprietà è selezionata nell’editor DITAVAL. (8234)
* Gli autori non possono inserire un&#39;immagine in un argomento utilizzando un percorso relativo. (8112)
* Rivedi la pagina delle attività che non mostra i file multimediali se nel nome del file sono presenti spazi. (8111)
* I riquadri di controllo aggiunti nella cella della tabella sono visualizzati in rosso. (8083)
* I collegamenti nell’attività di revisione non vengono aggiornati quando i file in esame vengono spostati. (8080)
* L’editor Web non esegue correttamente il rendering delle immagini con proprietà di ridimensionamento impostata su 75% o superiore. (8073)
* Le immagini GIF vengono riprodotte come immagini statiche nell’editor Web. (8024)
* Un riferimento a chiave in un elemento nota non viene visualizzato nell&#39;anteprima dell&#39;editor Web o nell&#39;output. (8006)
* xref a un elemento che è di per sé un riferimento non viene risolto nell’editor. (7933)
* Il rendering del titolo con chiave non viene eseguito correttamente nell’anteprima dell’editor e nel pannello Archivio. (7909)
* I frammenti con caratteri speciali non vengono memorizzati correttamente. (7908)
* Il salvataggio di un argomento dopo la formattazione delle equazioni MathML genera un errore. (7954)
* keydef have (tm) non viene riprodotto correttamente nell&#39;editor e l&#39;output del sito AEM conteneva simboli TM duplicati. (7859)
* Il trascinamento e il rilascio di uno snippet non funzionano in base alle DTD. (7758)
* HTML ignora le dimensioni definite personalizzate per la grafica. (7718)
* l&#39;attributo conrefend non viene aggiornato quando il file di origine viene spostato. (7698)
* L’utilizzo dei documenti di tipo argomento Riferimento causa diversi problemi di interfaccia utente. (7656)
* I file DITAVAL non vengono visualizzati quando l&#39;autore aggiunge ditavalref in una mappa. (7594)
* Spazio imprevisto trovato in ogni vuoto `<entry>` quando l&#39;attributo outputclass viene aggiunto a `<tgroup>` elemento. (7532)
* Il pulsante Origine non funziona per gli argomenti aperti tramite il dashboard mappa. (7465)
* Carina stampa inserisce linee e spazi vuoti che possono essere visti quando il file viene aperto in FrameMaker o Oxygen. (7408)
* Le mappe con href=&quot;/&quot; in uno degli argomenti non vengono pubblicate sui siti AEM. (7405)
* Problemi di prestazioni rilevati nell&#39;editor quando la mappa principale ha un numero elevato di keydefs. (7400)
* Lo stato del documento per una mappa con modello personalizzato non viene ereditato dal profilo degli stati corrispondenti. (7359)
* `<tm>` è stato erroneamente rappresentato come elemento di blocco. (7286)
* I modelli duplicati vengono visualizzati nel pannello dei modelli dell’editor quando viene creato un nuovo modello. (5814)
* I modelli definiti in ui_config per le immagini per l&#39;impostazione di attributi aggiuntivi non sono applicabili per i casi di trascinamento/rilascio. (5713)
* Aspetto predefinito errato di uicontrol in menucascade. (5483)
* I modelli personalizzati per argomento/mappa non mostrano un nuovo nome nell&#39;interfaccia utente. Mostra il nome come &quot;Topic&quot;/&quot;Map&quot; invece di mostrare il nome configurato. (4958)
* Possibilità di cancellare la rootmap dalle impostazioni delle preferenze utente. (8534)
* Una raccolta di mappe appena creata non è elencata, anche dopo l’aggiornamento della pagina.(8603)
* Impossibile chiudere l&#39;argomento sbloccato. (8545)
* Se si passa dalla modalità di origine a quella di authoring, l’argomento viene contrassegnato come non più valido e il contenuto deve essere nuovamente salvato.(8524)
* Riutilizza arresti anomali del pannello dei contenuti durante la ricerca di caratteri speciali `[` o `*` .(8279)
* Il cursore non viene visualizzato nella barra di ricerca quando si apre la finestra di dialogo inserisci elemento utilizzando la scelta rapida da tastiera Alt+Invio.(7912)
* L’opzione Ricerca esegue la ricerca solo nei nomi dei file e non nel contenuto. (7784)


### Connettore dell&#39;ossigeno

* I file la cui cartella padre ha caratteri speciali danno l&#39;errore durante il caricamento in Ossigeno. (8054)
* Quando un documento appena creato viene aperto in Ossigeno, viene generato l&#39;errore &quot;Impossibile trovare GUID&quot;. (7856)
* L&#39;opzione Check-in è disabilitata dopo il check-out del file da AEM utilizzando Modifica in Ossigeno. (7471)


### Recensione

* La sincronizzazione in tempo reale non funziona per i commenti. (7661)

### Dashboard mappa

* Impossibile visualizzare il contenuto di riferimento nel titolo di un argomento nella scheda degli argomenti o dei rapporti del dashboard della mappa. (8263)
* Uscita AEM Sites | jcr:title della pagina del sito generata non viene aggiornato quando il titolo dell’argomento DITA viene aggiornato. (8131)
* Download MAP non scarica i file video utilizzati all&#39;interno degli argomenti. (8070)
* I file multimediali non vengono scaricati quando l&#39;oggetto Tag viene utilizzato tramite l&#39;API di download bookmap. (8057)
* Nella scheda Rapporti viene visualizzato un rapporto errato se un argomento ha un riferimento a un file il cui titolo inizia con conref. (4698)
* La finestra di dialogo Applica etichette nella scheda Linea di base non visualizza le etichette nel menu a discesa. (8455)

### Pubblicazione

* La creazione di PDF non riesce per la prima volta quando si seleziona Abilita controllo versioni . (8053, 8294)
* Il carattere spazio vuoto viene aggiunto automaticamente dopo un &#39;tm; nell&#39;output AEM sito. (7964)
* Impossibile visualizzare i video YouTube nell&#39;output AEM sito. (7401)
* Filtrare per etichetta non riesce per il contenuto di riferimento dopo che l&#39;utente fa clic su sfoglia tutti gli argomenti nella scheda della linea di base del dashboard della mappa. (7388)
* Pubblicazione dell’argomento con l’elemento `<tm>` il valore di proprietà SM o reg viene visualizzato in modo errato nell&#39;output generato. (7239)
* La pubblicazione della linea di base con l’immagine non esegue la selezione della versione più recente dell’immagine nell’output pubblicato. (7231)
* Gli argomenti di riferimento correlati vengono visualizzati nella scheda della linea di base. (5424)
* La pubblicazione incrementale per un argomento con conkeyref nel titolo non funziona come previsto. (4474)
* Il titolo della pagina non viene utilizzato per la generazione dell’URL di output anche se è selezionata tale impostazione. (8257)
* Pubblicazione della linea di base scegliendo la versione corrente delle immagini invece del nodo congelato. Questo si verifica anche se un’immagine ha spazio o caratteri speciali nel nome del file. (8274, 8322)
* La pubblicazione incrementale non riesce per la mappa DITA con schema oggetto di tipo con mapref. (8218)
* Viene aggiunto Null ogni volta che una mappa viene aggiunta al dashboard Pubblicazione in blocco. (8695)
* Quando si utilizza la pubblicazione della linea di base con l’immagine come rif nell’argomento, l’immagine non viene pubblicata nell’output. (8564)
* La pubblicazione non riesce con un&#39;eccezione se la linea di base utilizzata nella pubblicazione AEM sito viene eliminata. (8572)
* La rigenerazione dell&#39;argomento non funziona. (8091)
* Sono presenti problemi relativi alla pubblicazione di note a piè di pagina nelle tabelle. (4709)

### AEM Assets

* Problemi di prestazioni rilevati durante l’esecuzione della selezione/eliminazione su un set di contenuti enorme nell’interfaccia utente di Assets. (8238)
* La funzione di ricerca salvata (raccolta avanzata) si interrompe se il predicato DITA viene aggiunto ai filtri di ricerca. (8048)
* Il ripristino dell&#39;immagine alla versione precedente non funziona. (DXML-7903)
* L’opzione Elimina è visibile anche per gli autori privi dell’autorizzazione per l’eliminazione. (7322)
* La sovrapposizione CCMS per l’Editor risorse interrompe il rendering dell’opzione Elimina. (8093)
* Il profilo del documento non viene eliminato. (8604)
* I riferimenti si interrompono quando si esegue &quot;Seleziona tutto&quot; e si sposta il contenuto multimediale/Dita_Content in un&#39;altra cartella. (8621)
* Durante lo spostamento delle risorse si verificano riferimenti errati nell’origine. (8627)
* La vista a elenco fisso non viene caricata. (8542)

### Importazione contenuto

* Conversione da HTML a DITA | La tabella con &#39;tr&#39; con voci &#39;td&#39; vuote causa righe aggiuntive nell&#39;output. (8132)
* Conversione da HTML a DITA | HTML con una tabella con più corpi non riesce, con eccezione. (7940)
* Conversione da HTML a DITA | restituisce un errore se HTML di origine contiene commenti. (7937)
* L&#39;importazione di file DITA 1.3 causa la trasformazione di alcuni href in collegamenti non validi. (8019)

## Problemi noti

L&#39;Adobe ha identificato i seguenti problemi noti per [!DNL AEM Guides] Versione as a Cloud Service di gennaio 2022.


### Problemi noti con la soluzione alternativa

Utilizza la soluzione alternativa indicata per i seguenti problemi noti:

* L&#39;autenticazione Web non funziona per il connettore Oxygen su Mac.
   **Soluzione alternativa**: Usa il connettore Oxygen su Windows per il momento.

* Nel browser Firefox, i commenti di revisione non possono essere importati senza aprire la visualizzazione affiancata.
   **Soluzione alternativa**: Usa il browser Chrome per il momento.

* I riferimenti si interrompono quando si spostano le immagini o i file multimediali che hanno spazio nei nomi dei file.
   **Soluzione alternativa**: Rinominare il file e rimuovere gli spazi dal nome del file prima di spostarli.

* Il dashboard mappa non viene caricato a intermittenza nell’ultima versione del browser Chrome.
   **Soluzione alternativa**: Aggiorna la pagina del dashboard della mappa.

### Altri problemi noti

* Se l&#39;ossigeno è collegato con [!DNL AEM Guides] la soluzione che utilizza l&#39;autenticazione web, quindi l&#39;uscita non riesce.
* Impossibile riassegnare le attività di revisione agli utenti.
* I problemi sono presenti nell&#39;interfaccia utente della raccolta Mappa come se il testo fosse distorto e **Seleziona tutto** funzionalità non funzionante correttamente.
