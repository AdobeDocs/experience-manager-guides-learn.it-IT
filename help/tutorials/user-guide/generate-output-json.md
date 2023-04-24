---
title: JSON
description: Scopri come utilizzare JSON
source-git-commit: 8b6294425c6e60d1c5b37d98e99114014a104ee6
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 1%

---


# JSON {#id231KK0180T4}

Puoi creare il predefinito JSON dall’editor web:

Nel pannello Archivio, apri il file mappa DITA in Vista mappa, quindi nella scheda Output seleziona l’icona + per creare un predefinito di output, quindi seleziona JSON dal menu a discesa Tipo nella finestra di dialogo Aggiungi predefinito.

Nell’editor web, le seguenti configurazioni sono state organizzate in **Generale** scheda:

- Percorso di output
- File di indice
- Applica condizioni utilizzando \(Se le condizioni sono definite per una mappa\)
- Usa linea di base \(se viene creata una linea di base per una mappa\)
- Proprietà da propagare nell&#39;output
- Flusso di lavoro di post-generazione

Per ulteriori informazioni, consulta [Configurazione JSON](#id231KJA00REJ).

**Dal dashboard mappa**

Per aprire i predefiniti di output per PDF, fai clic su un file di mappa DITA dall’interfaccia utente Assets, quindi fai clic su Predefiniti di output e quindi sull’opzione HTML5. Nel dashboard Mappa, fai clic su **Modifica** in alto per aggiornare le varie configurazioni, quindi fare clic su **Salva**.

**Configurazione JSON**

Per il predefinito JSON sono disponibili le seguenti opzioni:

>[!NOTE]
>
> È inoltre possibile modificare il file JSON nell’editor Web.

| Opzioni di output JSON | Descrizione |
| --- | --- |
| Percorso di output | Il percorso all’interno dell’archivio AEM in cui è memorizzato l’output JSON. |
| File di indice | Puoi assegnare un nome al file di indice che stai creando per l’output JSON. Per impostazione predefinita, seleziona il nome del file della mappa DITA e aggiunge un suffisso (come `map_filename_index.json`).<br><br>È inoltre possibile utilizzare le variabili durante l&#39;impostazione del file indice. Per ulteriori dettagli sull’utilizzo delle variabili, consulta [Utilizza le variabili per impostare le opzioni Percorso di destinazione, Nome sito o Nome file](generate-output-use-variables.md#id18BUG70K05Z). |
| Applicare condizioni utilizzando | Selezionare una delle opzioni seguenti:<br><br>* **Nessuno**: Selezionare questa opzione se non si desidera applicare alcuna condizione all&#39;output pubblicato.<br>* **File DIAVAL**: Seleziona i file DITAVAL per generare contenuti personalizzati. È possibile selezionare più file DITAVAL utilizzando la finestra di dialogo Sfoglia o digitando il percorso del file. Per rimuoverlo, utilizza l’icona a croce accanto al nome del file. I file DITAVAL vengono valutati nell&#39;ordine specificato, pertanto le condizioni specificate nel primo file hanno la precedenza rispetto alle condizioni corrispondenti specificate nei file successivi. È possibile mantenere l&#39;ordine dei file aggiungendo o eliminando file. Se il file DITAVAL viene spostato in un altro percorso o viene eliminato, non viene eliminato automaticamente dal dashboard mappa. È necessario aggiornare il percorso nel caso in cui i file vengano spostati o eliminati. Puoi passare il cursore sul nome del file per visualizzare il percorso nell’archivio AEM in cui è memorizzato il file. È possibile selezionare solo i file DITAVAL e viene visualizzato un errore se si è selezionato un altro tipo di file.<br>* **Predefinito condizione**: Seleziona un predefinito per condizioni dal menu a discesa per applicare una condizione durante la pubblicazione dell’output. L’opzione è visibile se hai aggiunto una condizione presente nella scheda Predefiniti condizione della console Mappa DITA. Per ulteriori informazioni sul predefinito di condizione, consulta [Utilizzare i predefiniti condizione](generate-output-use-condition-presets.md#id1825FL004PN). |
| Usa linea di base | Se è stata creata una baseline per la mappa DITA selezionata, selezionare questa opzione per specificare la versione da pubblicare.<br><br>Vedi [Utilizzare la linea di base](generate-output-use-baseline-for-publishing.md#id1825FI0J0PF) per maggiori dettagli. |
| Proprietà da propagare nell&#39;output | Seleziona le proprietà da elaborare come metadati. Queste proprietà vengono impostate dalla pagina Proprietà della mappa DITA o del file bookmap. Le proprietà selezionate dall’elenco a discesa sono elencate sotto il campo Proprietà .<br><br>**Nota**: È inoltre possibile definire proprietà personalizzate e trasmettere i metadati all&#39;output utilizzando la pubblicazione DITA-OT. Per maggiori dettagli vedi [Utilizzare i metadati](metadata-dita.md#id21BJ00QD0XA). |
| Flusso di lavoro di post-generazione | Quando scegli questa opzione, viene visualizzato un nuovo elenco a discesa Flusso di lavoro di post generazione contenente tutti i flussi di lavoro configurati in AEM. È necessario selezionare un flusso di lavoro da eseguire dopo il completamento del flusso di lavoro di generazione dell’output.<br><br>**Nota**: Per ulteriori informazioni sulla creazione di un flusso di lavoro personalizzato per la generazione dei post-output, vedi _Personalizzare il flusso di lavoro di generazione dei post-output_ nella guida Installazione e configurazione delle guide as a Cloud Service di Adobe Experience Manager . |

**Argomento principale:**[ Informazioni sui predefiniti di output](generate-output-understand-presets.md)

