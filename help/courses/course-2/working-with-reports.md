---
title: Utilizzo dei rapporti
description: Utilizzo dei rapporti in [!DNL Adobe Experience Manager Guides]
exl-id: 755506a6-c416-4a8c-8359-8db7e63a90a4
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 0%

---

# Utilizzo dei rapporti

La scheda Rapporti nel dashboard Mappa consente di identificare e risolvere i collegamenti interrotti, il contenuto a cui si fa riferimento e che viene riutilizzato (conref), i riferimenti incrociati o altre informazioni mancanti.

>[!VIDEO](https://video.tv.adobe.com/v/339039?quality=12&learn=on)

## Preparazione all&#39;esercizio

I file di esempio per l&#39;esercizio sono disponibili qui.

[Esercizio-Download](assets/exercises/working-with-reports.zip)

## Caricamento risorse

1. In Vista archivio, seleziona l’icona con i puntini di sospensione nella cartella principale per aprire il menu Opzioni.

   ![ellissi-9.png](images/ellipses-9.png)

1. Seleziona **[!UICONTROL Carica risorse]**.

   ![upload-assets.png](images/upload-assets.png)

1. Seleziona i file da caricare nella cartella e fai clic su **Carica**.

I file DITA vengono aperti ed è necessario esaminarli per individuare eventuali problemi relativi a contenuto, conref o riferimenti incrociati mancanti.

## Creazione di una mappa

1. Seleziona l’icona con i puntini di sospensione nella cartella principale per aprire il menu Opzioni.

   ![ellissi-9.png](images/ellipses-9.png)

1. Seleziona **Crea > Mappa**.

   ![create-map.png](images/create-map.png)

   Viene visualizzata la finestra di dialogo Crea nuova mappa.

1. Nel campo Modello, seleziona **Bookmap** (o **Mappa** in base al tipo di contenuto che stai creando) dal menu a discesa e assegna alla mappa un titolo.

1. Seleziona **Crea**.

La mappa viene creata e la barra a sinistra cambia automaticamente dalla vista Archivio alla vista Mappa.

## Inserimento di componenti mappa

1. Seleziona l’icona della matita nella barra a sinistra.
Questa è l’icona Modifica e ti consente di aprire la mappa nell’editor.

   ![edit-map.png](images/edit-map.png)

1. Torna alla vista Archivio selezionando l’icona Archivio.

   ![repository-button.png](images/repository-button.png)

1. Per aggiungere un argomento alla mappa, trascinalo dall’Archivio nella mappa nell’editor.
L&#39;indicatore di riga indica dove verrà posizionato l&#39;argomento.

1. Continua ad aggiungere argomenti in base alle esigenze.

1. Al termine, seleziona **Salva Come Nuova Versione.**

   ![salva come nuova versione.png](images/save-as-new-version.png)

1. In *Commenti per nuova versione* immettere un commento descrittivo.

1. Seleziona **Salva**.

## Generazione di un output del sito AEM

1. Nel repository, selezionare l&#39;icona con i puntini di sospensione sulla mappa per aprire il menu Opzioni, quindi **Apri Map Dashboard.**

   ![open-map-dashboard.png](images/open-map-dashboard.png)

   Il quadro comandi Mappa (Map Dashboard) si apre in un’altra scheda.
1. Nella scheda Predefiniti di output, selezionate **Sito AEM**.

   ![aem-site-checkbox](images/aem-site-checkbox.png)

1. Seleziona **Genera**.

1. Passare alla pagina Output per visualizzare lo stato degli output generati.
In caso di errori, nella scheda Output potrebbe essere visualizzato un cerchio arancione anziché verde sotto la colonna Impostazione generazione, a indicare che la generazione è stata completata.

1. Seleziona il collegamento nella colonna Impostazione generazione per aprire l’output generato.
Controlla l’output per individuare eventuali contenuti mancanti.

## Scheda Rapporti

Nella scheda Rapporti vengono visualizzati un riepilogo degli argomenti e una tabella contenente le informazioni sugli argomenti e i problemi presenti nella mappa.

Idealmente, dopo l’importazione dei contenuti, controlla sempre la presenza di una mappa nei Report.

![reports.png](images/reports.png)

La colonna Elementi mancanti indica il numero di immagini mancanti e di riferimenti interrotti. È possibile selezionare **Matita** per aprire l’argomento nell’editor.

## Risoluzione delle immagini mancanti

Se mancano immagini nei file, la causa comune potrebbe essere il caricamento del contenuto, ma non delle immagini. In tal caso, risolvi i problemi di immagine mancanti caricando le immagini in una cartella specifica corrispondente al percorso e ai nomi file previsti dai file.

1. In entrata *Vista archivio*, seleziona l’icona con i puntini di sospensione nella cartella delle immagini per aprire il menu Opzioni.

   ![image-ellipsis.png](images/image-ellipsis.png)

1. Seleziona **[!UICONTROL Carica risorse]** e seleziona le immagini mancanti.

1. Seleziona **Carica**.

Le immagini mancanti sono state caricate. Ora, un output del sito AEM appena generato visualizzerà queste immagini e la scheda Rapporti non mostrerà più eventuali errori di immagine mancanti.

## Risoluzione dei conflitti interrotti

Se il contenuto a cui si fa riferimento altrove (un riferimento conf) viene collegato a per un file all’interno di un’altra cartella (ad esempio, una denominata &quot;riutilizza&quot;). e il contenuto non viene caricato, è necessario risolvere un errore. Ad esempio, devi creare una sottocartella denominata &quot;riutilizza&quot; e caricare il file mancante in &quot;riutilizza&quot;.

### Caricamento di una risorsa con [!UICONTROL Risorse] UI

Oltre al [!UICONTROL Carica risorse] , puoi caricare le risorse trascinandole e rilasciandole nell’interfaccia utente Assets.

1. In Vista archivio, seleziona l’icona con i puntini di sospensione nella cartella Riutilizza per aprire il menu Opzioni.

   ![reuse-ellipsis.png](images/reuse-ellipsis.png)

1. Seleziona **Visualizza nell’interfaccia utente Assets**.

   ![assets_ui.png](images/assets_ui.png)

1. Trascina il file nella cartella.
Il file viene caricato e l’errore di conversione viene risolto.

Tutti gli errori sono stati risolti. La pagina Rapporti indica che non vi sono altri errori e la generazione di un sito AEM genera un output completo senza componenti mancanti.
