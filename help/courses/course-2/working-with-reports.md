---
title: Utilizzo dei rapporti
description: Utilizzo dei rapporti in [!DNL Adobe Experience Manager Guides]
exl-id: 755506a6-c416-4a8c-8359-8db7e63a90a4
source-git-commit: 1c4d278a05f2612bc55ce277efb5da2e6a0fa9a9
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 0%

---

# Utilizzo dei rapporti

La scheda Rapporti nella dashboard mappa consente di identificare e risolvere i collegamenti interrotti, i contenuti a cui si fa riferimento e che vengono riutilizzati (conref), i riferimenti incrociati o altre informazioni mancanti.

>[!VIDEO](https://video.tv.adobe.com/v/339039?quality=12&learn=on)

## Preparazione dell&#39;esercizio

Puoi scaricare file di esempio per l&#39;esercizio qui.

[Esercizio-Scarica](assets/exercises/working-with-reports.zip)

## Caricamento delle risorse

1. In Vista archivio, seleziona l’icona Ellissi nella cartella principale per aprire il menu Opzioni.

   ![ellissi-9.png](images/ellipses-9.png)

2. Seleziona **[!UICONTROL Caricare risorse]**.

   ![upload-assets.png](images/upload-assets.png)

3. Seleziona i file da caricare nella cartella e seleziona **Carica**.

I file DITA si aprono ed è necessario esaminarli per eventuali problemi relativi a contenuti mancanti, conref o riferimenti incrociati.

## Creazione di una mappa

1. Selezionare l&#39;icona Ellissi nella cartella principale per aprire il menu Opzioni.

   ![ellissi-9.png](images/ellipses-9.png)

2. Seleziona **Crea > Mappa**.

   ![create-map.png](images/create-map.png)

   Viene visualizzata la finestra di dialogo Crea nuova mappa .

3. Nel campo Modello , seleziona **Bookmap** o **Mappa** in base al tipo di contenuto che si sta creando) dal menu a discesa e assegna un titolo alla mappa.

4. Seleziona **Crea**.

La mappa viene creata e la barra a sinistra cambia automaticamente dalla vista Archivio alla vista Mappa.

## Inserimento di componenti mappa

1. Seleziona l’icona della matita nella barra a sinistra.
Questa è l’icona Modifica e consente di aprire la mappa nell’editor.

   ![edit-map.png](images/edit-map.png)

2. Torna alla vista Archivio selezionando l’icona Archivio .

   ![repository-button.png](images/repository-button.png)

3. Aggiungi un argomento alla mappa trascinandolo e rilasciandolo dall’archivio nella mappa nell’editor.
L’indicatore della riga indica dove verrà inserito l’argomento.

4. Continua ad aggiungere argomenti in base alle esigenze.

5. Al termine, seleziona **Salva come nuova versione.**

   ![save-as-new-version.png](images/save-as-new-version.png)

6. In *Commenti per la nuova versione* immettere un commento descrittivo.

7. Seleziona **Salva**.

## Generazione di un output del sito AEM

1. Nell&#39;archivio, seleziona l&#39;icona Ellissi sulla mappa per aprire il menu Opzioni, quindi **Apri dashboard mappa.**

   ![open-map-dashboard.png](images/open-map-dashboard.png)

   Il dashboard mappa si apre in un&#39;altra scheda.
2. Nella scheda Predefiniti di output, seleziona **Sito AEM**.

   ![aem-site-check](images/aem-site-checkbox.png)

3. Seleziona **Genera**.

4. Passa alla pagina Output per visualizzare lo stato degli output generati.
In caso di errori, nella scheda Output potrebbe essere visualizzato un cerchio arancione sotto la colonna Impostazioni generazione anziché verde, a indicare che la generazione è completa.

5. Seleziona il collegamento nella colonna Impostazioni generazione per aprire l’output generato.
Controlla l&#39;output per il contenuto mancante.

## Scheda Rapporti

Nella scheda Rapporti viene visualizzato un riepilogo dell’argomento e una tabella contenente le informazioni sull’argomento e i problemi all’interno della mappa.

È consigliabile controllare sempre la presenza di una mappa nei rapporti dopo l’importazione del contenuto.

![reports.png](images/reports.png)

La colonna Elementi mancanti indica il numero di immagini mancanti e conref interrotti. È possibile selezionare la **Matita** per aprire l’argomento nell’editor.

## Risoluzione delle immagini mancanti

Se mancano immagini dai file, una causa comune potrebbe essere che il contenuto è stato caricato, ma le immagini no. In tal caso, risolvi i problemi di immagine mancanti caricando le immagini in una cartella specifica che corrisponde al percorso e ai nomi dei file previsti dai file.

1. In *Visualizzazione archivio*, seleziona l’icona Ellissi nella cartella delle immagini per aprire il menu Opzioni .

   ![image-ellipsis.png](images/image-ellipsis.png)

2. Seleziona **[!UICONTROL Caricare risorse]**, quindi seleziona le immagini mancanti.

3. Seleziona **Carica**.

Le immagini mancanti sono state caricate. Ora, un nuovo output del sito AEM generato visualizzerà queste immagini e la scheda Rapporti non visualizzerà più errori di immagine mancanti.

## Risoluzione dei conflitti interrotti

Se il contenuto a cui si fa riferimento altrove (un rif) si collega a per un file all’interno di un’altra cartella (ad esempio, un file denominato &quot;riutilizzo&quot;). e il contenuto non viene caricato, è necessario risolvere un errore. Ad esempio, devi creare una sottocartella denominata &quot;riutilizzo&quot; e caricare il file mancante in &quot;riutilizzo&quot;.

### Caricamento di una risorsa con [!UICONTROL Risorse] Interfaccia

Oltre al [!UICONTROL Caricare risorse] Puoi caricare le risorse trascinandole e rilasciandole nell’interfaccia utente di Assets.

1. In Vista archivio, selezionare l&#39;icona Ellissi nella cartella di riutilizzo per aprire il menu Opzioni.

   ![riutilizzo-ellipsis.png](images/reuse-ellipsis.png)

2. Seleziona **Visualizzazione nell’interfaccia utente Assets**.

   ![assets_ui.png](images/assets_ui.png)

3. Trascina e rilascia il file nella cartella .
Il file viene caricato e l&#39;errore di controllo viene risolto.

Tutti gli errori sono stati risolti. La pagina Rapporti indica che non ci sono più errori e la generazione di un sito AEM genera un output completo senza componenti mancanti.
