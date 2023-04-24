---
title: Caricare file
description: Scopri come caricare i file
source-git-commit: cc0fbca257d82cc82db5b5da8d263309fd71de55
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---


# Caricare file {#id176FF000JUI}

Probabilmente si dispone di un archivio del contenuto DITA esistente che si desidera utilizzare con AEM Guide. Per tale contenuto esistente, puoi utilizzare uno dei seguenti approcci per caricare in massa il contenuto in AEM archivio:

>[!IMPORTANT]
>
> Vedi [Aggiungere risorse digitali ad Adobe Experience Manager as a Cloud Service Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/manage/add-assets.html) per informazioni dettagliate sui metodi di caricamento del contenuto supportati in AEM.

## Interfaccia utente della console Assets

È possibile selezionare il contenuto sul desktop e trascinare l&#39;interfaccia utente AEM \(browser Web\) nella cartella di destinazione. Per ulteriori dettagli, consulta [Caricare le risorse](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/manage/add-assets.html#upload-assets) nella documentazione AEM.

## App desktop AEM

Utilizza AEM’app desktop se sei un professionista e vuoi gestire le risorse sul desktop locale. Puoi aprire e modificare queste risorse con le tue applicazioni desktop. Puoi anche gestire le versioni e condividere i file con altri utenti. Per ulteriori dettagli, consulta [app desktop AEM](https://experienceleague.adobe.com/docs/experience-manager-desktop-app/using/using.html).

## Acquisizione in massa di risorse

Se disponi di migrazioni su larga scala e di ingestioni di massa occasionali, utilizza Asset Bulkingestor per caricare i contenuti. Utilizzando questo strumento, puoi caricare contenuti in blocco da archivi dati supportati come Azure o S3. Per ulteriori dettagli, consulta [Acquisizione in massa di risorse](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/manage/add-assets.html?lang=en#asset-bulk-ingestor).

## Utilizzare FrameMaker per il caricamento in serie

Adobe FrameMaker viene fornito con un potente connettore AEM che consente di caricare facilmente i documenti DITA e altri documenti FrameMaker esistenti \(`.book` e `.fm`\) in AEM. Puoi utilizzare varie funzionalità di caricamento dei file, ad esempio caricare un singolo file, caricare una cartella completa con o senza dipendenze \(come riferimenti di contenuto, riferimenti incrociati e grafica\).

Per ulteriori dettagli sull&#39;utilizzo della funzione di caricamento in serie in FrameMaker, consulta la sezione . *Creare una cartella CRX e caricare i file* in Guida utente di FrameMaker.

## Gestione degli errori durante il caricamento del contenuto {#id201MI0I04Y4}

In caso di errore nel caricamento di uno o più file, alla fine del processo di caricamento viene visualizzato un messaggio di richiesta con un elenco di file che non sono stati caricati:

![](images/uuid-files-failed-to-upload_cs.png){width="650" align="center"}

Per ulteriori dettagli sulle modalità di caricamento dei vari scenari di file, vedi [Carica contenuto DITA](authoring-file-management.md#).

Nel caso in cui utilizzi uno strumento come AEM’app desktop o l’inserimento di massa di risorse, l’azione da eseguire su un file duplicato è controllata da un’impostazione nel server AEM. Per informazioni su questa configurazione, contattare l&#39;amministratore di sistema.

**Argomento principale:**[ Gestire il contenuto](authoring.md)

