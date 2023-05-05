---
title: Genera output per una mappa DITA dalla console mappa
description: Scopri come generare l’output per una mappa DITA dalla console mappa
exl-id: 98afbdd2-56d7-44b0-ad2a-25e9143c88f3
source-git-commit: c74badebbcb4733fb9caa79c646b1d1e5c8bfe8e
workflow-type: tm+mt
source-wordcount: '1399'
ht-degree: 0%

---

# Genera output per una mappa DITA dalla console mappa {#id1825FG00UHT}

Esegui i seguenti passaggi per generare l&#39;output per una mappa DITA:

1. Nell’interfaccia utente Assets, individua e fai clic sul file di mappa DITA da pubblicare.

   Viene visualizzata la console mappa DITA con l’elenco dei predefiniti di output disponibili per generare l’output.

1. Selezionare uno o più predefiniti di output da utilizzare per generare l&#39;output.

   ![](images/generate-multiple-outputs-uuid.png){width="800" align="left"}

   >[!NOTE]
   >
   > Se si sta generando l&#39;output AEM del sito, il processo di pubblicazione utilizza la struttura definita in `.ditamap` per creare AEM struttura del sito.

1. Fai clic sull’icona Genera per avviare il processo di generazione dell’output.


Per visualizzare lo stato corrente della richiesta di generazione dell&#39;output, fai clic su Output. Per ulteriori informazioni, consulta [Visualizza lo stato dell&#39;attività di generazione dell&#39;output](#viewing_output_history)

>[!IMPORTANT]
>
> Se un processo di generazione dell&#39;output per un predefinito è in coda o in corso, non è possibile avviare un&#39;altra attività di generazione dell&#39;output per lo stesso predefinito.

È possibile generare l’output PDF per uno o più predefiniti di output creati per una mappa DITA dall’Editor Web. Per ulteriori dettagli, consulta [Utilizza il pannello Genera rapida per generare e visualizzare l’output per i predefiniti](web-editor-quick-generate-panel.md#).

È inoltre possibile generare l&#39;output AEM del sito per uno o più argomenti o l&#39;intera mappa DITA dall&#39;Editor Web. Per ulteriori dettagli, consulta [Pubblicazione basata su articoli dall’editor web](web-editor-article-publishing.md#id218CK0U019I).

## Generazione di output incrementale {#generating_standalone_topic}

>[!NOTE]
>
> La generazione di output incrementale è applicabile solo per l&#39;output AEM sito. Inoltre, è possibile rigenerare solo gli argomenti DITA \(.dita/.xml\) da una mappa o mappe DITA secondarie. Se si seleziona una mappa DITA, una sottomappa, un gruppo di argomenti o un argomento con `@processing-role="resource-only"`, l’opzione Rigenera non è disponibile.

Ci potrebbero essere diverse istanze in cui si aggiornerebbero solo alcuni argomenti nella mappa DITA e si invierebbero solo gli argomenti aggiornati in tempo reale. Per gestire tali scenari, AEM Guide ti consente di creare output incrementali. Se sono stati aggiornati alcuni argomenti, non è necessario rigenerare l&#39;intera mappa DITA. Puoi selezionare solo gli argomenti aggiornati e rigenerarli.

Se la mappa è bloccata e hai aggiornato un singolo argomento nella mappa, devi rigenerare l’intera mappa affinché l’argomento o il contenuto aggiornato si rifletta nell’output. L&#39;opzione di rigenerazione dell&#39;output non viene visualizzata a livello di argomento, ma è disponibile solo a livello di mappa \(chunked\). Questo è applicabile alla mappa padre e a tutte le mappe secondarie.

Esegui i seguenti passaggi per rigenerare l’output per un argomento specifico o un gruppo di argomenti:

>[!IMPORTANT]
>
> Quando si sta rigenerando l&#39;output AEM del sito, l&#39;output viene creato utilizzando la versione corrente dei file e non la baseline allegata.

1. Nell’interfaccia utente Assets, individua e fai clic sul file di mappa DITA.

   Viene visualizzata la console mappa DITA con l’elenco dei predefiniti di output disponibili per generare l’output.

1. Seleziona la **Argomenti** scheda .

   Viene visualizzato un elenco di argomenti disponibili nella mappa DITA.

1. Seleziona gli argomenti da rigenerare.

   >[!NOTE]
   >
   > Se hai aggiunto nuovi argomenti alla mappa DITA, non potrai generarli da qui. È innanzitutto necessario pubblicare gli argomenti appena aggiunti utilizzando la funzione di pubblicazione della mappa DITA.

   ![](images/regenerate-topics.png){width="800" align="left"}

1. Fai clic su **Rigenerare**.

   Viene visualizzata la pagina Rigenera argomenti selezionati .

1. Seleziona il predefinito di output da utilizzare per rigenerare gli argomenti selezionati.

1. Fai clic su **Rigenerare** per avviare il processo di generazione dell&#39;output.


>[!IMPORTANT]
>
> Se si rinomina un titolo dell&#39;argomento e si rigenera l&#39;argomento, il titolo dell&#39;argomento aggiornato non si riflette nel sommario della mappa DITA. Per aggiornare il titolo dell&#39;argomento nel sommario, è necessario generare l&#39;intera mappa DITA.

Per visualizzare lo stato corrente della richiesta di generazione dell&#39;output, fai clic su Output. Per ulteriori informazioni, consulta [Visualizza lo stato dell&#39;attività di generazione dell&#39;output](#viewing_output_history).

## Visualizza lo stato dell&#39;attività di generazione dell&#39;output {#viewing_output_history}

Dopo aver avviato l’attività di generazione dell’output per una mappa o rigenerato gli argomenti selezionati, AEM Guide invia l’attività alla coda di generazione dell’output. Questa coda viene aggiornata in tempo reale, mostrando lo stato di ogni attività di generazione dell&#39;output nella coda.

Esegui i seguenti passaggi per visualizzare la coda di generazione dell’output:

1. Nell’interfaccia utente Assets, individua e fai clic sul file mappa per il quale vuoi controllare lo stato di generazione dell’output.

1. Fai clic su **Uscite**.

   ![](images/output-queued.png){width="800" align="left"}

   La pagina Output è divisa in due parti:

   - **Uscite in coda:**

      Elenca gli output in attesa di generazione o in fase di generazione. Le attività in coda o in corso vengono visualizzate con un’icona di colore blu prima del nome del predefinito. È inoltre possibile trovare l&#39;impostazione di generazione dell&#39;output o il predefinito utilizzato per l&#39;attività in coda, il tipo, l&#39;utente che ha avviato l&#39;attività, l&#39;ora dal momento in cui l&#39;attività viene messa in coda e lo stato corrente.

      Fai clic sul collegamento per accedere al **Pubblica dashboard** e visualizza lo stato corrente in esecuzione. Un elenco di tutte le attività di pubblicazione attive è disponibile nel dashboard di pubblicazione. La **Uscite in coda** e **Pubblica dashboard** i collegamenti vengono visualizzati solo quando sono presenti output in attesa di essere generati o in fase di generazione. Non vengono visualizzate quando le attività di output sono state completate.Per ulteriori dettagli su Dashboard di pubblicazione, consulta [Gestione delle attività di pubblicazione tramite il dashboard di pubblicazione](generate-output-publish-dashboard.md#).

   - **Uscite generate**

      Elenca le attività di output completate. Anche in questo caso, le informazioni qui visualizzate sono simili alla sezione Output in coda con alcune differenze. È disponibile un nuovo set di informazioni sotto forma di icona dei risultati di output e il tempo di generazione dell’output.

      In questo elenco è possibile che le attività siano state eseguite correttamente, le attività eseguite con il messaggio o le attività non riuscite. Le attività riuscite vengono visualizzate con l’icona a colori verde, le attività con un messaggio hanno un’icona a colori arancione e le attività non riuscite sono visualizzate con l’icona a colori rosso.

      Per tutte le attività, il processo di pubblicazione crea un file di registro \(logs.txt\) a cui è possibile accedere facendo clic sul collegamento nella colonna Generated At (A generato). Per le attività che non sono riuscite o che contengono messaggi, è possibile controllare il file di registro, illustrato nella sezione [Visualizza e controlla il file di registro](generate-output-basic-troubleshooting.md#id1822G0P0CHS).

      >[!NOTE]
      >
      > Quando si fa clic su un collegamento dell’output di PDF generato, viene richiesto di scaricare PDF. Questo è il comportamento predefinito nelle AEM 6.5 e 6.4.


## Annullare un&#39;attività di generazione di output {#id2061H100T5Z}

AEM Guide offre agli editori un modo semplice e semplice per annullare qualsiasi attività di pubblicazione in corso. In qualità di editore, è possibile annullare un&#39;attività di pubblicazione in corso dalla console Mappa DITA o dalla [Pubblica dashboard](generate-output-publish-dashboard.md#).

Esegui i seguenti passaggi per annullare un&#39;attività di generazione dell&#39;output dalla console Mappa DITA:

1. Nell’interfaccia utente Assets, individua e fai clic sul file mappa per il quale vuoi annullare un’attività di generazione dell’output in corso.

1. Fai clic su **Uscite**.

1. Nell&#39;elenco Output in coda, posizionare il puntatore del mouse su un&#39;attività da annullare.

1. Fai clic sul pulsante *Annulla questo processo* icona.

   ![](images/cancel-publish-task-map-console.png){width="800" align="left"}

1. Fai clic su **Sì** al prompt dei messaggi Conferma annullamento.

   ![](images/confirm-cancel-output-map-condole.png){width="800" align="left"}

   Se l&#39;attività non è ancora stata avviata, il comando Annulla viene eseguito sull&#39;attività. Per un&#39;attività che viene annullata, lo stato è impostato su Annullamento.

   Quando l’attività viene annullata correttamente, viene spostata nella **Uscite generate** elenco con un **Annullato** stato. Quando si passa il mouse sull&#39;attività annullata, viene visualizzato il nome dell&#39;utente che ha annullato l&#39;attività. Nella schermata seguente, il *HTML5* attività annullata.

   ![](images/cancelled-output-task.png){width="800" align="left"}


## Eliminare un&#39;attività di output dalla console mappa DITA

Quando si generano più output per una mappa DITA, in un periodo di tempo l&#39;elenco degli output generati per tale mappa diventa molto lungo. In qualità di editore, puoi pulire la cronologia di output di qualsiasi file mappa rimuovendo le attività obsolete da *Uscite generate* elenco. L&#39;output non viene rimosso dal sistema, solo la voce dell&#39;output generato viene rimossa dal *Uscite generate* elenco.

Esegui i seguenti passaggi per rimuovere un&#39;attività di output dall&#39;elenco Output generato:

1. Nell’interfaccia utente Assets, individua e fai clic sul file mappa da cui desideri eliminare le attività.

1. Fai clic su **Uscite**.

1. Nell’elenco Output generato, posizionare il puntatore del mouse su un’attività da eliminare.

1. Fai clic sull’icona Elimina .

   ![](images/delete-output-task.png){width="800" align="left"}

1. Fai clic su **Sì** al prompt dei messaggi Conferma eliminazione .

   L&#39;attività viene eliminata dall&#39;elenco Output generati.


**Argomento principale:**[ Generazione di output](generate-output.md)
