---
title: Pubblicazione con condizioni
description: Pubblicazione con condizioni con Adobe Experience Manager Guides
exl-id: ea94824a-884b-447f-9562-e6c629b8133b
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 1%

---

# Pubblicazione con condizioni

La pubblicazione condizionale consente di scrivere un’origine di contenuto per uno o più tipi di pubblico, prodotti o piattaforme. Queste informazioni possono quindi essere pubblicate in modo dinamico e nell’output è incluso solo il contenuto specificamente richiesto.

>[!VIDEO](https://video.tv.adobe.com/v/339041?quality=12&learn=on)

## Preparazione all&#39;esercizio

I file di esempio per l&#39;esercizio sono disponibili qui.

[Esercizio-Download](assets/exercises/publishing-with-conditions.zip)

## Marcatura del contenuto con attributi condizionali

1. Aprire l&#39;argomento da modificare.

1. Immettere il testo da rendere condizionale. Ad esempio, uno o più paragrafi, un&#39;intera tabella, una figura o altro contenuto.

   ![Presenting-Information](images/presenting-info.png)

1. Seleziona il contenuto specifico a cui assegnare un attributo condizionale. Ad esempio, un singolo paragrafo all’interno dell’origine.

   ![Scelta modello](images/template-choice.png)

1. Nella barra a destra assicurati che vengano visualizzate le Proprietà.

1. Aggiungi un attributo per pubblico, prodotto o piattaforma.

1. Assegna un valore all’attributo. È stato applicato l’aggiornamento della visualizzazione del contenuto per mostrare il markup condizionale.

   ![Specify-Template](images/specify-template.png)

## Anteprima del contenuto condizionale

1. Clic **Anteprima**.

1. Sotto **Filtri**, seleziona o deseleziona le condizioni da mostrare o nascondere.

1. Seleziona o deseleziona **Testo condizioni di evidenziazione**.

   ![Anteprima-Condizionale-Contenuto](images/preview-conditional-content.png)

## Creazione di un predefinito condizione

Un predefinito di condizione è una raccolta di proprietà che definiscono cosa includere, escludere o contrassegnare in altro modo durante la generazione dell’output.

1. Dal Cruscotto Mappa, seleziona la **Predefiniti condizione** scheda.

1. Fai clic su **Crea**.

1. Seleziona **Aggiungi** (o **Aggiungi tutto**).

1. Denomina la condizione.

1. Seleziona una combinazione di attributo, etichetta e azione.

   ![Create-Condition-Preset](images/create-condition-preset.png)

1. Ripeti in base alle esigenze.  

1. Fai clic su **Salva**.

## Generazione dell’output condizionale

Una volta applicate le condizioni al contenuto, questo può essere generato come output. Può utilizzare un predefinito di condizione o un file DITAval.

## Generazione dell’output condizionale utilizzando un predefinito di condizione

1. Seleziona la **Predefiniti di output** scheda.

1. Seleziona un predefinito di output.

1. Clic **Modifica**.

1. Sotto **Applica condizione tramite** seleziona un predefinito condizione.

   ![Generate-Conditional-Output](images/generate-conditional-output.png)

1. Clic **Fine**.

1. Genera il predefinito di output ed esamina il contenuto.

## Generazione dell&#39;output condizionale tramite un file DITAval

Il file DITAval può essere utilizzato per pubblicare il contenuto condizionale. Questo richiede che un file sia creato o caricato e quindi a cui si fa riferimento durante la pubblicazione.

1. Seleziona la **Predefiniti di output** scheda.

1. Seleziona un predefinito di output.

1. Clic **Modifica**.

1. In Applica condizione mediante selezionare un file DITAval.

   ![Generate-Using-DITAval](images/generate-using-ditaval.png)

1. Clic **Fine**.

1. Genera il predefinito di output ed esamina il contenuto.
