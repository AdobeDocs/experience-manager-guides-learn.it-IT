---
title: Profili cartella
description: Creazione e utilizzo di profili di cartelle per le guide AEM
exl-id: 5a0daa68-51ae-42d0-8320-6e8bdb1fe545
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# Profili cartella

L’AEM fornisce un accesso rapido agli strumenti di configurazione. Personalizzando i profili cartella, diversi reparti o prodotti possono disporre di modelli, ambienti di authoring, profili di attributi condizionali, snippet o configurazioni dell’editor web univoche.

I file di esempio che puoi scegliere di utilizzare per questa lezione sono forniti nel file [folderprofiles.zip](assets/folderprofiles.zip).

>[!VIDEO](https://video.tv.adobe.com/v/342758?quality=12&learn=on)

## Accedere ai profili delle cartelle

Le configurazioni vengono gestite tramite l’icona Profili cartella.

1. Dalla schermata Navigazione, fai clic su [!UICONTROL **Strumenti**] icona.

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello sinistro.

1. Fai clic su [!UICONTROL **Profili cartella**] affiancare.

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Seleziona il profilo desiderato. Ad esempio, scegli **Profilo globale**, che è il profilo predefinito.

   ![Profilo globale](images/lesson-3/global-profile-tile.png)

## Modificare gli attributi condizionali nel profilo globale

Dopo aver effettuato l’accesso al Profilo globale puoi modificarne la configurazione. Le impostazioni Profilo globale vengono applicate a tutti gli utenti, salvo diversa indicazione.

1. Nel Profilo globale, seleziona la **Attributi condizionali** scheda.

1. Clic [!UICONTROL **Modifica**] nell’angolo in alto a sinistra dello schermo.

   ![Attributi condizionali](images/lesson-3/edit-conditional-attributes.png)

1. Clic [!UICONTROL **Aggiungi**].

1. Popolare il **Nome**, **Valore**, e **Etichetta** campi per la nuova condizione.

   ![nuova condizione](images/lesson-3/new-condition.png)

1. Clic [!UICONTROL **Salva**] nell&#39;angolo in alto a sinistra dello schermo.
La nuova condizione è ora disponibile per tutti gli utenti. Potete selezionarla nel pannello Proprietà contenuto e applicarla al contenuto in base alle esigenze.

## Creare un nuovo profilo cartella

Oltre al profilo globale predefinito, puoi creare profili personalizzati.

1. Dalla schermata Navigazione, fai clic su [!UICONTROL **Strumenti**] icona.

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello sinistro.

1. Fai clic su [!UICONTROL **Profili cartella**] affiancare.

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Fai clic su [!UICONTROL **Crea**].

1. Nella finestra di dialogo Crea profilo cartella.

   a. Denomina il profilo.

   b. Specifica un percorso.

   c. Fai clic su [!UICONTROL **Crea**].

   ![Crea profilo cartella](images/lesson-3/create-folder-profile.png)

Nella pagina Profili cartella viene visualizzata una sezione con il nuovo nome del profilo.

## Aggiungere utenti amministratori dalla scheda Generale

Gli utenti amministratori dispongono delle autorizzazioni per aggiornare Attributi condizionali, Modello di authoring e Predefiniti di output per il Profilo cartella.

1. Fai clic sul riquadro per aprire il profilo cartella desiderato.

   ![Modifica profilo cartella](images/lesson-3/edit-folder-profile.png)

1. Seleziona la **Generale** scheda.

1. Clic [!UICONTROL **Modifica**] in alto a sinistra sullo schermo.

1. In Utenti amministratori, seleziona un utente dal menu a discesa o digita il nome di un utente.

1. Clic [!UICONTROL **Aggiungi**].

   Se necessario, puoi aggiungere più utenti amministratore.

   ![Aggiungi amministratore](images/lesson-3/add-admin.png)

1. Clic [!UICONTROL **Salva**] nell’angolo in alto a destra dello schermo, quando tutti gli utenti sono stati aggiunti.

Gli utenti amministrativi vengono ora assegnati a questo profilo.

## Aggiungere un nuovo pubblico dalla scheda Attributi condizionali

Dopo aver effettuato l’accesso al Profilo globale puoi modificarne la configurazione. Le impostazioni Profilo globale vengono applicate a tutti gli utenti, salvo diversa indicazione.

1. Dall’interno del Profilo cartella desiderato, seleziona la **Attributi condizionali** scheda.

1. Clic [!UICONTROL **Modifica**] nell’angolo in alto a sinistra dello schermo.

   ![Modifica attributi condizionali 2](images/lesson-3/edit-conditional-attributes-2.png)

1. Clic [!UICONTROL **Aggiungi**].

1. Popolare il **Nome**, **Valore**, e **Etichetta** campi per la nuova condizione.

   Facendo clic su [!UICONTROL **Più**] consente di aggiungere altre coppie Valore ed Etichetta per l&#39;attributo denominato.

   ![Aggiungi condizioni](images/lesson-3/add-conditions.png)

1. Clic [!UICONTROL **Salva**] nell&#39;angolo in alto a sinistra dello schermo.

I nuovi Attributi condizionali sono stati aggiunti a questo profilo.

## Scegli un modello e mappalo dalla scheda Authoring dei modelli

Le guide AEM includono modelli e mappe per l’authoring pronti all’uso. Puoi limitarli a autori specifici. Per impostazione predefinita, i modelli vengono memorizzati nella posizione Risorse all&#39;interno di una cartella di modelli DITA.

1. Dall’interno del Profilo cartella desiderato, seleziona la scheda Authoring Templates (Creazione di modelli).

1. Fai clic su Modifica nell’angolo in alto a sinistra della schermata.

1. Aggiungi un modello mappa.

   a. Dal **Modelli mappa** , seleziona un’opzione dalle mappe disponibili.

   b. Fai clic su [!UICONTROL **Aggiungi**].

   ![Modelli mappa](images/lesson-3/map-templates.png)

1. Aggiungi un modello di argomento.

   a. Dal **Modelli di argomento** , seleziona un’opzione dai modelli disponibili.

   ![Modelli di argomento](images/lesson-3/topic-templates.png)

1. Clic [!UICONTROL **Aggiungi**].

1. Se necessario, aggiungi altri modelli di argomento.

1. Al termine, fai clic su [!UICONTROL **Salva**] in alto a sinistra sullo schermo.

A questo profilo sono stati aggiunti i nuovi modelli di authoring.

## Eliminare i predefiniti non essenziali dalla scheda Predefiniti di output

Puoi configurare ogni predefinito di output in base al profilo della cartella. I predefiniti di output non necessari devono essere rimossi.

1. Dall’interno del Profilo cartella desiderato, seleziona la **Predefiniti di output** scheda.

1. Nel pannello a sinistra, seleziona le caselle di controllo degli eventuali predefiniti che non sono necessari.

   ![Elimina predefiniti](images/lesson-3/delete-presets.png)

1. Clic [!UICONTROL **Elimina predefinito**] nell’angolo in alto a sinistra dello schermo.

1. Nella finestra di dialogo Elimina predefinito, fai clic su [!UICONTROL **Elimina**].

   ![Eliminare](images/lesson-3/delete.png)

Ora gli unici predefiniti di output mostrati sono quelli che verranno utilizzati.

## Caricare un frammento di codice dalla scheda Configurazione dell&#39;editor XML

1. Dall’interno del Profilo cartella desiderato, seleziona la **Configurazione editor XML** scheda.

1. In Snippet editor XML fare clic su [!UICONTROL **Carica**].

   ![Carica snippet](images/lesson-3/upload-snippet.png)

1. Passare a uno snippet creato in precedenza.

1. Clic [!UICONTROL **Apri**].

1. Clic [!UICONTROL **Salva**] in alto a sinistra sullo schermo.

La configurazione dell&#39;editor è stata modificata per includere snippet.

## Specificare il profilo della cartella nel repository

Nell’editor, puoi visualizzare i risultati delle modifiche apportate ai Profili cartella.

1. Accedi a **Vista archivio**.

1. Fai clic sulla cartella del contenuto che desideri utilizzare.

1. Fai clic su [!UICONTROL **Preferenze utente**] nella barra degli strumenti superiore.

   ![Preferenze utente](images/lesson-3/hr-user-prefs.png)

1. Nella finestra di dialogo Preferenze utente, seleziona il Profilo cartella desiderato dal menu a discesa.

   ![Seleziona preferenze utente](images/lesson-3/select-user-pref.png)

1. Fai clic su [!UICONTROL **Salva**].

Hai applicato il Profilo cartella al contenuto. Ora, quando si crea un nuovo argomento DITA, viene visualizzato un elenco limitato di tipi di argomento in base al profilo cartella. La Condizione pubblico contiene le impostazioni globali e quelle specifiche del Profilo cartella. Il file Snippet caricato ha creato un set di snippet predefiniti tra cui scegliere. Nel dashboard Mappa vengono visualizzati i predefiniti di output con restrizioni.
