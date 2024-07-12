---
title: Mappe e bookmap
description: Creazione e modifica di mappe e segnalibri in AEM Guides
exl-id: 9c717e4b-017b-4f2b-b93e-f2c0e7525c55
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 1%

---

# Mappe e Bookmap

Adobe Experience Manager Guides Map Editor consente di creare e modificare i file di mappa. Utilizzando l&#39;Editor mapping, è possibile modificare due tipi di file: DITA map e bookmap. Per i nostri scopi, consideriamo questi concetti ampiamente intercambiabili.
L&#39;Editor mappa è disponibile in due modalità: l&#39;Editor mappa di base e l&#39;Editor mappa avanzato.

>[!VIDEO](https://video.tv.adobe.com/v/342766?quality=12&learn=on)

## Creare una mappa

AEM Guides fornisce due modelli di mappe preconfigurati: mappa DITA e mappa segnalibro. Puoi anche creare modelli di mappa personalizzati e condividerli con gli autori per creare file di mappa.

Per creare un file di mappa, effettuare le seguenti operazioni.

1. Nell’interfaccia utente di Assets, individua il percorso in cui desideri creare il file mappa.

1. Fare clic su [!UICONTROL **Crea > Mappa DITA**].

1. Nella pagina Blueprint, seleziona il tipo di modelli di mappa che desideri utilizzare e fai clic su [!UICONTROL **Avanti**].

1. Nella pagina Proprietà, immetti un **Titolo** e un **Nome** per la mappa.

1. Fai clic su [!UICONTROL **Crea**].

## Apertura di una mappa con l’Editor mappe avanzato

1. Nell&#39;**interfaccia utente di Assets**, selezionare la mappa da modificare.

1. Fare clic su [!UICONTROL **Modifica argomenti**].

   ![Modifica interfaccia utente argomento](images/lesson-14/edit-topics.png)

Oppure

1. Passa il puntatore del mouse sull’icona della mappa.

1. Selezionare **Modifica argomenti** dal menu **Azione**.


## Aggiunta di contenuto a una mappa o a una mappa segnalibro

1. Passare alla **Visualizzazione archivio**.

1. Trascina e rilascia il contenuto dalla vista Archivio in posizioni valide nella mappa o nella mappa.

Oppure

1. Fare clic in una posizione valida all&#39;interno della mappa o della mappa.

1. Fare clic sull&#39;icona [!UICONTROL **Barra degli strumenti**] appropriata per aggiungere capitoli, argomenti o argomenti.

   ![Icone barra degli strumenti](images/lesson-14/toolbar-icons.png)

1. Scegli una o più Assets da aggiungere.

1. Fai clic su [!UICONTROL **Seleziona**].

### Promuovi o riduci di livello gli elementi di una mappa

Utilizza **Frecce della barra degli strumenti** per alzare di livello o abbassare di livello i capitoli e gli argomenti di una mappa o di un bookmap.

1. Seleziona un elemento nella mappa.

1. Fai clic sulla [!UICONTROL **freccia sinistra**] per promuovere un topicref in un capitolo o sulla [!UICONTROL **freccia destra**] per abbassare di livello un capitolo in un topicref.

   ![Icone freccia](images/lesson-14/toolbar-arrows.png)

1. Se necessario, salva e crea una versione della mappa.

Oppure

1. Trascina e rilascia gli elementi per riorganizzarli.

## Aggiunta di metadati a una mappa

1. Dalla **barra degli strumenti Mappa**, inserire un gruppo di argomenti.

   ![Aggiungi attributo](images/lesson-14/add-topicgroup.png)

1. Fare clic sull&#39;icona [!UICONTROL **Plus**] per inserire gli elementi.

1. Scegliere gli elementi da inserire.

   ![Inserisci metadati](images/lesson-14/insert-metadata.png)

1. Fai clic su [!UICONTROL **Chiudi**].

## Aggiunta di un reltable a una mappa

È possibile aggiungere un reltable dopo aver strutturato una mappa.

1. Fare clic nella mappa in cui si desidera inserire il reltable.

1. Utilizza l&#39;**icona della barra degli strumenti** per aggiungere il reltable alla mappa.

   ![Icona Reltable](images/lesson-14/reltable-icon.png)

1. Configura la finestra di dialogo.

1. Fare clic su [!UICONTROL **Inserisci**].

1. Trascinare gli argomenti richiesti dal **repository** nella tabella reltable.

1. È possibile copiare e incollare gli elementi richiesti dalla mappa nella tabella relable utilizzando le scelte rapide da tastiera standard.

## Assegnare attributi ai riferimenti argomento in una mappa

1. Evidenziare un topicref o una raccolta nidificata di topicref nella mappa.

1. In Altri attributi nel pannello Proprietà contenuto scegliere un **Attributo** e il relativo **Valore.**

   ![Aggiungi attributi](images/lesson-14/add-attribute.png)
