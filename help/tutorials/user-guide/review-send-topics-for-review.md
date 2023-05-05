---
title: Invia argomenti per la revisione
description: Scopri come inviare argomenti per la revisione
exl-id: 7a9b36ad-44d4-4952-9906-d95feb95d0c6
source-git-commit: 8823669fd29e8a40a41f9ca5d654b38fbea8e2fa
workflow-type: tm+mt
source-wordcount: '2733'
ht-degree: 0%

---

# Invia argomenti per la revisione {#id199RD0S035Z}

Il flusso di lavoro di revisione crea un ambiente per più revisori in cui l’iniziatore specifica un elenco di argomenti da esaminare, aggiunge più revisori e assegna una timeline per l’attività di revisione. AEM Guide consente agli utenti appartenenti ai gruppi Autori e Editori di avviare una revisione.

Poiché il flusso di lavoro di revisione è specifico per il progetto, l’iniziatore della revisione deve far parte del team del progetto o deve disporre dei diritti per creare un progetto. Al momento della creazione di un progetto, è possibile definire i membri del team per il progetto e assegnare loro vari ruoli o gruppi. Per ulteriori informazioni sui progetti, consulta [Creare un progetto DITA](authoring-create-dita-project.md#).

Puoi creare un&#39;attività di revisione da:

- **Editor web**: Consente di inviare un singolo argomento o una mappa DITA per la revisione. Il flusso di lavoro per la creazione di un’attività di revisione è comune nell’interfaccia utente di Editor web e Assets. Differisce solo il metodo di avvio del flusso di lavoro di revisione. Per informazioni sull&#39;avvio del flusso di lavoro di revisione dall&#39;editor Web, vedere [Crea attività di revisione](web-editor-features.md#id215OCJ00JXA) nell&#39;editor Web.

- **Interfaccia utente Assets**: Consente di inviare uno o più argomenti e la mappa DITA per la revisione. La condivisione di documenti per la revisione dal flusso di lavoro dell’interfaccia utente di Assets è trattata in questo argomento.


Dall’interfaccia utente Assets, sono disponibili due modi in cui un autore/editore può creare un’attività di revisione:

- Invia uno o più argomenti per la revisione
- Invia più argomenti da una mappa DITA per la revisione

## Invia uno o più argomenti per la revisione {#id1721E600FY4}

>[!IMPORTANT]
>
> Prima di creare un’attività di revisione, accertati di aver creato un progetto e aggiunto i revisori a tale progetto.

Per creare un&#39;attività di revisione e inviare argomenti per la revisione, esegui i seguenti passaggi:

>[!NOTE]
>
> È possibile creare un&#39;attività di revisione solo se si è un autore o un editore in un progetto DITA.

1. Passa alla cartella desiderata nell’interfaccia utente di Assets.

1. Fai clic sull’icona Seleziona nell’azione rapida e seleziona gli argomenti da inviare per la revisione.

   ![](images/select-asset-62.png){width="300" align="left"}

1. Nella barra degli strumenti, fai clic su **Crea attività di revisione**. Viene visualizzata la pagina di creazione dell’attività di revisione.

   >[!NOTE]
   >
   > È possibile creare un&#39;attività di revisione solo per gli argomenti con una revisione. Nel caso in cui l’argomento selezionato non disponga di una revisione, verrà visualizzato un prompt.

   ![](images/create-review-task-023.png){width="650" align="left"}

1. Inserisci un **Titolo** per l&#39;attività e selezionare un DITA **Progetto** dall’elenco a discesa.

1. In **Assegna a** campo a discesa, seleziona i revisori a cui desideri inviare gli argomenti per la revisione.

   È possibile assegnare un’attività di revisione a singoli utenti del progetto o a gruppi di utenti. È possibile assegnare un&#39;attività di revisione ai singoli utenti solo quando si fa parte del gruppo di amministratori del progetto, altrimenti verranno visualizzati solo i gruppi di utenti nel campo Assegna a.

   >[!NOTE]
   >
   > Il flusso di lavoro di revisione è specifico per il progetto. Quando crei progetti, aggiungi i membri del team al progetto e assegnali ai gruppi. Quindi quando si seleziona il progetto qui, si possono scegliere i membri che fanno parte del progetto. Per ulteriori informazioni sui progetti, consulta [Creare un progetto DITA](authoring-create-dita-project.md#).

1. Inserisci un **Descrizione** per l&#39;attività.

   Questa descrizione viene utilizzata come corpo dell’e-mail di notifica inviata ai revisori.

1. Seleziona la **Data di scadenza** e l&#39;ora per segnare il termine per la revisione.

   >[!NOTE]
   >
   > Una volta raggiunto il termine, viene inviata un’e-mail all’iniziatore con la notifica che l’attività di revisione è stata completata. L&#39;iniziatore può prorogare la scadenza dell&#39;attività di revisione dalla [Dashboard di revisione](review-manage-tasks-review-dashboard.md#).

1. Seleziona la mappa principale dal **Percorso del carrello**. Questa rootmap viene utilizzata per risolvere tutti i riferimenti chiave e i termini del glossario utilizzati nel contenuto della revisione. Se non si seleziona la rootmap, i riferimenti chiave o i termini del glossario associati all&#39;argomento DITA non verranno risolti prima di inviare l&#39;argomento per la revisione.

   Se si sta creando la revisione per una mappa DITA, per impostazione predefinita **Percorso del carrello** è impostato sul percorso di quella mappa. Se stai creando la revisione per uno o più argomenti, per impostazione predefinita la **Percorso del carrello** è impostato sulla mappa definita in Preferenze utente.

   >[!NOTE]
   >
   > La mappa radice selezionata ha la precedenza più alta per risolvere i riferimenti chiave. Per ulteriori dettagli, consulta [Risolvere i riferimenti chiave](map-editor-other-features.md#id176GD01H05Z).

1. Poiché puoi assegnare diversi revisori a diversi argomenti, **Consenti agli assegnatari di esaminare qualsiasi argomento** l&#39;opzione controlla se i revisori possono esaminare tutti gli argomenti di un&#39;attività di revisione o solo gli argomenti a cui sono assegnati per la revisione.

   Se si desidera consentire a tutti i revisori di esaminare qualsiasi argomento nell&#39;attività di revisione, selezionare **Consenti agli assegnatari di esaminare qualsiasi argomento**.

   Se non selezioni questa opzione, i revisori aggiunti nella **Assegna a** avrà accesso per rivedere solo gli argomenti ad essi assegnati.

1. Fai clic su **Avanti**.

   Viene visualizzata la pagina Contenuto .

   ![](images/content_page_review.png){width="800" align="left"}

1. Nella pagina Contenuto , seleziona una versione dell’argomento da condividere per la revisione.

   Per selezionare una versione è possibile utilizzare uno dei metodi seguenti:

   - *\(Predefinito\)* Scegli l’opzione **Versione più recente** per selezionare l&#39;ultima revisione salvata degli argomenti.
   - Scegli la **Versione attiva** e specifica la data e l’ora in cui selezionare una versione in base alla data e all’ora specificate. Se alla data specificata non è disponibile alcuna versione dell’argomento, viene selezionata una versione disponibile immediatamente dopo la data e l’ora specificate.
   - Scegli la **Seleziona un’etichetta** e seleziona un’etichetta dall’elenco a discesa.
1. Dopo aver selezionato una versione, fai clic su **Applica**.

   Per gli argomenti viene scelta la versione in base all’opzione selezionata.

   >[!NOTE]
   >
   > Puoi anche selezionare manualmente la versione desiderata dalla **Versione** elenco a discesa di ciascun argomento.

1. Fai clic su **Avanti**.

   Viene visualizzata la pagina Revisori in cui è possibile aggiungere o rimuovere i revisori. Per impostazione predefinita, i revisori aggiunti nel campo Assegna a vengono aggiunti automaticamente a ogni argomento selezionato per la revisione.

   ![](images/add-reviewers-topics.png){width="650" align="left"}

1. Nella pagina Revisori è possibile aggiungere o rimuovere revisori. Nella pagina Revisori sono disponibili le seguenti operazioni:

   - **Seleziona tutto**: Seleziona tutti gli argomenti nell’elenco degli argomenti. È possibile eseguire facilmente un&#39;operazione batch dopo aver selezionato tutti gli argomenti.
   - **Cancella selezione**: Deseleziona gli argomenti selezionati nell’elenco degli argomenti.

      >[!NOTE]
      >
      > Puoi anche selezionare o deselezionare un argomento singolarmente facendo clic sulla casella di controllo accanto all’argomento.

   - **Aggiungi**: Visualizza la finestra di dialogo Aggiungi revisori. È possibile digitare il nome di un revisore o di un ruolo utente \(o gruppo\) che si desidera aggiungere come revisore agli argomenti selezionati.
   - **Rimuovi**: Visualizza la finestra di dialogo Rimuovi revisori. È possibile digitare il nome di un revisore o di un ruolo utente \(o gruppo\) che si desidera rimuovere come revisore dagli argomenti selezionati.

      >[!NOTE]
      >
      > È inoltre possibile rimuovere una revisione da un argomento facendo clic sul segno a croce nella casella del revisore.

   - **Riassegna**: Visualizza la finestra di dialogo Riassegna revisori. È possibile digitare il nome di un revisore o di un ruolo utente \(o gruppo\) a cui si desidera assegnare l&#39;attività di revisione. Questo rimuove tutti i revisori esistenti dagli argomenti selezionati e assegna i revisori appena selezionati a tali argomenti.
   - **Esporta**: Consente di esportare i dettagli dell’attività di revisione in un file CSV. Il file contiene dettagli quali il percorso e il titolo dell&#39;argomento, il nome del revisore e la versione degli argomenti inviati per la revisione.
   - **Modifica revisori**: Fai clic su ![](images/edit_pencil_icon.svg)Nell’elenco degli argomenti viene visualizzata la finestra di dialogo Modifica revisori. È possibile aggiungere o rimuovere revisori per l&#39;argomento selezionato da questa finestra di dialogo.
1. Fai clic su **Crea** per creare l&#39;attività di revisione.

   Viene visualizzato un messaggio di conferma quando l’attività di revisione viene creata correttamente. La [Stato del documento](web-editor-document-states.md#) per gli argomenti inviati per la revisione è impostato su In-Review.

   >[!NOTE]
   >
   > È inoltre possibile fare clic sulla campana Notifiche in alto a destra dello schermo e confermare che l&#39;attività di revisione è stata creata correttamente. Nel pannello Notifiche, troverai una notifica per i revisori che facevano parte dell’attività di revisione e una notifica per l’iniziatore della revisione.


Viene inviata un&#39;e-mail a tutti i revisori con la notifica che gli è stato assegnato uno o più argomenti da esaminare. L’e-mail contiene un collegamento diretto che possono fare clic sull’argomento e accedervi in una finestra del browser.

Se vengono assegnati più argomenti, i revisori possono visualizzarli e selezionarli in un elenco a discesa di argomenti nel browser Web.

## Invia più argomenti per la revisione da una mappa DITA

Una mappa DITA è un&#39;organizzazione logica di argomenti all&#39;interno di un libro. Quando si invia un singolo argomento per la revisione, il revisore non riceve alcuna informazione sulla posizione di tale argomento nel libro. Se un revisore dispone di informazioni sulla posizione esatta dell&#39;argomento da rivedere, il revisore ottiene un contesto migliore dell&#39;argomento da rivedere.

AEM Guide consente di inviare uno o più argomenti in una mappa DITA per la revisione allo stesso tempo. Il revisore può visualizzare l&#39;intero file mappa insieme agli argomenti condivisi per la revisione. Questo rende più facile per il revisore ottenere un contesto dell&#39;argomento nella mappa o nel file del libro.

È possibile condividere la stessa mappa DITA in per la revisione in più attività di revisione. Ad esempio, se in una mappa DITA sono presenti gli argomenti A, B, C, D ed E. In un&#39;attività di revisione è possibile condividere A, B e C per la revisione e in un&#39;altra attività di revisione è possibile inviare gli argomenti C, D ed E per la revisione. Il processo di revisione consente di condividere lo stesso argomento e mappare il file in più attività di revisione. Per l&#39;argomento comune in più attività di revisione, i commenti forniti in un&#39;attività di revisione non sovrascrivono o uniscono i commenti nelle altre attività di revisione.

>[!IMPORTANT]
>
> Nel caso in cui un argomento di un file di mappa sia stato condiviso in più attività di revisione, il loro stato risulterebbe In-Review fino al completamento di tutte le attività di revisione.

Per inviare uno o più argomenti insieme al file della mappa per la revisione, esegui i seguenti passaggi:

>[!IMPORTANT]
>
> Una volta avviata la revisione tramite un file mappa, non è necessario modificare la struttura del file mappa aggiungendo nuovi argomenti o rimuovendo quelli esistenti.

1. Passa alla cartella desiderata nell’interfaccia utente di Assets.

   >[!NOTE]
   >
   > Assicurati che la vista della console sia impostata sulla vista a schede o a elenco.

1. Seleziona la mappa da cui vuoi inviare gli argomenti per la revisione.

1. Nella barra degli strumenti, fai clic su **Crea attività di revisione**. Viene visualizzata la pagina di creazione dell’attività di revisione.

1. Inserisci un **Titolo** per l&#39;attività e selezionare un DITA **Progetto** dall’elenco a discesa.

   >[!NOTE]
   >
   > È possibile creare un&#39;attività di revisione solo per gli argomenti con una revisione. Nel caso in cui la mappa contenga argomenti che non hanno una revisione, viene visualizzato un prompt con un elenco di tali file. I file senza revisione sono esclusi dall’attività di revisione.

1. In **Assegna a** campo a discesa, seleziona i revisori a cui desideri inviare gli argomenti per la revisione.

   È possibile assegnare un’attività di revisione a singoli utenti del progetto o a gruppi di utenti. È possibile assegnare un&#39;attività di revisione ai singoli utenti solo quando si fa parte del gruppo di amministratori del progetto, altrimenti verranno visualizzati solo i gruppi di utenti nel campo Assegna a.

   >[!NOTE]
   >
   > Il flusso di lavoro di revisione è specifico per il progetto. Quando crei progetti, aggiungi i membri del team al progetto e assegnali ai gruppi. Quindi quando si seleziona il progetto qui, si possono scegliere i membri che fanno parte del progetto. Per ulteriori informazioni sui progetti, consulta [Creare un progetto DITA](authoring-create-dita-project.md#).

1. Inserisci un **Descrizione** per l&#39;attività.

   Questa descrizione viene utilizzata come corpo dell’e-mail di notifica inviata ai revisori.

1. Seleziona la **Data di scadenza** e l&#39;ora per segnare il termine per la revisione.

   >[!NOTE]
   >
   > Una volta raggiunto il termine, viene inviata un’e-mail all’iniziatore con la notifica che l’attività di revisione è stata completata. L&#39;iniziatore può prorogare la scadenza dell&#39;attività di revisione dalla [Dashboard di revisione](review-manage-tasks-review-dashboard.md#).

1. Poiché puoi assegnare diversi revisori a diversi argomenti, **Consenti agli assegnatari di esaminare qualsiasi argomento** l&#39;opzione controlla se i revisori possono esaminare tutti gli argomenti di un&#39;attività di revisione o solo gli argomenti a cui sono assegnati per la revisione.

   Se si desidera consentire a tutti i revisori di esaminare qualsiasi argomento nell&#39;attività di revisione, selezionare **Consenti agli assegnatari di esaminare qualsiasi argomento**.

   Se non selezioni questa opzione, i revisori aggiunti nella **Assegna a** avrà accesso per rivedere solo gli argomenti ad essi assegnati.

1. Fai clic su **Avanti**.

   La pagina Contenuto viene visualizzata con tutti gli argomenti a cui si fa riferimento dal file mappa. Se la mappa DITA contiene mappe nidificate, vengono elencati anche gli argomenti delle mappe nidificate.

   ![](images/content-page-map-review.png){width="800" align="left"}

1. Nella pagina Contenuto , seleziona una versione dell’argomento da condividere per la revisione.

   Per selezionare una versione è possibile utilizzare uno dei metodi seguenti:

   - *\(Predefinito\)* Scegli l’opzione **Versione più recente** per selezionare l&#39;ultima revisione salvata degli argomenti.
   - Scegli la **Versione attiva** specifica la data e l’ora in cui selezionare una versione in base alla data e all’ora. Se alla data specificata non è disponibile alcuna versione dell’argomento, viene selezionata una versione disponibile immediatamente dopo la data e l’ora specificate.
   - Scegli la **Seleziona un’etichetta** e seleziona un’etichetta dall’elenco a discesa. Tutti gli argomenti contenenti l’etichetta selezionata vengono selezionati nella **Versione** elenco a discesa.
   - Scegli la **Selezionare una linea di base** e seleziona una baseline dall’elenco a discesa. Tutte le versioni degli argomenti che fanno parte della linea di base selezionata vengono selezionate nella **Versione** elenco a discesa.
1. Dopo aver selezionato una versione, fai clic su **Applica**.

   Per gli argomenti viene scelta la versione in base all’opzione selezionata.

   >[!NOTE]
   >
   > Puoi anche selezionare manualmente la versione desiderata dalla **Versione** elenco a discesa di ciascun argomento.

1. Fai clic su **Avanti**.

   Viene visualizzata la pagina Revisori in cui è possibile aggiungere o rimuovere i revisori. Per impostazione predefinita, i revisori aggiunti nel campo Assegna a vengono aggiunti automaticamente a ogni argomento selezionato per la revisione.

1. Nella pagina Revisori è possibile aggiungere o rimuovere revisori. Nella pagina Revisori sono disponibili le seguenti operazioni:

   - **Seleziona tutto**: Seleziona tutti gli argomenti nell’elenco degli argomenti. È possibile eseguire facilmente un&#39;operazione batch dopo aver selezionato tutti gli argomenti.
   - **Cancella selezione**: Deseleziona gli argomenti selezionati nell’elenco degli argomenti.

      >[!NOTE]
      >
      > Puoi anche selezionare o deselezionare un argomento singolarmente facendo clic sulla casella di controllo accanto all’argomento.

   - **Aggiungi**: Visualizza la finestra di dialogo Aggiungi revisori. È possibile digitare il nome di un revisore o di un ruolo utente \(o gruppo\) che si desidera aggiungere come revisore agli argomenti selezionati.
   - **Rimuovi**: Visualizza la finestra di dialogo Rimuovi revisori. È possibile digitare il nome di un revisore o di un ruolo utente \(o gruppo\) che si desidera rimuovere come revisore dagli argomenti selezionati.
   - **Riassegna**: Visualizza la finestra di dialogo Riassegna revisori. È possibile digitare il nome di un revisore o di un ruolo utente \(o gruppo\) a cui si desidera assegnare l&#39;attività di revisione. Questo rimuove tutti i revisori esistenti dagli argomenti selezionati e assegna i revisori appena selezionati a tali argomenti.
   - **Esporta**: Consente di esportare i dettagli dell’attività di revisione in un file CSV. Il file contiene dettagli quali il percorso e il titolo dell&#39;argomento, il nome del revisore e la versione degli argomenti inviati per la revisione.
   - **Modifica revisori**: Fai clic su ![](images/edit_pencil_icon.svg)Nell’elenco degli argomenti viene visualizzata la finestra di dialogo Modifica revisori. È possibile aggiungere o rimuovere revisori per l&#39;argomento selezionato da questa finestra di dialogo.

   >[!IMPORTANT]
   >
   > È necessario assegnare almeno un revisore per creare l&#39;attività di revisione.

1. Fai clic su **Crea** per creare l&#39;attività di revisione.

   Viene visualizzato un messaggio di conferma quando l’attività di revisione viene creata correttamente. La [Stato del documento](web-editor-document-states.md#) per gli argomenti inviati per la revisione è impostato su In-Review.

   >[!NOTE]
   >
   > Puoi anche fare clic sul pannello Notifiche in alto a destra dell’interfaccia e confermare che l’attività è stata creata correttamente. Nel pannello Notifiche, troverai una notifica per ciascuna delle revisioni che facevano parte dell&#39;attività di revisione e una notifica per l&#39;iniziatore della revisione.

   >[!IMPORTANT]
   >
   > Dopo aver avviato una revisione, non è necessario spostare o eliminare la mappa o gli argomenti DITA in una posizione diversa. In questo modo si interromperà il processo di revisione.


Viene inviata un&#39;e-mail a tutti i revisori con la notifica che gli argomenti sono stati assegnati per la revisione. L’e-mail contiene un collegamento diretto che possono fare clic sull’argomento e accedervi in una finestra del browser. Gli argomenti insieme alla mappa DITA vengono aperti in modalità di revisione.

**Argomento principale:**[ Esamina argomenti o mappe](review.md)
