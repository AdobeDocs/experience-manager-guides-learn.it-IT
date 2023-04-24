---
title: Configurazione dell’Editor AEM Guide
description: Configurazione dell’editor per AEM Guide
exl-id: 437d9598-4afc-431f-81bd-6762e22656b7
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 0%

---

# Configurazione editor XML

Se lavori in un ambiente restrittivo, puoi scegliere quali funzioni possono vedere i tuoi autori personalizzando la configurazione dell’editor all’interno di un profilo cartella specifico. L’applicazione di questo profilo cartella può modificare l’aspetto dell’editor stesso, dei modelli CSS, dei frammenti disponibili e delle etichette della versione contenuto.

I file di esempio che è possibile scegliere di utilizzare per questa lezione sono forniti nel file [xmleditorconfiguration.zip](assets/xmleditorconfiguration.zip).

>[!VIDEO](https://video.tv.adobe.com/v/342762?quality=12&learn=on)

## Personalizzare la configurazione predefinita dell’interfaccia utente dell’editor

Puoi sempre scaricare la configurazione dell’interfaccia utente predefinita nel sistema locale, apportare modifiche nell’editor di testo desiderato e caricarla nuovamente.

1. Nella schermata Navigazione, fai clic sul pulsante [!UICONTROL **Strumenti**] icona.

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello a sinistra.

1. Fai clic sul pulsante [!UICONTROL **Profili cartella**] piastrelle.

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Seleziona un profilo cartella.

1. Fai clic sul pulsante [!UICONTROL **Configurazione editor XML**] scheda .

1. Fai clic su [!UICONTROL **Scarica**] Predefinito.

   ![Scarica predefinito](images/lesson-4/download-default.png)

Ora puoi aprire e modificare il contenuto in un editor di testo. La _Installazione e configurazione delle guide AEM_ La guida contiene esempi su come rimuovere, personalizzare o aggiungere funzioni alla configurazione dell’interfaccia utente.

## Carica la configurazione dell&#39;interfaccia utente dell&#39;editor XML modificato

Dopo aver personalizzato la configurazione dell’interfaccia utente, puoi caricarla. Tieni presente che un file di configurazione di esempio _ui-config-limited-editor.json_ viene fornito con l’insieme di argomenti di supporto per questa lezione.

1. Nel profilo della cartella, fai clic sul pulsante [!UICONTROL **Configurazione editor XML**] scheda .

1. In Configurazione dell&#39;interfaccia utente dell&#39;editor XML, fai clic su [!UICONTROL **Carica**].

   ![Caricare](images/lesson-4/upload.png)

1. Fai doppio clic sul file per la configurazione dell’interfaccia utente modificata oppure, come mostrato qui, sul file di esempio fornito.

   ![File di configurazione di esempio](images/lesson-4/sample-config-file.png)

1. Fai clic su [!UICONTROL **Salva**] nell’angolo in alto a sinistra dello schermo.

Caricamento della configurazione dell&#39;interfaccia utente modificata completato.

## Personalizzare il layout del modello CSS

Come per la configurazione dell’interfaccia utente, puoi scaricare il layout del modello CSS. Puoi aprirlo in un editor di testo e apportare modifiche per personalizzare l’aspetto dell’argomento prima di caricarlo.

1. Nella schermata Navigazione, fai clic sul pulsante [!UICONTROL **Strumenti**] icona.

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello a sinistra.

1. Fai clic sul pulsante [!UICONTROL **Profili cartella**] piastrelle.

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Seleziona un profilo cartella.

1. Fai clic sul pulsante [!UICONTROL **Configurazione editor XML**] scheda .

1. In Layout modello CSS, fai clic su [!UICONTROL **Scarica**].

   ![Scarica CSS](images/lesson-4/download-css.png)

Ora puoi modificare e salvare il contenuto CSS in un editor di testo.

## Carica il layout del modello CSS modificato

Dopo aver personalizzato il layout del modello CSS, puoi caricarlo. Tieni presente che un file di esempio _css-layout-ONLY-draft-comment-change.css_ viene fornito con l’insieme di argomenti di supporto per questa lezione. Questo file contiene solo la bozza di modifica del commento, mentre _css-layout-draft-comment-change.css_ è l’intero file, disponibile solo a scopo di test o revisione.

1. Nel profilo della cartella, fai clic sul pulsante [!UICONTROL **Configurazione editor XML**] scheda .

1. In Layout modello CSS, fai clic su [!UICONTROL **Carica**].

   ![Carica CSS](images/lesson-4/upload-css.png)

1. Fai doppio clic sul file per il layout CSS personalizzato o sul file di esempio fornito qui.

   ![File CSS di esempio](images/lesson-4/sample-css-file.png)

1. Fai clic su [!UICONTROL **Salva**] nell’angolo in alto a sinistra dello schermo.
Il layout personalizzato del modello CSS è stato caricato correttamente.

## Modificare i frammenti dell’Editor XML

Gli snippet sono parti di contenuto riutilizzabili che possono essere specifiche di un prodotto o gruppo. Gli snippet di esempio vengono forniti con i file di supporto per questa lezione.

1. Nella schermata Navigazione, fai clic sul pulsante [!UICONTROL **Strumenti**] icona.

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello a sinistra.

1. Fai clic sul pulsante [!UICONTROL **Profili cartella**] piastrelle.

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Seleziona un profilo cartella.

1. Fai clic sul pulsante [!UICONTROL **Configurazione editor XML**] scheda .

1. In Frammenti editor XML, fai clic su **Carica**.

   ![Caricare snippet](images/lesson-4/upload-snippets.png)

1. Scegli i tuoi snippet o utilizza i campioni forniti.

   ![Frammento di esempio](images/lesson-4/sample-snippet.png)

1. Fai clic su [!UICONTROL **Salva**] nell’angolo in alto a sinistra dello schermo.

Sono stati aggiunti nuovi snippet all’editor.

## Personalizzare le etichette della versione del contenuto XML

Per impostazione predefinita, gli autori possono creare etichette a loro scelta e associarle a file di argomento. Ciò può portare a diverse variazioni sulla stessa etichetta. Per evitare etichette incoerenti, è inoltre possibile scegliere tra elenchi di etichette predefinite.

1. Nella schermata Navigazione, fai clic sul pulsante [!UICONTROL **Strumenti**] icona.

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello a sinistra.

1. Fai clic sul pulsante [!UICONTROL **Profili cartella**] piastrelle.

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Seleziona un profilo cartella.

1. Fai clic sul pulsante [!UICONTROL **Configurazione editor XML**] scheda .

1. In Etichette versione contenuto XML, fai clic su [!UICONTROL **Scarica**].

   ![Etichette di download](images/lesson-4/download-labels.png)

Ora puoi personalizzare le etichette in base alle tue esigenze.

## Caricare le etichette della versione del contenuto XML

Dopo aver scaricato e modificato le etichette, puoi caricare l’argomento Etichetta versione contenuto XML . È possibile scegliere di utilizzare il file di esempio _label.json_, con l’insieme di argomenti di supporto per questa lezione.

1. Nel profilo della cartella, fai clic sul pulsante [!UICONTROL **Configurazione editor XML**] scheda .

1. In Etichette versione contenuto XML, fai clic su [!UICONTROL **Carica**].

   ![Caricare etichette](images/lesson-4/upload-labels.png)

1. Fai doppio clic sul file per le etichette personalizzate o sul file di esempio fornito qui.

   ![File di etichette di esempio](images/lesson-4/sample-labels-file.png)

1. Fai clic su [!UICONTROL **Salva**] nell’angolo in alto a sinistra dello schermo.

Le etichette della versione del contenuto XML personalizzato sono state caricate.
