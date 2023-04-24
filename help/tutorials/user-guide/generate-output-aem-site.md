---
title: Sito AEM
description: Scopri come AEM sito
source-git-commit: 23d6c87b525f0763990166e46f4bd4ac2d6e7cd5
workflow-type: tm+mt
source-wordcount: '2545'
ht-degree: 0%

---


# Sito AEM {#id205BE3008SW}

Per l&#39;output Sito AEM sono disponibili le seguenti opzioni:

Puoi creare il predefinito del sito AEM in due modi:

**Dall’editor Web:** Nel pannello Repository, aprire il file di mappa DITA in Visualizzazione mappa, quindi nella scheda Output selezionare l&#39;icona + per creare un predefinito di output, quindi selezionare AEM sito dal menu a discesa Tipo nella finestra di dialogo Aggiungi predefinito.Nell&#39;editor Web le configurazioni sono state organizzate nelle schede Generale e Avanzate:

**Generale**

La **Generale** La scheda contiene le seguenti configurazioni:

- Nome sito
- Percorso di output
- Pagine di output esistenti
- Elimina pagine del sito orfano
- Applica condizioni utilizzando \(Se le condizioni sono definite per una mappa\)
- Usa linea di base \(se viene creata una linea di base per una mappa\)
- Flusso di lavoro di post-generazione

**Avanzate**

La scheda Avanzate contiene le seguenti configurazioni:

- Pulisci file temporanei DITA-OT
- Genera un PDF separato per ogni argomento
- Usa proprietà mappa come predefinite

Per ulteriori informazioni, consulta [Configurazione AEM sito](#id231KIM004X1).

**Dal dashboard mappa**

Per aprire i predefiniti di output per AEM sito, fare clic su un file di mappa DITA dall&#39;interfaccia utente Assets, quindi fare clic su Predefiniti di output, quindi fare clic sull&#39;opzione di output AEM sito.Nel dashboard di mapping, fare clic su **Modifica** in alto per aggiornare le varie configurazioni, quindi fare clic su **Salva**.

>[!TIP]
>
> Consulta la sezione *Pubblicazione AEM sito* nella guida alle best practice per le best practice relative alla creazione dell’output AEM sito.

## Configurazione AEM sito {#id_aem_site_config}

Per l&#39;output Sito AEM sono disponibili le seguenti opzioni:

| Opzioni AEM sito | Descrizione |
| --- | --- |
| Tipo di output | Tipo di output da generare. Per generare l&#39;output AEM sito reattivo, scegliete l&#39;opzione Sito AEM. |
| Nome impostazione | Assegna un nome descrittivo per le impostazioni del sito AEM che stai creando. Ad esempio, puoi specificare *Uscita clienti interni* o *output degli utenti finali*. |
| Nome sito | Un nome del sito in cui l’output viene memorizzato nell’archivio AEM.<br><br>Viene creato un nodo nell’archivio AEM con il nome specificato qui. Se non si specifica il nome del sito, il nodo del sito viene creato con il nome del file di mappa DITA.<br><br>Il nome del sito specificato viene utilizzato anche come titolo nella scheda del browser.<br><br>È inoltre possibile utilizzare le variabili durante l&#39;impostazione del nome del sito. Per ulteriori dettagli sull’utilizzo delle variabili, consulta [Utilizza le variabili per impostare le opzioni Percorso di destinazione, Nome sito o Nome file](generate-output-use-variables.md#id18BUG70K05Z). |
| Design | Selezionate il modello di progettazione da utilizzare per generare l’output.<br><br>Per informazioni sull’utilizzo dei modelli di progettazione personalizzati per generare l’output, contattare l’amministratore di pubblicazione. |
| Percorso di destinazione | Percorso all’interno dell’archivio AEM in cui è memorizzato l’output. Durante la generazione dell&#39;output finale, Nome sito e Percorso di destinazione vengono combinati. Ad esempio, se specifichi Nome sito come `user-guide` e il percorso di destinazione come `/content/output/aem-guides`, l&#39;output finale viene generato sotto la variabile `/content/output/aem-guides/user-guide` nodo.<br><br>È inoltre possibile utilizzare le variabili durante l&#39;impostazione del Percorso di Destinazione. Per ulteriori dettagli sull’utilizzo delle variabili, consulta [Utilizza le variabili per impostare le opzioni Percorso di destinazione, Nome sito o Nome file](generate-output-use-variables.md#id18BUG70K05Z). |
| Applica condizioni tramite | Selezionare una delle opzioni seguenti:<br><br>**Nessuno applicato**: Selezionare questa opzione se non si desidera applicare alcuna condizione all&#39;output pubblicato.<br>**File DITAVal**: Selezionare i file DITAVal per generare contenuto condizionale. È possibile selezionare più file DITAVal utilizzando la finestra di dialogo Sfoglia o digitando il percorso del file. Per rimuoverlo, utilizza l’icona a croce accanto al nome del file. I file DITAVal vengono valutati nell&#39;ordine specificato, quindi le condizioni specificate nel primo file hanno la precedenza rispetto alle condizioni corrispondenti specificate in file successivi. È possibile mantenere l&#39;ordine dei file aggiungendo o eliminando file. Se il file DITAVal viene spostato in un altro percorso o viene eliminato, non viene eliminato automaticamente dal dashboard mappa. È necessario aggiornare il percorso nel caso in cui i file vengano spostati o eliminati. Puoi passare il cursore sul nome del file per visualizzare il percorso nell’archivio AEM in cui è memorizzato il file. È possibile selezionare solo i file DITAVal e viene visualizzato un errore se si seleziona un altro tipo di file.<br>**Predefinito condizione**: Seleziona un predefinito per condizioni dal menu a discesa per applicare una condizione durante la pubblicazione dell’output. Questa opzione è visibile se è stata aggiunta una condizione per il file di mappa DITA. Le impostazioni condizionali sono disponibili nella scheda Predefiniti condizione della console mappa DITA. Per ulteriori informazioni sul predefinito di condizione, consulta [Utilizzare i predefiniti condizione](generate-output-use-condition-presets.md#id1825FL004PN). |
| Pagine di output esistenti | Seleziona la **Sovrascrivi contenuto** per sovrascrivere il contenuto delle pagine esistenti. Questa opzione sovrascrive solo il contenuto presente sotto i nodi contenuto e head della pagina. Questa opzione consente la pubblicazione combinata dei contenuti. Selezionando questa opzione è possibile selezionare l’eliminazione di pagine orfane dall’output pubblicato. Questo è anche il *default* per creare l&#39;output AEM del sito.<br><br>Seleziona la **Elimina e crea** per forzare l’eliminazione di tutte le pagine esistenti durante la pubblicazione. Questa opzione elimina il nodo della pagina con il relativo contenuto e tutte le pagine figlie al suo interno. Utilizza questa opzione se hai modificato il modello di progettazione del predefinito di output o se desideri rimuovere eventuali pagine aggiuntive già presenti nella destinazione. |
| Elimina pagine del sito orfano | Selezione della **Sovrascrivi contenuto** in **Pagine di output esistenti** presenta questa opzione. Se selezioni questa opzione, tutte le pagine orfane vengono eliminate dal sito AEM pubblicato. Affinché questa funzione possa essere eseguita correttamente, è necessario pubblicare l&#39;intera mappa DITA e non utilizzare la pubblicazione incrementale.<br><br>Supponiamo che sia stata pubblicata una mappa DITA contenente argomenti a.dita, b.dita e c.dita. Prima di pubblicare nuovamente la mappa, è stato rimosso l&#39;argomento b.dita dalla mappa. Ora, se si è selezionata questa opzione, tutti i contenuti relativi a b.dita vengono rimossi dall&#39;output AEM del sito e vengono pubblicati solo a.dita e c.dita.<br><br>Questa funzione non rimuove alcuna mappa figlio pubblicata. Ad esempio, se la mappa padre contiene una mappa figlio e si rimuove l’intera mappa figlio, il contenuto della mappa figlio non viene eliminato dall’output pubblicato. Tuttavia, se rimuovi un argomento da una mappa figlio e lo ripubblichi, il contenuto dell&#39;argomento rimosso viene eliminato dall&#39;output del sito.<br><br>Inoltre, se esiste un contenuto di riferimento e tale contenuto viene rimosso prima della ripubblicazione, i dati del contenuto di riferimento non vengono rimossi.<br><br>**Nota**: Le informazioni sulle pagine orfane eliminate vengono anche acquisite nei registri di generazione dell’output. Per ulteriori informazioni sull&#39;accesso ai file di log, vedi [Visualizza e controlla il file di registro](generate-output-basic-troubleshooting.md#id1821I0Y0G0A__id1822G0P0CHS). |
| Pulisci file temporanei DITA-OT | Selezionare questa opzione per pulire i file temporanei generati da DITA-OT. La posizione in cui DITA-OT memorizza i file temporanei si trova nel registro di generazione dell&#39;output.<br><br>Se si verificano errori durante la generazione dell&#39;output tramite DITA-OT, è possibile deselezionare questa opzione per mantenere i file temporanei. Puoi quindi utilizzare questi file per risolvere eventuali errori di generazione dell’output. |
| Genera un PDF separato per ogni argomento | Se selezionata, viene creato anche un PDF per ogni argomento della mappa DITA. Quando scegli questa opzione, viene visualizzata una nuova opzione Dividi percorso PDF.<br><br>Nel campo Percorso di PDF diviso specificare il percorso in cui memorizzare i PDF generati per ciascun argomento.<br><br>**Nota**: AEM Guide utilizza il plug-in DITA-OT denominato pdfx per generare PDF per ogni argomento. Questo plug-in è fornito in bundle con il pacchetto DITA-OT fornito out-of-the-box. Puoi personalizzare questo plug-in per generare PDF in base alle tue esigenze. Se utilizzi un plug-in DITA-OT personalizzato, assicurati di integrare il plug-in pdfx per disporre di funzionalità di generazione PDF a livello di argomento. |
| Esegui flusso di lavoro di post-generazione | Quando scegli questa opzione, viene visualizzato un nuovo elenco a discesa Flusso di lavoro di post generazione contenente tutti i flussi di lavoro configurati in AEM. È necessario selezionare un flusso di lavoro da eseguire dopo il completamento del flusso di lavoro di generazione dell’output. |
| Usa linea di base | Se è stata creata una baseline per la mappa DITA selezionata, selezionare questa opzione per specificare la versione da pubblicare.<br><br>**Importante**: Quando si genera l&#39;output incrementale per il sito AEM, l&#39;output viene creato utilizzando la versione corrente dei file e non la baseline allegata.<br><br>Vedi [Utilizzare la linea di base](generate-output-use-baseline-for-publishing.md#id1825FI0J0PF) per maggiori dettagli. |
| Proprietà | Seleziona le proprietà da elaborare come metadati. Queste proprietà vengono impostate dalla pagina Proprietà della mappa DITA o del file bookmap. Le proprietà selezionate dall’elenco a discesa sono elencate sotto il campo Proprietà e vengono rimosse dall’elenco a discesa.<br><br>**Nota**: Le proprietà dei metadati fanno distinzione tra maiuscole e minuscole.<br><br>*Se hai selezionato una baseline, i valori delle proprietà sono basati sulla versione della baseline selezionata.<br>* Se non hai selezionato una linea di base, i valori delle proprietà sono basati sulla versione più recente.<br><br>È inoltre possibile trasferire i metadati all&#39;output utilizzando la pubblicazione DITA-OT. Per maggiori dettagli vedi [Trasmettere i metadati all&#39;output utilizzando DITA-OT](pass-metadata-dita-ot.md#id21BJ00QD0XA).<br><br>**Nota**: Se non hai definito la `cq:tags` nell’opzione Proprietà , i valori per `cq:tags` vengono selezionati dalla copia di lavoro corrente anche se è stata selezionata una baseline per la pubblicazione. |
| Usa Proprietà Mappa Se Mancano Nell&#39;Argomento | Se selezionata, anche le proprietà definite per il file di mappa vengono copiate negli argomenti in cui tali proprietà non sono definite. Considera i seguenti punti durante l’utilizzo di questa opzione:<br><br>*Sulle pagine del sito AEM è possibile passare solo proprietà String, Date o Long (singole e con più valori).<br>* I valori dei metadati per una proprietà di tipo String non supportano caratteri speciali (ad esempio `@, #, " "`).<br>* Questa opzione deve essere utilizzata insieme al `Properties` opzione . |

## Nota aggiuntiva sul sito AEM

### Genera un output basato su articoli dall’editor web

È possibile generare l&#39;output AEM del sito per uno o più argomenti oppure l&#39;intera mappa DITA dall&#39;Editor Web. È necessario creare predefiniti di output per la mappa DITA e quindi è possibile generare facilmente l&#39;output AEM del sito per la mappa. Se hai aggiornato alcuni argomenti nella mappa, puoi anche generare l&#39;output AEM del sito solo per tali argomenti dall&#39;Editor Web. Per ulteriori dettagli, consulta [Pubblicazione basata su articoli dall’editor web](web-editor-article-publishing.md#id218CK0U019I).

### Genera argomenti di collegamento di output da altre mappe

È uno scenario molto comune avere un ampio set di documenti distribuiti su più cartelle e mappe DITA. Diventa estremamente complesso pubblicare contenuti collegati da diversi luoghi. Per impostazione predefinita, tutti i collegamenti `<xref>` vengono create con `local` `@scope`. La pubblicazione di tali argomenti non richiede alcuna sfida, in quanto utilizza un collegamento diretto all’argomento. Nel caso in cui l’argomento si trovi al di fuori della mappa DITA corrente, il collegamento non mostra il contenuto collegato.

Un altro modo per collegare i contenuti consiste nel creare un collegamento utilizzando il `peer` `@scope`. Per tale contenuto, il collegamento viene risolto in fase di esecuzione scegliendo il contesto configurato per l&#39;argomento collegato dal contesto di pubblicazione della mappa DITA. La schermata seguente mostra il pannello Proprietà per un collegamento con la `peer` `@scope`:

![](images/peer-link-scope-link.png){width="800" align="left"}

Per semplificare la pubblicazione di mappe e argomenti complessi che si collegano ad altri argomenti in altre mappe, AEM Guide ti consente di impostare il contesto di pubblicazione per ogni predefinito di output.

Il contesto di pubblicazione consente di specificare l’argomento da utilizzare per la mappatura della pubblicazione di un output specifico. Comprendiamo questo con l&#39;aiuto di un esempio — diciamo che avete quattro cartelle: campione a, campione b, campione c e campione d. Ogni cartella contiene una mappa DITA - Mappa DITA A, Mappa DITA B, Mappa DITA C e Mappa DITA D. Il collegamento Mappa incrociata si verifica quando un argomento nella Mappa DITA A si collega a un argomento nella Mappa DITA B, C o D. Nella schermata seguente, un argomento del concetto di esempio contiene collegamenti \(o riferimenti\) a file che fanno parte di altre mappe DITA.

![](images/sample-concept-link-to-other.png){width="450" align="left"}

Ora, quando configuri le impostazioni di pubblicazione AEM sito per il file di mappa che contiene questo argomento, puoi selezionare il contesto di pubblicazione per il contenuto collegato da utilizzare durante la pubblicazione. Un contesto di pubblicazione è una combinazione di mappa DITA e del relativo predefinito di output. Il predefinito di output, a sua volta, contiene una versione specifica del contenuto e dei predefiniti condizionali. L&#39;intera combinazione della mappa DITA, del predefinito di output, della versione \(files\) e delle condizioni definiscono il contesto di pubblicazione per una mappa collegata.

Esegui i seguenti passaggi per specificare il contesto di pubblicazione per i file collegati incrociati:

1. Apri **Predefiniti di output** scheda della mappa DITA da pubblicare.

1. Seleziona la **Sito AEM** predefinito di output.

   Vengono visualizzate le schede Impostazioni predefiniti AEM e Contesto pubblicazione .

   ![](images/aem-site-publish-settings.png){width="800" align="left"}

1. Apri **Contesto di pubblicazione** scheda .

   Viene visualizzato un elenco di argomenti dipendenti. Questi sono gli argomenti collegati da alcuni argomenti della mappa corrente, ma sono disponibili in altre mappe DITA.

   >[!NOTE]
   >
   > La scheda Contesto di pubblicazione mostra gli argomenti collegati tramite `peer` `@scope` solo. Per i collegamenti con `local` `@scope`, non è necessario specificare il contesto di pubblicazione.

   Per impostazione predefinita, per tutti gli argomenti collegati sono stati selezionati l’ultimo predefinito di output e la mappa.

   ![](images/default-publish-context.png){width="800" align="left"}

1. Per modificare la selezione predefinita della mappa e della preimpostazione DITA, fare clic su **Modifica** \(nella barra degli strumenti principale\).

1. Se desideri utilizzare l&#39;output pubblicato più di recente di ciascun file dipendente della mappa, seleziona **Usa contesto di pubblicazione generato più di recente per tutti gli argomenti dipendenti**.

1. In **Mappa padre** dall’elenco a discesa, seleziona il file mappa con il cui output desideri collegare l’output della mappa corrente.

   Quando selezioni un file di mappa, l’UUID della mappa viene visualizzato nella colonna UUID mappa padre . I predefiniti di output associati alla mappa selezionata sono elencati nell’elenco Predefiniti della mappa padre.

1. In **Preimpostazione mappa padre** dall’elenco a discesa, seleziona il predefinito di output con cui desideri collegare l’output della mappa corrente.

1. Seleziona la mappa richiesta e il relativo predefinito di output per tutti gli argomenti dipendenti e fai clic su **Fine**.

   Il contesto per gli argomenti dipendenti è ora impostato. Puoi generare l’output per la mappa corrente. Per ulteriori informazioni sulla generazione dell&#39;output, vedi [Genera output per una mappa DITA dalla console mappa](generate-output-for-a-dita-map.md#).

### Pubblicazione in fusione

AEM Guide supporta la pubblicazione di contenuto DITA all’interno del sito AEM esistente. Ad esempio, se si dispone di un sito esistente, è possibile utilizzare l&#39;output Sito AEM per pubblicare solo il contenuto DITA sul sito. In questo processo, il contenuto non DITA esistente non viene modificato dal processo di pubblicazione. Per ulteriori informazioni sull&#39;impostazione del sito per pubblicare solo il contenuto DITA, contattare l&#39;amministratore di pubblicazione.

### Pubblicazione `conref`

Se utilizzi `conref` nel contenuto, viene pubblicato come contenuto normale o incorporato insieme al contenuto nell&#39;argomento di origine \(o di provenienza\). La `conref` viene eseguito il rendering del contenuto insieme al contenuto principale e non viene creata alcuna pagina del sito separata per lo stesso contenuto. Quando si cerca il contenuto a cui si fa riferimento nel `conref`, quindi solo l&#39;argomento principale o la pagina contenente il `conref` il contenuto viene visualizzato nei risultati della ricerca.

>[!NOTE]
>
>Se hai generato pagine separate per `conref` utilizzando AEM Guide versione 3.5 o precedente, si consiglia di pulire/eliminare tali pagine utilizzando [Elimina pagine del sito orfano](#delete-orphan-page-aem-site) opzione .


### Cercare una stringa all’interno del contenuto

È possibile cercare una stringa nell&#39;output Sito AEM. Per impostazione predefinita, è possibile cercare la stringa solo nei titoli. Per cercare la stringa nel contenuto o nel corpo dell&#39;output del sito AEM, contattare l&#39;amministratore di sistema per abilitare la proprietà flattening.enabled.


<img src="images/aem-output-search.png" alt="Uscita AEM sito di ricerca" width="800">

Per ulteriori dettagli vedi *Configurare l&#39;appiattimento AEM struttura del nodo del sito* nella guida all’installazione e alla configurazione di guide Adobe Experience Manager .

**Argomento principale:**[ Informazioni sui predefiniti di output](generate-output-understand-presets.md)