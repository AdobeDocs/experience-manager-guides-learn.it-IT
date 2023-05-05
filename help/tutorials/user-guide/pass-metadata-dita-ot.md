---
title: Trasmettere i metadati all'output utilizzando DITA-OT
description: Scopri come passare i metadati all'output utilizzando DITA-OT
exl-id: 637895e5-aece-4827-a32e-f2ae3e3704ef
source-git-commit: c74badebbcb4733fb9caa79c646b1d1e5c8bfe8e
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Trasmettere i metadati all&#39;output utilizzando DITA-OT {#id21BJ00QD0XA}

I metadati sono informazioni aggiuntive sull’output. In Guide AEM puoi passare i metadati esistenti o creare tag di metadati personalizzati. È possibile passare i metadati agli output in formato AEM, PDF, HTML5, EPUB e personalizzato utilizzando la pubblicazione DITA-OT.

Esegui i seguenti passaggi per passare i metadati all&#39;output utilizzando la pubblicazione DITA-OT:

1. In **Interfaccia utente Assets**, passare al file di mappa DITA per il quale si desidera passare i metadati a DITA-OT e fare clic su di esso.
1. Seleziona e modifica un predefinito di output al quale desideri trasmettere i campi dei metadati. Ad esempio, selezionare PDF output preset.
1. Seleziona **DITA-OT** in Genera &lt;output> Utilizzo dell&#39;opzione nel predefinito di output selezionato.

   ![](images/custom-meta-data-output-preset.png){width="800" align="left"}

1. Dal menu a discesa Proprietà , seleziona i metadati che desideri passare alla pubblicazione DITA-OT.

   Nel menu a discesa Proprietà sono elencate sia le proprietà personalizzate che quelle predefinite. Ad esempio, nella schermata precedente l’autore è la proprietà personalizzata mentre `dc:description`, `dc:language`, `dc:title`e `docstate` sono le proprietà predefinite.

   >[!NOTE]
   >
   > Queste proprietà vengono raccolte dal file metadataList disponibile nel percorso seguente:`/libs/fmdita/config/metadataList`. Per impostazione predefinita, in questo file sono elencate quattro proprietà: `dc:description`, `dc:language`, `dc:title`e `docstate`.

   Questo file può essere sovrapposto in: `/apps/fmdita/config/metadataList`.

   Per passare una proprietà personalizzata per la quale hai già definito i valori, vedi [Utilizzare i metadati AEM nell&#39;output di PDF DITA-OT](https://experienceleaguecommunities.adobe.com/t5/xml-documentation-discussions/use-aem-metadata-in-dita-ot-pdf-output/td-p/411880).

1. Da **Proprietà** seleziona le proprietà personalizzate e predefinite richieste. Ad esempio, seleziona `author`, `dc:title`e `dc:description`. Questi sono gli standard `metadata/properties` viene creato una volta creato un file. Le proprietà selezionate sono elencate sotto il menu a discesa.

   ![](images/selected-metadata-properties.png){width="300" align="left"}

1. Fai clic su **Fine** in alto a sinistra per salvare le modifiche.
1. Genera l’output.

Le proprietà dei metadati selezionati verranno passate all&#39;output generato utilizzando DITA-OT.

**Argomento principale:**[ Generazione di output](generate-output.md)
