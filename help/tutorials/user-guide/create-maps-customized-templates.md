---
title: Creare mappe in base a modelli personalizzati
description: Scopri come creare mappe basate su modelli personalizzati
exl-id: 02513148-3876-4549-962a-9984f619030f
source-git-commit: 3bca42f0954afc2362ab24f369e698113324dbc3
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# Creare mappe in base a modelli personalizzati {#id225VF0808MP}

È possibile creare modelli di mappa personalizzati e utilizzarli per creare mappe DITA insieme ai modelli di argomento e ai modelli di mappa a cui si fa riferimento nel modello di mappa

Puoi fare riferimento ad altri modelli di mappa e modelli di argomento dal modello di mappa personalizzato. I modelli di mappa indicati possono fare riferimento a vari modelli di mappa, modelli di argomento, argomenti, mappe, immagini, video e altre risorse. Il modello di mappa personalizzato può aiutarti a replicare molto facilmente i modelli di mappa e l’intera struttura di cartelle a cui si fa riferimento. Questi modelli personalizzati sono particolarmente utili per creare e ricreare più mappe che hanno strutture e riferimenti ricorsivi.

>[!NOTE]
>
> I modelli di argomento non vengono creati ricorsivamente. Vengono generati solo i modelli di argomento che si trovano direttamente all&#39;interno del modello di mappa e qualsiasi modello di argomento all&#39;interno di un modello di argomento viene semplicemente indicato direttamente nell&#39;elemento padre.

## Creare modelli personalizzati

Le guide AEM consentono di creare mappe e argomenti personalizzati dalla cartella modelli dita. Puoi utilizzare questi modelli personalizzati per creare la mappa e l’argomento. Puoi anche condividere questi modelli con gli autori, che possono utilizzarli per creare i loro file. Utilizzando questi modelli, puoi consentire agli autori di conservare copie separate di determinate risorse all’interno della cartella dei modelli.

>[!NOTE]
>
> Tutte le risorse a cui fare riferimento e che devono essere mantenute in devono essere mantenute all’esterno della cartella dei modelli.

**Modello argomento**

Per creare un modello di argomento, effettuare le seguenti operazioni:

1. In **Interfaccia utente Assets**, passare alla cartella dita-templates.

   ![](images/dita-templates.png){width="800" align="left"}

1. Clic **argomenti** cartella per aprirla.Fare clic su **Crea \> modello DITA**.
1. Nella pagina Blueprint, seleziona **Argomento** e quindi fare clic su **Avanti.**
1. Nella pagina Proprietà specificare il modello di argomento **Titolo**.
1. Specifica il file **Nome**

   >[!NOTE]
   >
   > Il nome del file deve avere l&#39;estensione .dita.

1. \(Facoltativo\) Aggiungere una descrizione.
1. Fai clic su **Crea**. Viene visualizzato il messaggio di creazione del modello di argomento. È quindi possibile aprire il modello di argomento e modificarlo.

**Modello mappa**

Per creare un modello di mappa, effettua le seguenti operazioni:

1. In **Interfaccia utente Assets**, passare alla cartella dita-templates.
1. Clic **mappe** cartella per aprirla.
1. Clic **Crea \> Modello DITA.**

   ![](images/create-dita-template.png){width="300" align="left"}

1. Nella pagina Blueprint, seleziona **Mappa** e fai clic su **Successivo**.
1. Nella pagina Proprietà, specifica il modello di mappa **Titolo**.
1. Specifica il file **Nome**.

   >[!NOTE]
   >
   > Il nome del file deve avere l&#39;estensione .ditamap.

1. (Facoltativo\) Aggiungi una descrizione.Fai clic su **Crea**. Viene visualizzato il messaggio di creazione del modello di mappa. È quindi possibile aprire il modello di mappa e modificarlo. Puoi aggiungere i riferimenti per i modelli di argomento, i modelli di mappa e anche altre risorse nel modello di mappa.

## Trasmettere il titolo definito nei modelli

Se si desidera passare il titolo dell&#39;argomento o della mappa utilizzata all&#39;interno del modello alle mappe DITA create utilizzando tale modello, utilizzare parentesi graffe intorno al titolo.

Esempio

```XML
<pubtitle>
   <mainpubtitle outputclass="booktitle">
   {title}
   </mainpubtitle>
   <subtitle>Subtitle</subtitle>
</pubtitle>

The resultant DITA map with title "Rootmap1" will look like as follows:
<pubtitle>
   <mainpubtitle outputclass="booktitle">Rootmap1
   </mainpubtitle>
   <subtitle>Subtitle</subtitle>
</pubtitle>
```

>[!NOTE]
> Solo la prima occorrenza della parentesi graffa verrà sostituita con il titolo.

Se non si utilizzano parentesi graffe attorno al titolo, la mappa DITA risultante verrà selezionata solo per il primo elemento e la nidificazione del titolo non verrà selezionata dal modello e avrà il seguente aspetto:

```XML
<pubtitle> Rootmap1 </pubtitle>
```

>[!NOTE]
> È inoltre possibile utilizzare le parentesi graffe intorno al testo per passare la struttura nidificata dai modelli personalizzati alle mappe DITA.

Esempio

```XML
<title>    
    <sub>        
        <b>{title}</b>    
    </sub>
</title>
```

## Utilizza il modello di mappa per creare nuove mappe

>[!NOTE]
>
> Il modello di mappa deve essere configurato dall’amministratore e reso disponibile per l’authoring. Per ulteriori dettagli, consulta *Configurare i modelli di authoring* nella sezione Installare e configurare Adobe Experience Manager Guides as a Cloud Service.

Per creare una mappa utilizzando il modello di mappa personalizzato, effettua le seguenti operazioni:

1. In **Interfaccia utente Assets,** passa alla cartella in cui desideri creare la mappa.
1. Clic **Crea \> mappa DITA**.
1. Nella pagina Blueprint, seleziona il modello di mappa da utilizzare e fai clic su **Successivo**. Ad esempio, se hai creato un modello di mappa &quot;test-template&quot;, selezionalo.
1. Nella pagina Proprietà, specifica la mappa **Titolo**.
1. Specifica il file **Nome**.

   >[!NOTE]
   >
   > Il nome del file deve avere l&#39;estensione .ditamap.

1. Fai clic su **Crea**. Viene visualizzato il messaggio Mappa creata.


La mappa genera tutte le risorse a cui si fa riferimento all’interno della cartella dei modelli. Alcuni tipi di risorse a cui si fa riferimento in una mappa possono essere i seguenti:

- Se la mappa contiene il riferimento a un modello di argomento, ne viene creata una copia all&#39;interno della cartella, nella stessa gerarchia della cartella topic nel `dita-templates` cartella.
- Se la mappa contiene il riferimento a un modello di mappa, ne viene creata una copia all&#39;interno della cartella, nella stessa gerarchia della cartella mappe nella cartella `dita-templates` cartella.
- Se la mappa contiene il riferimento generico a un argomento o a una mappa esterna al `dita-templates/topics` o `dita-templates/maps` cartella, viene fatto riferimento solo allo stesso e non viene creata alcuna copia.

   >[!NOTE]
   >
   > `dita-templates/topics` e `dita-templates/maps` sono i percorsi predefiniti nelle Guide e sono configurabili.


   Se all’interno del modello mappa è presente una definizione di chiave del modello argomento, viene creata una nuova chiave \(quindi nuovo argomento\) a cui viene fatto riferimento nella mappa.

- Se nella cartella viene creato un altro argomento o mappa allo stesso livello, i nomi delle nuove risorse vengono aggiunti 0, 1, 2 e così via. È possibile scegliere di aprire la mappa per la modifica o salvare il file di mappa nel repository.

**Argomento padre:**[ Utilizzare l’Editor mappa](map-editor.md)
