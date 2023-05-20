---
title: Carica file
description: Scopri come caricare i file
exl-id: d6a73953-94dd-4fa5-b09c-5e4c77fead62
source-git-commit: 8073716bccacbe8d6a158b44d5106b083e3a5dcd
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Carica file {#id176FF000JUI}

È probabile che si disponga di un archivio di contenuti DITA esistenti che si desidera utilizzare con le guide AEM. Per tali contenuti esistenti, puoi utilizzare uno dei seguenti approcci per caricare in blocco i contenuti nell’archivio AEM:

>[!IMPORTANT]
>
> Consulta [Aggiungere risorse digitali alle risorse Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/manage/add-assets.html) per informazioni dettagliate sui metodi di caricamento dei contenuti supportati nell’AEM.

## Interfaccia utente di Assets Console

Puoi selezionare il contenuto sul desktop e trascinare l’interfaccia utente AEM \(browser Web\) nella cartella di destinazione. Per ulteriori dettagli, consulta [Caricare le risorse](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/manage/add-assets.html#upload-assets) nella documentazione AEM.

## App desktop AEM

Se sei un professionista creativo e desideri gestire le risorse sul desktop locale, utilizza l’app desktop AEM. Puoi aprire e modificare queste risorse con le tue applicazioni desktop. Puoi anche gestire le versioni e condividere i file con altri utenti. Per ulteriori dettagli, consulta [App desktop AEM](https://experienceleague.adobe.com/docs/experience-manager-desktop-app/using/using.html).

## Acquisizione in blocco delle risorse

In caso di migrazioni su larga scala e acquisizioni in blocco occasionali, utilizza l’acquisizione in blocco delle risorse per caricare i contenuti. Utilizzando questo strumento, puoi caricare contenuto in blocco da archivi di dati supportati come Azure o S3. Per ulteriori dettagli, consulta [Acquisizione in blocco delle risorse](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/manage/add-assets.html?lang=en#asset-bulk-ingestor).

## Usa FrameMaker per il caricamento in blocco

Adobe FrameMaker viene fornito con un potente connettore AEM che consente di caricare facilmente i documenti DITA e FrameMaker esistenti \(`.book` e `.fm`\) nell’AEM. Puoi utilizzare varie funzionalità di caricamento dei file, ad esempio il caricamento di un singolo file e di una cartella completa con o senza dipendenze \(come riferimenti a contenuti, riferimenti incrociati e elementi grafici\).

Per ulteriori dettagli sull&#39;utilizzo della funzione di caricamento in blocco in FrameMaker, consultate la sezione *Creare una cartella CRX e caricare i file* nella Guida utente di FrameMaker.

## Gestione degli errori durante il caricamento del contenuto {#id201MI0I04Y4}

In caso di errore durante il caricamento di uno o più file, al termine del processo di caricamento viene visualizzato un messaggio con l’elenco dei file che non è stato possibile caricare:

![](images/uuid-files-failed-to-upload_cs.png){width="650" align="center"}

Per ulteriori dettagli sui vari scenari di caricamento dei file, vedi [Carica contenuto DITA](authoring-file-management.md#).

Se utilizzi uno strumento come un’app desktop AEM o Asset Bulk Ingestor, l’azione da eseguire su un file duplicato è controllata da un’impostazione nel server AEM. Contatta l’amministratore di sistema per informazioni su questa configurazione.

**Argomento padre:**[ Gestire i contenuti](authoring.md)
