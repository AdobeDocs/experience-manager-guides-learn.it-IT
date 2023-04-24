---
title: Report mappa DITA dall'editor Web
description: Scopri come eseguire la mappatura DITA del report dall'editor Web
source-git-commit: 895d9bd3587c871d5223df5b71403d10bdc3d762
workflow-type: tm+mt
source-wordcount: '1608'
ht-degree: 0%

---


# Report mappa DITA dall&#39;editor Web {#id231HF0Z0NXA}

AEM Guide include una funzione nell’editor Web che consente di controllare l’integrità generale dei riferimenti e di generare rapporti per essi.

È possibile visualizzare l&#39;elenco degli argomenti, gestire i metadati di tutti i riferimenti e visualizzare l&#39;elenco multimediale per la mappa corrente dalla **Rapporti** nell&#39;editor Web.

## Generare un CSV dalla vista Elenco argomenti

La **Elenco argomenti** visualizza fornisce informazioni dettagliate sugli argomenti, ad esempio il tipo di riferimento, lo stato del documento e l&#39;autore.

Puoi creare un rapporto sugli argomenti eseguendo i seguenti passaggi:

1. In **Archivio** aprire il file mappa DITA in Vista mappa.
1. Fai clic sul pulsante **Gestisci** scheda .
1. Fare doppio clic **Elenco argomenti** a sinistra. Viene visualizzato l&#39;elenco degli argomenti presenti nella mappa DITA.

   ![](images/web-editor-topiclist-panel.png)

1. Da **Filtri** Il pannello consente di filtrare gli argomenti in base alla **Tipo di riferimento** \(diretto o indiretto\), **Stato del documento** \(lo stato corrente degli argomenti. Ad esempio, se gli argomenti sono nello stato Modifica, In revisione o Revisione, sono elencati\) o il **Autore** dell&#39;argomento.
1. È inoltre possibile utilizzare le seguenti opzioni di filtro argomento per scegliere di visualizzare le colonne seguenti nell’elenco:

   - **Argomento** Il titolo dell&#39;argomento viene specificato nella mappa DITA. Puoi fare clic sull’argomento per modificarlo.
   - **Nome file** Nome del file.
   - **UUID** Identificatore univoco universale \(UID\) del file.
   - **Posizione file** Percorso completo dell&#39;argomento.
   - **Tipo di riferimento** Tipo di riferimento - diretto o indiretto.
   - **Stato del documento** Lo stato corrente dell&#39;argomento.
   - **Autore** Utente che ha lavorato per ultimo sull&#39;argomento.
   - **Mappa padre** L&#39;elenco di tutte le mappe in cui l&#39;argomento è direttamente referenziato.

   >[!NOTE]
   >
   > Fai clic su **Aggiorna** per ottenere un nuovo elenco di argomenti e vedere eventuali modifiche nel file della mappa o se viene aggiornato un riferimento nel file dell&#39;argomento.

1. Fai clic su **Scarica CSV** per scaricare lo snapshot corrente degli argomenti nella mappa DITA. Il CSV contiene le colonne selezionate e gli argomenti filtrati nel **Elenco argomenti** visualizza. Puoi quindi aprire questo file CSV dell’elenco di argomenti in qualsiasi editor CSV.

**Gestire i metadati in blocco dal rapporto Metadati**

AEM Guide consente di assegnare tag al contenuto DITA dall’editor Web. È possibile applicare tag su un singolo argomento o utilizzare la funzione di assegnazione tag in blocco per applicare più tag su più argomenti, su una mappa DITA o su una mappa secondaria. È inoltre possibile modificare lo stato del documento di tutti gli argomenti selezionati al successivo stato comune del documento.

## Visualizzare i metadati

Per visualizzare i metadati dei riferimenti nella mappa DITA corrente, eseguire le operazioni seguenti:

1. Nel pannello Archivio, apri il file mappa DITA in Vista mappa.
1. Fai clic sul pulsante **Gestisci** scheda .
1. Fare doppio clic **Metadati** a sinistra. Viene visualizzato l&#39;elenco dei metadati di tutti i riferimenti nella mappa DITA. Questo include anche i riferimenti multimediali.

   ![](images/web-editor-metadata-panel.png)

1. Da **Filtri** puoi filtrare gli argomenti in base a **Stato del documento** \(lo stato corrente degli argomenti. Ad esempio, se gli argomenti sono nello stato Modifica, In revisione o Revisione, sono elencati\), **Riferimenti** \(diretto o indiretto\), **Tipo di file** \(Mappa, Argomento e Immagine\) del riferimento.
1. Puoi anche scegliere di visualizzare solo il **File senza tag** o anche scegliere tag specifici dal **Tag** per visualizzare i file associati.
   1. È inoltre possibile utilizzare le seguenti opzioni di filtro argomento per scegliere di visualizzare le colonne seguenti nell’elenco dei metadati:
      - **Titolo** \(selezionato per impostazione predefinita\) Il titolo del file di riferimento è specificato nella mappa DITA. È possibile fare clic sul file per modificarlo.È inoltre possibile fare clic e riprodurre un file audio o video nell&#39;Editor Web. È possibile modificare il volume o la visualizzazione del video. Nel menu di scelta rapida sono disponibili anche le opzioni per scaricare, modificare la velocità di riproduzione o visualizzare l&#39;immagine nell&#39;immagine.

         >[!NOTE]
         >
         > L’icona Estratto viene visualizzata anche accanto al titolo di un file estratto. Puoi passare il cursore sull’icona per visualizzare il nome dell’utente.

      - **Nome file** Nome del file.
      - **Posizione file** Percorso completo del file.
      - **Tag** \(selezionato per impostazione predefinita\) Tag applicati al file.

         >[!NOTE]
         >
         > Per impostazione predefinita, sono disponibili due tag per un file. Per visualizzare altri tag, fai clic su **Mostra altro**. Fai clic su **Mostra meno** per contrarre nuovamente l&#39;elenco.

      - **Tipo di riferimento** Tipo di riferimento - diretto o indiretto
      - **Stato del documento** \(selezionato per impostazione predefinita\) Lo stato corrente del file di riferimento.
      - **Tipo di file** \(selezionato per impostazione predefinita\) Tipo del file di origine. Le opzioni disponibili sono Mappa, Argomento e Immagine.
      - **Estratto da** Utente che ha estratto il file.
1. Fai clic su **Scarica CSV** per scaricare lo snapshot corrente dei riferimenti nella mappa DITA. Il CSV contiene le colonne selezionate e i riferimenti filtrati nella vista Elenco argomenti. Puoi quindi aprire questo file CSV di metadati in qualsiasi editor CSV.

**Aggiornare i metadati**

1. Per aggiornare i metadati, selezionare i file di cui si desidera aggiornare.

   >[!NOTE]
   >
   > Non è possibile selezionare alcun file estratto. L’icona Estratto viene visualizzata anche accanto al titolo di un file estratto. Puoi passare il cursore sull’icona per visualizzare il nome dell’utente.

1. Seleziona **Gestisci** dall&#39;alto.

   ![](images/web-editor-manage-metadata.png)

1. Per aggiungere nuovi tag, selezionateli dall’elenco a discesa per applicarli a tutti gli argomenti selezionati. Per eliminare un tag, fai clic sull’icona a croce accanto al tag .

   >[!NOTE]
   >
   > Vengono elencati i tag comuni applicati a tutti gli argomenti selezionati.

1. Selezionare un nuovo stato del documento se si desidera modificare lo stato del documento di tutti i riferimenti selezionati. Il menu a discesa visualizza lo stato possibile comune per tutti gli argomenti selezionati. Ad esempio, se lo stato corrente degli argomenti è In-Review, è possibile visualizzare lo stato Bozza, Approvato o Rivisto.
1. Fai clic su **Aggiorna** per aggiornare i metadati. Viene visualizzato un messaggio di conferma per i metadati, indipendentemente dal fatto che siano stati aggiornati correttamente o che siano presenti aggiornamenti non riusciti. Fai clic anche su **Download del rapporto** per scaricare i metadati CSV dalla finestra di dialogo di conferma. Questo CSV contiene i dettagli dello stato di aggiornamento dei riferimenti selezionati.

## Genera un rapporto multimediale

La **Multimedia** Il rapporto fornisce informazioni dettagliate sui file multimediali utilizzati nella mappa, ad esempio il titolo, il tipo \(audio, video e immagini\), i file in cui vengono utilizzati i file multimediali e il tipo di riferimento dei file in cui sono stati utilizzati. Puoi anche visualizzare l’UUID e la posizione dei file multimediali all’interno dell’archivio. È possibile creare un rapporto dei file multimediali eseguendo i seguenti passaggi:

1. In **Archivio** aprire il file mappa DITA in Vista mappa.
1. Fai clic sul pulsante **Gestisci** scheda .
1. Fare doppio clic **Multimedia** a sinistra. Viene visualizzato l&#39;elenco dei file multimediali presenti nella mappa DITA.
1. Da **Filtri** è possibile ordinare l’elenco per elementi multimediali o per i nomi utilizzati nei riferimenti.

   - Quando ordini per **Multimedia**, il nome****del file multimediale viene visualizzato nella prima colonna e quindi i nomi di tutti i riferimenti in cui sono stati utilizzati, vengono visualizzati in un&#39;altra colonna della stessa riga. Ad esempio, la schermata seguente mostra il WarmCoolForC.gif multimediale nella prima colonna e tre riferimenti in cui viene utilizzato, vengono visualizzati nella terza colonna sulla stessa riga.

      ![](images/multimedia-report-file-order.png)

   - Se ordini per **Utilizzato in** La vista trasposta è visibile quando i nomi dei riferimenti in cui sono stati utilizzati i contenuti multimediali sono elencati nella prima colonna, mentre i nomi multimediali sono elencati in un&#39;altra colonna su righe separate. Ad esempio, la schermata seguente mostra i nomi di tre riferimenti \(Regolare la temperatura del sedile, Cambiare la visualizzazione della temperatura del sedile e l&#39;area dell&#39;equipaggio\) nella prima colonna e il WarmCoolForC.gif multimediale viene visualizzato nella terza colonna su tre righe separate.

      ![](images/multimedia-report-used-in-order.png)

1. Puoi filtrare i contenuti multimediali in base al **Tipo multimediale** e **Tipo di riferimento**. L’elenco dei file multimediali viene visualizzato in base alla selezione effettuata nell’elenco a discesa. Ad esempio, è possibile scegliere di visualizzare solo i riferimenti audio nella mappa DITA e un file mostra solo i riferimenti audio utilizzati nella mappa.

   >[!NOTE]
   >
   > A seconda del tipo di contenuti multimediali utilizzati nella mappa, le opzioni Immagine, Video e Audio sono elencate nella **Tipo multimediale** e Diretta o Indiretta sono elencati in **Tipo di riferimento** a discesa.

1. È inoltre possibile utilizzare le seguenti opzioni di filtro per scegliere di visualizzare le colonne seguenti nell’elenco:

   - **Multimedia** \(selezionato per impostazione predefinita\) Il titolo del file multimediale è specificato nella mappa DITA. È possibile fare clic sui file multimediali per modificarli.
   - **Posizione multimediale** Il percorso completo del multimedia.
   - **UUID multimediale** Identificatore univoco universale \(UID\) del file.
   - **Tipo multimediale** \(selezionato per impostazione predefinita\) Tipo del file multimediale. Le opzioni disponibili sono Audio, Video o Immagine.
   - **Utilizzato in** \(selezionato per impostazione predefinita\) I riferimenti in cui è stato utilizzato il file multimediale. Puoi fare clic sul riferimento per modificarlo.
   - **Tipo di riferimento** \(selezionato per impostazione predefinita\) Il tipo di riferimento - diretto o indiretto.

   >[!NOTE]
   >
   > Fai clic su **Aggiorna** per ottenere un nuovo elenco di contenuti multimediali e vedere eventuali modifiche nel file mappa o se vengono aggiornati elementi multimediali nella mappa DITA.
1. È inoltre possibile fare clic e riprodurre un file audio o video nell’Editor Web. È possibile modificare il volume o la visualizzazione del video. Nel menu di scelta rapida sono disponibili anche le opzioni per scaricare, modificare la velocità di riproduzione o visualizzare l&#39;immagine nell&#39;immagine.
   ![](images/video-web-editor.png)

1. Fai clic su **Scarica CSV** per scaricare lo snapshot corrente del file multimediale nella mappa DITA. Il CSV contiene le colonne selezionate e i file multimediali filtrati nel **Multimedia** visualizza. Puoi quindi aprire questo file CSV multimediale in qualsiasi editor CSV.

**Argomento principale:**[ Rapporti](reports-intro.md)

