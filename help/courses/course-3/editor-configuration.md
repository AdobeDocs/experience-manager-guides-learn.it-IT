---
title: Configurazione editor guide AEM
description: Configurazione dell’editor per le guide AEM
exl-id: 437d9598-4afc-431f-81bd-6762e22656b7
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 0%

---

# Configurazione editor XML

Se lavori in un ambiente restrittivo, puoi scegliere quali funzioni gli autori possono visualizzare personalizzando la configurazione dell’editor all’interno di un profilo di cartella specifico. L’applicazione di questo profilo cartella può modificare l’aspetto dell’editor stesso, dei modelli CSS, dei frammenti disponibili e delle etichette di versione del contenuto.

I file di esempio che puoi scegliere di utilizzare per questa lezione sono forniti nel file [xmleditorconfiguration.zip](assets/xmleditorconfiguration.zip).

>[!VIDEO](https://video.tv.adobe.com/v/342762?quality=12&learn=on)

## Personalizzare la configurazione predefinita dell’interfaccia utente dell’editor

Puoi sempre scaricare la configurazione dell’interfaccia utente predefinita nel sistema locale, modificarla nell’editor di testo desiderato e caricarla di nuovo.

1. Dalla schermata Navigazione, fai clic su [!UICONTROL **Strumenti**] icona.

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello sinistro.

1. Fai clic su [!UICONTROL **Profili cartella**] affiancare.

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Seleziona un profilo cartella.

1. Fai clic su [!UICONTROL **Configurazione editor XML**] scheda.

1. Clic [!UICONTROL **Scarica**] Impostazione predefinita.

   ![Scarica predefinito](images/lesson-4/download-default.png)

Ora puoi aprire e modificare il contenuto in un editor di testo. Il _Installazione e configurazione delle guide AEM_ La Guida contiene esempi di come rimuovere, personalizzare o aggiungere funzioni alla configurazione dell’interfaccia utente.

## Carica la configurazione dell&#39;interfaccia utente dell&#39;editor XML modificato

Dopo aver personalizzato la configurazione dell’interfaccia utente, puoi caricarla. Un esempio di file di configurazione _ui-config-restricted-editor.json_ viene fornito con il set di argomenti di supporto per questa lezione.

1. Nel Profilo cartella, fai clic su [!UICONTROL **Configurazione editor XML**] scheda.

1. In Configurazione interfaccia utente editor XML fare clic su [!UICONTROL **Carica**].

   ![Caricare](images/lesson-4/upload.png)

1. Fai doppio clic sul file della configurazione dell’interfaccia utente modificata o, come mostrato qui, sul file di esempio fornito.

   ![File di configurazione di esempio](images/lesson-4/sample-config-file.png)

1. Clic [!UICONTROL **Salva**] nell’angolo in alto a sinistra dello schermo.

La configurazione dell&#39;interfaccia utente modificata è stata caricata correttamente.

## Personalizzare il layout del modello CSS

Come per la configurazione dell’interfaccia utente, puoi scaricare il layout del modello CSS. Puoi aprirlo in un editor di testo e apportare modifiche per personalizzare l’aspetto dell’argomento prima di caricarlo.

1. Dalla schermata Navigazione, fai clic su [!UICONTROL **Strumenti**] icona.

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello sinistro.

1. Fai clic su [!UICONTROL **Profili cartella**] affiancare.

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Seleziona un profilo cartella.

1. Fai clic su [!UICONTROL **Configurazione editor XML**] scheda.

1. In Layout modello CSS, fai clic su [!UICONTROL **Scarica**].

   ![Scarica CSS](images/lesson-4/download-css.png)

Ora puoi modificare e salvare il contenuto CSS in un editor di testo.

## Carica il layout modificato del modello CSS

Dopo aver personalizzato il layout del modello CSS, puoi caricarlo. Tieni presente che un file di esempio _css-layout-ONLY-draft-comment-change.css_ viene fornito con il set di argomenti di supporto per questa lezione. Questo file contiene solo la bozza di modifica del commento, mentre _css-layout-draft-comment-change.css_ è l’intero file, disponibile solo a scopo di test o revisione.

1. Nel Profilo cartella, fai clic su [!UICONTROL **Configurazione editor XML**] scheda.

1. In Layout modello CSS, fai clic su [!UICONTROL **Carica**].

   ![Carica CSS](images/lesson-4/upload-css.png)

1. Fai doppio clic sul file per il layout CSS personalizzato o sul file di esempio fornito, come mostrato qui.

   ![File CSS di esempio](images/lesson-4/sample-css-file.png)

1. Clic [!UICONTROL **Salva**] nell’angolo in alto a sinistra dello schermo.
Il layout del modello CSS personalizzato è stato caricato correttamente.

## Modifica snippet editor XML

I frammenti sono parti di contenuto riutilizzabili che possono essere specifiche per un prodotto o un gruppo. Gli esempi di snippet vengono forniti con i file di supporto per questa lezione.

1. Dalla schermata Navigazione, fai clic su [!UICONTROL **Strumenti**] icona.

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello sinistro.

1. Fai clic su [!UICONTROL **Profili cartella**] affiancare.

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Seleziona un profilo cartella.

1. Fai clic su [!UICONTROL **Configurazione editor XML**] scheda.

1. In Snippet editor XML fare clic su **Carica**.

   ![Carica snippet](images/lesson-4/upload-snippets.png)

1. Scegli i tuoi snippet o utilizza gli esempi forniti.

   ![Frammento di esempio](images/lesson-4/sample-snippet.png)

1. Clic [!UICONTROL **Salva**] nell’angolo in alto a sinistra dello schermo.

I nuovi snippet sono stati aggiunti all&#39;editor.

## Personalizza etichette versione contenuto XML

Per impostazione predefinita, gli autori possono creare etichette di propria scelta e associarle ai file di argomento. Questo può portare a diverse varianti sulla stessa etichetta. Per evitare etichette incoerenti, puoi anche scegliere tra elenchi di etichette predefinite.

1. Dalla schermata Navigazione, fai clic su [!UICONTROL **Strumenti**] icona.

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello sinistro.

1. Fai clic su [!UICONTROL **Profili cartella**] affiancare.

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Seleziona un profilo cartella.

1. Fai clic su [!UICONTROL **Configurazione editor XML**] scheda.

1. In Etichette versione contenuto XML fare clic su [!UICONTROL **Scarica**].

   ![Etichette di download](images/lesson-4/download-labels.png)

Ora puoi personalizzare le etichette in base alle esigenze.

## Carica etichette versione contenuto XML

Dopo aver scaricato e modificato le etichette, è possibile caricare l&#39;argomento Etichetta versione contenuto XML. È possibile scegliere di utilizzare il file di esempio _labels.json_, viene fornito con il set di argomenti di supporto per questa lezione.

1. Nel Profilo cartella, fai clic su [!UICONTROL **Configurazione editor XML**] scheda.

1. In Etichette versione contenuto XML fare clic su [!UICONTROL **Carica**].

   ![Carica etichette](images/lesson-4/upload-labels.png)

1. Fai doppio clic sul file per le etichette personalizzate o sul file di esempio fornito, come mostrato qui.

   ![File etichette di esempio](images/lesson-4/sample-labels-file.png)

1. Clic [!UICONTROL **Salva**] nell’angolo in alto a sinistra dello schermo.

Sono state caricate le etichette di versione del contenuto XML personalizzato.
