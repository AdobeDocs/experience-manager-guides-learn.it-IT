---
title: Anteprima di un argomento
description: Scopri come visualizzare in anteprima un argomento
source-git-commit: cc0fbca257d82cc82db5b5da8d263309fd71de55
workflow-type: tm+mt
source-wordcount: '1815'
ht-degree: 0%

---


# Anteprima di un argomento {#id1696II000QR}

Una volta creato un argomento, AEM Guide genera un’anteprima dell’argomento. La modalità Anteprima offre diverse funzioni che è possibile utilizzare per lavorare con il documento.

Esegui i seguenti passaggi per visualizzare l’anteprima di un argomento:

1. Nell’interfaccia utente Assets, passa all’argomento da visualizzare.
1. Fai clic sull’argomento da visualizzare.

   Nell’interfaccia utente Assets viene visualizzata un’anteprima dell’argomento.

   >[!NOTE]
   >
   > È possibile visualizzare la versione dell&#39;argomento attivo o la mappa DITA nell&#39;angolo in alto a destra della scheda file dell&#39;argomento.

   >[!IMPORTANT]
   >
   > Il posizionamento delle seguenti funzioni nella barra degli strumenti Anteprima potrebbe variare in base alla configurazione del server di AEM. Alcune delle funzioni potrebbero essere disponibili nella barra degli strumenti principale, mentre altre potrebbero essere disponibili nel menu Altro.

## Funzioni disponibili in modalità Anteprima

![](images/preview-screen.png){width="800" align="left"}

Nella modalità Anteprima è possibile eseguire le operazioni seguenti dalla barra degli strumenti:

**Proprietà**

Visualizza le proprietà dell’argomento selezionato. In base alla versione AEM, è possibile visualizzare proprietà come metadati, pianificazione dell&#39;attivazione \(de\)attivazione, riferimenti, stato del documento e altro ancora.

>[!NOTE]
>
> La proprietà title di un argomento viene compilata automaticamente dal `title` tag dell&#39;argomento o della mappa DITA. Se si apporta una modifica al titolo utilizzando la finestra delle proprietà che la modifica viene persa. Per aggiornare la proprietà title, è necessario utilizzare l&#39;editor Web.

La pagina Proprietà contiene informazioni utili sui riferimenti, ad esempio dove viene utilizzata una mappa o un argomento o quali riferimenti sono contenuti in un documento. Nella pagina Proprietà sono elencati due tipi di riferimenti per un documento: **Utilizzato in** e **Riferimenti in uscita**.

La **Utilizzato in** i riferimenti elencano i documenti in cui viene fatto riferimento o utilizzato il file corrente. La **Riferimenti in uscita** elenca i documenti a cui si fa riferimento nel documento corrente.

L&#39;icona \(+\) nel **Utilizzato in** la sezione riferimenti consente di spostarsi ulteriormente verso l’alto per trovare il punto in cui l’argomento viene utilizzato o a cui viene fatto riferimento.

![](images/used-in-dialog_cs.png){width="800" align="left"}

Fai clic su ![](images/right-arrow-used-in-dialog.svg)accanto a un documento viene visualizzata la mappa o i file di argomento in cui il documento viene ulteriormente referenziato.

**Filtro condizionale \(A/B\)**

Se l’argomento include contenuto condizionale, verrà visualizzata l’icona A/B sulla barra degli strumenti. Facendo clic su questa icona viene visualizzata una finestra a comparsa che consente di filtrare il contenuto in base alle condizioni disponibili nell’argomento.

>[!NOTE]
>
> Il contenuto condizionale viene evidenziato utilizzando un colore di sfondo chiaro nell’editor web.

![](images/conditional-popup_cs.png){width="300" align="left"}

**Modifica**

- Aprire l&#39;argomento per la modifica nell&#39;Editor Web. La **Modifica** l’opzione non sarà disponibile se l’amministratore ha abilitato la **Disattiva modifica senza pagamento** opzione . Se l’opzione è attivata, verrà visualizzata la **Modifica** solo dopo aver estratto un file di argomento.

**Risoluzione dei tasti**

- Se si desidera utilizzare un file di spazio chiave per l&#39;argomento, fare clic sull&#39;icona Risoluzione tasti. È quindi possibile scegliere uno spazio chiave dal pop-up Risoluzione chiave.

**Origine**

- Aprire il codice sorgente XML di un file. Per visualizzare il codice XML sottostante di una mappa, argomento o file DITAVAL, aprire il file in modalità Anteprima e fare clic sull&#39;icona Origine. Il pop-up Origine XML visualizza il codice sorgente XML. Puoi selezionare un codice specifico dal file o premere `Ctrl`+`a` per selezionare l’intero contenuto.

   >[!NOTE]
   >
   > Per ottenere la visualizzazione del codice sorgente di un file di mappa DITA, selezionare il file nell’interfaccia utente Assets e fare clic su Origine.

   ![](images/xml-source-code-view-from-preview_cs.png){width="800" align="left"}

**Condividi collegamento UUID**

- AEM Guide consente di condividere i collegamenti basati su UUID per mappe DITA, argomenti e file immagine dalle posizioni seguenti:

   - Interfaccia utente Assets
   - Console della mappa DITA
   - Anteprima argomento o immagine

Una nuova opzione **Condividi collegamento UUID** è mostrato nella barra degli strumenti delle aree sopra menzionate. La schermata seguente mostra la **Condividi collegamento UUID** in modalità Anteprima di un argomento:

![](images/share-uuid-link_cs.png){width="800" align="left"}

Nell’interfaccia utente delle risorse, questa opzione è visibile quando selezioni un file. In modalità Anteprima, questa opzione è disponibile per impostazione predefinita nella barra degli strumenti principale. In una console mappa DITA, questa opzione è visibile nella sezione Predefiniti di output .

Una volta copiato l’URL, lo stesso può essere condiviso con altri utenti per consentire loro l’accesso diretto al file . Questo collegamento rimane valido anche quando il file viene spostato in un’altra posizione nell’archivio. L’unica volta che il collegamento avrà esito negativo è quando il file viene eliminato dalla directory archivio.

Se si condivide il collegamento dalla console mappa DITA o dalla modalità anteprima di un file, l&#39;utente ha visualizzato lo stesso file. Tuttavia, quando condividi il collegamento di un file mappa dall’interfaccia utente di Assets, l’utente viene portato alla console della mappa. Analogamente, per un argomento o un file immagine viene visualizzata l’anteprima del file.

>[!IMPORTANT]
>
> Il collegamento non può essere utilizzato come collegamento di riferimento in un altro argomento, ma fornisce solo accesso diretto al file nell’archivio. Inoltre, il collegamento rimane valido finché il file è disponibile nell’archivio. Anche se il file viene spostato in un’altra posizione nell’archivio, il collegamento rimane valido. Il collegamento avrà esito negativo solo quando il file viene eliminato dalla directory archivio.

**Check-Out/Check-In**

- Attiva/disattiva le funzioni Check-Out e Check-In. Quando un file viene estratto, l&#39;utente corrente ottiene un&#39;autorizzazione di scrittura esclusiva sul file. Un file estratto può essere aperto nell&#39;editor Web per la modifica. Dopo aver apportato le modifiche necessarie, fai clic sull’icona Archivia per salvare il file in DAM.

Quando si estrae un argomento, lo stato del file viene visualizzato come estratto nella vista a schede e nella vista a elenco.

File estratto nella vista a schede:

![](images/checkout-card-62.png){width="300" align="left"}

File estratto nella vista a elenco:

![](images/checkout-list-62.png){width="550" align="left"}

Se la colonna Estratto non è visibile, selezionare **Visualizza impostazioni** sotto **Vista a elenco** e seleziona la **Estratto** lo stato **Configura colonne** finestra di dialogo.

![](images/list-view-settings-check-out_cs.png){width="800" align="left"}

>[!TIP]
>
> Per le best practice sull’utilizzo del check-out e del check-in dei file, consulta la sezione Controllo delle versioni dei contenuti nella guida alle best practice .

**Differenza di versione basata sul web**

- Se l’argomento è stato modificato, puoi trovare facilmente le modifiche apportate in diverse versioni di tale argomento. Per scoprire le modifiche apportate alle diverse versioni di un argomento:

   >[!IMPORTANT]
   >
   > Il metodo descritto nella procedura seguente è applicabile solo per i file DITA. Per i file non DITA, utilizzare la visualizzazione Timeline per creare versioni o ripristinare una versione esistente di un file.

   1. Apri l’argomento in modalità Anteprima.

   1. Nella barra a sinistra, fai clic su **Cronologia versioni** e seleziona una versione.

      ![](images/timeline-versions62_cs.png){width="800" align="left"}

   1. Dalle versioni elencate, seleziona quella che desideri utilizzare come versione di base e fai clic su **Anteprima versione**. L&#39;anteprima della versione selezionata viene visualizzata nella finestra Anteprima versione.

   1. Da **Mostra differenze** selezionare la versione con cui si desidera confrontare la versione di base.

      ![](images/show-diff-list-cropped.png){width="800" align="left"}

      Il contenuto modificato viene evidenziato nell’anteprima dell’argomento. Il contenuto evidenziato in verde indica che il contenuto appena aggiunto e quello in rosso è il contenuto eliminato.

      ![](images/version-difference.png){width="800" align="left"}


### Ramo, ripristino e versioni successive {#id193PG0Y051X}

- In un ambiente di authoring tipico, è necessario creare un nuovo ramo di un argomento per soddisfare una versione specifica. Come per qualsiasi altro sistema di gestione delle versioni, AEM Guide ti consente di creare un ramo da una versione esistente di un argomento o di ripristinare una versione precedente di un argomento. Utilizzando le funzioni di gestione delle versioni offerte AEM Guide, puoi eseguire le seguenti operazioni:

   - Creazione di un ramo da una versione esistente di un argomento
   - Creare versioni successive in un nuovo ramo
   - Ripristino di una versione specifica di un argomento

   L’illustrazione seguente mostra il tipico sistema di ramificazione e di controllo delle versioni successive:

   ![](images/branching_illustration.png){width="550" align="center"}

   Per qualsiasi nuovo argomento, la prima versione è numerata come 1.0. In seguito, ogni nuova versione dell’argomento viene salvata con un numero incrementale come 1.1, 1.2 e così via. Una volta creato un ramo di un argomento, viene creato un nuovo ramo prendendo il numero di versione da cui viene creato il ramo e aggiungendo un valore 0 alla fine della versione. Come illustrato nell’illustrazione, viene creato un nuovo ramo dalla versione 1.1 di un argomento. La versione del nuovo ramo è 1.1.0. In seguito, ogni volta che si salva una nuova versione dell’argomento in questo ramo, ottiene un numero di versione incrementale come 1.1.1, 1.1.2 e così via.

   Simile al diramazione, puoi anche ripristinare la versione corrente o quella in uso in qualsiasi versione presente nell’archivio. Per ripristinare una versione, seleziona semplicemente la versione desiderata dell’argomento e fai clic su **Ripristina questa versione** in **Cronologia versioni** pannello.

   Esegui le seguenti operazioni per creare un ramo, ripristinare una versione e mantenere le versioni successive di un argomento:

   >[!IMPORTANT]
   >
   > Il metodo descritto nella procedura seguente è applicabile solo per i file DITA. Per i file non DITA, utilizzare la visualizzazione Timeline per creare versioni o ripristinare una versione esistente di un file.

   1. Accedi all’argomento nell’interfaccia utente di Assets.

      >[!NOTE]
      >
      > È inoltre possibile aprire l’argomento in modalità Anteprima e procedere con il passaggio 3.

   1. Selezionare l&#39;argomento di cui si desidera creare un ramo.

   1. Nella barra a sinistra, fai clic su **Cronologia versioni**.

      >[!NOTE]
      >
      > Viene visualizzato un elenco delle versioni disponibili per l’argomento selezionato. Ogni versione contiene la marca temporale, il nome utente, il commento sulla versione e [etichetta](web-editor-use-label.md#) informazioni.

   1. Seleziona una versione da cui desideri creare un ramo. Nella schermata seguente, la versione 1.2 viene selezionata per la creazione di un ramo.

      ![](images/branching.png){width="300" align="left"}

      >[!NOTE]
      >
      > La versione corrente di un argomento contiene *\(Current\)* indicato accanto al numero di versione.

   1. Fai clic su **Ripristina questa versione**.

      Viene visualizzato un messaggio che richiede di confermare la creazione di un nuovo ramo.

   1. *\(Facoltativo\)* Nel prompt dei messaggi, ottieni un’opzione per selezionare il **Salva La Copia Di Lavoro Corrente Come Una Nuova Versione**. In base alla selezione di questa opzione è possibile effettuare le seguenti due azioni:

      - Se selezioni questa opzione, viene creato un ramo dalla versione 1.1. Inoltre, viene creata una nuova versione dell&#39;argomento dalla copia di lavoro corrente dell&#39;argomento e salvata come versione successiva - 1.4.

         ![](images/next_version_created_over_working_copy.png){width="300" align="left"}

         La versione 1.2 diventa la copia di lavoro corrente dell&#39;argomento. Qualsiasi versione salvata dopo la creazione nel nuovo ramo di 1.1. Ad esempio, la versione successiva di un nuovo argomento in questo ramo verrà salvata come 1.2.0.

         ![](images/new_version_in_branch.png){width="300" align="left"}

      - Se non selezioni questa opzione, non viene creata alcuna nuova versione dalla copia di lavoro corrente dell’argomento. Viene creato un nuovo ramo dalla versione 1.2 dell’argomento. Qualsiasi versione successiva dell’argomento viene salvata nel ramo 1.2 come 1.2.0, 1.2.1 e così via.

         ![](images/new_version_without_working_copy.png){width="300" align="left"}
   1. Fai clic su **OK**.
   Viene creato un nuovo ramo dalla versione selezionata dell’argomento. Il processo di cui sopra è applicabile anche per ripristinare una versione specifica di un argomento. Per ripristinare una versione specifica tecnicamente è necessario creare un nuovo ramo dalla versione selezionata e rendere tale versione la copia di lavoro corrente dell’argomento. È inoltre possibile visualizzare la cronologia dei file che sono stati ripristinati nel rapporto Cronologia ripristino versione. Per maggiori dettagli su questo rapporto, vedi [Rapporto sulla cronologia delle versioni dei file ripristinati](reports-reverted-file-version-history.md#).

**Argomento principale:**[ Creazione e visualizzazione in anteprima degli argomenti](create-preview-topics.md)

