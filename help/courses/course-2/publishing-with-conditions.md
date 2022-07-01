---
title: Pubblicazione con condizioni
description: Pubblicazione con le condizioni con le guide di Adobe Experience Manager
exl-id: ea94824a-884b-447f-9562-e6c629b8133b
source-git-commit: b5e64512956f0a7f33c2021bc431d69239f2a088
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 3%

---

# Pubblicazione con condizioni

La pubblicazione condizionale consente di scrivere una fonte di contenuto per uno o più tipi di pubblico, prodotti o piattaforme. Queste informazioni possono quindi essere pubblicate in modo dinamico e solo il contenuto specifico incluso nell’output.

>[!VIDEO](https://video.tv.adobe.com/v/339041)

## Preparazione dell&#39;esercizio

Puoi scaricare file di esempio per l&#39;esercizio qui.

[Esercizio-Scarica](assets/exercises/publishing-with-conditions.zip)

## Marcatura del contenuto con gli attributi condizionali

1. Apri l’argomento da modificare.

2. Inserisci il testo che deve diventare condizionale. Ad esempio, uno o più paragrafi, un’intera tabella, una figura o altro contenuto.

   ![Informazioni sulla presentazione](images/presenting-info.png)

3. Seleziona il contenuto specifico a cui assegnare un attributo condizionale. Ad esempio, un singolo paragrafo all’interno dell’origine.

   ![Scelta modello](images/template-choice.png)

4. Nella barra a destra assicurati che sia visualizzata la finestra Proprietà .

5. Aggiungi un attributo per pubblico, prodotto o piattaforma.

6. Assegna un valore all&#39;attributo. È stato applicato l’aggiornamento della visualizzazione del contenuto per mostrare il markup condizionale.

   ![Specifica modello](images/specify-template.png)

## Anteprima del contenuto condizionale

1. Fai clic su **Anteprima**.

2. Sotto **Filtri**, seleziona o deseleziona le condizioni da visualizzare o nascondere.

3. Seleziona o deseleziona **Testo in condizioni di evidenziazione**.

   ![Anteprima-Condizionale-Contenuto](images/preview-conditional-content.png)

## Creazione di un predefinito per condizioni

Un predefinito di condizione è una raccolta di proprietà che definiscono cosa deve essere incluso o escluso, o altrimenti contrassegnato, durante la generazione dell’output.

1. Dal dashboard di mappatura, seleziona la **Predefiniti condizione** scheda .

2. Fai clic su **Crea**.

3. Seleziona **Aggiungi** o **Aggiungi tutto**).

4. Denomina la condizione.

5. Seleziona un attributo, un’etichetta e una combinazione di azioni.

   ![Crea-Predefinito-Condizione](images/create-condition-preset.png)

6. Ripeti in base alle esigenze.  

7. Fai clic su **Salva**.

## Generazione dell’output condizionale

Una volta applicate le condizioni al contenuto, è possibile generarlo come output. Questo può utilizzare un predefinito di condizione o un file DITAval.

## Generazione dell’output condizionale tramite un predefinito per condizioni

1. Seleziona la **Predefiniti di output** scheda .

2. Seleziona un predefinito di output.

3. Fate clic su **Modifica**. 

4. Sotto **Applica condizione tramite** selezionate un predefinito di condizione.

   ![Genera-output condizionale](images/generate-conditional-output.png)

5. Fai clic su **Fine**.

6. Genera il predefinito di output e rivedi il contenuto.

## Generazione dell&#39;output condizionale tramite un file DITAval

Il file DITAval può essere utilizzato per pubblicare il contenuto condizionale. Questo richiede la creazione o il caricamento di un file a cui fare riferimento al momento della pubblicazione.

1. Seleziona la **Predefiniti di output** scheda .

2. Seleziona un predefinito di output.

3. Fate clic su **Modifica**. 

4. In Applica condizione con selezionare un file DITAval.

   ![Generate-Using-DITAval](images/generate-using-ditaval.png)

5. Fai clic su **Fine**.

6. Genera il predefinito di output e rivedi il contenuto.
