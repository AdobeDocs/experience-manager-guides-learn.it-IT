---
title: API REST per il flusso di lavoro di conversione
description: Scopri le API REST per il flusso di lavoro di conversione
source-git-commit: 8707acf3ba01b7488eea6597c434da73a901d037
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---


# API REST per il flusso di lavoro di conversione {#id175UB30E05Z}

Le seguenti API REST consentono di convertire documenti Word, HTML e InDesign in formato DITA.

## Convertire documenti di Word

Metodo di GET che converte i documenti di Word in formato DITA.

**URL richiesta**: http://*&lt;aem-guides-server>*: *&lt;port-number>*/bin/fmdita/conversion

**Parametri**: |Nome|Tipo|Obbligatorio|Descrizione| ----|----|--------|-----------| |``operation``|String|Yes|Nome dell&#39;operazione chiamata. Il valore di questo parametro è ``word2dita``. <br> **Nota:** Il valore non distingue tra maiuscole e minuscole. | |`inputFile`|String|Yes|Percorso assoluto dei file Word di origine nell&#39;archivio AEM.| |`destPath`|String|Yes|Percorso assoluto del percorso di destinazione in cui verranno salvati i file DITA convertiti.| |`createRev`|Booleano|Sì|Specifica se viene creata una revisione dei file \( `true`\) alla destinazione specificata o meno \( `false`\). Questo viene considerato solo quando il percorso di destinazione contiene una versione esistente dei file convertiti.| |`style2tagMap`|String|Yes|Percorso assoluto del file di mapping degli stili che verrà utilizzato per la conversione.|

**Valori di risposta**: restituisce una risposta HTTP 200 \(Riuscito\).

## Conversione di documenti HTML

Metodo GET che converte i documenti HTML in formato DITA.

**URL richiesta**: http://*&lt;aem-guides-server>*: *&lt;port-number>*/bin/fmdita/conversion

**Parametri**: |Nome|Tipo|Obbligatorio|Descrizione| ----|----|--------|-----------| |`operation`|String|Yes|Nome dell&#39;operazione chiamata. Il valore di questo parametro è ``html2dita``. <br> **Nota:** Il valore non distingue tra maiuscole e minuscole.| |`inputFile`|String|Yes|Percorso assoluto dei file HTML di origine nell&#39;archivio AEM.| |`destPath`|String|Yes|Percorso assoluto del percorso di destinazione in cui verranno salvati i file DITA convertiti.| |`createRev`|Booleano|Sì|Specifica se viene creata una revisione dei file \( `true`\) alla destinazione specificata o meno \( `false`\). Questa opzione viene considerata solo se il percorso di destinazione contiene una versione esistente dei file convertiti.|

**Valori di risposta**: restituisce una risposta HTTP 200 \(Riuscito\).

## Conversione di documenti InDesign

Metodo GET che converte i documenti InDesign in formato DITA.

**URL richiesta**: http://*&lt;aem-guides-server>*: *&lt;port-number>*/bin/fmdita/conversion

**Parametri**: |Nome|Tipo|Obbligatorio|Descrizione| ----|----|--------|-----------| |``operation``|String|Yes|Nome dell&#39;operazione chiamata. Il valore di questo parametro è ``idml2dita``. <br> **Nota:** Il valore non distingue tra maiuscole e minuscole.| |`inputFile`|String|Yes|Percorso assoluto dei file InDesign di origine nell&#39;archivio AEM.| |`destPath`|String|Yes|Percorso assoluto del percorso di destinazione in cui verranno salvati i file DITA convertiti.| |`createRev`|Booleano|Sì|Specifica se viene creata una revisione dei file \( `true`\) alla destinazione specificata o meno \( `false`\). Questa opzione viene considerata solo se il percorso di destinazione contiene una versione esistente dei file convertiti.|

**Valori di risposta**: restituisce una risposta HTTP 200 \(Riuscito\).
