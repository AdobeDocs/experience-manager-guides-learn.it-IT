---
title: Utilizzare la linea di base
description: Scopri come utilizzare la linea di base
source-git-commit: 8b6294425c6e60d1c5b37d98e99114014a104ee6
workflow-type: tm+mt
source-wordcount: '1917'
ht-degree: 0%

---


# Utilizzare la linea di base {#id1825FI0J0PF}

La funzione Linea di base ti consente di creare una versione degli argomenti e delle risorse da utilizzare per la pubblicazione o la traduzione. Ad esempio, se la mappa DITA ha `topicA` e `imageA`, puoi creare una baseline per utilizzare la 3a versione di `topicA`, ma la quarta versione di `ImageA`. Una volta che hai impostato una Linea di base, puoi pubblicare o tradurre argomenti di versioni diverse con un solo clic.

La selezione di una baseline è facoltativa per i predefiniti di output e una mappa DITA può avere più di una baseline. Tuttavia, ogni predefinito di output all&#39;interno di una mappa DITA può essere associato a una sola linea di base. Se al momento della pubblicazione non è specificata alcuna linea di base, l’output viene pubblicato utilizzando la versione più recente del contenuto.

Analogamente, la selezione di una linea di base per tradurre il contenuto è facoltativa. Tuttavia, se scegli di tradurre il contenuto utilizzando una Linea di base, anche il contenuto della Linea di base viene salvato insieme alle copie tradotte. Puoi quindi utilizzare la Linea di base tradotta per eseguire ulteriori operazioni, ad esempio condividerla con editori esterni o archiviarla. Per ulteriori informazioni sull&#39;esportazione di una baseline tradotta, vedere [Esporta linea di base tradotta](#id196SE600GHS).

>[!TIP]
>
> Consulta la sezione *Linea* nella guida alle best practice per le best practice sull’utilizzo delle linee di base.

L’amministratore può configurare la scheda Linea di base nel dashboard della mappa. Per ulteriori dettagli, consulta *Configura la scheda Linea di base nel dashboard mappa DITA* nella sezione Guida all&#39;installazione e alla configurazione.

Per accedere alla feature di linea di base, effettuate le seguenti operazioni:

1. Nell’interfaccia utente Assets, individua e fai clic sul file di mappa DITA.
1. Vai a **Linee di base** scheda .

Nella scheda Linee di base è possibile eseguire le azioni seguenti:

- [Creare una baseline](#id195FI0I0MUQ)
- [Visualizzare il contenuto di una linea di base](#id195FI0I0TLN)
- [Modificare, duplicare o rimuovere le linee di base](#id195FI0I0YJL)
- [Aggiungere etichette a una linea di base](#id184KD0T305Z)

## Creare una baseline {#id195FI0I0MUQ}

È possibile creare una baseline con una versione specifica degli argomenti e il contenuto a cui si fa riferimento disponibile in una data e in un&#39;ora specifiche oppure con un&#39;etichetta definita per una versione degli argomenti. È possibile specificare individualmente le versioni degli argomenti selezionati in una linea di base in modo che ogni volta che si applica la linea di base nel flusso di lavoro di pubblicazione o traduzione, gli argomenti selezionati e le relative versioni corrispondenti vengano inclusi nella generazione o nella traduzione dell&#39;output.

Per creare una linea di base, effettua le seguenti operazioni:

1. Nella pagina Linee di base, fai clic su **Crea**.
1. Immettere un nome per la linea di base in **Nome linea di base**.
1. In **Imposta la versione in base a**, seleziona una delle seguenti opzioni:

   - **Etichetta**: Seleziona questa opzione per scegliere gli argomenti in base all’etichetta applicata. Immetti un’etichetta per filtrare l’elenco in base alla stringa immessa. Dall’elenco a discesa filtrato, puoi scegliere un’etichetta per selezionare argomenti e altre risorse con l’etichetta specificata.

      Quando selezioni **Etichetta**, ti viene inoltre offerta un’opzione aggiuntiva per utilizzare la versione più recente degli argomenti a cui non è stata applicata l’etichetta specificata. Se non selezioni questa opzione e ci sono argomenti o file multimediali che non hanno l&#39;etichetta specificata, il processo di creazione della linea di base non riuscirà. Per ulteriori informazioni sull’aggiunta di etichette, consulta [Usa etichette](web-editor-use-label.md#).

   - **Versione su** &lt;*timestamp*\>: Seleziona la versione degli argomenti in base alla data e all&#39;ora specificate. L’ora specificata corrisponde al fuso orario del server AEM. Se il server si trova in un fuso orario diverso, gli argomenti verranno rilevati in base al fuso orario del server e non in base al fuso orario locale.

   Dopo aver selezionato un&#39;etichetta o una versione come data, tutti gli argomenti e i file multimediali a cui si fa riferimento all&#39;interno della mappa vengono selezionati di conseguenza. Questa selezione di argomenti non viene visualizzata nell’interfaccia utente, ma viene salvata nel backend.

1. Se desideri utilizzare una versione diversa per uno o più argomenti, puoi farlo selezionando manualmente tali argomenti. Fai clic su **Sfoglia argomento**, seleziona l’argomento di cui desideri utilizzare una versione diversa. Dall’elenco a discesa Seleziona una versione per l’argomento selezionato, seleziona una versione dell’argomento da utilizzare nella baseline e fai clic su **OK**.

   ![](images/baseline-select-version-drop-down.png)

   Le informazioni sull&#39;argomento e la relativa versione selezionata vengono memorizzate nel backend. Puoi ripetere questo passaggio per modificare la versione selezionata per più argomenti.

1. Fai clic sul pulsante **Sfoglia tutti gli argomenti** link per caricare tutti gli argomenti e i file multimediali di cui alla mappa DITA.L&#39;UUID degli argomenti e dei file multimediali viene anche mostrato sotto il titolo dell&#39;argomento o il nome del file \(media\).

   >[!NOTE]
   >
   > Se nella mappa DITA è presente un set molto ampio di file con mappe e argomenti nidificati, fare clic su Sfoglia tutti gli argomenti potrebbe richiedere un po&#39; di tempo per caricare tutti i file.

   I contenuti della mappa sono presentati nelle tre sezioni: il file mappa, il contenuto \(riferimenti argomento\) e il contenuto di riferimento \(argomenti nidificati, mappe e altre risorse\). Una volta disponibile tutto il contenuto a cui si fa riferimento, puoi selezionare singolarmente la versione dell’argomento da utilizzare nella linea di base.

   La **Versione** l&#39;elenco a discesa mostra le versioni disponibili degli argomenti o il contenuto a cui si fa riferimento. Per il contenuto a cui si fa riferimento, è possibile scegliere automaticamente una versione.

   Se scegli **Seleziona automaticamente** per il contenuto a cui si fa riferimento, il sistema seleziona automaticamente la versione del contenuto a cui si fa riferimento corrispondente alla versione del contenuto a cui si fa riferimento. Ad esempio, supponiamo che un argomento A abbia un riferimento a un&#39;immagine B. Quando è stata creata la versione 1.5 dell&#39;argomento A, la versione dell&#39;immagine B era 1.2 nell&#39;archivio. Ora, quando viene creata una linea di base con la versione 1.5 dell’argomento A con l’immagine B impostata su **Seleziona automaticamente**, il sistema sceglierà automaticamente la versione 1.2 dell&#39;immagine B.

   Se create una baseline utilizzando le etichette, **Seleziona automaticamente** viene applicata alla versione di tutto il contenuto di riferimento.

   Se al contenuto o alle risorse a cui si fa riferimento \(argomento, mappe secondarie, immagini o video\) non viene applicata una versione \(ad esempio, contenuto appena caricato\), la creazione di una linea di base creerà una versione per tali file. Tuttavia, se i file sono sottoposti a versione, non viene creata alcuna versione incrementale per tali file. Questo comportamento è controllato dall’impostazione di creazione automatica della versione, abilitata per impostazione predefinita. Questo è necessario anche per tradurre il contenuto in cui il processo di traduzione prevede che tutti i file abbiano una versione.

   >[!NOTE]
   >
   > Per specificare una versione diversa per una particolare risorsa, scegli la versione desiderata dalla sezione **Versione** elenco a discesa.

1. Fai clic su **Salva**.

## Visualizzare il contenuto di una linea di base {#id195FI0I0TLN}

Per visualizzare il contenuto di una linea di base esistente, fai clic sulla scheda Linee di base e seleziona la versione della linea di base desiderata dall’elenco. La pagina Baselines è divisa in tre parti: file mappa DITA, contenuto o argomenti della mappa e contenuto a cui si fa riferimento. Se la mappa contiene mappe secondarie, gli argomenti a cui fa riferimento la mappa secondaria vengono visualizzati anche nella sezione Contenuto . Di seguito sono descritte le varie colonne della pagina Linea di base:

- **Nome**: Elenca la mappa DITA o il titolo dell&#39;argomento o il nome della risorsa, ad esempio il nome del file di un&#39;immagine.

- **Gentile**: Elenca il tipo o il tipo di risorsa nella mappa come mappa DITA, argomento DITA o formato immagine.

- **Versione**: Elenca la versione della risorsa disponibile nella baseline.

- **Data e ora della versione**: Elenca la data e l’ora di creazione della risorsa per la versione selezionata.

- **Più recente**: Indica se la versione più recente della risorsa viene utilizzata nella baseline.

- **Mappa padre**: Se il tuo file di mappa contiene delle mappe secondarie, allora questa colonna contiene il nome della mappa in cui viene fatto riferimento a un argomento.

- **Etichetta**: Elenca le etichette applicate alla versione dell&#39;argomento.

- **A cui fa riferimento**: Questa colonna è disponibile solo per il contenuto a cui si fa riferimento. Indica l’argomento principale della risorsa di riferimento. Nel caso in cui a una risorsa facciano riferimento più argomenti, gli argomenti sono separati da virgole.

## Modificare, duplicare o rimuovere le linee di base {#id195FI0I0YJL}

**Modificare le linee di base**

Per modificare una linea di base esistente, effettua le seguenti operazioni:

1. Selezionare la baseline e fare clic su **Modifica**.
1. Apporta le modifiche necessarie nella linea di base. Puoi modificare il nome e la versione dell’argomento o del contenuto a cui si fa riferimento.
1. Fai clic su **Salva**.

**Linee di base duplicate**

Selezionare la baseline e fare clic su **Duplica** per creare una copia di una baseline esistente. Specifica un nome diverso per la baseline, scegli il numero di versione per gli argomenti e il contenuto a cui si fa riferimento, quindi fai clic su **Salva**.

**Rimuovi linee di base**

Seleziona la versione Baselines e fai clic su **Rimuovi** per rimuovere una baseline.

## Aggiungere etichette a una linea di base {#id184KD0T305Z}

L&#39;aggiunta di etichette a ogni singolo argomento può richiedere molto tempo. AEM Guide offre un meccanismo con un solo clic per aggiungere etichette a più argomenti e contenuti di riferimento in una mappa DITA.

Esegui i seguenti passaggi per aggiungere un’etichetta a più argomenti e contenuto a cui si fa riferimento in una mappa DITA:

1. Nella pagina Linee di base, seleziona una linea di base contenente gli argomenti e il contenuto a cui si fa riferimento in cui desideri aggiungere un’etichetta.

   >[!NOTE]
   >
   > Assicurati che la tua baseline non abbia la versione più recente di un argomento o di una risorsa. Un’etichetta può essere aggiunta solo a un argomento o a una risorsa con versione.

1. Fai clic su **Aggiungi etichette**.

   ![](images/add-label-baseline-uuid.png)

1. In **Aggiungi etichetta** specificare un&#39;etichetta univoca da associare a questa baseline.

   Se l’amministratore ha configurato le etichette predefinite, queste vengono visualizzate in un elenco a discesa. È necessario scegliere un’etichetta dall’elenco.

1. Se desideri applicare l’etichetta agli argomenti a cui si fa riferimento nelle mappe secondarie, seleziona **Applica etichetta alle mappe figlio e ai dipendenti** opzione .

   - Fai clic su **Aggiungi**.
L&#39;etichetta specificata viene aggiunta alla mappa DITA e agli argomenti e al contenuto a cui si fa riferimento.

      ![](images/label-added-baseline-uuid.png)


## Esporta linea di base tradotta {#id196SE600GHS}

Puoi utilizzare Linea di base per tradurre il contenuto. Ad esempio, puoi creare una baseline per la versione 1.1 pronta per la traduzione in francese. Nella scheda Traduzione, devi utilizzare Linea di base per filtrare il contenuto, quindi selezionare la Linea di base per la versione 1.1 del contenuto. L’utilizzo della linea di base per la traduzione dei contenuti semplifica la gestione dei contenuti.

Una volta tradotto il contenuto, puoi esportare la baseline tradotta per l’archiviazione o condividerla con team diversi dell’organizzazione. È necessario tenere in considerazione i seguenti punti prima di esportare una baseline tradotta:

- L’esportazione di una linea di base è possibile solo dopo la traduzione del contenuto della linea di base. Se tenti di esportare una linea di base per la quale la traduzione non viene avviata o non è completa, ottieni un errore.
- È possibile trasferire la Linea di base solo per una versione già tradotta. Ad esempio, se hai creato una baseline per la versione 1.1 del contenuto e lo stesso viene tradotto, puoi esportare questa baseline. Tuttavia, se hai creato una baseline per la versione 1.2 che non è tradotta, non puoi esportare questa baseline.
- Se una baseline è già esportata, puoi sovrascrivere la baseline esistente selezionando la *Sovrascrivi linea di base esistente* durante l&#39;esportazione.

Esegui i seguenti passaggi per esportare una baseline tradotta:

1. Aprire la mappa DITA contenente la baseline tradotta.

1. In **Traduzione** scheda , espandi **Linea** disponibile nella barra a sinistra.

   ![](images/export-baseline.png)

1. Seleziona la **Usa linea di base** e scegliete la baseline da esportare.

1. Fai clic su **Esporta linea di base**.

   Viene visualizzato lo stato di esportazione. Se il processo ha esito positivo, viene visualizzato un messaggio in cui viene indicata la lingua per la quale viene esportata la baseline. In caso di errore, viene visualizzata la causa dell’errore.

   Se tenti di esportare la baseline già esportata, viene visualizzato anche il messaggio di errore di creazione della baseline.

1. \(Facoltativo\) Per esportare una baseline già esportata, selezionare **Sovrascrivi linea di base esistente** quindi fai clic su **Esporta linea di base**.


**Argomento principale:**[ Generazione di output](generate-output.md)

