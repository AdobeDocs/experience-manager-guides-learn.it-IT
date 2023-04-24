---
title: Scaricare i file
description: Scopri come scaricare i file
source-git-commit: cc0fbca257d82cc82db5b5da8d263309fd71de55
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---


# Scaricare i file {#id216MC0H0BE8}

È possibile scaricare risorse tra cui file DITA e non DITA. Esistono diversi modi in cui è possibile scaricare le risorse, alcuni metodi sono nativi di AEM e altri sono supportati dalle guide AEM. Per informazioni sul download di risorse AEM native, consulta [Scaricare risorse da Adobe Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/manage/download-assets-from-aem.html) nella documentazione AEM. La sezione seguente spiega il meccanismo di download dei file tramite la console mappa DITA in Guide AEM.

## Esportare un file di mappa DITA

Una volta che il file mappa DITA è presente nell&#39;archivio AEM, è possibile scaricare il file mappa insieme ai relativi dipendenti. Questo offre la flessibilità di condividere l&#39;intero file mappa per la modifica offline, la convalida, la revisione o semplicemente la creazione di un backup.

Esegui i seguenti passaggi per scaricare un file mappa DITA insieme ai relativi file dipendenti:

1. Nell’interfaccia utente Assets, passa alla mappa DITA da scaricare.

1. Fare clic sulla mappa DITA per aprirla nella console Mappa DITA.

1. Seleziona la **Argomenti** scheda per visualizzare un elenco degli argomenti disponibili nella mappa DITA.

1. Nella barra degli strumenti principale, fai clic su **Scarica mappa**.

   Viene visualizzata la finestra di dialogo Scarica mappa.

   ![](images/download-map.png){width="300" align="left"}

1. Fai clic su **Scarica**. Nella finestra di dialogo Scarica mappa puoi scegliere le seguenti opzioni:

   - **Usa linea di base**: Selezionare questa opzione per ottenere un elenco delle baseline create per la mappa DITA. Se si desidera scaricare il file di mappa e il relativo contenuto in base a una linea di base specifica, selezionare la linea di base dall&#39;elenco a discesa. Per ulteriori dettagli sull&#39;utilizzo delle linee di base, consulta [Utilizzare la linea di base](generate-output-use-baseline-for-publishing.md#).
   - **Gerarchia file appiattita**: Selezionare questa opzione per salvare tutti gli argomenti e i file multimediali di riferimento in un&#39;unica cartella.

   >[!NOTE]
   >
   > Puoi anche scaricare il file mappa senza selezionare alcuna opzione. In tal caso, viene scaricata l&#39;ultima versione persistente degli argomenti e dei file multimediali di riferimento.

1. Dopo aver fatto clic sul pulsante **Scarica** , la richiesta di download della mappa viene messa in coda. Riceverai la seguente notifica quando la mappa sarà pronta per il download.

   ![](images/download-map-prompt.png){width="550" align="left"}

   - Fai clic su **Scarica** per scaricare il file mappa in formato .zip.

   - Fai clic su **Scarica più tardi** per scaricare il file mappa in un secondo momento. Il collegamento di download è accessibile dalla casella in entrata della notifica AEM. Fai clic sulla notifica della mappa generata nella casella in entrata per scaricare la mappa in formato .zip.
   >[!NOTE]
   >
   > Per impostazione predefinita, le mappe scaricate rimangono per cinque giorni nella casella in entrata della notifica AEM.

![](images/download-map-inbox.png){width="300" align="left"}

Una volta scaricata la mappa, puoi selezionare la mappa e utilizzare l’icona Apri nella parte superiore per aprire il rapporto selezionato.

**Argomento principale:**[ Gestire il contenuto](authoring.md)

