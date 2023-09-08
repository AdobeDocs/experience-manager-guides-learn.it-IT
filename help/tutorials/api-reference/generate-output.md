---
title: API basata su Java per lavorare con la generazione di output
description: Scopri l’API basata su Java per lavorare con la generazione dell’output
source-git-commit: fad5049962f258bbe59c7d172436d82b3d6cd68f
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---


# API basata su Java per lavorare con la generazione di output {#id175UB30E05Z}

La seguente API basata su Java consente di generare l&#39;output per una mappa DITA. Questa API è disponibile sotto forma di bundle. Per utilizzare queste API, devi includere questo bundle nel codice.

Dettagli bundle:

- ID gruppo: **com.adobe.fmdita**

- ID artefatto: **api**

- Versione: **3,4**

- Pacchetto ****com.adobe.fmdita.api.maps****

- Dettagli classe:

  ```JAVA
  public class **PublishUtils** extends Object
  ```

  Il **`PublishUtils`** La classe contiene un metodo per generare l&#39;output per uno o più predefiniti di output.


## Genera output

Il ``generateOutput`` Il metodo genera l&#39;output per un file di mappa DITA utilizzando i predefiniti di output specificati.

**Sintassi**:

```JAVA
public static void generateOutput(Session session,
String sourcePath,
String outputName)
throws GuidesApiException
```

**Parametri**: |Nome|Tipo|Descrizione| ----|----|-----------| |`session`|javax.jcr.Session|Sessione JCR valida.| |``sourcePath``|String|Percorso \(nel repository AEM\) del file di mapping DITA per il quale deve essere generato l&#39;output.| |``outputName``|String|Nome del predefinito di output\(s\) da utilizzare per generare l&#39;output. È possibile specificare più predefiniti di output utilizzando un delimitatore pipe \(&quot;\|&quot;\), ad esempio `aemsite\|pdfoutput`.|

**Eccezione**: proiezioni ``javax.jcr.RepositoryException``, `java.io.IOException`, e `java.lang.Exception`.

