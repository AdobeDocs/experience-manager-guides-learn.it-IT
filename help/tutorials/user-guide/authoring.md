---
title: Gestire il contenuto
description: Scopri come gestire il contenuto
source-git-commit: bad2f5cea2c00ca6c9758da27f0dba89a8579eb7
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 10%

---


# Gestire il contenuto {#id164JBG0M0T1}

Prima di iniziare con la creazione effettiva dei contenuti, è necessario acquisire familiarità con alcuni concetti di base sulla gestione dei contenuti nelle AEM guide. Quindi, inizia con la creazione di diversi gruppi di utenti e l’organizzazione delle risorse.

## Concetti chiave

Alcuni concetti chiave della gestione dei contenuti in AEM sono i seguenti:

**Gestione delle risorse**

AEM Guide utilizza AEM gestione delle risorse digitali \(DAM\) per gestire i file DITA. I file caricati o archiviati in DAM vengono memorizzati come risorse digitali. Puoi gestire e modificare le risorse in AEM Assets. Per ulteriori informazioni sulla gestione delle risorse, consulta [Gestire le risorse](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/manage-digital-assets.html?lang=en).

**Gestione dei collegamenti**

Spostare o rinominare i file o modificare la struttura delle cartelle nell’archivio dei contenuti, senza preoccuparsi di riferimenti interrotti. Tutti i riferimenti al contenuto interessato e da esso vengono aggiornati automaticamente. Ricevi avvisi durante l’eliminazione di contenuti a cui si fa riferimento altrove, per evitare interruzioni non intenzionali.

**Gestione delle versioni**

AEM Guide offre la gestione delle versioni per le risorse digitali. È possibile abilitare facilmente questa funzionalità da un&#39;applicazione di creazione DITA scelta. Consente agli autori di eseguire le funzioni standard di controllo della versione, ad esempio il check-in e il check-out.

Per ulteriori informazioni sulla creazione di versioni o sul ripristino di una versione specifica, consulta [Ramo, ripristino e versioni successive](web-editor-preview-topics.md#id193PG0Y051X).

**Gestione DITA nativa**

Mentre AEM Guide mantiene la struttura dei file DITA, consente anche AEM gestire DITA in modo nativo utilizzando la mappatura degli elementi per mappare gli elementi DITA su componenti AEM. La gestione DITA nativa viene utilizzata in funzioni quali anteprima argomento, pubblicazione AEM Sites e flussi di lavoro di revisione.

## Identificare il ruolo e le autorizzazioni {#id181TF0K0MHT}

AEM Guide fornisce tre gruppi predefiniti. Questi gruppi sono: *Autori*, *Revisori* e *Editori*. A seconda del gruppo a cui sei associato, disponi delle autorizzazioni necessarie per eseguire attività specifiche come indicato nella tabella riportata di seguito. Ad esempio, l’attività di pubblicazione può essere eseguita solo da un editore, ma non da un autore o da un revisore. Analogamente, un autore può creare un nuovo argomento e un revisore può solo esaminare un argomento.

>[!TIP]
>
> Consulta la sezione *Autorizzazioni* nella guida alle best practice per le best practice relative all’impostazione delle autorizzazioni per gli utenti.

Nella tabella seguente sono elencate le varie attività e i gruppi che possono eseguire tali attività:

| Attività | Autori | Revisori | Editori |
|----|-------|---------|----------|
| Crea argomento DITA | Sì |   | Sì |
| Crea mappa DITA | Sì |   | Sì |
| Mappa raccolte | Sì |   | Sì |
| Crea attività di revisione | Sì |   | Sì |
| Argomento di revisione[1](#fntarg_1) | Sì | Sì | Sì |
| Risoluzione dei tasti | Sì |   | Sì |
| Check-out/check-in | Sì |   | Sì |
| Modifica argomento | Sì |   | Sì |
| Sposta argomento | Sì |   | Sì |
| Modifica proprietà argomento | Sì |   | Sì |
| Copiare | Sì |   | Sì |
| Eliminare | Sì |   | Sì |
| Condividi | Sì |   | Sì |
| **Stato del documento** |
| Creare/modificare il profilo dello stato del documento |   |   | Sì |
| Cambia stato del documento[2](#fntarg_2) | Sì | Sì | Sì |
| **Funzioni disponibili nella console mappa DITA \(scheda Predefiniti output\)** |
| Genera |   |   | Sì |
| Modifica |   |   | Sì |
| Duplica |   |   | Sì |
| Creare |   |   | Sì |
| Elimina predefinito |   |   | Sì |
| **Funzioni disponibili nella console mappa DITA \(scheda Output\)** |
| Visualizza output generato | Sì |   | Sì |
| **Funzioni disponibili nella console mappa DITA \(scheda Argomenti\)** |
| Crea attività di revisione | Sì |   | Sì |
| Modifica | Sì |   | Sì |
| **Funzioni disponibili nella console mappa DITA \(scheda Linee di base\)** |
| Creare |   |   | Sì |
| Modifica |   |   | Sì |
| Duplica |   |   | Sì |
| Rimuovi |   |   | Sì |
| Console mappa DITA \(scheda Rapporti\) | Sì |   | Sì |
| **Funzioni disponibili nella console mappa DITA \(Predefiniti condizione\)** |
| Creare/modificare un predefinito di condizione |   |   | Sì |

[1](#fnsrc_1) Se *Autori* e *Editori* sono invitati a una revisione.

[2](#fnsrc_2) A seconda dei diritti concessi all’utente nel profilo dello stato del documento.

## Prerequisiti per la creazione di contenuti

**Utilizzare profili globali o a livello di cartella**

In un&#39;azienda, diversi gruppi o prodotti possono utilizzare diversi modelli di authoring, modelli di output, profili di attributi condizionali \(o schemi soggetti\) e configurazioni dell&#39;editor Web. La configurazione di questi elementi solo a livello aziendale \(o globale\) può rendere difficile l’esperienza degli autori, in quanto vedranno modelli o profili non rilevanti per loro.

AEM Guide ti consente di configurare modelli di authoring \(topic or map\), modelli di output, attributi condizionali e configurazioni di editor Web a livello aziendale \(global\) e a livello di cartella. In questo modo, puoi separare le configurazioni per diversi reparti o prodotti della tua azienda.

Inoltre, puoi delegare le configurazioni specifiche per le cartelle a un reparto o agli amministratori di prodotto per decentrare l&#39;amministrazione.

Per informazioni dettagliate sulla configurazione dei profili globali e a livello di cartella, consulta *Configurare profili globali o a livello di cartella* in Installare e configurare le guide di Adobe Experience Manager as a Cloud Service.





