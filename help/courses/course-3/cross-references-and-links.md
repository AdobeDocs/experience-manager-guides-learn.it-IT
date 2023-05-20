---
title: Riferimenti incrociati e collegamenti
description: Creazione di riferimenti incrociati e collegamenti nelle guide AEM
exl-id: bee7d50f-cbdd-4ac8-b15b-101febc4ae80
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Riferimenti incrociati e collegamenti

L&#39;editor XML e DITA consentono di creare collegamenti efficaci tra gli argomenti. È importante gestire in modo efficace i riferimenti ai contenuti, e ciò include l’utilizzo di valori ID univoci.

I file di esempio che puoi scegliere di utilizzare per questa lezione sono forniti nel file
[crossreferencesandlinks.zip](assets/crossreferencesandlinks.zip)

>[!VIDEO](https://video.tv.adobe.com/v/342764?quality=12&learn=on)

## Creare un rimando a un argomento esterno

È possibile creare un riferimento incrociato esterno trascinando un argomento dal repository in un file aperto. Tuttavia, per evitare riferimenti incrociati interrotti, un ID deve prima essere definito a un valore correlato all&#39;elemento padre. Questo è un modo semplice per creare un riferimento incrociato e al contempo garantire che gli ID siano assegnati correttamente.

1. Aprite un file in cui desiderate inserire un riferimento incrociato esterno.

1. Assegna un ID all’elemento a cui fare riferimento.

   a. Fai clic all’interno dell’elemento.

   b. Nel pannello Proprietà contenuto, scegliete **ID** dal menu a discesa Attributo.

   c. Digitare un nome logico nel campo Valore.

   d. Visualizzare l’elemento e il relativo valore in **Visualizzazione Struttura** se desiderato.

1. **Salva** l’argomento per garantire che l’archivio abbia l’ID aggiornato.

1. Fai clic su [!UICONTROL **Riferimento**] nella barra degli strumenti superiore.

   ![Barra degli strumenti](images/lesson-7/references-icon.png)

1. Dalla sezione **Riferimento contenuto** , selezionare l&#39;ID e l&#39;accoppiamento di elementi che si desidera inserire come riferimento incrociato.

1. Clic [!UICONTROL **Seleziona**].

Il riferimento incrociato è stato aggiunto all&#39;argomento.

## Collegamento a un sito Web

È possibile inserire un collegamento a un sito Web all&#39;interno di qualsiasi argomento. Per ulteriori informazioni, consulta il video sulle guide dell’AEM al corso 1 sul collegamento ai siti web.


## Visualizza collegamenti interrotti

Alcune modifiche possono causare la rottura dei riferimenti incrociati. Queste includono l’eliminazione di un argomento, la riorganizzazione di una sezione che contiene un riferimento incrociato o la modifica di un ID dopo l’inserimento del riferimento incrociato. Tieni presente che un argomento di esempio _crossreferencesandlinks.zip_ viene fornito con questa lezione che causerà l’interruzione di diversi riferimenti incrociati al contenuto interno tra puntati.

1. Accedi a **Visualizzazione Struttura** nel pannello sinistro.

1. Fai clic su [!UICONTROL **Filtro**] icona.

1. Seleziona **Collegamenti interrotti**.

   ![Menu a discesa Filtro](images/lesson-7/broken-links.png)

I collegamenti interrotti vengono visualizzati come oggetti cliccabili. Puoi identificarli in rosso nell’argomento.
