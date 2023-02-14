---
title: Risoluzione dei problemi di pubblicazione
description: Risoluzione dei problemi di pubblicazione in [!DNL Adobe Experience Manager Guides]
exl-id: b37ea3e7-59cf-4fc5-8fae-e1fadd26f8d8
source-git-commit: 1c4d278a05f2612bc55ce277efb5da2e6a0fa9a9
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Risoluzione dei problemi di pubblicazione

Pubblicare una mappa è solitamente semplice. Apri la mappa, seleziona un predefinito di output e genera un output. Tuttavia, se una mappa o i relativi argomenti presentano errori, la generazione dell’output può non riuscire. Quando questo accade, è importante sapere come risolvere i problemi.

>[!VIDEO](https://video.tv.adobe.com/v/338990?quality=12&learn=on)

## Preparazione dell&#39;esercizio

Puoi scaricare file di esempio per l&#39;esercizio qui.

[Esercizio-Scarica](assets/exercises/publishing-basic-to-advanced.zip)

## Cause comuni di errori di pubblicazione

Gli errori possono essere introdotti nel contenuto sorgente. Esempio:

* Riferimento a un percorso di file non correttamente denominato

* Cartella denominata in modo errato

* Grafico o file mancante

* Riferimento di contenuto configurato in modo errato

* Riferimento incrociato interrotto

* Errori nei valori di un attributo (ad esempio una stringa anziché un numero)

* Configurazione errata dei componenti utilizzati da [!DNL AEM Guides]

## Impatto degli errori

Un errore può essere minore e causare una semplice nota per comunicare che un file non è stato compilato correttamente o sufficientemente grave da causare un errore completo nella generazione dell&#39;output. La scheda Outputs visualizza icone con colori codificati per mostrare il successo, gli errori o gli errori relativi alla generazione dell&#39;output.

![impatto](images/error-impact.png)

## Apertura e revisione dei registri degli errori

Il file di registro generato può essere aperto per la revisione.

1. In **Uscite** fai clic sulla scheda **data/ora in Generated At.**

   ![registro degli errori](images/error-log.png)

2. Scorri il registro degli errori.

## Visualizzazione e eliminazione dei tipi di errore

Il registro degli errori visualizza ogni tipo di errore in un colore univoco.

![errori di navigazione](images/navigate-errors.png)

1. **Seleziona** o **deseleziona** qualsiasi tipo di errore per mostrare o nascondere l&#39;evidenziazione.

2. Navigare tra gli errori utilizzando **next** o **precedente** tasti (frecce).

## Risoluzione degli errori

A seconda del tipo di errore, la risoluzione può essere semplice o complessa. Può essere completato da un autore in XML Editor oppure può richiedere l&#39;intervento di un amministratore [!DNL AEM Guides]. Le correzioni specifiche dipendono dall’errore, dall’impatto e dai flussi di lavoro organizzativi.

* Riferimento a un percorso di file non correttamente denominato

       Gli autori possono aggiornare il riferimento al percorso nel documento di origine.
       
   
* Cartella denominata in modo errato

       Gli autori possono aggiornare il nome della cartella o spostare i file in base alle esigenze.
       
   
* Grafico o file mancante

       Gli autori possono caricare un elemento grafico/file mancante, rinominare un elemento grafico/file o spostare un elemento grafico/file
       
   
* Riferimento di contenuto configurato in modo errato

       Gli autori possono correggere la posizione del contenuto a cui si fa riferimento o modificare il percorso del riferimento al contenuto.
       
   
* Riferimento incrociato interrotto

       Gli autori possono correggere la posizione in cui si trovano i punti di riferimento incrociato o modificare il nome o le proprietà del file di destinazione
       
   
* Errori nei valori di un attributo (ad esempio una stringa anziché un numero)

       Gli autori possono aggiornare l’attributo a un valore corretto oppure gli amministratori possono aggiornare il sistema per supportare i nuovi valori.
       
   
* Configurazione errata dei componenti utilizzati da [!DNL AEM Guides]

       Gli amministratori possono aggiornare l’installazione del sistema, dei suoi componenti o delle relative autorizzazioni.
       
   