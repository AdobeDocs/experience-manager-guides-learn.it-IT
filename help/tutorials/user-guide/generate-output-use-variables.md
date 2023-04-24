---
title: Utilizza le variabili per impostare le opzioni Percorso di destinazione, Nome sito o Nome file
description: Scopri come utilizzare le variabili per impostare le opzioni Percorso di destinazione, Nome sito o Nome file
source-git-commit: 8b6294425c6e60d1c5b37d98e99114014a104ee6
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---


# Utilizza le variabili per impostare le opzioni Percorso di destinazione, Nome sito o Nome file


Durante la generazione degli output in AEM sito o PDF, puoi utilizzare le variabili per definire le opzioni Percorso di destinazione, Nome AEM sito o Nome file di PDF. Puoi utilizzare una singola o una combinazione di variabili per definire queste opzioni.

Nella tabella seguente sono elencate le variabili supportate come predefinite:

| Variabile | Percorso di destinazione finale | Esempio |
| --- | --- | --- |
| `${map_filename}` | Utilizza il nome dei file di mappa DITA per creare il percorso di destinazione. | **Nome file mappa DITA**:<br>`AEMGuides.ditamap`<br><br>**Percorso di Destinazione** configurato come:<br>`/content/output/sites/${map_filename}`<br><br>**Luogo di uscita finale**:<br>`/content/output/sites/aemGuides/AEMGuides.html` |
| `${map_title}` | Utilizza il titolo della mappa DITA per creare il percorso di destinazione. | **Nome file mappa DITA**:<br>`AEMGuides.ditamap`<br><br>**Titolo mappa DITA**:<br>`AEMGuides`<br><br>**Percorso di Destinazione** configurato come:<br>`/content/output/sites/${map_title}`<br><br>**Luogo di uscita finale**:<br>`/content/output/sites/AEMGuides/AEMGuides.html` |
| `${preset_name}` | Utilizza il nome del predefinito di output per creare il percorso di destinazione. | **Nome predefinito di output**:<br>`AEM Guides PDF Output`<br><br>**Nome file mappa DITA**:<br>`SampleDita.ditamap`<br><br>**Percorso di Destinazione** configurato come:<br>`/content/output/sites/${preset_name}`<br><br>**Luogo di uscita finale**:<br>`/content/output/sites/AEM Guides PDF Output/SampleDita.html` |
| `${language_code}` | Utilizza il codice della lingua in cui si trova il file di mappa per creare il percorso di destinazione. | **Nome file mappa DITA**:<br>`SampleDita.ditamap`<br><br>**Percorso file mappa DITA**:<br>`/content/dam/projects/AEM-Guides/en/user-guide/`<br><br>**Percorso di Destinazione** configurato come:<br>`/content/output/sites/${language_code}`<br><br>**Luogo di uscita finale**:<br>`/content/output/sites/en/SampleDita.html` |
| `${map_parentpath}` | Utilizza il percorso completo del file mappa per creare il percorso di destinazione.<br><br>**Nota**:Questa variabile non può essere utilizzata per specificare il nome del sito AEM o il nome del file di PDF. | **Nome file mappa DITA**:<br>`SampleDita.ditamap`<br><br>**Percorso file mappa DITA**:<br>`/content/dam/projects/AEM-Guides/en/user-guide`/<br><br>**Percorso di Destinazione** configurato come:<br>`/content/output/sites/${map_parentpath}`<br><br>**Luogo di uscita finale**:<br>`/content/output/sites/content/dam/projects/AEM-Guides/en/user-guide/SampleDita.html` |
| `${path_after_langfolder}` | Utilizza il percorso del file di mappa dopo la cartella della lingua per creare il percorso di destinazione.<br><br>**Nota**: Questa variabile non può essere utilizzata per specificare il nome AEM del sito o il nome del file di PDF. | **Nome file mappa DITA**:<br>`SampleDita.ditamap`<br><br>**Percorso file mappa DITA**:<br>`/content/dam/projects/AEM-Guides/en/user-guide/`<br><br>**Percorso di Destinazione** configurato come:<br>`/content/output/sites/${path\_after\_langfolder}`<br><br>**Luogo di uscita finale**:<br>`/content/output/sites/user-guide/SampleDita.html` |

Inoltre, è possibile utilizzare i metadati definiti per la mappa DITA o il file bookmap come variabili. I metadati sono disponibili nella sezione `/jcr:content/metadata` nodo della mappa DITA o del file della libreria. Ad esempio, una delle proprietà dei metadati definite nel `/jcr:content/metadata` nodo `dc:title`. Puoi specificare `${dc:title}` e il valore del titolo viene utilizzato nell&#39;output finale.
**Argomento principale:**[ Generazione di output](generate-output.md)

