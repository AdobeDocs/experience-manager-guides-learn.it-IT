---
title: Condizioni
description: Utilizzo delle condizioni nelle AEM
exl-id: 2cb670d9-1a22-47c6-8409-52d1d526010a
source-git-commit: 01083e771baced42146044bf319d3897a2c5f51b
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 3%

---

# Condizioni

In DITA, le condizioni sono spesso guidate da attributi come Prodotto, Piattaforma e Pubblico. A queste possono anche essere assegnati valori specifici. Gli utenti possono controllare tutto questo tramite Profili cartella.

I file di esempio che è possibile scegliere di utilizzare per questa lezione sono forniti nel file [condition.zip](assets/conditions.zip).

>[!VIDEO](https://video.tv.adobe.com/v/342755)

## Assegnare condizioni a un profilo cartella

1. Seleziona la **Profili cartella** piastrelle.

2. Fai clic su [!UICONTROL **Attributi condizionali**].

3. Fai clic su [!UICONTROL **Modifica**] nell’angolo in alto a sinistra del profilo.

4. Fate clic su [!UICONTROL **Aggiungi**].

   ![Condizioni nei profili cartella](images/lesson-13/add-name.png)

5. Compila i campi richiesti.

   - Il Nome deve corrispondere a un attributo utilizzato per il profiling.

   - Il valore è la voce esatta che verrà utilizzata nell&#39;origine del codice DITA.

   - Etichetta è la parola che verrà visualizzata dall’utente che immette gli attributi.

6. Fai clic su [!UICONTROL **Salva**].

>[!NOTE]
>
>NOTA: la configurazione di un profilo globale può essere un modo rapido ed efficiente per controllare l’uso di attributi e valori per seguire una guida di stile coerente.

## Assegnare attributi agli elementi

Se a un concetto non è stato assegnato alcun profilo cartella personalizzato, puoi assegnare attributi a elementi specifici, ad esempio paragrafi.

1. Da **Visualizzazione archivio**, fai clic sull’elemento con cui desideri lavorare per selezionarlo.

2. In **Proprietà contenuto** fai clic sul pulsante [!UICONTROL **Attributo**] a discesa.

3. Scegliere l&#39;attributo da assegnare.

4. Aggiungi un **Valore**.

L’associazione attributo e valore ora viene assegnata all’elemento selezionato.

## Assegnare coppie attributo e valore utilizzando le condizioni

Il pannello Condizioni consente l’assegnazione controllata delle coppie Attributo e Valore.

1. Modifica la **Preferenze utente**.

   a) Fai clic sull’icona Preferenze utente .

   ![Icona Preferenze utente](images/lesson-13/user-prefs-icon.png)

   b) Compila i campi richiesti nella sezione **Preferenze utente** finestra di dialogo. Esempio:

   ![Preferenze utente](images/lesson-13/user-preferences.png)

   c. Fai clic su [!UICONTROL **Salva**].

2. Dal pannello condizioni, espandi i menu a discesa per Audience e Platform. Le condizioni disponibili sono specifiche per il profilo cartella.

3. Trascina e rilascia una condizione sull’elemento desiderato per assegnarla.

## Assegnare uno schema soggetto

Le mappe dello Schema dell&#39;oggetto sono una forma specializzata di mappa a fossato e sono indicate da una mappa. Gli schemi soggetti vengono utilizzati per definire le tassonomie. Essi forniscono il controllo sui valori disponibili.

1. Passa a **Visualizzazione archivio**.

2. Selezionare una mappa che fa riferimento alla mappa a video dell&#39;oggetto Schema. In questo esempio viene utilizzata la mappa denominata _Progettazione e layout_.

   ![Preferenze utente](images/lesson-13/subject-scheme-map.png)

3. Configura le preferenze utente.

   a) Fai clic sul pulsante [!UICONTROL **Preferenze utente**] icona.

   ![Preferenze utente](images/lesson-13/user-prefs-icon-2.png)

   b) Popolare i campi nel **Preferenze utente** finestra di dialogo.

   c. Fai clic sul simbolo della cartella accanto al campo Percorso base per scegliere il percorso del file desiderato.

   d. Fai clic su [!UICONTROL **Seleziona**].

   e. Fai clic sul simbolo di chiave accanto al **Mappa principale** per inserire un percorso.

   >[!IMPORTANT]
   >
   >Importante: la mappa radice selezionata deve essere la mappa contenente lo schema soggetto.

   ![Preferenze utente](images/lesson-13/user-preferences-2.png)

   f. Per limitare le risorse visualizzate, seleziona le cartelle da utilizzare.

   g. Fai clic su [!UICONTROL **Seleziona**].

   h. Fai clic su [!UICONTROL **Salva**].

È stato assegnato lo schema oggetto.

## Visualizza lo schema oggetto dal pannello Condizioni

1. Passa a **Impostazioni editor**.

2. Seleziona la **Condizioni** scheda .

3. Seleziona la casella **Mostra schema oggetto nel pannello Condizioni**
