---
title: Configurare nomi di file validi per l'output del sito AEM
description: Scopri come configurare nomi di file validi per l’output del sito AEM
source-git-commit: 801c306fa120e7889d4b9428fd5bee2849bf1956
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Configurare nomi di file validi per l&#39;output del sito AEM {#id214GK0X0KXA}

Analogamente all&#39;elenco di caratteri validi per i nomi di file consentiti per gli argomenti DITA, è inoltre possibile configurare un elenco di caratteri validi per i nomi di file per l&#39;output del sito AEM. Alcuni dei caratteri noti non consentiti in un URL sono: ```'<>`@$```. Questi caratteri sono configurati per la conversione automatica in un carattere di sottolineatura &quot;_&quot; quando vengono trovati durante la generazione dei nomi dei file di output del sito AEM. La configurazione che consente di impostare caratteri validi nell’output del sito AEM è presente in `com.adobe.fmdita.common.SanitizeNodeNameImpl` pacchetto. **Impostare il set di caratteri non consentiti per la pubblicazione su AEM Sites** impostazione per includere i caratteri che si desidera sostituire con un carattere di sottolineatura nei nomi dei file di output del sito AEM.

**Argomento padre:**[ Configura nomi file](conf-file-names.md)

