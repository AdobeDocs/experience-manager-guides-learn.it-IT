---
title: Creare mappe basate su modelli personalizzati
description: Scopri come creare mappe basate su modelli personalizzati
source-git-commit: 66915827a0b169069cc482763f0f50b9e9b6aa64
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---


# Creare mappe basate su modelli personalizzati {#id225VF0808MP}

È possibile creare modelli di mappa personalizzati e utilizzarli per creare mappe DITA insieme ai modelli di argomento e di mappa a cui si fa riferimento nel modello di mappa

È possibile fare riferimento ad altri modelli mappa e modelli argomento dal modello mappa personalizzato. I modelli di mappa a cui si fa riferimento possono fare riferimento a vari modelli di mappa, modelli di argomento, argomenti, mappe, immagini, video e altre risorse. Il modello di mappa personalizzato può aiutarti a replicare molto facilmente i modelli di mappa e l&#39;intera struttura di cartelle di riferimento. Questi modelli personalizzati sono particolarmente utili per creare e ricreare più mappe con strutture e riferimenti ricorsivi.

>[!NOTE]
>
> I modelli di argomento non vengono creati in modo ricorsivo. Vengono generati solo modelli di argomento direttamente all’interno del modello di mappa e qualsiasi modello di argomento all’interno di un modello di argomento viene semplicemente indicato direttamente nell’elemento padre.

## Creare modelli personalizzati

AEM Guide consente di creare mappe e argomenti personalizzati dalla cartella dei modelli dita. Puoi utilizzare questi modelli personalizzati per creare la mappa e l&#39;argomento. Puoi anche condividere questi modelli con i tuoi autori, che possono utilizzare per creare i loro file. Utilizzando questi modelli, puoi consentire agli autori di conservare copie separate di alcune risorse all’interno della cartella dei modelli.

>[!NOTE]
>
> Tutte le risorse alle quali si deve fare riferimento e che devono essere mantenute devono essere mantenute al di fuori della cartella dei modelli.

**Modello argomento**

Esegui i seguenti passaggi per creare un modello di argomento:

1. In **Interfaccia utente Assets**, passare alla cartella dei modelli dita.

   ![](images/dita-templates.png)

1. Fai clic su **argomenti** cartella per aprirla.Fai clic su **Crea modello \> DITA**.
1. Nella pagina Blueprint, seleziona **Argomento** quindi fai clic su **Avanti.**
1. Nella pagina Proprietà , specifica il modello di argomento **Titolo**.
1. Specifica il file **Nome**

   >[!NOTE]
   >
   > Il nome file deve avere l&#39;estensione .dita.

1. \(Facoltativo\) Aggiungi una descrizione.
1. Fai clic su **Crea**. Viene visualizzato il messaggio del modello di argomento creato. Puoi quindi aprire il modello di argomento e modificarlo.

**Modello mappa**

Esegui i seguenti passaggi per creare un modello di mappa:

1. In **Interfaccia utente Assets**, passare alla cartella dei modelli dita.
1. Fai clic su **mappe** cartella per aprirla.
1. Fai clic su **Crea \> modello DITA.**

   ![](images/create-dita-template.png)

1. Nella pagina Blueprint, seleziona **Mappa** e fai clic su **Successivo**.
1. Nella pagina Proprietà , specifica il modello di mappa **Titolo**.
1. Specifica il file **Nome**.

   >[!NOTE]
   >
   > Il nome del file deve avere l&#39;estensione ditamap.

1. (Facoltativo\) Aggiungi una descrizione.Fai clic su **Crea**. Viene visualizzato il messaggio del modello di mappa creato. Puoi quindi aprire il modello di mappa e modificarlo. Puoi aggiungere nel modello mappa i riferimenti per i modelli di argomento, i modelli di mappa e altre risorse.

## Passa il titolo definito nei modelli

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

Se non si utilizzano parentesi graffe intorno al titolo, la mappa DITA risultante verrà selezionata solo il primo elemento e la nidificazione del titolo non verrà prelevata dal modello e avrà il seguente aspetto:

```XML
<pubtitle> Rootmap1 </pubtitle>
```

>[!NOTE]
> È inoltre possibile utilizzare le parentesi graffe intorno al testo per passare la relativa struttura nidificata dai modelli personalizzati alle mappe DITA.

Esempio

```XML
<title>	<sub>		<b>{title}</b>	</sub></title>
```

## Utilizza il modello di mappa per creare nuove mappe

>[!NOTE]
>
> Il modello di mappa deve essere configurato e reso disponibile per l’authoring dall’amministratore. Per ulteriori dettagli, consulta *Configurare i modelli di authoring* in Installazione e configurazione delle guide Adobe Experience Manager as a Cloud Service.

Esegui i seguenti passaggi per creare una mappa utilizzando il modello di mappa personalizzato:

1. In **Interfaccia utente Assets,** passa alla cartella in cui desideri creare la mappa.
1. Fai clic su **Crea \> Mappa DITA**.
1. Nella pagina Blueprint, seleziona il modello di mappa da utilizzare e fai clic su **Successivo**. Ad esempio, se hai creato un modello di mappa &quot;test-template&quot;, selezionalo.
1. Nella pagina Proprietà , specifica la mappa **Titolo**.
1. Specifica il file **Nome**.

   >[!NOTE]
   >
   > Il nome del file deve avere l&#39;estensione ditamap.

1. Fai clic su **Crea**. Viene visualizzato il messaggio della mappa creata.


La mappa genera tutte le risorse a cui si fa riferimento all’interno della cartella del modello. Alcuni tipi di risorse indicati in una mappa possono essere i seguenti:

- Se la mappa contiene il riferimento a un modello di argomento, all’interno della cartella viene creata una copia di tale modello, nella stessa gerarchia della cartella degli argomenti nella cartella `dita-templates` cartella.
- Se la mappa contiene il riferimento a un modello di mappa, all’interno della cartella viene creata una copia di tale modello, nella stessa gerarchia della cartella delle mappe nella cartella `dita-templates` cartella.
- Se la mappa contiene il riferimento generico a un argomento o una mappa al di fuori della `dita-templates/topics` o `dita-templates/maps` viene fatto riferimento solo alla cartella e non viene creata alcuna copia.

   >[!NOTE]
   >
   > `dita-templates/topics` e `dita-templates/maps` sono i percorsi predefiniti in Guide e sono configurabili.


   Se nel modello di mappa è presente una definizione di chiave del modello di argomento, viene creata una nuova chiave \(quindi nuovo argomento\) a cui viene fatto riferimento nella mappa.

- Se nella cartella viene creata un’altra mappa o un altro argomento allo stesso livello, ai nomi delle risorse appena create viene aggiunto 0,1,2 e così via. Puoi scegliere di aprire la mappa per la modifica o salvare il file mappa nell&#39;archivio.

**Argomento principale:**[ Utilizzare l’Editor mappa](map-editor.md)

