---
title: Creare e gestire le baseline dall'editor Web
description: Scopri come creare e gestire le linee di base dall’editor web
exl-id: 9e390489-16f5-4f9a-a821-5150a66c2ed4
source-git-commit: 3bca42f0954afc2362ab24f369e698113324dbc3
workflow-type: tm+mt
source-wordcount: '1190'
ht-degree: 0%

---

# Creare e gestire le baseline dall&#39;editor Web {#id223MB0ZF043}

>[!TIP]
>
> Si consiglia di utilizzare questa funzione della linea di base dell’editor web se è stato effettuato l’aggiornamento alla versione di marzo as a Cloud Service delle guide AEM o successiva.

Le guide AEM forniscono la funzione Baseline integrata nell’editor web che consente agli utenti di creare linee di base e utilizzarle per pubblicare o tradurre argomenti di versioni diverse.

## Creare una baseline

È possibile creare una baseline dall&#39;editor Web eseguendo le operazioni riportate di seguito.

1. Nel pannello Repository, aprire il file mappa DITA in Vista mappa.
1. Fai clic su **Gestisci** scheda. Il **Linea di base** Nel pannello vengono visualizzate le linee di base della mappa DITA.

   ![](images/baseline-manage.png){width="800" align="left"}

1. Il giorno **Linea di base** fai clic sull’icona + in alto a destra. È possibile creare una baseline con una versione specifica degli argomenti e del contenuto di riferimento disponibile in una data e un&#39;ora specifiche oppure con un&#39;etichetta definita per una versione degli argomenti.
1. Immettere un nome per la baseline in **Nome linea di base**.
1. In entrata **Opzione linea di base**, puoi scegliere **Usa versione file** opzione o **Usa etichette** opzione:

   **Usa versione file**: è possibile creare una linea di base statica con una versione specifica degli argomenti e del contenuto di riferimento disponibile in una data e un&#39;ora specifiche oppure con un&#39;etichetta definita per una versione degli argomenti:

   - In entrata **Imposta la versione più recente in base a,** selezionare una delle opzioni seguenti:


      1. **Data** &lt;time stamp=&quot;&quot;>: seleziona la versione degli argomenti in base alla data e all’ora specificate.
      1. **Etichetta**: seleziona questa opzione per scegliere gli argomenti in base all’etichetta ad essi applicata. Se per gli argomenti sono specificate etichette, queste sono elencate nel menu a discesa. È possibile scegliere un&#39;etichetta dall&#39;elenco. È inoltre possibile aggiungere un&#39;etichetta nella casella di testo.\
         Quando selezioni **Etichetta** potete scegliere i riferimenti diretti e indiretti.
      - Per i riferimenti diretti all&#39;interno della mappa DITA, è possibile utilizzare la versione più recente degli argomenti a cui non è stata applicata l&#39;etichetta specificata.

      >[!NOTE]
      >
      > Se si immette un&#39;etichetta che non esiste e si seleziona l&#39;opzione **Non creare una baseline** la creazione della baseline ha esito negativo e viene visualizzato un messaggio di errore accanto al nome della baseline nel pannello Baseline.

      - Per i riferimenti indiretti all&#39;interno della mappa DITA, è disponibile un&#39;opzione aggiuntiva che consente di utilizzare la versione più recente degli argomenti a cui non è applicata l&#39;etichetta specificata. Puoi anche scegliere di **Scegli automaticamente** per il contenuto a cui si fa riferimento e il sistema seleziona automaticamente la versione del contenuto a cui si fa riferimento corrispondente alla versione del contenuto in cui viene fatto riferimento.

   Dopo aver selezionato un&#39;etichetta o una versione come alla data, tutti gli argomenti e i file multimediali a cui si fa riferimento nella mappa vengono selezionati di conseguenza. Questa selezione di argomenti non viene visualizzata nell&#39;interfaccia utente, ma viene salvata nel back-end.

   **Usa etichette**: selezionare questa opzione per la creazione della linea di base per scegliere gli argomenti in base all&#39;etichetta ad essi applicata.

   Le linee di base basate sulle etichette vengono aggiornate in modo dinamico. Se si genera una baseline, si scarica una baseline o si crea un progetto di traduzione utilizzando una baseline, i file vengono selezionati in modo dinamico in base alle etichette aggiornate. Ad esempio, se è stata utilizzata la versione 1.2 di un argomento con Label Release 1.0 per la baseline e successivamente è stata aggiornata la versione 1.5 con Label Release 1.0, la baseline verrà aggiornata dinamicamente e verrà utilizzata la versione 1.5.

   ![](images/dynamic-baseline.png){width="550" align="left"}

   - **Seleziona etichette**: se per gli argomenti sono specificate etichette, queste sono elencate nella **Seleziona etichette** a discesa. Puoi scegliere l&#39;etichetta\(s\) dall&#39;elenco. Alle etichette selezionate per prime viene assegnata una priorità maggiore rispetto a quelle successive.
1. **Riferimenti indiretti**: per i riferimenti indiretti all&#39;interno della mappa DITA, sono disponibili le seguenti opzioni:

   - **Scegli automaticamente**: puoi scegliere di **Scegli automaticamente** per il contenuto a cui si fa riferimento e il sistema seleziona automaticamente la versione del contenuto a cui si fa riferimento corrispondente alla versione del contenuto in cui viene fatto riferimento.

   - **Usa etichetta selezionata**: è possibile creare una baseline con l&#39;etichetta selezionata definita per una versione degli argomenti.
   - **Usa la versione più recente o la copia di lavoro**: utilizzare la versione più recente degli argomenti a cui non è applicata l&#39;etichetta specificata oppure, se non è stata creata alcuna versione, utilizzare la copia di lavoro degli argomenti per creare la baseline.
1. Clic **Applica**.

Viene creata la baseline. La creazione della baseline viene eseguita in modo asincrono, pertanto è possibile continuare a lavorare su altri file nell&#39;editor Web. Una volta creata la baseline, viene visualizzato un messaggio a comparsa che conferma la creazione della baseline e viene visualizzata una notifica della casella in entrata per la baseline.

## Gestisci linee di base

Potete gestire le baseline esistenti utilizzando le varie funzioni del dashboard Baseline.

- Potete cercare una baseline esistente utilizzando la casella di testo nel pannello Baseline. Utilizza il **Applica filtro** per visualizzare tutte le baseline o elencarle con lo stato di creazione Completato, In corso o Non riuscito.
- Utilizza il **Aggiorna** nel pannello Baseline per verificare nuovamente tutte le baseline e visualizzare un nuovo elenco di baseline per la mappa DITA aperta nella vista Mappa.
- Potete visualizzare o modificare il contenuto di una baseline esistente facendo doppio clic sulla baseline dall&#39;elenco nel pannello Baseline. Nella finestra di modifica della baseline al centro vengono visualizzati il file di mappa DITA, il contenuto o gli argomenti della mappa e il contenuto a cui si fa riferimento.


![](images/baseline-options.png){width="550" align="left"}

È inoltre possibile eseguire le operazioni riportate di seguito sulla baseline dal menu Opzioni.

- **Modifica**, **Duplicato,** o **Elimina** una baseline esistente.
- Aggiungi, rimuovi o modifica le etichette esistenti dal **Gestisci etichette** opzione. Se l&#39;amministratore ha configurato etichette predefinite, queste vengono visualizzate nell&#39;elenco a discesa Aggiungi etichetta. Per ulteriori informazioni sull&#39;aggiunta di etichette, vedere [Usa etichette](web-editor-use-label.md#).

   >[!NOTE]
   >
   > Il processo di aggiunta o rimozione delle etichette viene eseguito in modo asincrono, pertanto è possibile continuare a lavorare su altri file nell&#39;editor Web. Una volta aggiunta o rimossa l’etichetta, viene visualizzato un messaggio a comparsa che conferma che l’etichetta è stata aggiunta o rimossa e che si riceve anche una notifica nella casella in entrata per la stessa etichetta.

- **Modifica proprietà** di una baseline esistente impostata durante la creazione della baseline.
- Esportare lo snapshot di una baseline in un file CSV con **Esporta previsione** opzione.

**Filtri della linea di base**

Utilizzo dell’icona Filtri in **Filtri linea di base** pannello puoi applicare filtri alla linea di base aperta nella finestra di modifica della linea di base:

![](images/baseline-filter.png){width="350" align="left"}

- Filtra i file in base ai nomi o alla posizione.
- Filtrare i file in base ai valori per colonne diverse, ad esempio Tipo file, Tipo riferimento e così via.
- Scegliere le colonne da visualizzare nella finestra di modifica della baseline.

>[!NOTE]
>
> È possibile fare clic su un&#39;intestazione di colonna e ordinare i file in base alle colonne nella finestra di modifica della baseline.

**Salvare o reimpostare una baseline**

Dopo aver modificato la baseline, è possibile fare clic su **Salva** nella parte superiore per salvare le modifiche apportate alla baseline. Puoi fare clic su **Reimposta** se non si desidera salvare la modifica e reimpostare la previsione. Quando fai clic su **Reimposta** pulsante viene visualizzato un avviso che segnala la perdita delle modifiche non salvate.

**Argomento padre:**[ Utilizzare l’editor web](web-editor.md)
