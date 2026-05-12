---
title: Riferimenti incrociati e collegamenti
description: Creazione di rimandi e collegamenti in AEM Guides
exl-id: bee7d50f-cbdd-4ac8-b15b-101febc4ae80
TQID: https://experienceleague.adobe.com/K55H51fnM7bsR68-HQWbNHrSxHgQBPkM-jnGG-OFIbw
product_v2:
  - id: fae5e35a-80c9-4b94-9352-1a060a6aab1d
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: f5c2a4bb-71ca-4d7e-8efd-442250e6ba48
source-git-commit: 27ffc636d63300fb2e99903d92cab12f0cfcbb25
workflow-type: tm+mt
source-wordcount: 362
ht-degree: 0%

---

# Riferimenti incrociati e collegamenti

L&#39;editor XML e DITA consentono di creare collegamenti efficaci tra gli argomenti. È importante gestire in modo efficace i riferimenti ai contenuti, e ciò include l’utilizzo di valori ID univoci.

I file di esempio che puoi scegliere di utilizzare per questa lezione sono forniti nel file
[riferimenti incrociati andlinks.zip](assets/crossreferencesandlinks.zip)

>[!VIDEO](https://video.tv.adobe.com/v/342764?quality=12&learn=on)

## Creare un rimando a un argomento esterno

È possibile creare un riferimento incrociato esterno trascinando un argomento dal repository in un file aperto. Tuttavia, per evitare riferimenti incrociati interrotti, un ID deve prima essere definito a un valore correlato all&#39;elemento padre. Questo è un modo semplice per creare un riferimento incrociato e al contempo garantire che gli ID siano assegnati correttamente.

1. Aprite un file in cui desiderate inserire un riferimento incrociato esterno.

1. Assegna un ID all’elemento a cui fare riferimento.

   a. Fai clic all’interno dell’elemento.

   b. Nel pannello Proprietà contenuto scegliere **ID** dal menu a discesa Attributo.

   c. Digitare un nome logico nel campo Valore.

   d. Visualizzare l&#39;elemento e il relativo valore in **Visualizzazione struttura**, se necessario.

1. **Salva** l&#39;argomento per verificare che l&#39;archivio disponga dell&#39;ID aggiornato.

1. Fai clic sull&#39;icona [!UICONTROL **Riferimento**] nella barra degli strumenti superiore.

   ![Barra degli strumenti](images/lesson-7/references-icon.png)

1. Dalla scheda **Riferimento contenuto**, selezionare l&#39;associazione ID ed elemento che si desidera inserire come riferimento incrociato.

1. Fai clic su [!UICONTROL **Seleziona**].

Il riferimento incrociato è stato aggiunto all&#39;argomento.

## Collegamento a un sito Web

È possibile inserire un collegamento a un sito Web all&#39;interno di qualsiasi argomento. Per ulteriori informazioni, consulta il video di AEM Guides Course 1 sul collegamento ai siti web.


## Visualizza collegamenti interrotti

Alcune modifiche possono causare la rottura dei riferimenti incrociati. Queste includono l’eliminazione di un argomento, la riorganizzazione di una sezione che contiene un riferimento incrociato o la modifica di un ID dopo l’inserimento del riferimento incrociato. Si noti che con questa lezione viene fornito un argomento di esempio _crossreferencesandlinks.zip_ che causerà l&#39;interruzione di diversi riferimenti incrociati puntati al contenuto interno.

1. Passa alla **visualizzazione Struttura** nel pannello a sinistra.

1. Fai clic sull&#39;icona [!UICONTROL **Filtro**].

1. Seleziona **Collegamenti interrotti**.

   ![Elenco a discesa dei filtri](images/lesson-7/broken-links.png)

I collegamenti interrotti vengono visualizzati come oggetti cliccabili. Puoi identificarli in rosso nell’argomento.
