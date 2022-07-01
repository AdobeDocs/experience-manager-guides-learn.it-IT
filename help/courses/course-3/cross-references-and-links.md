---
title: Collegamenti e riferimenti incrociati
description: Creazione di riferimenti incrociati e collegamenti nelle guide AEM
exl-id: bee7d50f-cbdd-4ac8-b15b-101febc4ae80
source-git-commit: b5e64512956f0a7f33c2021bc431d69239f2a088
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Collegamenti e riferimenti incrociati

L&#39;Editor XML e DITA forniscono un modo potente per collegare gli argomenti. È importante gestire in modo efficace i riferimenti al contenuto e ciò include l&#39;utilizzo di valori ID univoci.

I file di esempio che è possibile scegliere di utilizzare per questa lezione sono forniti nel file
[crossreferencesandlinks.zip](assets/crossreferencesandlinks.zip)

>[!VIDEO](https://video.tv.adobe.com/v/342764)

## Creare un riferimento incrociato a un argomento esterno

È possibile creare un riferimento incrociato esterno trascinando e rilasciando un argomento dal Repository in un file aperto. Tuttavia, per evitare i riferimenti incrociati interrotti, un ID deve prima essere definito in un valore relativo all&#39;elemento padre. Questo è un modo semplice per creare un riferimento incrociato e allo stesso tempo per garantire che gli ID siano correttamente assegnati.

1. Aprire un file in cui si desidera inserire un riferimento incrociato esterno.

2. Assegna un ID all’elemento a cui fare riferimento.

   a) Fai clic all’interno dell’elemento.

   b) Nel pannello Proprietà contenuto , scegli **ID** dal menu a discesa Attributo .

   c. Digitare un nome logico nel campo Valore.

   d. Visualizza l’elemento e il relativo valore in **Vista struttura** se desiderato.

3. **Salva** l’argomento per verificare che l’archivio disponga dell’ID aggiornato.

4. Fai clic sul pulsante [!UICONTROL **Riferimento**] nella barra degli strumenti superiore.

   ![Barra degli strumenti](images/lesson-7/references-icon.png)

5. Da **Riferimento contenuto** , seleziona l’ID e l’associazione degli elementi da inserire come riferimento incrociato.

6. Fai clic su [!UICONTROL **Seleziona**].

Il riferimento incrociato è stato aggiunto all’argomento.

## Collegamento a un sito web

Puoi inserire un collegamento a un sito web in qualsiasi argomento. Per ulteriori informazioni, consulta il video sulle AEM guide al corso 1 sul collegamento ai siti web .


## Visualizza collegamenti interrotti

Alcune modifiche possono causare l’interruzione di riferimenti incrociati. Ad esempio, l’eliminazione di un argomento, la riorganizzazione di una sezione contenente un riferimento incrociato o la modifica di un ID dopo l’inserimento del riferimento incrociato. Si noti un argomento di esempio _crossreferencesandlinks.zip_ viene fornita con questa lezione che causerà l’interruzione di diversi riferimenti incrociati puntati al contenuto interno.

1. Passa a **Vista struttura** nel pannello a sinistra.

2. Fai clic sul pulsante [!UICONTROL **Filtro**] icona.

3. Seleziona **Collegamenti interrotti**.

   ![Elenco a discesa Filtro](images/lesson-7/broken-links.png)

I collegamenti interrotti vengono visualizzati come oggetti selezionabili. Puoi identificarli in testo rosso nell’argomento.
