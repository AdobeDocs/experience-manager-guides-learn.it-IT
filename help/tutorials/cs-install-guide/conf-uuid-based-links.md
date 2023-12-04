---
title: Configurare la visualizzazione dei collegamenti basati su UUID
description: Scopri come configurare la visualizzazione dei collegamenti basati su UUID
source-git-commit: 880cd344ceb65ea339be699ebcad41c0d62e168a
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 1%

---

# Configurare la visualizzazione dei collegamenti basati su UUID {#id2035G20M0QN}

Per impostazione predefinita, quando si crea un collegamento utilizzando l&#39;opzione Inserisci riferimento o Inserisci contenuto riutilizzo nell&#39;editor Web, il collegamento viene creato utilizzando l&#39;UUID del contenuto di riferimento. Il **Collegamento** La proprietà \(nel pannello Proprietà\) del contenuto a cui si fa riferimento può essere configurata in modo da visualizzare il percorso del file relativo del contenuto a cui si fa riferimento o l’UUID. Per impostazione predefinita, l’UUID del contenuto a cui si fa riferimento viene visualizzato nel pannello Proprietà.

Utilizzare le istruzioni fornite in [Sostituzioni configurazione](download-install-additional-config-override.md#) per creare il file di configurazione. Nel file di configurazione, fornisci i seguenti dettagli \(property\) per visualizzare il percorso relativo o l’UUID del contenuto a cui si fa riferimento nell’editor Web:

| PID | Chiave proprietà | Valore proprietà |
|---|------------|--------------|
| `com.adobe.fmdita.xmleditor.config.XmlEditorConfig` | `xmleditor.uuid` | Booleano \(true/false\). Se desideri visualizzare il percorso relativo del contenuto collegato, imposta questa proprietà su false. <br> **Valore predefinito**: true |

**Argomento padre:**[ Personalizza editor web](conf-web-editor.md)
