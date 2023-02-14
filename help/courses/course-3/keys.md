---
title: Chiavi
description: Le chiavi consentono di includere informazioni sulle variabili quando si lavora con DITA nelle guide AEM
exl-id: cb64e094-fe6d-4a5e-8f0e-25ae58aaa2c6
source-git-commit: 1c4d278a05f2612bc55ce277efb5da2e6a0fa9a9
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Chiavi

Diversi tipi di materiali possono contenere informazioni simili che devono essere personalizzate in luoghi selezionati. Le chiavi consentono di includere informazioni sulle variabili in quando si lavora con DITA.

I file di esempio che è possibile scegliere di utilizzare per questa lezione sono forniti nel file [keys.zip](assets/keys.zip).

>[!VIDEO](https://video.tv.adobe.com/v/342756?quality=12&learn=on)

## Abilita chiavi

1. Carica il set di file di esempio forniti.

   a) Carica il file zip.

   b) Aggiorna l’ambiente AEM.

   c. Seleziona il file da estrarre.

   ![Seleziona ZIP](images/lesson-9/select-zip.png)

   d. Fai clic su [!UICONTROL **Extract Archive**] nella barra degli strumenti superiore.

   ![Barra degli strumenti](images/lesson-9/extract-archive.png)

   e. Nella finestra di dialogo, scegli il percorso specifico per i file da estrarre, ad esempio una cartella denominata Tasti.

   f. Fai clic su [!UICONTROL **Successivo**].

   g. Ignora eventuali conflitti in quanto non esistono per contenuti mai caricati in precedenza.

   h. Seleziona [!UICONTROL **Extract**] in alto a destra dello schermo.

2. Al termine dell&#39;estrazione, fai clic su [!UICONTROL **Vai alla cartella di destinazione**].

   ![Conferma](images/lesson-9/go-to-target.png)

## Risolvere le chiavi ai valori di riferimento

Per utilizzare correttamente le chiavi, le Preferenze utente devono fare riferimento a una mappa specifica come mappa principale. All&#39;interno di questa mappa è presente una raccolta di chiavi, raggruppate all&#39;interno di un gruppo di argomenti. L&#39;apertura della mappa e degli argomenti risolve le chiavi in base ai valori a cui fa riferimento questa mappa.

1. Specificare una mappa principale.

   a) Dalla schermata Chiavi, apri una mappa.

   b) Configura le preferenze utente.

   c. Fai clic sul pulsante [!UICONTROL **Preferenze utente**] nella barra degli strumenti superiore.

   ![Barra degli strumenti superiore](images/lesson-9/author-view.png)

   d. Fai clic sull’icona chiave per specificare un **Mappa principale** che verrà utilizzato per risolvere i tasti.

   e. Seleziona le caselle di controllo per le risorse desiderate.

   ![Elenco a discesa Risorse](images/lesson-9/select-assets.png)

   f. Fai clic su [!UICONTROL **Seleziona**].

   g. **Salva** Preferenze utente.

2. Passa a **Vista mappa**.

3. Apri la mappa specificata.

Le chiavi sono risolte.

## Aggiungi manualmente un nuovo keydef

1. Apri una mappa con una mappa radice specificata.

2. Selezionare una chiave.

   ![Elenco a discesa Chiave](images/lesson-9/hybrid-key.png)

3. Inserisci un nuovo keydef.

   a) Fai clic su in una posizione valida nella mappa.

   b) Seleziona la **Keydef** nella barra degli strumenti superiore.

   ![Barra degli strumenti Keydef](images/lesson-9/key-icon.png)

   c. Nella finestra di dialogo Inserisci chiave, immetti un valore univoco per Tasti che abbia senso per la definizione che stai creando.

   d. Fai clic su [!UICONTROL **Inserisci**].

4. Aggiungi topicmeta all&#39;interno del keydef.

   a) Fai clic sul pulsante [!UICONTROL **Inserisci elemento**] nella barra degli strumenti superiore.

   ![Barra degli strumenti Keydef](images/lesson-9/add-icon.png)

   b) Nella finestra di dialogo Inserisci elemento, cerca e seleziona &quot;topicmeta&quot;.

5. Aggiungi le parole chiave all&#39;interno della topicmeta.

   a) Fai clic sul pulsante [!UICONTROL **Inserisci elemento**] nella barra degli strumenti superiore.

   ![Barra degli strumenti Keydef](images/lesson-9/add-icon.png)

   b) Nella finestra di dialogo Inserisci elemento, cerca e seleziona &quot;parole chiave&quot;.

6. Aggiungi una parola chiave all’interno di topicmeta.

   a) Fai clic sul pulsante [!UICONTROL **Inserisci elemento**] nella barra degli strumenti superiore.

   ![Barra degli strumenti Keydef](images/lesson-9/add-icon.png)

   b) In **Inserisci elemento** finestra di dialogo, cerca e seleziona &quot;parola chiave&quot;

7. Digita il valore per keydef nella parola chiave.

Nella mappa, il tuo keydef dovrebbe ora essere simile al seguente:

![Keydef completato](images/lesson-9/keydef.png)

## Configurare un keydef come frammento

Gli snippet sono piccoli frammenti di contenuto che possono essere riutilizzati in vari argomenti del progetto di documentazione. Invece di generare manualmente ogni keydef, puoi configurare un singolo keydef come snippet.

1. Seleziona un elemento keydef nella mappa.

2. Nel menu contestuale, fai clic su [!UICONTROL **Crea frammento**].

3. Nella finestra di dialogo Nuovo frammento, aggiungi un titolo e una descrizione.
È inoltre possibile rimuovere le chiavi o le definizioni di parole chiave esistenti dal Contenuto.

4. Fai clic su [!UICONTROL **Crea**].

5. Nel pannello a sinistra, seleziona **Frammenti**.

6. Trascina il frammento appena creato dal pannello Frammenti alla mappa.

7. Aggiorna la definizione chiave in base alle esigenze utilizzando Proprietà contenuto.
Una volta salvato e aggiornato, questo set di chiavi sarà disponibile per tutti gli utenti che hanno definito una mappa che contiene la stessa mappa principale.
