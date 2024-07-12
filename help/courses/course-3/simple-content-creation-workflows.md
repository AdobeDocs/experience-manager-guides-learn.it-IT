---
title: Flussi di lavoro semplici per la creazione di contenuti
description: Creazione di contenuti in AEM Guides
exl-id: e4b8e512-0688-44f7-b981-78af33b57b08
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 1%

---

# Flussi di lavoro per la creazione di contenuti semplici

L’editor di AEM Guides dispone di più scelte rapide che semplificano il flusso di lavoro di creazione dei contenuti. Queste scelte rapide consentono agli utenti di aggiungere e modificare rapidamente immagini, utilizzare più argomenti contemporaneamente, correggere errori, scaricare PDF di argomenti e utilizzare versioni ed etichette.

>[!VIDEO](https://video.tv.adobe.com/v/342770?quality=12&learn=on)

## Aggiungi un&#39;immagine

Le immagini possono essere aggiunte direttamente da un&#39;unità locale.

1. Trascina e rilascia l’immagine direttamente nell’argomento. Viene visualizzata la finestra di dialogo **Carica Assets**.

   ![Carica finestra di dialogo Assets](images/lesson-15/upload-assets-dialog.png)

1. Modifica il percorso della cartella con il percorso immagine desiderato.

1. Modifica il nome dell’immagine in un elemento rappresentativo del suo scopo.

1. Fai clic su [!UICONTROL **Carica**].

## Modificare un’immagine

1. Per ridimensionare un&#39;immagine, trascinare un angolo.

1. Per spostare un&#39;immagine in un&#39;altra posizione all&#39;interno dell&#39;argomento, trascinarla.

1. Utilizza **Proprietà contenuto** nel pannello laterale destro per modificare le proprietà di un&#39;immagine

   - scala

   - position

   - allineamento, oppure

   - altri attributi.

   ![Proprietà contenuto](images/lesson-15/content-properties.png)

## Utilizzare più argomenti

La Visualizzazione suddivisa è utile per confrontare argomenti, copiare e incollare tra argomenti oppure trascinare e rilasciare contenuto da un argomento all&#39;altro.

1. Aprire due o più argomenti correlati.

1. Fai clic sulla scheda Titolo di un file per aprire il menu contestuale.

1. Seleziona [!UICONTROL **Dividi**].

1. Scegli **Destra**.

   ![Visualizzazione divisa](images/lesson-15/split-view.png)

## Correggere gli errori tipografici

1. Individuare la parola o la frase contenente l&#39;errore.

1. Tenere premuto [!UICONTROL **Ctrl**].

1. Fare clic sul pulsante secondario del mouse sull&#39;errore.

1. Selezionare l&#39;ortografia corretta.

L&#39;errore è stato corretto nel testo dell&#39;argomento.

## Scaricare un PDF di argomenti

Gli utenti potrebbero voler scaricare un PDF dell’argomento corrente per iscriversi o condividerlo con altri utenti.

1. Fai clic su [!UICONTROL **Anteprima**] in alto a destra dello schermo.

1. Fai clic sull&#39;icona [!UICONTROL **PDF**] sopra l&#39;argomento. Viene visualizzata una finestra di dialogo.

   ![Esportazione PDF](images/lesson-15/pdf-export.png)

1. Immettere le informazioni per **Nome trasformazione** o **Argomenti riga di comando DITA-OT** se necessario. Tieni presente che un PDF genera comunque se tutti i campi vengono lasciati vuoti.

1. Fai clic su [!UICONTROL **Scarica**]. Il PDF genera.

1. Utilizza le icone disponibili per configurare, scaricare o condividere l’argomento di PDF.

## Individuare un argomento nel repository o nella mappa

1. Aprire l&#39;argomento.

1. Fare clic con il pulsante secondario del mouse sulla scheda Titolo.

1. Seleziona **Individua In**.

1. Scegliere **Archivio** o **Mappa** per passare alla posizione desiderata dell&#39;argomento.

## Versione di un argomento

1. Apportare una modifica a un argomento.

1. Salva l&#39;argomento.

1. Fai clic sull&#39;icona **Archivio** nel menu in alto a sinistra.

   ![Icona archivio](images/lesson-15/repository-icon.png)

1. Nella finestra di dialogo, aggiungi **Commenti per la nuova versione**.

   ![Finestra di dialogo Nuova versione](images/lesson-15/version-dialog.png)

1. Fai clic su [!UICONTROL **Salva**].

Il numero di versione viene aggiornato.

## Carica etichette versione

Tentare di tenere traccia dello stato di un argomento in base solo al numero di versione può essere difficile. Le etichette consentono di identificare più facilmente lo stato esatto di un argomento che è stato sottoposto a più revisioni.

1. Seleziona un **profilo cartella**.

1. All&#39;interno del Profilo cartella, configura l&#39;editor XML.

   a. Seleziona Modifica in alto a sinistra nella schermata.

   b. In Etichette versione contenuto XML aggiungere un nuovo argomento o utilizzarne uno esistente.

   ![Etichette versione contenuto](images/lesson-15/version-labels.png)

1. Seleziona [!UICONTROL **Carica**].

1. Scegli un file come ReviewLabels.json o simile. I dettagli su come creare un file di questo tipo sono trattati in un altro video.

1. Fai clic su [!UICONTROL **Apri**].

1. Fai clic su [!UICONTROL **Salva**] in alto a sinistra nella schermata Profilo cartella.

1. Fai clic su [!UICONTROL **Chiudi**] in alto a destra.

Le etichette di versione sono ora caricate.

## Assegna etichette di versione

1. Carica etichette versione.

1. Fai clic sull&#39;icona [!UICONTROL **Preferenze utente**] in alto a sinistra nell&#39;argomento corrente.

   ![Profilo cartella](images/lesson-15/folder-profile-icon.png)

1. Seleziona lo stesso Profilo cartella in cui erano state precedentemente caricate le etichette di versione.

1. Nella finestra di dialogo Preferenze utente, assicurati che il Percorso base faccia riferimento alle stesse informazioni a cui è stato applicato il Profilo cartella.

   ![Preferenze utente](images/lesson-15/user-preferences.png)

1. Fai clic su [!UICONTROL **Salva**].

1. Versione dell&#39;argomento.

1. Aggiungi un commento e seleziona un’etichetta di versione dal menu a discesa.

   ![Finestra di dialogo Etichetta nuova versione](images/lesson-15/labels-dialog.png)

1. Fai clic su [!UICONTROL **Salva**].

Il numero di versione viene aggiornato.

## Visualizzare la cronologia delle versioni e le etichette

1. Dal pannello a sinistra, individua il titolo dell’argomento corrente.

1. Fai clic sul titolo per aprire il menu contestuale.

1. Seleziona [!UICONTROL **Visualizza nell&#39;interfaccia utente di Assets**].

   ![Interfaccia utente di Assets](images/lesson-15/view-assets-ui.png)

   - La cronologia delle versioni con le etichette viene visualizzata a sinistra.

   ![Cronologia versioni](images/lesson-15/version-history.png)

1. Fare clic su una versione per accedere ad opzioni quali **Ripristina questa versione** e **Anteprima versione**.

## Crea un nuovo modello

Esistono modelli sia per gli argomenti che per le mappe. Gli amministratori possono accedere ai modelli nel pannello a sinistra.

1. Fai clic su [!UICONTROL **Modelli**] nel pannello a sinistra.

1. Seleziona Mappa o Argomento per aprire il menu contestuale associato.

1. Fai clic su per aggiungere il nuovo modello.

   ![Nuovo modello di argomento](images/lesson-15/version-history.png)

1. Compila i campi nella finestra di dialogo risultante.

Viene visualizzato il modello di shell, contenente il contenuto di esempio e una struttura di esempio.
