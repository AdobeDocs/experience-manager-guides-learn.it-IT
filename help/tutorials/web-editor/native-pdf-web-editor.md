---
title: PDF nativo | Generazione di output PDF
description: Genera l’output di PDF nelle guide Adobe Experience Manager as a Cloud Service
exl-id: ec3d59b7-1dda-4fd1-848e-21d8a36ff5e4
source-git-commit: e03ef8e99b2d60dc8d34a76d0a02180eab41e35f
workflow-type: tm+mt
source-wordcount: '2663'
ht-degree: 1%

---

# Pubblicare l’output di PDF

Con AEM Guide puoi generare PDF di singoli argomenti o un intero file mappa. Puoi pubblicare il contenuto in un formato PDF utilizzando uno dei tre metodi seguenti:

* **DITA-OT**

Utilizza questo metodo per generare un output PDF per una mappa dal dashboard mappa. È possibile impostare le proprietà di pubblicazione prima di generare PDF creando un predefinito di output per la mappa aperta nel dashboard mappa. Per creare o modificare un predefinito di output, la *Informazioni sui predefiniti di output* nella sezione [Guida utente as a Cloud Service delle AEM](https://helpx.adobe.com/content/dam/help/en/xml-documentation-solution/cs-apr-22/XML-Documentation-for-Adobe-Experience-Manager_CS_User-Guide_EN.pdf).

Per ulteriori informazioni sulla generazione di un PDF utilizzando il metodo DITA-OT, vedere [Generare PDF utilizzando DITA-OT](https://help.adobe.com/en_US/xml-documentation-for-adobe-experience-manager/index.html#t=DXML-master-map%2Fgenerate-output-pdf.html).

* **FrameMaker Publishing Server (FMPS)**

Utilizzare questo metodo per generare un output PDF non solo dal contenuto DITA, ma anche dai documenti FrameMaker (.book e .fm) disponibili nel repository AEM. È possibile creare PDF configurando un predefinito di output e pubblicandolo tramite FrameMaker Publishing Server (FMPS). È possibile progettare e configurare l’aspetto dell’output per PDF e altri formati e memorizzarlo in un file di impostazione (.sts). Questo file di impostazione viene quindi utilizzato da FMPS per generare l&#39;output per una mappa DITA o un file .book. Per creare o modificare un predefinito di output, vedi  *Informazioni sui predefiniti di output* nella sezione [Guida utente as a Cloud Service delle AEM](https://helpx.adobe.com/content/dam/help/en/xml-documentation-solution/cs-apr-22/XML-Documentation-for-Adobe-Experience-Manager_CS_User-Guide_EN.pdf).

Per ulteriori informazioni sulla configurazione di FMPS, vedi [Genera output da documenti FrameMaker](https://help.adobe.com/en_US/xml-documentation-for-adobe-experience-manager/index.html#t=DXML-master-map%2Ffm-output-generatation.html).

* **Pubblicazione nativa di PDF**

Utilizza questo metodo per generare un output PDF ricco di funzioni basato sugli standard W3C CSS3 e CSS per i file multimediali. Con la pubblicazione di Native PDF, è possibile utilizzare i modelli per impostare il layout e lo stile dei contenuti e applicare varie impostazioni per perfezionare il proprio PDF. Inoltre, puoi modificare e creare modelli personalizzati con l’editor modelli.

Per ulteriori informazioni sulla pubblicazione di Native PDF, consulta [Utilizzo della pubblicazione nativa di PDF](#native-pdf-publishing).


## Utilizzo della pubblicazione Native PDF {#native-pdf-publishing}

Durante l’authoring dei contenuti, diventa essenziale garantire che i contenuti siano ottimizzati per la visualizzazione, la modifica e la stampa. Utilizzando standard quali W3C CSS3 per lo stile dei contenuti e gli standard CSS per i contenuti multimediali di pagina per le proprietà di definizione della pagina, quali dimensioni, margini, orientamento, interruzioni di pagina, intestazioni, piè di pagina e numerazione di pagina, è possibile impostare la visualizzazione e il layout del documento PDF per garantire coerenza e usabilità. La funzione di pubblicazione Native PDF utilizza questi standard per generare un PDF.

Con la pubblicazione nativa di PDF, è possibile utilizzare modelli predefiniti per garantire la coerenza del layout e della struttura del contenuto, applicare fogli di stile per modificare l’aspetto dell’output, ottimizzare PDF, impostare i segni di stampa, consentire il supporto degli assistenti vocali, impostare la conformità di PDF, incorporare font e molto altro ancora.

La generazione di un PDF utilizzando la pubblicazione di Native PDF presenta due aspetti:

* Utilizzare i modelli per applicare lo stile al contenuto, impostare i layout di pagina e varie impostazioni per ottimizzare il PDF. Gli autori possono scegliere di utilizzare/modificare i modelli di esempio forniti o creare modelli personalizzati e impostare opzioni di configurazione avanzate utilizzate da editori e sviluppatori.

* Crea o configura un predefinito di output PDF per controllare le impostazioni di PDF. Una volta creato un predefinito di output di PDF, è possibile generare PDF.

Per ulteriori informazioni, consulta [Generare un output PDF](#generate-pdf-output).

## Creare un predefinito di output PDF {#create-output-preset}

Il primo passaggio nella generazione di un output di PDF consiste nel creare un predefinito di output di PDF, ovvero una raccolta di proprietà di pubblicazione assegnate a una mappa. Puoi creare un predefinito di output per qualsiasi mappa aperta nel pannello Visualizzazione mappa o configurare un predefinito esistente per generare rapidamente un PDF per la stessa mappa.

Dal predefinito di output di PDF puoi selezionare un modello, applicare condizioni, impostare restrizioni per controllare il modo in cui un utente interagisce con il tuo PDF, configurare impostazioni avanzate come compressione, conformità e altro ancora.

Per creare o configurare un predefinito di output di PDF:

1. Nella scheda Output, fai clic su **Predefiniti** nella barra laterale sinistra.
Viene visualizzato il pannello Predefinito .

<img src="assets/preset-panel.png" alt="pannello predefinito" width="600">

1. Nell&#39;output **Predefiniti** , effettua una delle seguenti operazioni:
   * Fare doppio clic su un predefinito di output di PDF per visualizzarlo.
   * Fai clic sull’icona + contro **Predefiniti** per aggiungere un nuovo predefinito di output **Tipo: PDF**

1. Per configurare le impostazioni di un predefinito PDF esistente:
   * Fai clic sul pulsante  **Opzioni** ![options](assets/options.svg) accanto al predefinito di output desiderato e seleziona **Modifica**.
Puoi utilizzare le seguenti impostazioni nella **Generale**, **Metadati**, **Layout**, **Sicurezza** e **Avanzate** schede per configurare un predefinito di output PDF:

**Generale**

Utilizzare per specificare le impostazioni di output di base, ad esempio specificare il percorso di output, il nome del file PDF e altro ancora.

| Impostazione | Descrizione |
| --- | --- |
| **Percorso di output** | Il percorso all’interno dell’archivio AEM in cui è memorizzato l’output di PDF. Assicurati che il percorso di output non si trovi nella cartella del progetto. Se lasciato vuoto, l&#39;output viene generato nella posizione di output della mappa DITA predefinita.<br>Puoi anche utilizzare le seguenti variabili predefinite per definire il percorso di output. Puoi utilizzare una singola o una combinazione di variabili per definire questa opzione. <br> `${map_filename}`: Utilizza il nome dei file di mappa DITA per creare il percorso di destinazione. <br> `${map_title}`: Utilizza il titolo della mappa DITA per creare il percorso di destinazione. <br>`${preset_name}`: Utilizza il nome del predefinito di output per creare il percorso di destinazione. <br> `${language_code}`: Utilizza il codice della lingua in cui si trova il file di mappa per creare il percorso di destinazione. <br> `${map_parentpath}`: Utilizza il percorso completo del file mappa per creare il percorso di destinazione.  <br>`${path_after_langfolder}`: Utilizza il percorso del file di mappa dopo la cartella della lingua per creare il percorso di destinazione. |
| **File PDF** | Specificare un nome di file per salvare il PDF. Per impostazione predefinita, il nome del file PDF aggiunge il nome della mappa DITA insieme al nome del predefinito. Ad esempio, ditamap è &quot;TestMap&quot; e il nome del predefinito è &quot;preset1&quot;, il nome predefinito del pdf sarà &quot;TestMap_preset1.pdf&quot;. <br>È inoltre possibile utilizzare le seguenti variabili predefinite per definire il file PDF. Puoi utilizzare una singola o una combinazione di variabili per definire questa opzione. <br>`${map_filename}`<br>`${map_title}`<br>`${preset_name}` <br> `${language_code}`. |
| **Applica condizioni tramite** | Per il contenuto condizionale, scegli tra le seguenti opzioni per generare un output PDF in base a tali condizioni: <br>* **Nessuno applicato** Seleziona questa opzione se non desideri applicare alcuna condizione sulla mappa e sul contenuto sorgente. <br>* **File Ditaval** Selezionare un file DITAVAL per generare contenuto condizionale. Per selezionare, fare clic su Predefinito condizione e individuare il file. <br> * **Predefinito condizione** Seleziona un predefinito per condizioni dal menu a discesa per applicare una condizione durante la pubblicazione dell’output. Questa opzione è visibile se è stata aggiunta una condizione per il file di mappa DITA. Le impostazioni condizionali sono disponibili nella scheda Predefiniti condizione della console mappa DITA. Per ulteriori informazioni sul predefinito di condizione, consulta [Utilizzare i predefiniti condizione](https://help.adobe.com/en_US/xml-documentation-for-adobe-experience-manager/index.html#t=DXML-master-map%2Fgenerate-output-use-condition-presets.html). <br> |
| **Usa linea di base** | Se è stata creata una baseline per la mappa DITA selezionata, selezionare questa opzione per specificare la versione da pubblicare. Vedi [Utilizzare la linea di base](https://help.adobe.com/en_US/xml-documentation-for-adobe-experience-manager/index.html#t=DXML-master-map%2Fgenerate-output-use-baseline-for-publishing.html) per ulteriori dettagli. |
| **Crea PDF con barra di modifica tra le versioni pubblicate** | Utilizzare le seguenti opzioni per creare un PDF che mostra le differenze di contenuto tra due versioni utilizzando le barre delle modifiche:   <br>* **Linea di base della versione precedente** Scegli la versione della linea di base da confrontare con la versione corrente o con un&#39;altra linea di base. In PDF viene visualizzata una barra di modifica per indicare il contenuto modificato. Una barra di modifica è una linea verticale che identifica visivamente il contenuto nuovo o rivisto. La barra delle modifiche viene visualizzata a sinistra del contenuto inserito, modificato o eliminato. <br> **Nota**: Se si seleziona **Usa linea di base** e scegli una baseline da pubblicare, il confronto verrà effettuato tra le due versioni della baseline selezionate. Ad esempio, se scegli la versione della linea di base 1.3 in **Usa linea di base** e versione 1.1 in **Linea di base della versione precedente**, il confronto verrà effettuato tra la versione di base 1.1 e la versione di base 1.3. <br>* **Mostra testo aggiunto** Selezionare questa opzione per visualizzare il testo inserito in verde e sottolineato. Per impostazione predefinita, questa opzione è selezionata. <br> * **Mostra testo eliminato** Selezionare questa opzione per visualizzare il testo eliminato in rosso e contrassegnato con barrato. Per impostazione predefinita, questa opzione è selezionata. <br>**Nota** È inoltre possibile personalizzare lo stile della barra delle modifiche, del contenuto inserito o del contenuto eliminato utilizzando il foglio di stile.<br> |
| **Flusso di lavoro di post-generazione** | Seleziona per visualizzare un elenco a discesa contenente tutti i flussi di lavoro configurati in AEM. È possibile selezionare il flusso di lavoro da eseguire dopo il completamento del flusso di lavoro di generazione di PDF. |

**Metadati**

I metadati sono la descrizione o la definizione del contenuto. I metadati sono utili per la gestione dei contenuti e per la ricerca di file su Internet.

Utilizzare la scheda Metadati per impostare il titolo, l’autore, l’oggetto e le parole chiave per l’output di PDF. Questi metadati vengono mappati sui metadati nella scheda Descrizione all’interno delle Proprietà documento del PDF di output.

**Nota**: Questi metadati sostituiscono i metadati definiti a livello di libro.

<img src="assets/pdf-metadata.png" alt="scheda metadati" width="600">


| Impostazione | Descrizione |
|---|---|
| **Titolo** | Specificare un titolo breve e chiaro per definire il documento. |
| **Autore** | Specifica i nomi degli autori che hanno creato il documento. |
| **Oggetto** | Definire l&#39;oggetto o la raccolta con cui il documento è correlato. |
| **Parole chiave** | Utilizza le parole chiave pertinenti per migliorare l’ottimizzazione SEO (Search Engine Optimization) e aiutare gli utenti a trovare il contenuto correlato. |

**Layout**

Utilizzare per impostare i layout di pagina e specificare le opzioni di visualizzazione della pagina per l’output di PDF, ad esempio Visualizzazione pagina e impostare i livelli di zoom.

| Impostazione | Descrizione |
| --- | --- |
| **Modello PDF** | I modelli di PDF forniscono una struttura chiara per la definizione dei layout di pagina, lo stile del contenuto e l’applicazione di varie impostazioni all’output di PDF. Seleziona dall’elenco a discesa del modello di PDF per scegliere il modello preferito. |
| **Visualizzazione pagina** | Utilizzare Visualizzazione pagina per la visualizzazione di pagina che mostra come viene visualizzato il PDF quando viene aperto. Seleziona dall’elenco a discesa Visualizzazione pagina per scegliere una visualizzazione preferita. <br>* **Predefinito**  Viene visualizzata in base all’impostazione predefinita del visualizzatore PDF sul computer di un utente.  <br> * **Visualizzazione a pagina singola** Visualizza una pagina alla volta.   <br> * **Scorrimento a pagina singola** Visualizza una singola pagina in una colonna verticale continua.  <br> * **Visualizzazione a due pagine** Visualizza due pagine affiancate alla volta. .<br> * **Scorrimento di due pagine** Visualizza le pagine affiancate a due pagine con scorrimento continuo. |
| **Zoom** | Selezionare questa opzione per ridimensionare la visualizzazione della pagina che mostra la modalità di visualizzazione di PDF all’apertura.  <br>* **Predefinito** Viene visualizzato in base all’impostazione predefinita del visualizzatore PDF sul computer di un utente    <br> * **100%** Visualizza la pagina nelle sue dimensioni effettive.     <br> * **Adatta a pagina** Adatta la larghezza e l’altezza della pagina al riquadro del documento. .<br> * **Adatta a larghezza pagina** Fa corrispondere la larghezza della pagina a quella del riquadro del documento.  <br> * **Adatta altezza pagina** Fa corrispondere l’altezza della pagina all’altezza del riquadro del documento. |

**Sicurezza**

Protect in PDF aggiungendo restrizioni per aprire e leggere il file. Utilizza le opzioni seguenti per evitare accessi non autorizzati.

| Impostazione | Descrizione |
| --- | --- |
| **Imposta password per aprire il documento** | Selezionare questa opzione per aggiungere una password sicura per visualizzare il file PDF. Specifica una password nel **Password utente** campo . Gli utenti possono aprire PDF solo immettendo la password fornita in questo campo. |
| **Impostare le restrizioni relative al documento** | Selezionare questa opzione per limitare le modalità di interazione degli utenti con il PDF. Specifica una password nel **Password proprietario** per il funzionamento delle seguenti impostazioni di restrizione.  <br>* **Stampa** Selezionare questa opzione per consentire a un utente di stampare il PDF. <br> * **Stampa di qualità bozza** Selezionare questa opzione per consentire a un utente di stampare il PDF in una risoluzione inferiore.  <br> * **Copia dei contenuti** Seleziona per consentire a un utente di copiare i contenuti da PDF.   <br> * **Annotazioni** Selezionare questa opzione per consentire a un utente di aggiungere una nota o un commento in PDF.  <br> * **Modifiche al contenuto** Seleziona per consentire a un utente di modificare il contenuto in PDF.  <br> * **Copia dei contenuti per l’accessibilità** Selezionare questa opzione per consentire agli assistenti vocali di leggere e navigare nel contenuto di PDF.  <br> * **Assemblaggio documenti** Seleziona per consentire agli utenti di inserire pagine in PDF.  <br> **Nota**: Gli utenti devono immettere la password del proprietario per modificare eventuali restrizioni da File > Proprietà in Adobe Acrobat. |

**Avanzate**

Utilizza le seguenti opzioni per specificare impostazioni avanzate per unire PDF, utilizzare la compressione, selezionare standard di conformità e altro ancora.

| Impostazione | Descrizione |
| --- | --- |
| **Creare un PDF con accesso facilitato (con tag)** | Selezionare questa opzione per generare un PDF con tag. Un PDF con tag semplifica la lettura e la navigazione dei contenuti, dei collegamenti ipertestuali, dei segnalibri e così via da parte degli assistenti vocali. Ad esempio, se una tabella è contrassegnata, l’assistente vocale saprà che sta leggendo la tabella e non solo righe e testo. |
| **PDF di unione inclusi nel sommario** | Selezionare questa opzione per unire i PDF esistenti nell&#39;output aggiungendoli al sommario. I PDF vengono inseriti nella posizione rappresentata nel sommario e le pagine vengono incrementate di conseguenza. |
| **Incorpora font utilizzati** | Selezionare questa opzione quando si utilizzano font che potrebbero non essere installati nel computer dell’utente finale. Con questa opzione selezionata, i font utilizzati vengono incorporati in PDF, garantendo all’utente la possibilità di vedere PDF come previsto anche se i font non sono installati sul computer. <br> **Nota**: Un font può essere incorporato solo se contiene un&#39;impostazione del fornitore del font che ne consente l&#39;incorporazione. Verificare di disporre dell&#39;impostazione o della licenza necessaria prima di incorporare un font. |
| **Usa sillabazione automatica** | Se la sillabazione automatica è attivata, le parole alla fine delle linee vengono interrotte in punti grammaticalmente corretti con un trattino. |
| **Abilita JavaScript** | Abilita questa opzione se disponi di un codice JavaScript da utilizzare per trasformare il contenuto in modo dinamico prima di generare un PDF. |
| **Incorporare file multimediali** | Seleziona questa opzione per includere audio, video ed eventuali contenuti interattivi in PDF. |
| **Utilizzare la compressione completa per ottimizzare le dimensioni del PDF** | Selezionare questa opzione se si desidera comprimere/ridurre le dimensioni di un PDF di grandi dimensioni. Tenere presente che la compressione di PDF può ridurre la qualità del file. |
| **Utilizzare la compressione dell&#39;immagine per ottimizzare le dimensioni del PDF** | Selezionare questa opzione se si desidera comprimere/ridurre le dimensioni delle immagini utilizzate in PDF. La compressione di un&#39;immagine può ridurre la qualità dell&#39;immagine. |
| **Usa risoluzione personalizzata (pixel per pollice)** | È la risoluzione del display della pagina in pixel per pollice. Immettere un valore preferito nel campo visualizzato quando si seleziona questa opzione. Il valore predefinito è 96 pixel per pollice. Imposta un valore più alto per adattare più contenuto in pollici e viceversa, se imposti un valore più basso. |
| **Mostra filigrana** | Seleziona questa opzione per eseguire il rendering delle equazioni MathML presenti nel contenuto. In caso contrario, le equazioni verranno ignorate. |
| **Abilita equazioni MathML** | Seleziona questa opzione per eseguire il rendering delle equazioni MathML presenti nel contenuto. Le equazioni verranno ignorate altrimenti per impostazione predefinita. |
| **Conformità PDF** | Si tratta dello standard a cui si intende salvare il PDF per assicurarsi che sia conforme. Seleziona dall’elenco a discesa per scegliere tra gli standard PDF disponibili. Per ulteriori dettagli sugli standard supportati, vedi [Informazioni sugli standard PDF](https://helpx.adobe.com/acrobat/using/pdf-conversion-settings.html#about_pdf_x_pdf_e_and_pdf_a_standards). |

## Generare un output PDF {#generate-pdf-output}

Una volta configurato il predefinito di output, è possibile generare l&#39;output dal pannello Predefiniti, utilizzando **Genera predefinito** funzionalità.

1. Sotto la **Autore** seleziona la scheda **Archivio** Visualizza.\
   Viene aperto il pannello Archivio .

2. Nel pannello Repository, apri il file di mappa DITA in **Vista mappa**.

3. In **Uscita** scheda , fai clic su **Predefiniti** per visualizzare il pannello Preimpostazioni .
Per creare o configurare un predefinito di output, vedi [Creare un predefinito di output PDF](#create-output-preset).
4. Per salvare le impostazioni, fai clic sul pulsante **Salva tutto** ![salva tutto](assets/SaveFloppy_icon.svg) nell’angolo in alto a sinistra della barra degli strumenti standard nella vista Output.
5. Fai clic sul pulsante **Genera predefinito** ![genera predefinito](assets/generate-output.svg) sulla barra superiore.
Nel pannello Predefiniti di output potete visualizzare una barra di avanzamento accanto al predefinito di output selezionato.
6. Una volta completata la generazione dell&#39;output, fai clic su  **Visualizza output** ![visualizza output](assets/view-output.svg) sulla barra superiore per visualizzare l&#39;output.\
   A **Completato** nell’angolo inferiore destro dello schermo è visibile una finestra di dialogo.
Se un output non ha esito positivo, viene visualizzato il seguente messaggio di errore.
<img src="assets/error-log.png" alt="registro degli errori" width="250">

Per visualizzare il registro degli errori, fai clic su **Elimina**, passa il puntatore sulla scheda del predefinito selezionato e fai clic su ![options](assets/options.svg) **Opzioni** > **Visualizza registro**.
