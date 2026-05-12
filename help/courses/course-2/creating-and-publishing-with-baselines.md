---
title: Creazione e pubblicazione con le linee di base
description: Creazione e pubblicazione con linee di base in [!DNL Adobe Experience Manager Guides]
exl-id: 3c229c30-f2e0-4fb0-b60c-7bae60ef1a5b
TQID: https://experienceleague.adobe.com/P2NbWdOXSWFs40gpSWNrtDLR3VKofXymN5FlZSQRJ7Y
product_v2: id: fae5e35a-80c9-4b94-9352-1a060a6aab1did: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
feature_v2: id: a3bd6397-2eb2-4908-a61c-226e26855dcaid: d90290ec-3e61-4ebd-8649-bcafe0836803
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 27ffc636d63300fb2e99903d92cab12f0cfcbb25
workflow-type: tm+mt
source-wordcount: 764
ht-degree: 2%

---

# Creazione e pubblicazione con le linee di base

L&#39;utilizzo di una linea di base consente di creare una versione degli argomenti delle mappe e del relativo contenuto di riferimento. Può essere basato su una data o un’ora specifica oppure su etichette.

>[!VIDEO](https://video.tv.adobe.com/v/338993?quality=12&learn=on)

## Accesso alla scheda Baseline nel dashboard Mappa

Puoi accedere alle linee di base nel dashboard Mappa.

1. Vista archivio, seleziona l&#39;icona con i puntini di sospensione sulla mappa per aprire il menu Opzioni, quindi **Apri dashboard mappa.**

   ![puntini di sospensione-mappa-dashboard.png](images/ellipsis-map-dashboard.png)
Il quadro comandi Mappa (Map Dashboard) si apre in un’altra scheda.

1. Seleziona **Base Line**.

   ![baseline-tab.png](images/baseline-tab.png)

Viene visualizzata la scheda Baseline.

## Creazione di una baseline in base alle etichette

1. Nella scheda Baseline selezionare **Crea**.

   ![create-baseline.png](images/create-baseline.png)

   Vengono visualizzate le informazioni della nuova baseline. Il nome predefinito è basato sulla data di creazione.

1. Se necessario, assegnare un nuovo nome alla linea di base.

1. Sotto l&#39;intestazione &quot;Imposta la versione basata su&quot;, selezionare il cerchio per Etichetta.
   ![set-the-version.png](images/set-the-version.png)

   >[!NOTE]
   >
   >NOTA: la casella di controllo *Usa versione più recente se l&#39;etichetta non è presente* è selezionata per impostazione predefinita. Se questa opzione non è selezionata e nella mappa sono presenti argomenti o file multimediali senza l&#39;etichetta scelta, il processo di creazione della linea di base avrà esito negativo.

1. Immetti l’etichetta che desideri utilizzare.

1. Seleziona **Salva**.

Viene creata la baseline. Viene visualizzata una tabella con tutti gli argomenti e le informazioni associate.

### Utilizzo della funzione Sfoglia tutti gli argomenti

La funzione Sfoglia tutti gli argomenti consente di visualizzare le informazioni dell&#39;argomento, incluse la versione e l&#39;etichetta, nonché di specificare la versione utilizzata. Puoi accedervi selezionando **Sfoglia tutti gli argomenti** durante la creazione o la modifica della linea di base.

![sfoglia-tutti-argomenti.png](images/browse-all-topics.png)

## Creazione di una baseline in base a data e ora

È inoltre possibile creare baseline che rappresentano un&#39;istantanea nel tempo.

1. Assicurati che la scheda Baseline sia aperta e seleziona Crea.

   ![create-baseline.png](images/create-baseline.png)

1. Sotto l&#39;intestazione &quot;Imposta la versione basata su&quot;, selezionare il cerchio &quot;Versione attivata&quot;.

   ![version-on.png](images/version-on.png)

1. Seleziona l’icona del calendario e specifica la data e l’ora desiderate.

   ![calendario.png](images/calendar.png)

1. Se necessario, assegnare un nuovo nome alla linea di base.

1. Seleziona **Salva**.

Viene creata la baseline. Viene visualizzata una tabella con tutti gli argomenti e le informazioni associate.

### Aggiunta di etichette alla linea di base

Puoi assegnare una nuova etichetta in blocco a tutto il contenuto della mappa.

1. Selezionare la baseline per la quale si desidera aggiungere le etichette.

1. Seleziona **Aggiungi etichette**.

   ![add-labels.png](images/add-labels.png)

   Viene visualizzata la finestra di dialogo Aggiungi etichetta.

1. Immettere l&#39;etichetta che si desidera assegnare e selezionare **Aggiungi**.

L&#39;etichetta è stata aggiunta a tutti gli argomenti.

## Generazione di un output del sito AEM utilizzando una baseline

1. Passate alla scheda Predefiniti di output nel quadro comandi Mappa (Map Dashboard).

1. Seleziona la casella di controllo Sito AEM.

   ![aem-site-checkbox.png](images/aem-site-checkbox.png)

1. Seleziona **Modifica**.

   ![modifica-aem.png](images/edit-aem.png)

   Viene visualizzata una nuova pagina.

1. Selezionare la casella di controllo Usa baseline e scegliere la baseline da utilizzare dal menu a discesa.

   ![baseline.png](images/baseline.png)

1. Seleziona **Fine**.

   ![fine.png](images/done.png)

1. Seleziona **Genera**.

   ![generate.png](images/generate.png)

   L&#39;output è stato generato con una baseline.

## Visualizzazione dell’output generato

1. Passa alla scheda Output nel dashboard Mappa.

1. Selezionate il testo nella colonna Impostazione generazione (Generation Setting) per aprire l&#39;output.
   ![aem-site-link.png](images/aem-site-link.png)

## Rimozione di una baseline

1. Nella scheda Baseline selezionare la baseline da rimuovere.

1. Selezionare **Rimuovi**.

   ![remove-baseline.png](images/remove-baseline.png)

   Viene visualizzata la finestra di dialogo Rimuovi baseline.

1. Selezionare **Rimuovi**.

La baseline viene rimossa.

## Duplicazione di una baseline

1. Nella scheda Baseline selezionare la baseline da duplicare.

1. Seleziona **Duplica**.

   ![duplicate.png](images/duplicate.png)

1. Seleziona **Salva**.

   ![salva.png](images/save.png)

Viene creata la baseline duplicata.

## Modifica di una baseline

È possibile specificare direttamente la versione di un argomento utilizzata in una baseline.

1. Nella scheda Baseline selezionare la baseline da modificare.
1. Seleziona **Modifica**.

   ![modifica-aem.png](images/edit-aem.png)

1. Selezionare **Sfoglia tutti gli argomenti**.

   ![sfoglia-tutti-argomenti.png](images/browse-all-topics.png)

   Viene visualizzata una tabella di argomenti con le relative informazioni associate.

1. Per gli argomenti che desideri modificare, seleziona la versione desiderata dal menu a discesa sotto la colonna Versione.

   ![version-dropdown.png](images/version-dropdown.png)

1. Seleziona **Salva**.

Le modifiche sono state salvate. La baseline utilizzerà le versioni dell&#39;argomento specificate.

## Creazione di un predefinito di output per siti AEM personalizzato

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
