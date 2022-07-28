---
title: Funzione di pubblicazione nativa di PDF | Progettazione di un layout di pagina
description: 'Scopri come progettare il layout di pagina per presentare informazioni in diverse sezioni dell’output di PDF. '
hide: true
hidefromtoc: true
source-git-commit: 77256556d9222ffd096a599e5875c94108ebb8ed
workflow-type: tm+mt
source-wordcount: '3300'
ht-degree: 0%

---

# Progettazione di un layout di pagina

Quando si crea un documento PDF, sono disponibili sezioni diverse per presentare diversi tipi di informazioni. Ad esempio, un documento PDF parte da una pagina iniziale o di copertina, contenente il logo, il titolo del libro o le informazioni sulla versione della tua azienda. Ci sarebbero poi capitoli, appendici o pagine del glossario. Ogni sezione di un documento PDF ha un aspetto diverso e questo si ottiene creando e personalizzando il layout della pagina.

Quando si progetta un layout di pagina, è possibile definire i vari elementi che compongono una pagina. Ad esempio, è possibile definire le dimensioni della pagina, i margini, l’intestazione e il piè di pagina, l’orientamento e altre specifiche di pagina in una pagina. La funzione Pubblicazione nativa di PDF ti consente di progettare la pagina in base agli standard CSS Paged Media. La maggior parte delle impostazioni coperte dal supporto di pagina CSS può essere facilmente personalizzata utilizzando l’interfaccia utente della funzione di PDF nativa. Per altre formattazioni avanzate, puoi utilizzare la vista Origine per scrivere il tuo codice CSS.

Una volta progettati i layout di pagina, è necessario associare questi layout alle rispettive sezioni nelle impostazioni di layout di pagina di PDF. Consulta la sezione _Creare e personalizzare i layout di pagina_ per informazioni dettagliate su come creare e aprire un layout di pagina per la personalizzazione.

## Tipi di layout di pagina e relative varianti

Un documento PDF contiene in genere le sezioni seguenti:

* Pagina copertina
* Sommario
* Incremento delle cifre
* Incremento delle tabelle
* Pagine dei capitoli o degli argomenti
* Glossario
* Indice
* Pagina posteriore

Per presentare le informazioni in un formato specifico, è necessario disporre di un layout di pagina corrispondente. Inoltre, è possibile disporre di una pagina vuota utilizzata come compilatore per iniziare un nuovo capitolo da una pagina dispari o pari. In tal caso, è necessario un layout di pagina vuoto.

Le impostazioni Layout di pagina nella sezione **Modello > Impostazioni** consente di definire quale modello deve essere utilizzato per diverse sezioni del PDF. Ogni layout di pagina può inoltre presentare diverse combinazioni di pagina prima, destra o sinistra. Sono disciplinate dalle regole definite nel *File multimediali pagina CSS* standard.

## Creare il primo layout di pagina, a destra o a sinistra

I diversi layout di pagina nel modello di PDF possono essere ulteriormente personalizzati utilizzando diversi layout di pagina iniziale, destra o sinistra. È possibile progettare queste pagine in modo diverso utilizzando Progettazione layout pagina.

> **Nota**: Se si desidera avere un layout di pagina singolo per una sezione del libro, non è necessario creare il layout di pagina Primo, Destro o Sinistro.

Quando crei i layout di pagina, considera quanto segue:

* Se si desidera utilizzare un layout di pagina singolo per tutte le pagine di un capitolo, è necessario creare un solo layout di pagina Capitolo.
* Se vuoi avere un aspetto diverso per la prima pagina dei capitoli del libro, devi creare un layout di prima pagina per i capitoli.
* Se vuoi avere un aspetto diverso per ogni pagina a sinistra e a destra del tuo libro, allora devi creare le varianti a sinistra e a destra per il layout della pagina dei capitoli.
* Se desideri che i capitoli inizino da una pagina dispari o pari, dovrai creare un layout di pagina vuoto. Questo layout di pagina viene utilizzato per colmare il gap tra due capitoli in modo che il capitolo inizi dalla pagina dispari o pari desiderata.

L’esempio seguente illustra il processo di creazione delle varianti di un layout di pagina:

1. Creare un layout di pagina &quot;Capitolo&quot; utilizzando i passaggi descritti in *Creare un nuovo layout di pagina* procedura.

   Viene creato e aggiunto un layout vuoto della pagina Capitolo in Layout di pagina.

   Per impostazione predefinita, quando si crea un layout di pagina, questo viene aperto anche per la modifica. La schermata seguente mostra un layout di pagina vuoto (predefinito):

   <img src="./assets/default-blank-page-layout.png" height="400">

   L’intestazione, il piè di pagina e l’area contenuto di un modello vengono creati per impostazione predefinita. Puoi personalizzare facilmente queste aree utilizzando gli strumenti, le proprietà della pagina e le proprietà del contenuto forniti nell’interfaccia utente. Per la configurazione avanzata, puoi utilizzare la vista Origine e aggiungere codice HTML e CSS personalizzati.

1. Per creare una variante per il layout della pagina Capitolo:

   1. Passa il puntatore del mouse sopra **Capitolo** layout e fai clic su **Opzioni** per visualizzare il menu di scelta rapida.

   1. Passa il puntatore del mouse sopra **Aggiungi variante layout** e scegli il layout di pagina desiderato (Primo, Sinistra o Destra) da creare.

   Il layout di pagina selezionato viene creato utilizzando una copia del layout Capitolo di base. Ciò significa che se sono state apportate modifiche al layout predefinito della pagina Capitolo, le stesse modifiche vengono replicate nel layout della pagina variante.

## Operazioni con le immagini in un layout di pagina

In base alle tue esigenze, puoi aggiungere un’immagine che viene visualizzata su ogni prima pagina di un output di capitolo (PDF). La <u>**Aggiungi immagine**</u> Lo strumento nell’editor del layout di pagina viene utilizzato per inserire le immagini in un layout di pagina.

Ad esempio, se si desidera inserire un&#39;immagine nell&#39;area di intestazione della prima pagina dell&#39;output del capitolo, eseguire le operazioni seguenti:

1. Apri il layout di pagina necessario per la modifica.

   > **Nota**: Vedi _Personalizzare un layout di pagina_ per aprire un layout di pagina da personalizzare o modificare.

1. Fai clic su Modifica intestazione (<img src="./assets/header-icon.svg" width="25">) per spostare il cursore nell’area di intestazione.

1. Fai clic su Inserisci immagine (<img src="./assets/insert-image-icon.svg" width="25"> ) icon.

   Viene visualizzata la finestra a comparsa Seleziona percorso .

1. Individuare il percorso dell&#39;immagine e fare clic su Seleziona per inserirlo nell&#39;area di intestazione.

   La schermata seguente mostra un esempio di immagine aggiunta nell’area di intestazione.

   <img src="./assets/image-in-header-area.png" width="500">

   Una volta inserita un’immagine, puoi modificarne gli attributi per ottenere l’aspetto desiderato. Per modificare l’aspetto di un’immagine o di qualsiasi altro elemento nel layout di pagina in modo semplice, utilizza il pannello Proprietà contenuto . Vedi _Utilizzare il pannello Proprietà contenuto_ per le varie proprietà che sono disponibili tramite l’interfaccia utente per personalizzare.

## Utilizzare i campi

I campi sono molto utili quando si desidera inserire informazioni predefinite. Ad esempio, è possibile includere un campo Titolo capitolo nell’area di intestazione del capitolo che viene sostituito con il titolo del capitolo effettivo quando viene pubblicato.

Sono disponibili le seguenti categorie di campi che è possibile inserire nel layout di pagina:

* Data
* stimato
* Titolo argomento
* Titolo progetto
* Numero pagina
* Pagina totale
* Titolo capitolo
* Numero del capitolo
* Metadati

Ciascuna di queste categorie di campi contiene diverse varianti in cui è possibile inserire le informazioni sul campo. Ad esempio, un campo Data può presentare varianti diverse, ad esempio `YYYY-MM-DD`, `MM/DD/YY`, `MM/DD/YYYY` e così via.

Nell’esempio seguente, verranno inseriti un numero di pagina e un titolo di argomento nell’area del piè di pagina del layout di pagina.

1. Apri il layout di pagina necessario per la modifica.

   Nota: Vedi _Personalizzare un layout di pagina_ per aprire un layout di pagina da personalizzare o modificare.

1. Fai clic su Modifica piè di pagina (![](./assets/footer-icon.svg)) per spostare il cursore nell’area piè di pagina.

1. Inserire un elemento paragrafo facendo clic su Inserisci elementi di HTML <img src="./assets/insert-html-element-2.svg" width="25"> e selezionare Paragrafo dall’elenco degli elementi.

1. Fai clic su Inserisci campi ( ![](./assets/insert-fields-icon.svg)).

   Viene visualizzata la finestra a comparsa Campi.

1. Seleziona la **Numero pagina** dall&#39;elenco Campo, la **default(1)** formato del numero di pagina dall&#39;elenco Formato e fare clic su **Inserisci**.

   <img src="./assets/insert-page-number-field.svg" width="400">

   > **Nota**: È inoltre possibile modificare il formato di tutti i campi, ad eccezione del formato predefinito. A tale scopo, fare clic sull&#39;icona Modifica accanto al formato da modificare, apportare modifiche e fare clic su OK.

   Il campo numero pagina predefinito viene inserito nell’area piè di pagina del layout di pagina.

   <img src="./assets/page-number-field-in-footer.png" width="400">

   La breadcrumb superiore elenca gli elementi in cui vengono memorizzate le informazioni.

1. Immettere uno spazio vuoto dopo il campo del numero di pagina e fare clic sul pulsante **Inserisci campi** icona.

1. Seleziona la **Titolo argomento** dall&#39;elenco Campo, la **Capitolo.ptl** formato titolo dall&#39;elenco Formato e fare clic su Inserisci.

   La `Chapter.ptl` Il campo , che viene compilato con il titolo dell’argomento al momento della pubblicazione, viene inserito nell’area piè di pagina. Al momento, i campi numero pagina e titolo argomento sono separati da uno spazio.

   <img src="./assets/page-number-topic-title-near-footer.png" width="400">

1. Per allineare a destra il titolo dell&#39;argomento, esegui le seguenti operazioni:

   1. Fai clic sull’elemento Campo nella breadcrumb per selezionare il campo del titolo dell’argomento.

   1. Nel pannello di destra, fai clic su Proprietà contenuto HTML.

      <img src="./assets/right-pane-content-properties.png" width="350">

   1. Espandi la **Layout** e imposta la sezione delle proprietà **Mobile** valore della proprietà su **right**.

      <img src="./assets/float-prop-html-content.png" width="350">

      Il campo titolo dell’argomento è allineato verso il lato destro del piè di pagina della pagina.

      <img src="./assets/topic-title-moved-right-footer.png" width="500">

> **Angolo sviluppatore:**  ![](./assets/developer-corner-icon.svg)

Se desideri lavorare direttamente con il codice CSS e HTML, puoi farlo anche passando alla vista Origine del layout di pagina e apportando modifiche al codice. Lo snippet di codice seguente mostra la stessa impostazione a piè di pagina eseguita attraverso il codice:

```md
…
<div data-region="footer">
	<p>
		<span data-field="page-number" data-format="default">1</span>
		<span data-field="title" data-format="default" style="float: right">Chapter.plt</span>
	</p>
</div>
…
```

## Aggiungi un sommario capitolo

Un capitolo o un mini sommario funge da riferimento rapido per consentire ai lettori di sapere cosa c&#39;è nel capitolo. In genere, un sommario di capitolo viene aggiunto all&#39;inizio di un capitolo. Quindi, se si desidera utilizzare un sommario di capitolo, è possibile aggiungerlo al layout della pagina del capitolo principale o al layout della prima pagina di un capitolo.

Nell’esempio seguente verrà inserito un sommario di capitolo nel layout Prima pagina di un capitolo:

1. Apri il layout di pagina necessario per la modifica.

   Nota: Vedi _Personalizzare un layout di pagina_ per aprire un layout di pagina da personalizzare o modificare.

1. Posizionare il cursore nell’area contenuto del layout di pagina.
1. Fai clic sul sommario capitolo (<img src="./assets/chapter-toc-icon.svg">) icon.

   Il capitolo TOC predefinito viene inserito nell’area contenuto.

   <img src="./assets/chapter-toc-default.png" width="400">

   > **Nota**: Il capitolo predefinito TOC contiene le intestazioni da 1 a 4. In questo caso, Titolo 1 è il Titolo del Capitolo stesso. Pertanto, potrebbe non essere necessario riavere il titolo del capitolo nel sommario o aumentare il livello dei titoli desiderati nel sommario. Puoi personalizzare il sommario modificando le proprietà.

1. Apri il pannello Proprietà contenuto di HTML per personalizzare i livelli di intestazione del sommario.

   Ad esempio, se si desidera iniziare da Titolo 2, modificare il primo elenco a discesa in modo che inizi da 2.

   <img src="./assets/customize-chapter-toc.png" width="400">

   Allo stesso modo, se si desidera impostare i titoli fino al livello 5, modificare il secondo elenco a discesa in 5. Il sommario aggiornato verrà visualizzato come mostrato di seguito:

   <img src="./assets/chapter-toc-updated.png" width="400">

   > **Nota**: Nella versione finale di PDF verranno visualizzate solo le voci del sommario in base al contenuto dei capitoli. Se in un capitolo non sono presenti titoli di livello 5, questo non verrà visualizzato nell&#39;output finale.

## Utilizzo del layout di pagina a più colonne

I layout di pagina a più colonne sono molto comuni nella pubblicazione di riviste o indici in un libro. La funzione di pubblicazione nativa di PDF consente di dividere facilmente il documento in più colonne. Utilizzando layout di pagina diversi, è possibile scegliere di mantenere solo una sezione specifica divisa in più colonne mantenendo le altre sezioni in un layout a colonna singola (o normale).

Per creare un layout di pagina con più colonne, effettua le seguenti operazioni:

1. Apri il layout di pagina necessario per la modifica.

   > **Nota**: Vedi _Personalizzare un layout di pagina_ per aprire un layout di pagina da personalizzare o modificare.

1. Poiché il layout a più colonne viene applicato al contenuto, escludendo l’area intestazione e piè di pagina, è necessario selezionare l’elemento contenuto nella breadcrumb.

   Una volta selezionata la breadcrumb del contenuto, il pannello Proprietà contenuto di HTML mostrerà le proprietà per Colonne multiple.

   <img src="./assets/multiple-columns-properties.png" width="400">

1. Utilizza le proprietà a più colonne per personalizzare il layout di pagina a più colonne:

   * **Conteggio colonne:** Specifica il numero di colonne da dividere la pagina. Utilizzare le icone freccia su e giù oppure immettere un numero per impostare il numero di colonne.

   * **Larghezza colonna:** Specifica la larghezza di una colonna in un layout a più colonne. Per impostazione predefinita, la dimensione è impostata in pixel (px), è inoltre possibile specificarla in pt, rem, em, % o in unità.

      >**Nota:** Se non si specifica una dimensione, le colonne vengono ridimensionate automaticamente per adattarsi ai margini di pagina specificati.

   * **Gap tra colonne** : Specifica lo spazio tra le singole colonne.

   * **Estensione colonna** : Se desideri che un elemento nel layout di pagina si estenda su più colonne, devi utilizzare questa proprietà. Questo si ottiene modificando lo stile dell’elemento desiderato utilizzando i fogli di stile, per ulteriori informazioni vedi _\&lt;section explaining=&quot;&quot; style=&quot;&quot; customization=&quot;&quot;>_.

   Nel layout di pagina, se si desidera che un determinato testo venga visualizzato nella prima pagina di tutti i layout di pagina dei capitoli, è possibile aggiungerlo alla variante Prima pagina del layout di pagina Capitolo.

   Come mostrato nell’esempio seguente, la proprietà Colonna a 360 gradi per il testo dell’intestazione è impostata su tutte. In questo modo, anche se il documento è a più colonne, l’intestazione si estende su più colonne.

   <img src="./assets/element-span-across-columns.png" width="400">

   >[**IMPORTANTE**]
   È possibile applicare la proprietà Span Column a qualsiasi elemento DITA.

   * **Riempimento a colonne** : Specifica come il contenuto riempie le colonne. Per impostazione predefinita, è impostato su Saldo che riempie ogni colonna con la stessa quantità di contenuto.

   * **Regola colonna** : Se si desidera inserire una riga tra le colonne, utilizzare questa proprietà per definire gli stili di linea o di regola. Specificare i valori per Stile, Colore e Larghezza regola per aggiungere una linea tra le colonne.


## Usa proprietà pagina per diversi orientamenti di pagina**

Durante la progettazione di un layout di pagina, è essenziale avere il controllo su varie proprietà di pagina. La funzione PDF nativa racchiude tutte le proprietà principali della pagina nel pannello Proprietà pagina. Il pannello Proprietà pagina consente di accedere a varie proprietà nelle sezioni seguenti:

* **Dimensioni pagina**: Specifica le dimensioni della pagina da utilizzare per il layout di pagina. L’elenco a discesa Dimensione pagina consente di scegliere tra più di 15 dimensioni di pagina.

* **Orientamento**: Specifica l’orientamento della pagina da utilizzare per il layout di pagina. È possibile scegliere tra l’orientamento della pagina Verticale o Orizzontale. È possibile scegliere di applicare orientamenti diversi a varianti di pagina diverse in un layout di pagina. Ad esempio, è possibile impostare l’orientamento Verticale nei layout di pagina Prima pagina e Orizzontale nei layout di pagina Sinistra e Destra.

* **Rotazione vista**: Specifica la visualizzazione o la direzione in cui viene disposto il contenuto della pagina. È possibile scegliere tra 90 in senso orario, 90 in senso antiorario o 180 gradi in senso antiorario. Questo è molto utile in una situazione in cui si desidera utilizzare una combinazione di layout Verticale e Orizzontale nell&#39;output. Ad esempio, è possibile utilizzare il formato verticale come layout di pagina generico e impostare il layout orizzontale della pagina per l’acquisizione di tabelle lunghe. In questa situazione, puoi scegliere di visualizzare il contenuto della tabella in senso orario di 90 gradi. In questo modo la pagina verrà orientata in orizzontale e il contenuto verrà ruotato di 90 gradi per mantenere la continuità della visualizzazione. Vedremo come questo si ottiene come esempio più avanti in questa sezione.

* **Riavvia numerazione da**: Specificare il numero di pagina da cui partirà la numerazione per il layout di pagina. Ad esempio, è possibile creare un layout di pagina per la sezione Appendice del libro e impostare la numerazione da riavviare da 1.

* **Layout**: Specifica i margini della pagina e la spaziatura per i lati superiore, inferiore, sinistro e destro.

* **Sfondo**: Includi un’immagine come immagine di sfondo nel layout della pagina. È possibile specificare l’altezza e la larghezza dell’immagine, insieme alle proprietà di ripetizione e posizione.

* **Nota**: Specifica le proprietà per visualizzare le note a piè di pagina nell’output. È possibile scegliere di specificare i margini e le proprietà di spaziatura insieme a uno stile di bordo.

Vediamo un esempio in cui viene utilizzata una combinazione di orientamento della pagina verticale e orizzontale e di proprietà di rotazione della vista. In questo esempio verrà creato un PDF con orientamento verticale predefinito, ma verrà eseguito il rendering di una tabella con orientamento orizzontale con contenuto nella visualizzazione a 90 gradi in senso orario. L&#39;output finale avrà un aspetto simile a:

<img src="./assets/portrait-landscape-page-layouts.png" height="800">

Nell’output precedente, le informazioni dell’elenco contatti vengono presentate in modalità orizzontale con contenuto ruotato anche di 90 gradi. Il contenuto rimanente viene visualizzato nella modalità normale verticale.

Per ottenere questo tipo di output, è necessario eseguire le seguenti attività principali:

1. Crea un layout di pagina con orientamento Orizzontale.
1. Modifica la proprietà Visualizza rotazione per eseguire il rendering del contenuto in senso orario a 90 gradi.
1. Creare uno stile personalizzato per utilizzare il nuovo layout di pagina.
1. Aggiungi lo stile nella definizione di output della tabella da eseguire nel layout della pagina con orientamento orizzontale.

Esegui i seguenti passaggi per eseguire le attività di cui sopra:

1. Crea un layout di pagina con orientamento Orizzontale.
   1. Creare un layout di pagina &quot;Orizzontale&quot; utilizzando i passaggi descritti nella procedura &quot;Creare un nuovo layout di pagina&quot;.

   1. Nel pannello di destra, fai clic su **Proprietà pagina**.

      <img src="./assets/page-properties-panel.png" width="300">
   1. Modificare la **Orientamento** a **Orizzontale**.

1. Modifica la proprietà Visualizza rotazione per eseguire il rendering del contenuto in senso orario a 90 gradi.

   1. Seleziona **90° in senso orario** dall’elenco a discesa Rotazione vista .

   1. Fai clic su **Salva tutto** per salvare le proprietà di layout di pagina aggiornate.

1. Creare uno stile personalizzato per utilizzare il nuovo layout di pagina.
   1. Espandi la barra laterale sinistra e fai doppio clic sul modello in cui desideri creare lo stile.

   1. Espandi la sezione Foglio di stile.

   1. Passa il puntatore del mouse sul foglio di stile Layout e fai clic su (_Opzioni_ icona) **...** e scegli **Modifica**.

      Il foglio di stile Layout viene aperto per la modifica.

   1. Fai clic con il pulsante destro del mouse **Altri stili** e scegli **Nuovo stile**.

      <img src="./assets/stylesheet-other-new-style.png" width="300">

   1. In **Aggiungi stile** popup, immettere `landscape-style` in **Classe** campo nome.

      <img src="./assets/stylesheet-new-landscape-style.png" width="400">

   1. Fai clic su **Fine**.

      Nuovo stile denominato `.landscape-style` viene creato e aggiunto alla fine di **Altri stili** elenco.

   1. Fai doppio clic sul pulsante `.landscape-style` per aprirlo in modalità di modifica.

   1. Espandi la **Impaginazione** proprietà.

   1. Invio `Landscape` in **Layout pagina** proprietà.

      <img src="./assets/new-style-with-landscape-layout.png" width="500">

1. Aggiungi lo stile nella definizione di output della tabella da eseguire nel layout della pagina con orientamento orizzontale.

   1. Nell&#39;Editor Web aprire il file in cui si desidera applicare il nuovo layout di pagina.

   1. Trova il `<table>` che deve essere riprodotto in modalità Orizzontale.

   1. Nel breadcrumb, fai clic sul pulsante `table` per selezionare la tabella.

      <img src="./assets/new-style-table-element.png" width="400">

   1. Nel pannello di destra, fai clic su e apri le **Proprietà contenuto** pannello.

   1. In **Proprietà contenuto** , aggiungi un nuovo `outputclass` proprietà con `landscape-style` come valore di proprietà.

      <img src="./assets/new-style-table-outputclass.png" height="400">

   1. Fai clic su **Salva tutto** per salvare il file aggiornato.

   1. Genera l’output di PDF.

Il contenuto della tabella finale verrà riprodotto in modalità orizzontale, come illustrato all’inizio dell’esempio.

## Utilizzare il pannello Proprietà contenuto

Il pannello Proprietà contenuto consente di aggiornare facilmente l’aspetto degli elementi nel layout di pagina. Le proprietà nel pannello Proprietà contenuto sono suddivise nelle sezioni seguenti:

>**Nota**: Per ulteriori dettagli sull&#39;utilizzo di queste proprietà, consulta la documentazione W3C CSS Page Media Standards .

* **Attributi**: Contiene le proprietà ID, Classe e Traduci. Se imposti la proprietà Traduci su no, il contenuto di tale elemento specifico non viene tradotto.

* **Font**: Contiene proprietà relative al font. È possibile impostare Famiglia font, Peso, Dimensioni, Decorazione testo (come sottolineato, sovrapposto, linea-through), Stile testo (come grassetto, corsivo e altro ancora), Allineamento testo (come sinistra, destra, centro o giustificato), gestione spazi bianchi (come formato predefinito, no-wrapping, break-space e altro), Altezza linea, Spaziatura lettere e rientro testo.

* **Bordo**: Contiene le proprietà per aggiungere e formattare un bordo a un elemento nel layout di pagina. È possibile impostare Bordo laterale (come tutti, superiore, inferiore, destro o sinistro), Stile bordo (come linea piena, tratteggiata, punteggiata o più), Colore bordo, Larghezza e Raggio per avere bordo curvo. Nell’esempio seguente, è stato aggiunto un bordo curvo nell’area di intestazione della pagina.

   <img src="./assets/border-properties.png" width="500">

* **Layout**: Contiene le proprietà per configurare il layout di un elemento nel layout di pagina. È possibile impostare Altezza, Larghezza, Margini e Spaziatura (per superiore, inferiore, sinistra o destra), Allineamento orizzontale o verticale, Mobile (come sinistro, destro o nessuno), Cancella (come sinistro, destro, entrambi o nessuno), Posizione dell’elemento (come assoluta, fissa, relativa o più), Visualizza (come blocco, contenuto, correzione o più), Indice Z, Trasparenza, Trasformazione (ruotando o ridimensionando) e Origine del modulo (per offset X e Y).

* **Sfondo**: Contiene le proprietà per includere un’immagine di sfondo o un’ombreggiatura colore. È possibile impostare le dimensioni dell&#39;immagine (impostando Altezza o Larghezza), Ripeti sfondo (come ripetizione, non ripetizione, arrotondata o più) e Posizione sfondo (come superiore sinistro, centro destro, centro centrale o più).

* **Colonne multiple**: Contiene le proprietà per configurare le proprietà a più colonne per la pagina o per qualsiasi elemento specifico, ad esempio sommario capitolo. Per ulteriori dettagli sulle proprietà e su come utilizzarle, consulta _Utilizzo del layout di pagina a più colonne_.

