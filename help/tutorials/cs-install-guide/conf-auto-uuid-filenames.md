---
title: Configurare nomi di file automatici basati su UUID
description: Scopri come configurare i nomi di file automatici in base all’UUID
source-git-commit: 4f15166b1b250578f07e223b0260aacf402224be
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 1%

---


# Configurare nomi di file automatici basati su UUID {#id205QG070D5Z}

Per impostazione predefinita, quando viene creato un file argomento o mappa, agli autori viene data un&#39;opzione per specificare anche il nome del file. Gli autori possono assegnare i nomi dei file in base alle proprie esigenze. Tuttavia, questo può causare incoerenza e un’ampia gamma di nomi di file può essere vista in un ampio sistema di documentazione. In qualità di amministratore, puoi impedire agli autori di assegnare nomi di file per i file creati nel sistema. Per ogni nuovo argomento o file mappa, puoi scegliere di assegnare automaticamente nomi di file basati su UUID.

Utilizzare le istruzioni fornite in [Sostituzioni configurazione](download-install-additional-config-override.md#) per creare il file di configurazione. Nel file di configurazione, fornisci i seguenti dettagli \(property\) per configurare i nomi di file automatici in base all’UUID:

| PID | Chiave proprietà | Valore proprietà |
|---|------------|--------------|
| `com.adobe.fmdita.xmleditor.config.XmlEditorConfig` | `xmleditor.uniquefilenames` | Booleano \(true/false\).<br> **Valore predefinito**: false |

>[!NOTE]
>
> Quando questa opzione è attivata, gli autori non visualizzeranno l&#39;opzione per specificare il nome del file durante la creazione di un nuovo argomento o di un nuovo file di mappa. È possibile creare un nuovo argomento o un nuovo file di mappa dall’interfaccia utente di Assets e dall’editor web.

**Argomento padre:**[ Configura nomi file](conf-file-names.md)
