---
title: Profili cartella
description: Creazione e utilizzo di profili cartella per le guide AEM
exl-id: 5a0daa68-51ae-42d0-8320-6e8bdb1fe545
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# Profili cartella

AEM fornisce accesso rapido agli strumenti di configurazione. Personalizzando i Profili cartella, diversi reparti o prodotti possono disporre di modelli univoci, ambienti di authoring, profili di attributi condizionali, snippet o anche configurazioni dell’editor web.

I file di esempio che è possibile scegliere di utilizzare per questa lezione sono forniti nel file [cartella profiles.zip](assets/folderprofiles.zip).

>[!VIDEO](https://video.tv.adobe.com/v/342758?quality=12&learn=on)

## Accedere ai profili delle cartelle

Le configurazioni vengono gestite tramite l’icona Profili cartella .

1. Nella schermata Navigazione, fai clic sul pulsante [!UICONTROL **Strumenti**] icona.

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello a sinistra.

1. Fai clic sul pulsante [!UICONTROL **Profili cartella**] piastrelle.

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Seleziona il profilo desiderato. Ad esempio, scegli **Profilo globale**, che è il profilo predefinito.

   ![Profilo globale](images/lesson-3/global-profile-tile.png)

## Modificare gli attributi condizionali nel profilo globale

Una volta effettuato l’accesso al profilo globale, puoi modificarne la configurazione. Le impostazioni del profilo globale vengono applicate a tutti gli utenti, se non diversamente specificato.

1. Nel profilo globale, seleziona la **Attributi condizionali** scheda .

1. Fai clic su [!UICONTROL **Modifica**] nell’angolo in alto a sinistra dello schermo.

   ![Attributi condizionali](images/lesson-3/edit-conditional-attributes.png)

1. Fai clic su [!UICONTROL **Aggiungi**].

1. Popolare **Nome**, **Valore** e **Etichetta** campi per la nuova condizione.

   ![nuova condizione](images/lesson-3/new-condition.png)

1. Fai clic su [!UICONTROL **Salva**] nell’angolo in alto a sinistra dello schermo.
La nuova condizione è ora disponibile per tutti gli utenti. Puoi selezionarlo nel pannello Proprietà contenuto e applicarlo al contenuto come necessario.

## Creare un nuovo profilo cartella

Oltre al profilo globale predefinito, puoi creare profili personalizzati.

1. Nella schermata Navigazione, fai clic sul pulsante [!UICONTROL **Strumenti**] icona.

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello a sinistra.

1. Fai clic sul pulsante [!UICONTROL **Profili cartella**] piastrelle.

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Fai clic su [!UICONTROL **Crea**].

1. Nella finestra di dialogo Crea profilo cartella .

   a) Assegna un nome al profilo.

   b) Specifica un percorso.

   c. Fai clic su [!UICONTROL **Crea**].

   ![Crea profilo cartella](images/lesson-3/create-folder-profile.png)

Nella pagina Profili cartella viene visualizzata una porzione con il nuovo nome profilo.

## Aggiungi utenti amministrativi dalla scheda Generale

Gli utenti amministratori dispongono dei diritti per aggiornare gli attributi condizionali, i modelli di authoring e i predefiniti di output per il profilo cartella.

1. Fai clic sulla tessera per aprire il profilo cartella desiderato.

   ![Modifica profilo cartella](images/lesson-3/edit-folder-profile.png)

1. Seleziona la **Generale** scheda .

1. Fai clic su [!UICONTROL **Modifica**] in alto a sinistra sullo schermo.

1. In Utenti amministratori , seleziona un utente dal menu a discesa o digita il nome di un utente.

1. Fai clic su [!UICONTROL **Aggiungi**].

   Se necessario, puoi aggiungere più utenti amministratori.

   ![Aggiungi amministratore](images/lesson-3/add-admin.png)

1. Fai clic su [!UICONTROL **Salva**] nell’angolo in alto a destra dello schermo quando tutti gli utenti sono stati aggiunti.

Gli utenti amministratori vengono ora assegnati a questo profilo.

## Aggiungere un nuovo pubblico dalla scheda Attributi condizionali

Una volta effettuato l’accesso al profilo globale, puoi modificarne la configurazione. Le impostazioni del profilo globale vengono applicate a tutti gli utenti, se non diversamente specificato.

1. Dall’interno del profilo cartella desiderato, seleziona la **Attributi condizionali** scheda .

1. Fai clic su [!UICONTROL **Modifica**] nell’angolo in alto a sinistra dello schermo.

   ![Modifica attributi condizionali 2](images/lesson-3/edit-conditional-attributes-2.png)

1. Fai clic su [!UICONTROL **Aggiungi**].

1. Popolare **Nome**, **Valore** e **Etichetta** campi per la nuova condizione.

   Fai clic su [!UICONTROL **Plus**] sign consente di aggiungere coppie di valori ed etichette aggiuntive per l’attributo denominato.

   ![Aggiungi condizioni](images/lesson-3/add-conditions.png)

1. Fai clic su [!UICONTROL **Salva**] nell’angolo in alto a sinistra dello schermo.

I nuovi Attributi condizionali sono stati aggiunti a questo profilo.

## Scegliere un modello e una mappa dalla scheda Modelli di authoring

AEM Guide include modelli e mappe di authoring preconfigurati. Puoi limitarli a autori specifici. Per impostazione predefinita, i modelli sono memorizzati nella posizione Risorse all’interno di una cartella di modelli DITA.

1. Dall’interno del profilo cartella desiderato, seleziona la scheda Modelli di authoring .

1. Fai clic su Modifica nell’angolo in alto a sinistra dello schermo.

1. Aggiungi un modello mappa.

   a) Da **Modelli mappa** a discesa, seleziona un’opzione dalle mappe disponibili.

   b) Fai clic su [!UICONTROL **Aggiungi**].

   ![Modelli mappa](images/lesson-3/map-templates.png)

1. Aggiungi un modello di argomento.

   a) Da **Modelli di argomento** a discesa, seleziona un’opzione dai modelli disponibili.

   ![Modelli di argomento](images/lesson-3/topic-templates.png)

1. Fai clic su [!UICONTROL **Aggiungi**].

1. Aggiungi altri modelli di argomento come necessario.

1. Al termine, fai clic su [!UICONTROL **Salva**] in alto a sinistra sullo schermo.

I nuovi modelli di authoring sono stati aggiunti a questo profilo.

## Eliminare i predefiniti non essenziali dalla scheda Predefiniti di output

Puoi configurare ogni predefinito di output in base al profilo cartella. I predefiniti di output non necessari devono essere rimossi.

1. Dall’interno del profilo cartella desiderato, seleziona la **Predefiniti di output** scheda .

1. Nel pannello a sinistra, seleziona le caselle di controllo di eventuali predefiniti non richiesti.

   ![Elimina predefiniti](images/lesson-3/delete-presets.png)

1. Fai clic su [!UICONTROL **Elimina predefinito**] nell’angolo in alto a sinistra dello schermo.

1. Nella finestra di dialogo Elimina predefinito, fai clic su [!UICONTROL **Elimina**].

   ![Eliminare](images/lesson-3/delete.png)

Gli unici predefiniti di output visualizzati sono quelli che verranno utilizzati.

## Caricare un frammento dalla scheda Configurazione dell’editor XML

1. Dall’interno del profilo cartella desiderato, seleziona la **Configurazione editor XML** scheda .

1. In Frammenti editor XML, fai clic su [!UICONTROL **Carica**].

   ![Carica snippet](images/lesson-3/upload-snippet.png)

1. Passa a uno snippet creato in precedenza.

1. Fai clic su [!UICONTROL **Apri**].

1. Fai clic su [!UICONTROL **Salva**] in alto a sinistra sullo schermo.

La configurazione dell’editor è stata modificata per includere i frammenti.

## Specificare il profilo cartella nel repository

Nell’Editor è possibile visualizzare i risultati delle modifiche apportate ai Profili cartella.

1. Passa a **Visualizzazione archivio**.

1. Fai clic sulla cartella del contenuto con cui desideri lavorare.

1. Fai clic sul pulsante [!UICONTROL **Preferenze utente**] nella barra degli strumenti superiore.

   ![Preferenze utente](images/lesson-3/hr-user-prefs.png)

1. Nella finestra di dialogo Preferenze utente, seleziona il profilo cartella desiderato dal menu a discesa.

   ![Seleziona Preferenze utente](images/lesson-3/select-user-pref.png)

1. Fai clic su [!UICONTROL **Salva**].

Hai applicato il profilo cartella al contenuto. Ora, quando si crea un nuovo argomento DITA, viene visualizzato un elenco ristretto di tipi di argomento in base al profilo cartella. La condizione di pubblico contiene le impostazioni globali e quelle specifiche del profilo cartella. Il file Snippets caricato ha creato un set di snippet predefiniti tra cui scegliere. Il dashboard mappa visualizza i predefiniti di output con restrizioni.
