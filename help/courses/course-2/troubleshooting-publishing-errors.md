---
title: Risoluzione dei problemi di pubblicazione
description: Risoluzione dei problemi relativi agli errori di pubblicazione in [!DNL Adobe Experience Manager Guides]
exl-id: b37ea3e7-59cf-4fc5-8fae-e1fadd26f8d8
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Risoluzione dei problemi di pubblicazione

La pubblicazione di una mappa è in genere semplice. Apri la mappa, seleziona un predefinito di output e genera l’output. Tuttavia, se una mappa o i relativi argomenti contengono errori, la generazione dell’output potrebbe non riuscire. In questo caso, è importante sapere come risolvere i problemi.

>[!VIDEO](https://video.tv.adobe.com/v/338990?quality=12&learn=on)

## Preparazione all&#39;esercizio

I file di esempio per l&#39;esercizio sono disponibili qui.

[Esercizio-Download](assets/exercises/publishing-basic-to-advanced.zip)

## Cause comuni di errori di pubblicazione

Gli errori possono essere introdotti nel contenuto sorgente. Ad esempio:

* Riferimento percorso file con nome errato

* Cartella con nome errato

* File o elemento grafico mancante

* Riferimento al contenuto configurato in modo errato

* Riferimento incrociato interrotto

* Errori nei valori di un attributo (ad esempio, stringa anziché numero)

* Impostazione errata dei componenti utilizzati da [!DNL AEM Guides]

## Impatto degli errori

Un errore può essere non grave e causare una semplice nota per comunicare che un file non è stato correttamente compilato o sufficientemente grave da impedire completamente la generazione dell’output. Nella scheda Output vengono visualizzate icone codificate a colori per indicare operazioni riuscite, errori o errori correlati alla generazione dell’output.

![impatto errore](images/error-impact.png)

## Apertura e revisione dei registri di errore

Il file di registro generato può essere aperto per la revisione.

1. Nella scheda **Output**, fare clic su **data/ora in Generato alle.**

   ![registro errori](images/error-log.png)

1. Scorri il registro degli errori.

## Mostrare e nascondere i tipi di errore

Nel registro degli errori ogni tipo di errore viene visualizzato in un colore univoco.

![errori di navigazione](images/navigate-errors.png)

1. **Seleziona** o **deseleziona** qualsiasi tipo di errore per mostrare o nascondere l&#39;evidenziazione.

1. Spostarsi tra gli errori utilizzando i pulsanti **avanti** o **precedente** (frecce).

## Risoluzione degli errori

A seconda del tipo di errore, la risoluzione può essere semplice o complessa. Può essere completata da un autore in XML Editor o richiedere a un amministratore di lavorare con [!DNL AEM Guides]. Le correzioni specifiche dipendono dall’errore, dall’impatto e dai flussi di lavoro organizzativi.

* Riferimento percorso file con nome errato

      Gli autori possono aggiornare il riferimento al percorso nel documento di origine.
     
  
* Cartella con nome errato

      Gli autori possono aggiornare il nome della cartella o spostare i file in base alle esigenze.
     
  
* File o elemento grafico mancante

      Gli autori possono caricare un elemento grafico/file mancante, rinominare un elemento grafico/file o spostare un elemento grafico/file
     
  
* Riferimento al contenuto configurato in modo errato

      Gli autori possono correggere il percorso del contenuto a cui si fa riferimento o modificare il percorso del riferimento al contenuto.
     
  
* Riferimento incrociato interrotto

      Gli autori possono correggere la posizione in cui il riferimento incrociato fa riferimento o modificare il nome o le proprietà del file di destinazione
     
  
* Errori nei valori di un attributo (ad esempio, stringa anziché numero)

      Gli autori possono aggiornare l&#39;attributo con un valore corretto oppure gli amministratori possono aggiornare il sistema per supportare nuovi valori.
     
  
* Impostazione errata dei componenti utilizzati da [!DNL AEM Guides]

      Gli amministratori possono aggiornare l&#39;installazione del sistema, i relativi componenti o le autorizzazioni.
     
  