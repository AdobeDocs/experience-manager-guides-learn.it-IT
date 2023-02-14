---
title: Creazione e pubblicazione con le linee di base
description: Creazione e pubblicazione con le linee di base in [!DNL Adobe Experience Manager Guides]
exl-id: 3c229c30-f2e0-4fb0-b60c-7bae60ef1a5b
source-git-commit: 1c4d278a05f2612bc55ce277efb5da2e6a0fa9a9
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%

---

# Creazione e pubblicazione con le linee di base

L’utilizzo di una linea di base consente di creare una versione degli argomenti della mappa e del relativo contenuto di riferimento. Può essere basato su una data o un&#39;ora specifica o su etichette.

>[!VIDEO](https://video.tv.adobe.com/v/338993?quality=12&learn=on)

## Accesso alla scheda Linee di base nella dashboard Mappa

Puoi accedere alle tue linee di base nella Dashboard mappa.

1. Vista archivio, seleziona l’icona Ellissi sulla mappa per aprire il menu Opzioni, quindi **Apri dashboard mappa.**

   ![ellipsis-map-dashboard.png](images/ellipsis-map-dashboard.png)
Il dashboard mappa si apre in un&#39;altra scheda.

2. Seleziona **Linee di base**.

   ![baseline-tab.png](images/baseline-tab.png)

Viene visualizzata la scheda Linee di base .

## Creazione di una baseline basata su etichette

1. Nella scheda Linee di base, seleziona **Crea**.

   ![create-baseline.png](images/create-baseline.png)

   Vengono visualizzate le informazioni della nuova baseline. Il nome predefinito dipende dalla data di creazione.

2. Se necessario, assegna alla baseline un nuovo nome.

3. Sotto l&#39;intestazione &quot;Imposta la versione in base a&quot;, selezionare il cerchio per Etichetta.
   ![set-the-version.png](images/set-the-version.png)

   >[!NOTE]
   >
   >NOTA: La *Utilizza la versione più recente se l’etichetta non è presente* casella di controllo selezionata per impostazione predefinita. Se questa opzione non è selezionata e nella mappa sono presenti argomenti o file multimediali senza l’etichetta selezionata, il processo di creazione della linea di base non riuscirà.

4. Inserisci l’etichetta da utilizzare.

5. Seleziona **Salva**.

Viene creata la baseline. Viene visualizzata una tabella di tutti gli argomenti e delle relative informazioni associate.

### Utilizzo della funzione Sfoglia tutti gli argomenti

La funzione Sfoglia tutti gli argomenti consente di visualizzare le informazioni dell’argomento, inclusa la versione e l’etichetta, nonché di specificare la versione utilizzata. Puoi accedervi selezionando **Sfoglia tutti gli argomenti** durante la creazione o la modifica della baseline.

![browse-all-topic.png](images/browse-all-topics.png)

## Creazione di una baseline in base a data e ora

È inoltre possibile creare linee di base che rappresentano un&#39;istantanea nel tempo.

1. Assicurati che la scheda Linee di base sia aperta e seleziona Crea.

   ![create-baseline.png](images/create-baseline.png)

2. Sotto l&#39;intestazione &quot;Imposta la versione in base a&quot;, selezionare il cerchio per &quot;Versione su&quot;.

   ![version-on.png](images/version-on.png)

3. Seleziona l’icona del calendario e specifica la data e l’ora desiderate.

   ![calendar.png](images/calendar.png)

4. Se necessario, assegna alla baseline un nuovo nome.

5. Seleziona **Salva**.

Viene creata la baseline. Viene visualizzata una tabella di tutti gli argomenti e delle relative informazioni associate.

### Aggiunta di etichette alla baseline

Puoi assegnare una nuova etichetta in blocco a tutto il contenuto della mappa.

1. Seleziona la linea di base per la quale desideri aggiungere le etichette.

2. Seleziona **Aggiungi etichette**.

   ![add-label.png](images/add-labels.png)

   Viene visualizzata la finestra di dialogo Aggiungi etichetta.

3. Immettere l&#39;etichetta da assegnare e selezionare **Aggiungi**.

L’etichetta è stata aggiunta a tutti gli argomenti.

## Generazione di un output del sito AEM utilizzando una linea di base

1. Passa alla scheda Predefiniti di output nel dashboard Mappa.

2. Selezionare la casella di controllo Sito AEM.

   ![aem-site-check.png](images/aem-site-checkbox.png)

3. Seleziona **Modifica**.

   ![edit-aem.png](images/edit-aem.png)

   Viene visualizzata una nuova pagina.

4. Selezionate la casella di controllo Usa linea di base e scegliete la linea di base da utilizzare dal menu a discesa.

   ![baseline.png](images/baseline.png)

5. Seleziona **Fine**.

   ![done.png](images/done.png)

6. Seleziona **Genera**.

   ![generate.png](images/generate.png)

   L&#39;output è stato generato con una linea di base.

## Visualizzazione dell&#39;output generato

1. Passate alla scheda Outputs (Output) nel dashboard della mappa.

2. Selezionare il testo nella colonna Impostazione generazione per aprire l&#39;output.
   ![aem-site-link.png](images/aem-site-link.png)

## Rimozione di una baseline

1. Nella scheda Linee di base selezionare la linea di base da rimuovere.

2. Seleziona **Rimuovi**.

   ![removebaseline.png](images/remove-baseline.png)

   Viene visualizzata la finestra di dialogo Rimuovi linea di base.

3. Seleziona **Rimuovi**.

La linea di base viene rimossa.

## Duplicazione di una linea di base

1. Nella scheda Linee di base selezionare la linea di base da duplicare.

2. Seleziona **Duplica**.

   ![duplicate.png](images/duplicate.png)

3. Seleziona **Salva**.

   ![save.png](images/save.png)

Viene creata la baseline duplicata.

## Modifica di una linea di base

Puoi specificare direttamente la versione di un argomento utilizzato in una linea di base.

1. Nella scheda Linee di base selezionare la linea di base da modificare.
2. Seleziona **Modifica**.

   ![edit-aem.png](images/edit-aem.png)

3. Seleziona **Sfoglia tutti gli argomenti**.

   ![browse-all-topic.png](images/browse-all-topics.png)

   Viene visualizzata una tabella degli argomenti e le relative informazioni associate.

4. Per gli argomenti da modificare, seleziona la versione desiderata dal menu a discesa nella colonna Versione .

   ![version-menu a discesa.png](images/version-dropdown.png)

5. Seleziona **Salva**.

Le modifiche sono state salvate. La baseline ora utilizza le versioni dell’argomento specificate.

## Creazione di un predefinito di output AEM sito personalizzato

È difficile distinguere tra output predefiniti dello stesso tipo nella scheda Outputs. L&#39;utilizzo di un predefinito di output personalizzato con un nome univoco e semplice da usare consente di risolvere il problema.

In questo caso, stiamo creando un predefinito di output basato su una linea di base.

1. Passa alla scheda Predefiniti di output nel dashboard Mappa.

2. Seleziona **Crea**.

   ![create-output-preset.png](images/create-output-preset.png)

   Viene visualizzata una nuova pagina preimpostata di output, denominata Nuovo output.
3. Nel campo Nome impostazione immettere un nome descrittivo.

4. Selezionate la casella di controllo Usa linea di base e selezionate la linea di base desiderata dal menu a discesa.

   ![baseline.png](images/baseline.png)

5. Seleziona **Fine**.

Il nuovo predefinito di output è stato creato e viene visualizzato nella pagina dei predefiniti di output.
