---
title: Gestire i predefiniti di output del profilo globale e della cartella
description: Scopri come gestire i predefiniti di output per profili globali e cartelle
source-git-commit: 3b33b27e4acb8d0b185427725e23b8beac0c2a46
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---


# Gestire i predefiniti di output del profilo globale e della cartella {#id22BLJ0D0V1U}

I predefiniti Profilo globale e Profilo cartella sono disponibili solo per gli utenti amministratori a livello di cartella.

In qualità di amministratore, AEM Guide ti consente di creare e gestire i predefiniti di output per i profili globali e cartelle. Puoi quindi utilizzare facilmente questi predefiniti di output per generare l’output per tutte le mappe correlate a tale profilo globale o di cartelle.

Per creare un predefinito di output per i profili globali e cartelle, effettua le seguenti operazioni:

1. Selezionare la mappa DITA per la quale si desidera creare un predefinito di output.
1. Seleziona la **Modifica argomenti** dall&#39;opzione **Opzioni** menu del file mappa. Il file mappa viene aperto per la modifica nell&#39;editor Web.
1. In **Uscita** selezionare l&#39;icona + per creare un predefinito di output per la mappa DITA.

   ![](images/add-global-output-preset.png){width="350" align="left"}

1. Immetti i seguenti dettagli nella **Aggiungi predefinito** finestra di dialogo:
   - Tipo
   - Nome
   - Target \(per Knowledgebase preset\)
1. Seleziona la **Aggiungi al profilo della cartella** casella di controllo per creare un predefinito di output per il profilo di cartella correlato, quindi fai clic su **Aggiungi**. Il predefinito viene creato e viene visualizzato sotto il **Uscita** scheda di tutte le mappe correlate. \( ![](images/global-preset-icon.svg)\) indica un predefinito a livello di profilo cartella.
1. Immetti i dettagli di configurazione.

   >[!NOTE]
   >
   > Questi predefiniti aggiunti al profilo della cartella sono indipendenti dalle mappe, pertanto le configurazioni specifiche della mappa non sono presenti per questi predefiniti.

1. È possibile selezionare la **Genera predefinito** nella parte superiore per generare l&#39;output per le mappe relative al predefinito di output creato. Verrà visualizzato lo stato del processo di generazione dell&#39;output. Per visualizzare l&#39;output, posiziona il puntatore del mouse sull&#39;argomento e fai clic su **Visualizza output**.

>[!NOTE]
>
> AEM Guide fornisce anche un predefinito di output PDF predefinito per generare l’output per le mappe DITA.

**Altre operazioni dal menu Opzioni**

Puoi anche eseguire le seguenti operazioni sul predefinito dal menu Opzioni :

- Selezionare il predefinito come predefinito pdf predefinito. Quindi il predefinito selezionato viene utilizzato come predefinito predefinito per generare l’output di PDF utilizzando **Scarica come PDF** opzione per una mappa.
- **Modifica**, **Rinomina**, **Duplica** oppure **Elimina** un predefinito di output esistente dal **Opzioni** menu.

>[!NOTE]
>
> Quando un predefinito di output in Profili globali e cartelle viene eliminato, si rifletterà in tutte le mappe correlate e non verrà visualizzato sotto **Uscita** scheda .

**Argomento principale:**[ Utilizzare l’editor Web](web-editor.md)

