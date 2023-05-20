---
title: Creazione e pubblicazione con le linee di base
description: Creazione e pubblicazione di con le baseline in [!DNL Adobe Experience Manager Guides]
exl-id: 3c229c30-f2e0-4fb0-b60c-7bae60ef1a5b
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%

---

# Creazione e pubblicazione con le linee di base

L&#39;utilizzo di una linea di base consente di creare una versione degli argomenti delle mappe e del relativo contenuto di riferimento. Può essere basato su una data o un’ora specifica oppure su etichette.

>[!VIDEO](https://video.tv.adobe.com/v/338993?quality=12&learn=on)

## Accesso alla scheda Baseline nel dashboard Mappa

Puoi accedere alle linee di base nel dashboard Mappa.

1. Vista archivio, seleziona l’icona con i puntini di sospensione sulla mappa per aprire il menu Opzioni, quindi **Apri Map Dashboard.**

   ![ellipsis-map-dashboard.png](images/ellipsis-map-dashboard.png)
Il quadro comandi Mappa (Map Dashboard) si apre in un’altra scheda.

1. Seleziona **Linee di base**.

   ![baseline-tab.png](images/baseline-tab.png)

Viene visualizzata la scheda Baseline.

## Creazione di una baseline basata su etichette

1. Nella scheda Baseline, seleziona **Crea**.

   ![create-baseline.png](images/create-baseline.png)

   Vengono visualizzate le informazioni della nuova baseline. Il nome predefinito è basato sulla data di creazione.

1. Se necessario, assegnare un nuovo nome alla linea di base.

1. Sotto l&#39;intestazione &quot;Imposta la versione basata su&quot;, selezionare il cerchio per Etichetta.
   ![set-the-version.png](images/set-the-version.png)

   >[!NOTE]
   >
   >NOTA: il *Usa la versione più recente se l’etichetta non è presente* è selezionata per impostazione predefinita. Se questa opzione non è selezionata e nella mappa sono presenti argomenti o file multimediali senza l&#39;etichetta scelta, il processo di creazione della linea di base avrà esito negativo.

1. Immetti l’etichetta che desideri utilizzare.

1. Seleziona **Salva**.

Viene creata la baseline. Viene visualizzata una tabella con tutti gli argomenti e le informazioni associate.

### Utilizzo della funzione Sfoglia tutti gli argomenti

La funzione Sfoglia tutti gli argomenti consente di visualizzare le informazioni dell&#39;argomento, incluse la versione e l&#39;etichetta, nonché di specificare la versione utilizzata. Puoi accedervi selezionando **Sfoglia tutti gli argomenti** durante la creazione o la modifica della baseline.

![browse-all-topic.png](images/browse-all-topics.png)

## Creazione di una baseline in base a data e ora

È inoltre possibile creare baseline che rappresentano un&#39;istantanea nel tempo.

1. Assicurati che la scheda Baseline sia aperta e seleziona Crea.

   ![create-baseline.png](images/create-baseline.png)

1. Sotto l&#39;intestazione &quot;Imposta la versione basata su&quot;, selezionare il cerchio &quot;Versione attivata&quot;.

   ![version-on.png](images/version-on.png)

1. Seleziona l’icona del calendario e specifica la data e l’ora desiderate.

   ![calendar.png](images/calendar.png)

1. Se necessario, assegnare un nuovo nome alla linea di base.

1. Seleziona **Salva**.

Viene creata la baseline. Viene visualizzata una tabella con tutti gli argomenti e le informazioni associate.

### Aggiunta di etichette alla linea di base

Puoi assegnare una nuova etichetta in blocco a tutto il contenuto della mappa.

1. Selezionare la baseline per la quale si desidera aggiungere le etichette.

1. Seleziona **Aggiungi etichette**.

   ![add-labels.png](images/add-labels.png)

   Viene visualizzata la finestra di dialogo Aggiungi etichetta.

1. Inserisci l’etichetta da assegnare e seleziona **Aggiungi**.

L&#39;etichetta è stata aggiunta a tutti gli argomenti.

## Generazione di un output del sito AEM utilizzando una linea di base

1. Passate alla scheda Predefiniti di output nel quadro comandi Mappa (Map Dashboard).

1. Selezionare la casella di controllo Sito AEM.

   ![aem-site-checkbox.png](images/aem-site-checkbox.png)

1. Seleziona **Modifica**.

   ![edit-aem.png](images/edit-aem.png)

   Viene visualizzata una nuova pagina.

1. Selezionare la casella di controllo Usa baseline e scegliere la baseline da utilizzare dal menu a discesa.

   ![baseline.png](images/baseline.png)

1. Seleziona **Fine**.

   ![done.png](images/done.png)

1. Seleziona **Genera**.

   ![generate.png](images/generate.png)

   L&#39;output è stato generato con una baseline.

## Visualizzazione dell’output generato

1. Passa alla scheda Output nel dashboard Mappa.

1. Selezionate il testo nella colonna Impostazione generazione (Generation Setting) per aprire l&#39;output.
   ![aem-site-link.png](images/aem-site-link.png)

## Rimozione di una baseline

1. Nella scheda Baseline selezionare la baseline da rimuovere.

1. Seleziona **Rimuovi**.

   ![remove-baseline.png](images/remove-baseline.png)

   Viene visualizzata la finestra di dialogo Rimuovi baseline.

1. Seleziona **Rimuovi**.

La baseline viene rimossa.

## Duplicazione di una baseline

1. Nella scheda Baseline selezionare la baseline da duplicare.

1. Seleziona **Duplica**.

   ![duplicate.png](images/duplicate.png)

1. Seleziona **Salva**.

   ![save.png](images/save.png)

Viene creata la baseline duplicata.

## Modifica di una baseline

È possibile specificare direttamente la versione di un argomento utilizzata in una baseline.

1. Nella scheda Baseline selezionare la baseline da modificare.
1. Seleziona **Modifica**.

   ![edit-aem.png](images/edit-aem.png)

1. Seleziona **Sfoglia tutti gli argomenti**.

   ![browse-all-topic.png](images/browse-all-topics.png)

   Viene visualizzata una tabella di argomenti con le relative informazioni associate.

1. Per gli argomenti che desideri modificare, seleziona la versione desiderata dal menu a discesa sotto la colonna Versione.

   ![version-dropdown.png](images/version-dropdown.png)

1. Seleziona **Salva**.

Le modifiche sono state salvate. La baseline utilizzerà le versioni dell&#39;argomento specificate.

## Creazione di un predefinito di output per il sito AEM personalizzato

Nella scheda Output è difficile distinguere tra output predefiniti dello stesso tipo. L’utilizzo di un predefinito di output personalizzato con un nome univoco e intuitivo consente di risolvere questo problema.

In questo caso, creiamo un predefinito di output basato su una linea di base.

1. Passate alla scheda Predefiniti di output nel quadro comandi Mappa (Map Dashboard).

1. Seleziona **Crea**.

   ![create-output-preset.png](images/create-output-preset.png)

   Viene visualizzata una nuova pagina di predefinito di output, denominata Nuovo output.
1. Nel campo Nome impostazione immettere un nome descrittivo.

1. Selezionare la casella di controllo Usa baseline e selezionare la baseline desiderata dal menu a discesa.

   ![baseline.png](images/baseline.png)

1. Seleziona **Fine**.

Il nuovo predefinito di output è stato creato e viene visualizzato nella pagina dei predefiniti di output.
