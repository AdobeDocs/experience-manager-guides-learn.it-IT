---
title: Preimpostazione EPUB
description: Scopri come utilizzare EPUB Preset
source-git-commit: 8b6294425c6e60d1c5b37d98e99114014a104ee6
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 1%

---


# EPUB {#id205BED020YT}

Puoi creare il predefinito EPUB dal dashboard mappa.

>[!NOTE]
>
> È possibile scegliere il metodo per generare HTML5 utilizzando DITA-OT o FMPS \(se è stato configurato dall&#39;amministratore di sistema\).

Per aprire i predefiniti di output per EPUB, fare clic su un file di mappa DITA, quindi fare clic su Predefiniti di output, quindi fare clic sull&#39;opzione EPUB. Per l&#39;uscita EPUB sono disponibili le seguenti opzioni:

| Opzioni EPUB | Descrizione |
| --- | --- |
| Tipo di output | Tipo di output da generare. Per generare l’output EPUB, scegli l’opzione EPUB. |
| Nome impostazione | Assegna un nome descrittivo per le impostazioni di output EPUB che stai creando. Ad esempio, puoi specificare _Uscita clienti interni_ o _output degli utenti finali_. |
| Argomenti della riga di comando DITA-OT | Specificare gli argomenti aggiuntivi che si desidera elaborare DITA-OT durante la generazione dell&#39;output. Per informazioni dettagliate sugli argomenti della riga di comando supportati in DITA-OT, vedere [Documentazione DITA-OT](https://www.dita-ot.org/). |
| Genera EPUB utilizzando | Selezionare DITA-OT per generare l&#39;output EPUB. |
| Applicare condizioni utilizzando | Selezionare una delle opzioni seguenti:<br><br>* **Nessuno**: Selezionare questa opzione se non si desidera applicare alcuna condizione all&#39;output pubblicato.<br>* **File DITAVal**: Selezionare i file DITAVal per generare contenuti personalizzati. È possibile selezionare più file DITAVal utilizzando la finestra di dialogo Sfoglia o digitando il percorso del file. Per rimuoverlo, utilizza l’icona a croce accanto al nome del file. I file DITAVal vengono valutati nell&#39;ordine specificato, quindi le condizioni specificate nel primo file hanno la precedenza rispetto alle condizioni corrispondenti specificate in file successivi. È possibile mantenere l&#39;ordine dei file aggiungendo o eliminando file. Se il file DITAVal viene spostato in un altro percorso o viene eliminato, non viene eliminato automaticamente dal dashboard mappa. È necessario aggiornare il percorso nel caso in cui i file vengano spostati o eliminati. Puoi passare il cursore sul nome del file per visualizzare il percorso nell’archivio AEM in cui è memorizzato il file. È possibile selezionare solo i file DITAVal e viene visualizzato un errore se si è selezionato un altro tipo di file. FrameMaker Publishing Server non supporta più file DIAVAL.<br>* **Predefinito condizione**: Seleziona un predefinito per condizioni dal menu a discesa per applicare una condizione durante la pubblicazione dell’output. L’opzione è visibile se hai aggiunto una condizione presente nella scheda Predefiniti condizione della console Mappa DITA. Per ulteriori informazioni sul predefinito di condizione, consulta [Utilizzare i predefiniti condizione](generate-output-use-condition-presets.md#id1825FL004PN). |
| Percorso di destinazione | Percorso all’interno dell’archivio AEM in cui è memorizzato l’output EPUB. |
| Nome file | Specificare il nome file con cui salvare l&#39;output EPUB.<br><br>**Nota**: Se non si specifica un nome di file, il titolo della mappa DITA viene utilizzato per generare il nome finale del file di output EPUB. Se la mappa non ha un titolo, il nome del file della mappa DITA viene utilizzato per denominare è l&#39;output finale dell&#39;EPUB. Il nome del file viene bonificato utilizzando le regole configurate nel sistema per gestire eventuali caratteri non validi. |
| Nome trasformazione | Specifica il tipo di output da generare. Questo è necessario se si desidera generare l&#39;output utilizzando il proprio plug-in personalizzato, integrato nel plug-in DITA-OT. Ad esempio, se desideri generare l’output XHTML, specifica `xhtml`. Per un elenco delle trasformazioni disponibili in DITA-OT, vedere [Trasformazioni DITA-OT (formati di output)](http://www.dita-ot.org/2.3/user-guide/AvailableTransforms.md) in OASIS DITA-OT User Guide. |
| Pulisci file temporanei DITA-OT | Selezionare questa opzione per pulire i file temporanei generati da DITA-OT. La posizione in cui DITA-OT memorizza i file temporanei si trova nel registro di generazione dell&#39;output.<br><br>Se si verificano errori durante la generazione dell&#39;output tramite DITA-OT, è possibile deselezionare questa opzione per mantenere i file temporanei. Puoi quindi utilizzare questi file per risolvere eventuali errori di generazione dell’output. |
| Esegui flusso di lavoro di post-generazione | Quando scegli questa opzione, viene visualizzato un nuovo elenco a discesa Flusso di lavoro di post generazione contenente tutti i flussi di lavoro configurati in AEM. È necessario selezionare un flusso di lavoro da eseguire dopo il completamento del flusso di lavoro di generazione dell’output.<br><br>**Nota**: Per ulteriori informazioni sulla creazione di un flusso di lavoro personalizzato per la generazione dei post-output, vedi _Personalizzare il flusso di lavoro di generazione dei post-output_ in Installare e configurare le guide di Adobe Experience Manager as a Cloud Service. |
| Usa linea di base | Se è stata creata una baseline per la mappa DITA selezionata, selezionare questa opzione per specificare la versione da pubblicare.<br><br>Vedi [Utilizzare la linea di base](generate-output-use-baseline-for-publishing.md#id1825FI0J0PF) per maggiori dettagli. |
| Proprietà | Seleziona le proprietà da elaborare come metadati. Queste proprietà vengono impostate dalla pagina Proprietà della mappa DITA o del file bookmap. Le proprietà selezionate dall’elenco a discesa sono elencate sotto il campo Proprietà e vengono rimosse dall’elenco a discesa. Una volta impostate, queste proprietà vengono copiate anche negli argomenti all&#39;interno della mappa.<br><br>**Nota**: È inoltre possibile trasferire i metadati all&#39;output utilizzando la pubblicazione DITA-OT. Per maggiori dettagli vedi [Trasmettere i metadati all&#39;output utilizzando DITA-OT](pass-metadata-dita-ot.md#id21BJ00QD0XA). |

**Argomento principale:**[ Informazioni sui predefiniti di output](generate-output-understand-presets.md)

