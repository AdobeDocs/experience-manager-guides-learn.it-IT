---
title: Funzione di pubblicazione nativa di PDF | Utilizzare JavaScript per lavorare con contenuto o stile
description: Scopri come creare e utilizzare fogli di stile e creare stili per i contenuti.
source-git-commit: 09918abbdade934468dea1c55d0ca2cd60622b35
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---


# Utilizzare JavaScript per lavorare con contenuto o stile

La funzione di pubblicazione nativa di PDF consente di eseguire JavaScript per manipolare il contenuto o lo stile applicato al contenuto prima che venga generato il PDF finale. Questa funzione offre un controllo completo sulla generazione dell’output finale. Ad esempio, è possibile aggiungere informazioni di avviso legale all’output di PDF, che si trova in un altro PDF. Utilizzando JavaScript, è possibile aggiungere le informazioni di avviso legale una volta che PDF è stato creato per il contenuto di base, ma prima che sia generato il PDF finale.\
Per supportare l’esecuzione di JavaScript, la funzione Pubblicazione nativa di PDF fornisce le seguenti funzioni di callback:

* `window.pdfLayout.onBeforeCreateTOC(callback)`: Questa funzione di callback viene eseguita prima della generazione del sommario.
* `window.pdfLayout.onBeforePagination(callback)`: Questa funzione di callback viene eseguita dopo la generazione del sommario, ma prima dell’aggiunta di interruzioni di pagina in PDF.
* `window.pdfLayout.onAfterPagination(callback)`: Questa funzione di callback viene eseguita dopo il sommario e le interruzioni di pagina vengono aggiunte in PDF.

>[!NOTE]
>
>Internamente, viene mantenuta una sequenza di esecuzione per queste funzioni di callout. Innanzitutto, viene eseguito onBeforeCreateTOC, seguito da onBeforePagination e, infine, viene eseguito onAfterPagination.

In base al tipo di contenuto o alla modifica dello stile che si desidera eseguire, è possibile scegliere quale funzione di callback utilizzare. Ad esempio, se desideri aggiungere contenuto, è consigliabile farlo prima che venga generato il sommario. Allo stesso modo, se desideri eseguire alcuni aggiornamenti dello stile, questi possono essere eseguiti prima o dopo l’impaginazione.

Nell&#39;esempio seguente, la posizione dei titoli delle figure viene modificata da a sopra le immagini a sotto le immagini. A questo scopo, devi abilitare l’opzione di esecuzione JavaScript nel predefinito. A questo scopo, esegui le seguenti operazioni:

1. Apri il predefinito per la modifica.
1. Vai a **Avanzate** scheda .
1. Seleziona la **Abilita JavaScript** opzione .
1. Salva il predefinito e chiudi.

Quindi, crea un file JavaScript con il seguente codice e salvalo all’interno della cartella Resources del modello:

```css
...
/*
* DITA only allows the figure title to be placed above images 
* This JavaScript code is used to move the figure title below the image
* */
window.addEventListener('DOMContentLoaded', function () {
    window.pdfLayout.onBeforeCreateTOC(function() {
        var titleNodes = document.querySelectorAll('.fig > .title')
        for (var i = 0; i < titleNodes.length; i++) {
            var titleNode = titleNodes[i]
            var figNode = titleNode.parentNode
            var imageNode = figNode.querySelector('.image')
            if(imageNode && imageNode.parentNode !== figNode) {
              imageNode = imageNode.parentNode
            }
            if (figNode && imageNode && imageNode.parentNode === figNode) {
                figNode.insertBefore(imageNode, titleNode)
            }
        }
    })
});
...
```

>[!NOTE]
>
>La `window.addEventListener('DOMContentLoaded', function ()` deve essere chiamata prima delle funzioni di callback.

Successivamente, questo script deve essere richiamato da un file modello utilizzato per generare l’output di PDF. Per il nostro esempio, lo aggiungeremo nel modello sommario. Assicurati che `<script>` viene aggiunto all’interno di un `<div>` all’interno del tag `<body>` tag . Se lo aggiungi nel `<head>` o all’esterno del tag `<body>` , lo script non verrà eseguito.

<img src="./assets/js-added-resources-template.png" width="500">

L&#39;output generato utilizzando questo codice e il modello visualizza il titolo della figura sotto l&#39;immagine:

<img src="./assets/fig-title-below-image.png" width="500">
