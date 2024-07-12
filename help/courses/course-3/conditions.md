---
title: Condizioni
description: Utilizzo delle condizioni nelle guide AEM
exl-id: 2cb670d9-1a22-47c6-8409-52d1d526010a
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 1%

---

# Condizioni

In DITA, le condizioni sono spesso guidate tramite attributi come Prodotto, Piattaforma e Pubblico. A questi possono essere assegnati anche valori specifici. Gli utenti possono controllare tutto questo tramite Profili cartella.

I file di esempio che si può scegliere di utilizzare per questa lezione sono forniti nel file [conditions.zip](assets/conditions.zip).

>[!VIDEO](https://video.tv.adobe.com/v/342755?quality=12&learn=on)

## Assegnare condizioni a un profilo cartella

1. Selezionare il riquadro **Profili cartella**.

1. Fare clic su [!UICONTROL **Attributi condizionali**].

1. Fai clic su [!UICONTROL **Modifica**] nell&#39;angolo superiore sinistro del profilo.

1. Fare clic su [!UICONTROL **Aggiungi**].

   ![Condizioni nei profili cartella](images/lesson-13/add-name.png)

1. Compila i campi obbligatori.

   - Il nome deve corrispondere a un attributo utilizzato per la profilatura.

   - Il valore è la voce esatta che verrà utilizzata nell&#39;origine del codice DITA.

   - Etichetta è la parola che verrà visualizzata dall&#39;utente che immette gli attributi.

1. Fai clic su [!UICONTROL **Salva**].

>[!NOTE]
>
>NOTA: la configurazione di un profilo globale può essere un modo rapido ed efficiente per controllare l’utilizzo di attributi e valori in modo da seguire una guida di stile coerente.

## Assegna attributi agli elementi

Se a un concetto non è stato assegnato alcun profilo di cartella personalizzato, è possibile assegnare attributi a elementi specifici, ad esempio i paragrafi.

1. Dalla **Vista archivio**, fare clic sull&#39;elemento che si desidera utilizzare per selezionarlo.

1. Nel pannello **Proprietà contenuto**, fai clic sul menu a discesa [!UICONTROL **Attributo**].

1. Scegliere l&#39;attributo che si desidera assegnare.

1. Aggiungi un **valore**.

L’associazione di attributi e valori viene ora assegnata all’elemento selezionato.

## Assegnare coppie di attributi e valori utilizzando le condizioni

Il pannello Condizioni consente l’assegnazione controllata delle coppie Attributo/Valore.

1. Modifica le **preferenze utente**.

   a. Fai clic sull’icona Preferenze utente.

   ![Icona Preferenze Utente](images/lesson-13/user-prefs-icon.png)

   b. Compila i campi obbligatori nella finestra di dialogo **Preferenze utente**. Ad esempio:

   ![Preferenze utente](images/lesson-13/user-preferences.png)

   c. Fai clic su [!UICONTROL **Salva**].

1. Dal pannello Condizioni, espandi i menu a discesa per Pubblico e Platform. Le condizioni disponibili sono specifiche per il profilo della cartella.

1. Trascina e rilascia una condizione sull’elemento desiderato per assegnarla.

## Assegna uno schema soggetto

Le mappe dello schema dei soggetti sono una forma specializzata di mappa digitale e sono referenziate da una mappa. Gli schemi oggetto vengono utilizzati per definire le tassonomie. Essi forniscono il controllo sui valori disponibili.

1. Passare alla **Visualizzazione archivio**.

1. Selezionate una mappa che faccia riferimento al mapping dello schema soggetto. In questo esempio viene utilizzata la mappa denominata _Progettazione e layout_.

   ![Preferenze utente](images/lesson-13/subject-scheme-map.png)

1. Configurare le preferenze utente.

   a. Fai clic sull&#39;icona [!UICONTROL **Preferenze utente**].

   ![Preferenze utente](images/lesson-13/user-prefs-icon-2.png)

   b. Compila i campi nella finestra di dialogo **Preferenze utente**.

   c. Fare clic sul simbolo della cartella accanto al campo Percorso base per scegliere il percorso del file desiderato.

   d. Fai clic su [!UICONTROL **Seleziona**].

   e. Fai clic sul simbolo della chiave accanto al campo **Root Map** per immettere un percorso.

   >[!IMPORTANT]
   >
   >Importante: la mappa principale selezionata deve essere la mappa che contiene lo schema dell&#39;oggetto.

   ![Preferenze utente](images/lesson-13/user-preferences-2.png)

   f. Limita le risorse visualizzate selezionando le cartelle da utilizzare.

   g. Fai clic su [!UICONTROL **Seleziona**].

   h. Fai clic su [!UICONTROL **Salva**].

Lo schema soggetto è stato assegnato.

## Visualizzare lo schema soggetto dal pannello Condizioni

1. Passa a **Impostazioni editor**.

1. Selezionare la scheda **Condizioni**.

1. Selezionare la casella **Mostra schema soggetto nel pannello Condizioni**
