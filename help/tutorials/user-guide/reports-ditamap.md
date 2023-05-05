---
title: Report mappa DITA dal dashboard mappa
description: Scopri come eseguire il report mappa DITA dal dashboard mappa
exl-id: 8ba1dc83-fa96-4ae0-bfa8-89b5a8949f08
source-git-commit: c74badebbcb4733fb9caa79c646b1d1e5c8bfe8e
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 0%

---

# Report mappa DITA dal dashboard mappa {#id205BB800EEN}

AEM Guide offre agli amministratori le funzionalità di reporting per verificare l’integrità generale della documentazione prima che venga pubblicata o resa disponibile agli utenti finali. Il rapporto mappa DITA dal dashboard mappa in Guide AEM fornisce informazioni utili come gli argomenti mancanti, gli argomenti con elementi mancanti, l&#39;UUID degli argomenti e dei file multimediali di riferimento e lo stato di ogni argomento. Un rapporto dettagliato a livello di argomento fornisce anche informazioni relative al contenuto DITA, come riferimenti al contenuto e immagini mancanti o riferimenti incrociati.

>[!NOTE]
>
> AEM Guide aggiorna questo rapporto su ogni evento che determina una modifica nel file della mappa o quando viene aggiornato un riferimento all’interno del file dell’argomento.

Esegui i seguenti passaggi per visualizzare il rapporto Mappa DITA:

1. Nell’interfaccia utente Assets, individua e fai clic sul file di mappa DITA per il quale desideri visualizzare il rapporto.

1. Fai clic su **Rapporti**.

   ![](images/reports-page-uuid.png){width="800" align="left"}

   La pagina Rapporti è divisa in due parti:

   - **Riepilogo argomento:**

      Elenca il riepilogo complessivo del file di mappa selezionato. Osservando il Riepilogo, puoi rapidamente conoscere il numero totale di argomenti nella mappa, gli argomenti mancanti, il numero di argomenti con elementi mancanti, lo stato degli argomenti — In bozza, In revisione o Stato rivisto.

   - **Dettagli:**

      Quando fai clic su un argomento, viene visualizzato un rapporto dettagliato dell’argomento selezionato.

      ![](images/detailed-report-uuid.png){width="800" align="left"}

      Elementi evidenziati in **A**, **B**, **C** e **D** sono descritti di seguito:

      - **Argomento**: Titolo dell&#39;argomento specificato nella mappa DITA. Passando il puntatore del mouse sul titolo dell&#39;argomento viene visualizzato il percorso completo dell&#39;argomento. Se l’argomento presenta problemi, ad esempio riferimenti o immagini mancanti, prima del titolo dell’argomento viene visualizzato un punto rosso.

      - **Nome file**: Nome del file.

      - **UUID**: Identificatore univoco universale \(UID\) del file.

      - **Autore**: Utente che ha lavorato per ultimo su questo argomento.

      - **Stato del documento**: Lo stato corrente del documento: Bozza, In-Review o Revisione.

      - **Argomenti mancanti \(B\)**: Se sono presenti argomenti con riferimenti interrotti, tali argomenti sono elencati nell&#39;elenco Argomenti mancanti.

      - **Elementi mancanti**: Elenca il numero di immagini mancanti o eventuali riferimenti incrociati interrotti.

      - **Apri nell&#39;editor \(D\)**: Fare clic su questa icona per aprire l&#39;argomento nell&#39;editor Web.

   Elementi evidenziati in **E** sono descritti di seguito:

   - **Multimedia**: Il percorso delle immagini utilizzate nell’argomento viene mostrato insieme al relativo UID. Se fai clic sul percorso dell&#39;immagine, l&#39;immagine corrispondente viene aperta in una finestra a comparsa. I collegamenti immagine interrotti sono elencati in rosso.

   - **Riferimenti contenuto**: Il percorso del contenuto menzionato nell’argomento viene mostrato insieme al relativo UID. Se fai clic sul titolo del contenuto a cui si fa riferimento, l’argomento corrispondente viene aperto in modalità Anteprima.

   - **Riferimenti incrociati**: Il percorso del contenuto a cui si fa riferimento viene mostrato insieme al relativo UID. Se fai clic sul titolo del contenuto a cui si fa riferimento, l’argomento corrispondente viene aperto in modalità Anteprima. I riferimenti incrociati interrotti sono elencati in rosso.

   - **Revisione**: Mostra lo stato dell&#39;attività di revisione dell&#39;argomento. È possibile visualizzare lo stato \(apertura o chiusura\), la data di scadenza e l&#39;assegnatario dell&#39;argomento in esame. Se fai clic sul collegamento dell’argomento, questo apre l’argomento in modalità di revisione.

   - **Utilizzato in**: Mostra un elenco di altri argomenti o mappe in cui viene utilizzato l&#39;argomento. È inoltre elencato l’UUID di tutti questi argomenti e mappe.



Oltre al rapporto per ogni singolo argomento, gli amministratori possono accedere anche a informazioni quali la cronologia di pubblicazione di una mappa DITA. Per ulteriori informazioni sulla cronologia degli output generati, consulta [Visualizza lo stato dell&#39;attività di generazione dell&#39;output](generate-output-for-a-dita-map.md#viewing_output_history).

## Genera il rapporto di mappatura DITA CSV

Puoi scaricare ed esportare il CSV di un rapporto di mappa DITA. Il CSV contiene il rapporto dettagliato sulla mappa DITA.

Esegui i seguenti passaggi per generare il CSV di un rapporto di mappa DITA:

1. Fai clic su **Genera report** in alto a sinistra per generare il report mappa DITA.

   ![](images/generate-DITA-map-report.png){width="800" align="left"}

1. Riceverai una notifica quando il report sarà pronto per essere scaricato. Fai clic su **Scarica** per scaricare il CSV del rapporto generato.

   ![](images/download-report-dialog.png){width="550" align="left"}


   Puoi anche scaricare il CSV del rapporto generato in un secondo momento dalla casella in entrata della notifica AEM.

   Fai clic sul rapporto generato nella casella in entrata per scaricare il rapporto.

   ![](images/report-inbox--notification.png){width="300" align="left"}

Una volta scaricato il rapporto nella casella in entrata, puoi anche selezionarlo e utilizzare l’icona Apri nella parte superiore per aprire il rapporto selezionato.

**Argomento principale:**[ Rapporti](reports-intro.md)
