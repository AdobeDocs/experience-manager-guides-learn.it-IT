---
title: Profili cartella
description: Creazione e utilizzo di profili di cartelle per AEM Guides
exl-id: 5a0daa68-51ae-42d0-8320-6e8bdb1fe545
TQID: https://experienceleague.adobe.com/ztMvUcFQ-GJTOEU3ikB-2WFgj--ttbY7JoSyGW6Poa8
product_v2: id: fae5e35a-80c9-4b94-9352-1a060a6aab1did: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
feature_v2: id: ab01a588-7dea-43f2-a699-0b3f128465d6id: cb8c6a2a-3c38-4e40-867c-756f8c36bb0e
subfeature_v2: id: ad602516-aca3-4247-9ae8-f393d958efa9id: b0521e56-a0b2-40b6-bf47-ebc98751f9baid: b1ef4d86-3917-4b76-a0bc-4a4771f9b3b0id: f89f75b0-cf2e-4e96-aec8-fe8c39cbd0ef
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 27ffc636d63300fb2e99903d92cab12f0cfcbb25
workflow-type: tm+mt
source-wordcount: 917
ht-degree: 1%

---

# Profili cartella

AEM fornisce un accesso rapido agli strumenti di configurazione. Personalizzando i profili cartella, diversi reparti o prodotti possono disporre di modelli, ambienti di authoring, profili di attributi condizionali, snippet o configurazioni dell’editor web univoche.

I file di esempio che si può scegliere di utilizzare per questa lezione sono forniti nel file [folderprofiles.zip](assets/folderprofiles.zip).

>[!VIDEO](https://video.tv.adobe.com/v/342758?quality=12&learn=on)

## Accedere ai profili delle cartelle

Le configurazioni vengono gestite tramite l’icona Profili cartella.

1. Dalla schermata Navigazione, fai clic sull&#39;icona [!UICONTROL **Strumenti**].

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello a sinistra.

1. Fare clic sul riquadro [!UICONTROL **Profili cartella**].

   ![Profili cartella](images/reuse/folder-profiles-tile.png)

1. Seleziona il profilo desiderato. Scegliere ad esempio **Profilo globale**, che è il profilo predefinito.

   ![Profilo globale](images/lesson-3/global-profile-tile.png)

## Modificare gli attributi condizionali nel profilo globale

Dopo aver effettuato l’accesso al Profilo globale puoi modificarne la configurazione. Le impostazioni Profilo globale vengono applicate a tutti gli utenti, salvo diversa indicazione.

1. Nel profilo globale, selezionare la scheda **Attributi condizionali**.

1. Fai clic su [!UICONTROL **Modifica**] nell&#39;angolo superiore sinistro della schermata.

   ![Attributi condizionali](images/lesson-3/edit-conditional-attributes.png)

1. Fai clic su [!UICONTROL **Aggiungi**].

1. Compilare i campi **Nome**, **Valore** e **Etichetta** per la nuova condizione.

   ![nuova condizione](images/lesson-3/new-condition.png)

1. Fai clic su [!UICONTROL **Salva**] nell&#39;angolo superiore sinistro della schermata.
La nuova condizione è ora disponibile per tutti gli utenti. Potete selezionarla nel pannello Proprietà contenuto e applicarla al contenuto in base alle esigenze.

## Creare un nuovo profilo cartella

Oltre al profilo globale predefinito, puoi creare profili personalizzati.

1. Dalla schermata Navigazione, fai clic sull&#39;icona [!UICONTROL **Strumenti**].

   ![Icona Strumenti](images/reuse/tools-icon.png)

1. Seleziona **Guide** nel pannello a sinistra.

1. Fare clic sul riquadro [!UICONTROL **Profili cartella**].

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

1. Selezionare la scheda **Generale**.

1. Fai clic su [!UICONTROL **Modifica**] in alto a sinistra nella schermata.

1. In Utenti amministratori, seleziona un utente dal menu a discesa o digita il nome di un utente.

1. Fai clic su [!UICONTROL **Aggiungi**].

   Se necessario, puoi aggiungere più utenti amministratore.

   ![Aggiungi amministratore](images/lesson-3/add-admin.png)

1. Fai clic su [!UICONTROL **Salva**] nell&#39;angolo in alto a destra dello schermo quando tutti gli utenti sono stati aggiunti.

Gli utenti amministrativi vengono ora assegnati a questo profilo.

## Aggiungere un nuovo pubblico dalla scheda Attributi condizionali

Dopo aver effettuato l’accesso al Profilo globale puoi modificarne la configurazione. Le impostazioni Profilo globale vengono applicate a tutti gli utenti, salvo diversa indicazione.

1. Dall&#39;interno del Profilo cartella desiderato, selezionare la scheda **Attributi condizionali**.

1. Fai clic su [!UICONTROL **Modifica**] nell&#39;angolo superiore sinistro della schermata.

   ![Modifica attributi condizionali 2](images/lesson-3/edit-conditional-attributes-2.png)

1. Fai clic su [!UICONTROL **Aggiungi**].

1. Compilare i campi **Nome**, **Valore** e **Etichetta** per la nuova condizione.

   Facendo clic sul segno [!UICONTROL **Plus**] è possibile aggiungere altre coppie Valore/Etichetta per l&#39;attributo denominato.

   ![Aggiungi condizioni](images/lesson-3/add-conditions.png)

1. Fai clic su [!UICONTROL **Salva**] nell&#39;angolo superiore sinistro della schermata.

I nuovi Attributi condizionali sono stati aggiunti a questo profilo.

## Scegli un modello e mappalo dalla scheda Authoring dei modelli

AEM Guides viene fornito con modelli e mappe di authoring pronti all’uso. Puoi limitarli a autori specifici. Per impostazione predefinita, i modelli vengono memorizzati nella posizione Assets all&#39;interno di una cartella di modelli DITA.

1. Dall’interno del Profilo cartella desiderato, seleziona la scheda Authoring Templates (Creazione di modelli).

1. Fai clic su Modifica nell’angolo in alto a sinistra della schermata.

1. Aggiungi un modello mappa.

   a. Dal menu a discesa **Modelli mappa**, seleziona un&#39;opzione dalle mappe disponibili.

   b. Fai clic su [!UICONTROL **Aggiungi**].

   ![Modelli mappa](images/lesson-3/map-templates.png)

1. Aggiungi un modello di argomento.

   a. Dal menu a discesa **Modelli argomento**, seleziona un&#39;opzione dai modelli disponibili.

   ![Modelli di argomento](images/lesson-3/topic-templates.png)

1. Fai clic su [!UICONTROL **Aggiungi**].

1. Se necessario, aggiungi altri modelli di argomento.

1. Al termine, fai clic su [!UICONTROL **Salva**] in alto a sinistra nella schermata.

A questo profilo sono stati aggiunti i nuovi modelli di authoring.

## Eliminare i predefiniti non essenziali dalla scheda Predefiniti di output

Puoi configurare ogni predefinito di output in base al profilo della cartella. I predefiniti di output non necessari devono essere rimossi.

1. Dall&#39;interno del Profilo cartella desiderato, selezionare la scheda **Predefiniti output**.

1. Nel pannello a sinistra, seleziona le caselle di controllo degli eventuali predefiniti che non sono necessari.

   ![Elimina predefiniti](images/lesson-3/delete-presets.png)

1. Fai clic su [!UICONTROL **Elimina predefinito**] nell&#39;angolo superiore sinistro della schermata.

1. Nella finestra di dialogo Elimina predefinito fare clic su [!UICONTROL **Elimina**].

   ![Elimina](images/lesson-3/delete.png)

Ora gli unici predefiniti di output mostrati sono quelli che verranno utilizzati.

## Caricare un frammento di codice dalla scheda Configurazione dell&#39;editor XML

1. Dall&#39;interno del profilo cartella desiderato, selezionare la scheda **Configurazione editor XML**.

1. In Frammenti editor XML fare clic su [!UICONTROL **Carica**].

   ![Carica snippet](images/lesson-3/upload-snippet.png)

1. Passare a uno snippet creato in precedenza.

1. Fai clic su [!UICONTROL **Apri**].

1. Fai clic su [!UICONTROL **Salva**] in alto a sinistra nella schermata.

La configurazione dell&#39;editor è stata modificata per includere snippet.

## Specificare il profilo della cartella nel repository

Nell’editor, puoi visualizzare i risultati delle modifiche apportate ai Profili cartella.

1. Passare a **Visualizzazione archivio**.

1. Fai clic sulla cartella del contenuto che desideri utilizzare.

1. Fai clic sull&#39;icona [!UICONTROL **Preferenze utente**] nella barra degli strumenti superiore.

   ![Preferenze utente](images/lesson-3/hr-user-prefs.png)

1. Nella finestra di dialogo Preferenze utente, seleziona il Profilo cartella desiderato dal menu a discesa.

   ![Seleziona Preferenze Utente](images/lesson-3/select-user-pref.png)

1. Fai clic su [!UICONTROL **Salva**].

Hai applicato il Profilo cartella al contenuto. Ora, quando si crea un nuovo argomento DITA, viene visualizzato un elenco limitato di tipi di argomento in base al profilo cartella. La Condizione pubblico contiene le impostazioni globali e quelle specifiche del Profilo cartella. Il file Snippet caricato ha creato un set di snippet predefiniti tra cui scegliere. Nel dashboard Mappa vengono visualizzati i predefiniti di output con restrizioni.
