---
title: Funzione di pubblicazione nativa di PDF | Personalizzare e configurare la funzione Native PDF
description: Scopri come personalizzare e configurare i vari componenti della funzione nativa di PDF.
hide: true
hidefromtoc: true
exl-id: 7660da8e-8a1e-4493-b99b-9b5de9a7483f
source-git-commit: 563a301e4db20cd8076eaffd970d53b7a8743449
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# Modello PDF {#PDF-template}

L’utilizzo di un modello garantisce la coerenza del layout e della struttura del contenuto. Poiché i modelli sono predefiniti, puoi evitare di rielaborare i problemi di formattazione che insorgono per ogni nuovo progetto o aggiornamento. I modelli consentono di progettare layout di pagina, contenuti di stile e di applicare varie impostazioni per personalizzare il PDF.

Sebbene gli autori possano utilizzare i predefiniti di PDF per generare l’output, gli sviluppatori possono creare i propri modelli. Sono disponibili modelli di esempio pronti per l’uso, che possono essere ulteriormente personalizzati o duplicati dagli sviluppatori in base ai loro requisiti organizzativi.


## Creare un nuovo modello PDF {#create-pdf-template}

È possibile creare modelli PDF personalizzati con layout di pagina specifici e definire la formattazione per i componenti di layout di pagina (come sommario, indice, glossario) o i componenti DITA (come intestazione, paragrafo, elenco) utilizzando fogli di stile. Puoi creare un nuovo modello da zero o generarlo utilizzando un modello di esempio.

Per creare un nuovo modello PDF, effettua le seguenti operazioni:
1. Nell’Editor web, passa alla pagina **Uscita** scheda .
1. Espandi la barra laterale sinistra e fai clic su **Modelli**.
<img src="assets/create-pdf-template.png" alt="Creare un modello PDF" width="400">
1. Nel pannello **Modelli**, fai clic sull’icona **+** accanto a **Modelli** e scegli **Modello PDF**.
1. Specifica un nome per il modello nella finestra di dialogo **Nuovo modello**.
1. Fai clic su **Fine**.

Il nuovo modello viene creato e aggiunto nel *Modelli* pannello.

## Duplicare un modello di PDF {#duplicate-pdf-template}

Se si desidera creare un nuovo modello con gli stessi layout di pagina e la stessa formattazione di un modello esistente, è possibile creare una copia. Una volta duplicato un modello, puoi personalizzarne ulteriormente i componenti in base alle esigenze.

Per duplicare un modello PDF esistente, effettua le seguenti operazioni:
1. Nell’Editor web, passa alla pagina **Uscita** scheda .
1. Espandi la barra laterale sinistra e fai clic su **Modelli**.

   Viene aperto il pannello Modelli .
1. Passa il puntatore del mouse sul modello da duplicare e seleziona il (*Opzioni* icona) **...** e scegli **Duplica** dal menu di scelta rapida.

   Viene visualizzata la finestra di dialogo Duplica modello (Duplicate Template).\
   <img src="assets/duplicate-template.png" alt="Duplica modello PDF" width="250">
1. Specifica un nome per il campione.

   La **Nome** viene precompilato come copia con lo stesso nome del modello di origine.

1. Per specificare un nome preferito, rimuovere il nome prepopolato e specificare un nome.
1. Fai clic su **Fine**.

   Un modello duplicato viene creato e aggiunto in Modelli.

## Personalizzare un modello di PDF {#customize-pdf-template}

È possibile personalizzare i modelli modificando i componenti del modello e applicando formati di stile utilizzando fogli di stile.

Per personalizzare un modello di PDF, effettua le seguenti operazioni:
1. Nell&#39;Editor Web passare alla scheda Output.
1. Espandi la barra laterale sinistra e fai clic su Modelli .

   Viene aperto il pannello Modelli .
1. Per visualizzare i componenti di un modello, effettua una delle seguenti operazioni:

   * Fai clic sull’icona > accanto a un modello o fai doppio clic sul nome del modello.
   * Passa il puntatore del mouse su un modello e fai clic su ... (icona Opzioni), quindi scegli Modifica dal menu di scelta rapida.

      Per impostazione predefinita, viene aperto il pannello Impostazioni nell’editor modelli.
   <img src="assets/customize-pdf-template.png" alt="Personalizza campione PDF" width="350">

   I vari componenti modello che è possibile personalizzare sono suddivisi nelle sezioni seguenti:
   * Layout di pagina: Un PDF tipico contiene pagine diverse, ad esempio una copertina anteriore o una pagina titolo, sommario, capitolo, indice e altro ancora. La sezione Layout di pagina consente di progettare l’aspetto di pagine diverse che compongono il PDF. Oltre all’aspetto, è anche possibile definire la disposizione degli elementi della pagina, come l’intestazione, il piè di pagina e le aree contenuto di una pagina. Per ulteriori informazioni sulla personalizzazione del layout di una pagina, consulta [Creare e personalizzare i layout di pagina](components-pdf-template.md#create-customize-page-layout).
   * Fogli di stile: Le impostazioni nella sezione Foglio di stile consentono di personalizzare l’aspetto dei componenti di layout della pagina come sommario, indice, glossario e altro ancora. Inoltre, è possibile personalizzare gli stili per il contenuto DITA come intestazioni, paragrafi, elenchi e altro ancora. Per ulteriori informazioni sull’utilizzo dei fogli di stile, consulta [Utilizzare fogli di stile per personalizzare PDF](components-pdf-template.md#stylesheet-customization).
   * Risorse: Archiviare i file di risorse che è necessario personalizzare o progettare modelli di PDF. Risorse quali loghi, font personalizzati, immagini di sfondo e altro ancora sono memorizzate in Risorse. Per ulteriori informazioni sull’utilizzo delle risorse, consulta [Utilizzare le risorse](components-pdf-template.md#work-with-resources).
   * Impostazioni: Configura le impostazioni di output per generare un PDF utilizzando il modello . Questa sezione ti consente di definire la mappatura dei modelli per diverse pagine in PDF, la pagina iniziale dei capitoli, i marcatori di stampa e altro ancora. Per ulteriori informazioni sull’applicazione delle impostazioni, consulta [Impostazioni avanzate di PDF](components-pdf-template.md#advanced-pdf-settings).
1. Per personalizzare un componente modello, fai doppio clic su un componente modello oppure fai clic sull’icona > prima di esso.

   Ad esempio, fai doppio clic su *Layout di pagina* o fai clic su *>* icona prima *Layout di pagina* per visualizzare i layout di pagina disponibili.
1. Dopo aver apportato le modifiche desiderate, fai clic su *Salva tutto* o `Ctrl+S`).
