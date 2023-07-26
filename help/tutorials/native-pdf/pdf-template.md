---
title: Creazione e personalizzazione di modelli di PDF nativi
description: Scopri come creare e personalizzare modelli Native PDF.
exl-id: 7660da8e-8a1e-4493-b99b-9b5de9a7483f
source-git-commit: 49fa930483f48cafd057002ee26c9499ce967c60
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 0%

---

# Modello PDF {#PDF-template}

L’utilizzo di un modello garantisce coerenza nel layout e nella struttura del contenuto. Poiché i modelli sono predefiniti, è possibile evitare la rielaborazione dei problemi di formattazione che si verificano per ogni nuovo progetto o aggiornamento. I modelli consentono di progettare layout di pagina, applicare stili al contenuto e applicare varie impostazioni per personalizzare il PDF.

Anche se gli autori possono utilizzare i predefiniti di PDF per generare l’output, gli sviluppatori possono creare modelli personalizzati. Sono disponibili modelli di esempio forniti con il prodotto, che possono essere ulteriormente personalizzati o duplicati dagli sviluppatori in base ai loro requisiti organizzativi.


## Crea un nuovo modello di PDF {#create-pdf-template}

È possibile creare modelli di PDF personalizzati con layout di pagina specifici e definire la formattazione per i componenti layout di pagina (come sommario, indice, glossario) o per i componenti DITA (come intestazione, paragrafo, elenco) utilizzando i fogli di stile. Puoi creare un nuovo modello da zero o generarlo utilizzando un modello di esempio.

Per creare un nuovo modello di PDF, effettua le seguenti operazioni:
1. Nell’editor web, vai al **Output** scheda.
1. Espandi la barra laterale a sinistra e seleziona **Modelli**.
<img src="assets/create-pdf-template.png" alt="Crea modello PDF" width="400">
1. Nel pannello **Modelli**, seleziona l’icona **+** accanto a **Modelli** quindi scegli **Modello PDF**.
1. Specifica un nome per il modello nella finestra di dialogo **Nuovo modello**.
1. Fai clic su **Fine**.

Il nuovo modello viene creato e aggiunto nel *Modelli* pannello.

## Duplicare un modello PDF {#duplicate-pdf-template}

Se si desidera creare un nuovo modello con gli stessi layout di pagina e la stessa formattazione di un modello esistente, è possibile crearne una copia. Una volta duplicato un modello, puoi personalizzarne ulteriormente i componenti in base alle esigenze.

Per duplicare un modello di PDF esistente, effettua le seguenti operazioni:
1. Nell’editor web, vai al **Output** scheda.
1. Espandi la barra laterale a sinistra e seleziona **Modelli**.

   Viene aperto il pannello Modelli.
1. Passa il puntatore del mouse sul modello da duplicare e seleziona l’opzione (*Opzioni* ) **...** e scegli **Duplica** dal menu di scelta rapida.

   Viene visualizzata la finestra di dialogo Duplica modello.\
   <img src="assets/duplicate-template.png" alt="Duplica modello PDF" width="250">
1. Specificare un nome per il team.

   Il **Nome** viene precompilato come copia con lo stesso nome del modello di origine.

1. Per specificare un nome preferito, rimuovi il nome precompilato e specifica un nome.
1. Clic **Fine**.

   Un modello duplicato viene creato e aggiunto in Modelli.

## Personalizzare un modello di PDF {#customize-pdf-template}

È possibile personalizzare i modelli modificando i componenti del modello e applicando formati di stile utilizzando i fogli di stile.

Per personalizzare un modello di PDF, attieniti alla procedura seguente:
1. Nell’editor web, passa alla scheda Output.
1. Espandi la barra laterale a sinistra e seleziona Modelli.

   Viene aperto il pannello Modelli.
1. Per visualizzare i componenti di un modello, effettuate una delle seguenti operazioni:

   * Seleziona l’icona > accanto a un modello o fai doppio clic sul nome del modello.
   * Passa il puntatore del mouse su un modello, seleziona l’icona ... (Opzioni) e scegli Modifica dal menu di scelta rapida.

     Per impostazione predefinita, questo apre il pannello Impostazioni nell’editor modelli.
   <img src="assets/customize-pdf-template.png" alt="Personalizza team PDF" width="350">

   >[!NOTE]
   >
   >  L’amministratore può scaricare i modelli più recenti dal percorso seguente e sostituire quelli esistenti:
   >
   > `/libs/fmdita/pdf`

   I vari componenti modello che è possibile personalizzare sono suddivisi in categorie nelle sezioni seguenti:
   * Layout di pagina: un tipico PDF contiene pagine diverse, ad esempio una copertina o una pagina del titolo, un sommario, un capitolo, un indice, delle citazioni e altro ancora. La sezione Layout di pagina consente di progettare l’aspetto di pagine diverse che costituirebbero il PDF. Per ulteriori dettagli, vedi [Layout di pagina](../native-pdf/components-pdf-template.md#page-layouts).

     Oltre all&#39;aspetto, è possibile definire la disposizione degli elementi della pagina, ad esempio l&#39;intestazione, il piè di pagina e le aree contenuto di una pagina. Per ulteriori informazioni sulla personalizzazione del layout di una pagina, consulta [Creare e personalizzare layout di pagina](components-pdf-template.md#create-customize-page-layout).

   * Fogli di stile: le impostazioni nella sezione Fogli di stile consentono di personalizzare l’aspetto dei componenti di layout di pagina come il sommario, l’indice, il glossario, le citazioni e altro ancora. È inoltre possibile personalizzare gli stili per il contenuto DITA, ad esempio intestazioni, paragrafi, elenchi e altro ancora. Per ulteriori informazioni sull&#39;utilizzo dei fogli di stile, vedere [Utilizzare i fogli di stile per personalizzare PDF](components-pdf-template.md#stylesheet-customization).
   * Risorse: archivia i file di risorse necessari per personalizzare o progettare modelli di PDF. Le risorse come loghi, font personalizzati, immagini di sfondo e altro ancora sono memorizzate nelle Risorse. Per ulteriori informazioni sull’utilizzo delle risorse, consulta [Utilizzare le risorse](components-pdf-template.md#work-with-resources).
   * Impostazioni: configura le impostazioni di output per la generazione di un PDF utilizzando il modello. Questa sezione ti consente di definire la mappatura dei modelli per varie pagine di un PDF, pagina iniziale del capitolo, marcatori di stampa, citazioni e altro ancora.
Puoi anche impostare l’ordine in cui devono essere visualizzate nell’output PDF finale.
Per ulteriori informazioni sull&#39;applicazione delle impostazioni, vedere [Impostazioni avanzate di PDF](components-pdf-template.md#advanced-pdf-settings).


1. Per personalizzare un componente modello, fai doppio clic su un componente modello o seleziona l’icona > prima di esso.

   Ad esempio, fare doppio clic su *Layout di pagina* o seleziona la *>* icona prima di *Layout di pagina* per visualizzare i layout di pagina disponibili.
1. Dopo aver apportato le modifiche desiderate, seleziona *Salva tutto* (o `Ctrl+S`).
