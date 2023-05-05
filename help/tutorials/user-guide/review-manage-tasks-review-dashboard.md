---
title: Gestire le attività di revisione utilizzando il dashboard di revisione
description: Scopri come gestire le attività di revisione utilizzando il dashboard di revisione
exl-id: 617017fe-59b6-4b38-b375-a126fa9dddf5
source-git-commit: 8823669fd29e8a40a41f9ca5d654b38fbea8e2fa
workflow-type: tm+mt
source-wordcount: '1282'
ht-degree: 0%

---

# Gestire le attività di revisione utilizzando il dashboard di revisione {#id2056B0Y70X4}

Il flusso di lavoro di gestione delle revisioni può includere diverse attività. Ad esempio, puoi aggiungere revisori per un particolare argomento o prorogare la scadenza per una revisione. Puoi anche contrassegnare l’attività di revisione come completa se pensi che tutte le parti interessate abbiano fornito il loro feedback. Queste attività possono essere gestite tramite la dashboard di revisione.

Esegui i seguenti passaggi per accedere e utilizzare il Dashboard di revisione:

>[!NOTE]
>
> È possibile gestire le attività di revisione solo per i progetti per i quali si è l&#39;autore \(o iniziatore\). Anche se sei un revisore o un editore \(utente\), non potrai accedere ad alcuna attività del progetto.

1. In **Progetti** fare clic sul progetto di revisione che si desidera gestire.

   Viene visualizzato un pannello Progetto con riquadri attività.

   ![](images/review-management.png){width="800" align="left"}

1. Fai clic sui tre punti nel **Recensioni** piastrelle.

   Viene visualizzato il Dashboard di revisione. Il dashboard elenca tutte le attività di revisione create.

   ![](images/review-dashboard.png){width="800" align="left"}

   Nella dashboard di revisione vengono visualizzati i dettagli relativi all&#39;attività di revisione, ad esempio il nome dell&#39;attività, l&#39;autore che ha avviato la revisione, la data di inizio della revisione, la data di scadenza, lo stato, il numero di nuovi commenti che non sono stati accettati o rifiutati dall&#39;autore e il nome dei revisori. Le attività vengono elencate nell&#39;ordine delle attività create di recente in base alle attività precedenti.

   >[!NOTE]
   >
   > Se fai clic sul collegamento Attività di revisione , viene aperto l’argomento o il file di mappa inviato per la revisione.

1. Selezionare un&#39;attività di revisione.

   Viene visualizzata la finestra Modifica proprietà e [Stato](#check-review-status-id199RF0A0UHS) nella barra degli strumenti.

1. Se fai clic su **Modifica proprietà**, viene visualizzata la pagina Dettagli attività .

   Nella pagina Dettagli attività sono disponibili tre schede: Attività, Contenuto e Revisori. Le sezioni seguenti spiegano le varie funzioni disponibili in ciascuna scheda.


## Scheda Attività

![](images/review-task-page.png){width="800" align="left"}

Puoi eseguire le seguenti azioni in **Attività** scheda:

- Modifica il titolo dell&#39;attività nella **Titolo** campo .
- Aggiungi le assegne predefinite nel **Assegna a** elenco a discesa. I revisori aggiunti da qui hanno accesso a tutti gli argomenti che fanno parte di questa attività di revisione. Puoi scegliere di rimuovere o aggiungere in modo selettivo altri revisori a specifici argomenti dal [Scheda Revisori](#reviewer-tab-id199RF0N0MUI).
- Aggiorna la descrizione dell’attività nella **Descrizione** campo .
- Modifica la **Data di scadenza**. È possibile posticipare o posticipare la scadenza per il completamento dell&#39;attività.
- Seleziona l’opzione per limitare gli utenti a esaminare solo gli argomenti a essi assegnati.
- Fai clic su **Aggiorna** per aggiornare i dettagli modificati.
- Fai clic su **Completa** per contrassegnare l’attività di revisione come completa prima della data di scadenza. Quando l’attività di un singolo argomento è contrassegnata come Completa, la revisione dell’argomento selezionato viene chiusa. Tuttavia, nel caso di argomenti condivisi per la revisione tramite una mappa DITA, contrassegnando l&#39;attività mappa DITA come Completata verrà chiusa la revisione di tutti gli argomenti all&#39;interno della mappa condivisi per la revisione.
- Fai clic su **Duplica** per creare una copia dell&#39;attività di revisione. Il processo di creazione di un&#39;attività di revisione duplicata è simile alla creazione di una nuova attività di revisione. Una volta avviato il flusso di lavoro dell’attività duplicata, viene visualizzata la pagina Crea attività di revisione . È necessario fornire i nuovi dettagli dell&#39;attività, come spiegato in [Invia argomenti per la revisione](review-send-topics-for-review.md#).

   Se è stata selezionata un&#39;attività di revisione creata da una mappa DITA, vengono visualizzati gli argomenti che fanno parte della mappa. È quindi possibile scegliere gli argomenti da includere nella nuova attività di revisione.

   In caso di attività di revisione duplicata da uno o più argomenti di revisione, solo tali argomenti vengono visualizzati nell&#39;elenco delle attività di revisione. Puoi scegliere di condividere questi argomenti per la revisione con un diverso set di revisori.

- Fai clic su **Chiudi** per passare alla pagina Posta in arrivo.

## Scheda Contenuto

![](images/review-content-page.png){width="800" align="left"}

Puoi eseguire le seguenti azioni in **Contenuto** scheda:

- Modifica la versione dell’argomento inviato per la revisione. È possibile scegliere la versione più recente dell&#39;argomento, la versione come data, la versione con etichetta specifica o la versione con una linea di base specifica \(per una mappa DITA\).

- Fai clic su **Aggiorna** per condividere la versione aggiornata dell&#39;argomento con i revisori. I revisori ricevono una notifica e-mail in cui viene indicato che la versione più recente dell’argomento è stata inviata per la revisione. Alla successiva apertura dell’argomento da parte di un revisore, viene visualizzata la versione aggiornata dell’argomento.

   >[!NOTE]
   >
   > Nel caso di una versione aggiornata di un argomento, i vecchi commenti vengono mantenuti anche nella versione più recente. I revisori possono anche vedere le differenze tra le due versioni.

- Fai clic su **Completa** per contrassegnare l’attività di revisione come completa prima della data di scadenza. Quando l’attività di un singolo argomento è contrassegnata come Completa, la revisione dell’argomento selezionato viene chiusa. Tuttavia, nel caso di argomenti condivisi per la revisione tramite una mappa DITA, contrassegnando l&#39;attività mappa DITA come Completata verrà chiusa la revisione di tutti gli argomenti all&#39;interno della mappa condivisi per la revisione.

- Fai clic su **Duplica** per creare una nuova attività di revisione utilizzando l&#39;attività corrente come base.


## Scheda Revisori {#reviewer-tab-id199RF0N0MUI}

![](images/reviewers-tab.png){width="800" align="left"}

Puoi eseguire le seguenti azioni in **Revisori** scheda:

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

## Controllare lo stato di un&#39;attività di revisione {#check-review-status-id199RF0A0UHS}

Dalla pagina principale Dashboard di revisione, se selezioni un&#39;attività di revisione e fai clic su **Stato**, viene visualizzato il rapporto sullo stato dell’attività di revisione:

![](images/review-status-report.png){width="800" align="left"}

Il rapporto sullo stato dell&#39;attività di revisione contiene i seguenti dettagli:

- Nome\(i\) del revisore a cui è assegnata l&#39;attività di revisione.
- La colonna Stato indica lo stato della revisione. Lo stato può essere uno dei seguenti:
   - **Non avviato**: Il revisore non ha ancora aperto il collegamento di revisione.
   - **In corso**: Il revisore ha aperto il collegamento di revisione ed è in corso la revisione dell&#39;argomento.
   - **Completa**: Il revisore ha completato la revisione completando l&#39;attività di revisione assegnata loro. L&#39;attività di revisione si trova nella casella in entrata notifica AEM per ogni revisore.
- Quando un revisore apre un collegamento di revisione e passa a un particolare argomento che viene aggiunto all&#39;elenco Argomenti revisionati. Questo consente agli autori di determinare se i revisori hanno aperto o meno le rispettive sezioni. Eventuali osservazioni sono riportate tra parentesi.
- Numero totale di commenti effettuati su tutti gli argomenti. Nel caso di più argomenti in esame, il numero di commenti per ciascun argomento viene indicato \(tra parentesi\) rispetto al nome dell&#39;argomento.
- Data dell&#39;ultimo accesso a un argomento da parte del revisore.

**Argomento principale:**[ Esamina argomenti o mappe](review.md)
