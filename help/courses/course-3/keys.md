---
title: Chiavi
description: Le chiavi consentono di includere informazioni sulle variabili in quando si lavora con DITA in AEM Guides
exl-id: cb64e094-fe6d-4a5e-8f0e-25ae58aaa2c6
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Chiavi

Diversi set di materiali possono contenere informazioni simili che devono essere personalizzate in punti selezionati. Le chiavi consentono di includere informazioni sulle variabili in quando si lavora con DITA.

I file di esempio che si può scegliere di utilizzare per questa lezione sono forniti nel file [keys.zip](assets/keys.zip).

>[!VIDEO](https://video.tv.adobe.com/v/342756?quality=12&learn=on)

## Abilita chiavi

1. Carica il set di file di esempio forniti.

   a. Carica il file zip.

   b. Aggiornare l’ambiente AEM.

   c. Seleziona il file per l’estrazione.

   ![Seleziona ZIP](images/lesson-9/select-zip.png)

   d. Fai clic su [!UICONTROL **Estrai archivio**] nella barra degli strumenti superiore.

   ![Barra degli strumenti](images/lesson-9/extract-archive.png)

   e. Nella finestra di dialogo, scegli il percorso specifico dei file da estrarre, ad esempio una cartella denominata Chiavi.

   f. Fai clic su [!UICONTROL **Avanti**].

   g. Ignora eventuali conflitti in quanto non esisteranno per contenuti mai caricati in precedenza.

   h. Seleziona [!UICONTROL **Estrai**] in alto a destra dello schermo.

1. Al termine dell&#39;estrazione, fare clic su [!UICONTROL **Vai alla cartella di destinazione**].

   ![Conferma](images/lesson-9/go-to-target.png)

## Risolvi chiavi ai valori di riferimento

Per utilizzare correttamente le chiavi, Preferenze utente deve fare riferimento a una mappa specifica come mappa principale. All&#39;interno di questa mappa è presente una raccolta di chiavi, raggruppate all&#39;interno di un gruppo di argomenti. L&#39;apertura della mappa e degli argomenti risolve le chiavi nei valori a cui fa riferimento la mappa.

1. Specificare una mappa radice.

   a. Dalla schermata Chiavi, apri una mappa.

   b. Configurare le preferenze utente.

   c. Fai clic sull&#39;icona [!UICONTROL **Preferenze utente**] nella barra degli strumenti superiore.

   ![Barra degli strumenti superiore](images/lesson-9/author-view.png)

   d. Fai clic sull&#39;icona chiave per specificare una **mappa principale** che verrà utilizzata per risolvere le chiavi.

   e. Seleziona le caselle di controllo per qualsiasi Assets desiderato.

   ![Elenco a discesa Assets](images/lesson-9/select-assets.png)

   f. Fai clic su [!UICONTROL **Seleziona**].

   g. **Salva** le preferenze utente.

1. Passare alla **vista mappa**.

1. Apri la mappa specificata.

Le chiavi vengono risolte.

## Aggiungere manualmente un nuovo keydef

1. Apri una mappa con una mappa radice specificata.

1. Seleziona una chiave.

   ![Elenco a discesa chiavi](images/lesson-9/hybrid-key.png)

1. Inserisce un nuovo keydef.

   a. Fai clic in una posizione valida nella mappa.

   b. Seleziona l&#39;icona **Keydef** nella barra degli strumenti superiore.

   ![Barra degli strumenti Keydef](images/lesson-9/key-icon.png)

   c. Nella finestra di dialogo Inserisci keydef, immettere un valore univoco per Chiavi che abbia senso per la definizione che si sta creando.

   d. Fare clic su [!UICONTROL **Inserisci**].

1. Aggiungere topicmeta all&#39;interno del keydef.

   a. Fai clic sull&#39;icona [!UICONTROL **Inserisci elemento**] nella barra degli strumenti superiore.

   ![Barra degli strumenti Keydef](images/lesson-9/add-icon.png)

   b. Nella finestra di dialogo Inserisci elemento, cerca e seleziona &quot;topicmeta&quot;.

1. Aggiungere parole chiave all&#39;interno dell&#39;argomento meta.

   a. Fai clic sull&#39;icona [!UICONTROL **Inserisci elemento**] nella barra degli strumenti superiore.

   ![Barra degli strumenti Keydef](images/lesson-9/add-icon.png)

   b. Nella finestra di dialogo Inserisci elemento, cerca e seleziona &quot;parole chiave&quot;.

1. Aggiungete una parola chiave all&#39;interno dell&#39;argomento meta.

   a. Fai clic sull&#39;icona [!UICONTROL **Inserisci elemento**] nella barra degli strumenti superiore.

   ![Barra degli strumenti Keydef](images/lesson-9/add-icon.png)

   b. Nella finestra di dialogo **Inserisci elemento**, cerca e seleziona &quot;parola chiave&quot;

1. Digitate il valore del keydef nella parola chiave.

Nella mappa, il keydef dovrebbe ora avere un aspetto simile al seguente:

![Keydef completato](images/lesson-9/keydef.png)

## Configurare un keydef come snippet

I frammenti sono piccoli frammenti di contenuto che possono essere riutilizzati in vari argomenti nel progetto di documentazione. Invece di generare manualmente ogni keydef, potete configurare un singolo keydef come snippet.

1. Selezionare un elemento keydef nella mappa.

1. Nel menu contestuale, fare clic su [!UICONTROL **Crea snippet**].

1. Nella finestra di dialogo Nuovo snippet, aggiungi un titolo e una descrizione.
Puoi anche rimuovere dal Contenuto le chiavi o le definizioni di parole chiave esistenti.

1. Fai clic su [!UICONTROL **Crea**].

1. Nel pannello sinistro, seleziona **Snippet**.

1. Trascinate sulla mappa lo snippet appena creato dal pannello Snippet.

1. Aggiorna il keydef in base alle esigenze utilizzando Proprietà contenuto.
Quando viene salvato e aggiornato, questo set di chiavi sarà disponibile per tutti gli utenti che hanno definito una mappa contenente la stessa mappa principale.
