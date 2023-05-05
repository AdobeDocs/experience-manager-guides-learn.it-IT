---
title: Tradurre documenti dall'editor Web
description: Scopri come tradurre documenti dall’editor Web
exl-id: 02fc2b51-5b9a-4ad6-9e2e-726ab7602514
source-git-commit: 3bca42f0954afc2362ab24f369e698113324dbc3
workflow-type: tm+mt
source-wordcount: '1517'
ht-degree: 0%

---

# Tradurre documenti dall&#39;editor Web {#id21BKF0Z0YZF}

>[!TIP]
>
> Si consiglia di utilizzare questa funzione di traduzione dell’editor web se è stato effettuato l’aggiornamento AEM versione Guide as a Cloud Service di febbraio 2022 o successiva.

AEM Guide offre una potente funzione nell’editor web che consente di tradurre i contenuti in più lingue. Puoi creare un nuovo progetto di traduzione e successivamente aggiungere i lavori di traduzione al progetto di traduzione esistente. Puoi anche creare un progetto di traduzione multilingue che include i lavori di traduzione per tutte le lingue selezionate.

>[!NOTE]
>
> L&#39;amministratore può configurare la scheda Gestisci \(utilizzata per la traduzione\) nell&#39;editor Web. Per ulteriori dettagli, consulta *Configurare la funzione di traduzione nell’editor Web* in Installazione e configurazione delle guide Adobe Experience Manager as a Cloud Service.

## Prima di iniziare

Prima di eseguire i passaggi descritti in questa procedura, verificare di aver creato le cartelle principali e di destinazione della lingua richieste

1. Crea una cartella principale per memorizzare il contenuto sorgente. La cartella principale deve essere creata con il nome della lingua \(ad esempio English\) o con il codice della lingua \(en\).
1. Crea le cartelle di destinazione in cui tradurre il contenuto. Ad esempio, per tradurre il contenuto in tedesco o francese, è necessario creare una cartella denominata -de \(per tedesco\) o -fr \(per francese\).

>[!NOTE]
>
> La cartella principale e le cartelle di destinazione devono essere create allo stesso livello.

## Crea un progetto di traduzione

1. Nel pannello Repository, aprire il file di mappa DITA nella vista Mappa.
1. Fai clic sul pulsante **Gestisci** scheda . Nel pannello Traduzione viene visualizzato il titolo ipercollegato della mappa DITA insieme al **Lingue** elenco.
1. Da **Lingue** seleziona le impostazioni internazionali in cui tradurre il progetto. È possibile selezionare **Tutto** tradurre il progetto in tutte le lingue disponibili.

   >[!NOTE]
   >
   > L&#39;elenco contiene le cartelle della lingua insieme ai relativi codici della lingua. Ad esempio, Francese \(fr\) e Tedesco \(de\).

   >[!IMPORTANT]
   >
   > Lingua mostra solo le lingue per le quali viene creata una cartella di lingua parallela alla lingua di origine. Non viene visualizzata anche una cartella di lingua creata a un altro livello, ad esempio un livello inferiore dalla cartella della lingua di origine. Assicurati di creare tutte le cartelle della lingua di destinazione allo stesso livello della cartella della lingua di origine.

   ![](images/translation-languages.png){width="350" align="left"}

1. Puoi inoltre utilizzare le seguenti opzioni:

   **Usa linea di base:** Puoi selezionare una baseline per tradurre il progetto. Fare clic su Usa linea di base e scegliere una linea di base creata sulla mappa. Tutti i file che fanno parte della baseline selezionata vengono visualizzati nella pagina Traduzione. Una volta tradotto il contenuto, puoi esportare la baseline tradotta. Per ulteriori dettagli sull&#39;esportazione della linea di base tradotta, vedi [Esporta linea di base tradotta](generate-output-use-baseline-for-publishing.md#id196SE600GHS).

   **Usa versione più recente come attiva**: Scegli di filtrare la versione degli argomenti in base alla data e all’ora di creazione. Quando selezioni una data e un’ora, viene visualizzata solo la versione più recente dei file creati alla data e all’ora selezionate o prima di quella selezionata.

1. Fai clic su **Applica**. Viene visualizzato un elenco con dettagli sugli argomenti e sulle risorse associate.
1. Seleziona gli argomenti da inviare per la traduzione.

   Puoi anche utilizzare le seguenti opzioni di filtro degli argomenti:

   - **Titolo**: Titolo del file di origine
   - **Nome file**: Nome del file di origine
   - **Tipo di file**: Tipo di file di origine. Le opzioni disponibili sono Mappa, Argomento e Immagine.
   - **Tipo di riferimento**: Riferimenti diretti o indiretti
   - **Versione**: Numero di versione del file di origine
   - **Etichetta versione**: Etichetta per la versione selezionata del file di origine
   - **Versione di destinazione**: Numero di versione del file di destinazione
   - **Stato del documento**: Stato del file di origine. Le opzioni disponibili sono Bozza, In-Review e Revisione.
   - **Lingua di destinazione**: Lingua in cui si desidera tradurre il file di origine
   - **Stato della traduzione**: Le opzioni disponibili sono: Out of Sync, missing Copy, In Progress e In Sync.
   - **Etichetta di Target**: Etichetta per la versione selezionata del file di destinazione
1. Fai clic su **Invia per traduzione** nell&#39;angolo in alto a destra.

   ![](images/translation-send.png){width="800" align="left"}

1. Dal menu a discesa, seleziona **Creare un nuovo progetto di traduzione**.

   ![](images/translation-project-types.png){width="350" align="left"}

   Oltre a un nuovo progetto di traduzione, puoi anche scegliere tra le seguenti opzioni:

   - Puoi scegliere di **Creare una struttura** solo per il progetto di traduzione.
   - È possibile selezionare **Crea un nuovo progetto di traduzione multilingue** che includerà i lavori di traduzione per tutte le lingue selezionate per la traduzione. Ad esempio, se hai selezionato Francese, Tedesco e Spagnolo, creerà un progetto che contiene lavori di traduzione per tutte e tre le lingue.
   - Se disponi già di un progetto di traduzione, puoi aggiungere argomenti a tale progetto. Seleziona Aggiungi a **Progetto di traduzione esistente** dall’elenco Progetto e scegli un progetto dall’elenco Progetto di traduzione esistente. Puoi ordinare questi progetti in base all’ordine più recente, crescente o decrescente.

      >[!NOTE]
      >
      > Se il progetto esistente è un progetto di ambito, al nome del progetto è aggiunto &quot;\(Scoping\)&quot;.

   - Se devi creare l’ambito di un progetto da tradurre, puoi selezionare **Crea un nuovo progetto di traduzione dell&#39;ambito**. Questo non invierà le copie per la traduzione e lo stato di traduzione originale dei file viene mantenuto. Non vi è alcun impatto sulla copia in lingua di destinazione degli argomenti di cui si fa riferimento che vengono inviati per l&#39;ambito.
1. Nel campo **Titolo progetto**, inserisci un titolo.
1. Fai clic su **Crea** per creare un nuovo progetto di traduzione.

   Viene creato un nuovo progetto di traduzione con la versione selezionata degli argomenti. Al momento, viene visualizzato un messaggio pop-up di conferma della creazione del progetto di traduzione. Una volta che tutte le copie della lingua di destinazione sono disponibili nel progetto di traduzione, viene visualizzata una notifica nella casella in entrata. Una volta che le copie della lingua di destinazione sono disponibili nel progetto di traduzione, puoi procedere e avviare il lavoro di traduzione. Per maggiori dettagli vedi [Avvia il processo di traduzione](translation-first-time.md#id225IK030OE8).

   >[!NOTE]
   >
   > Se si rifiuta la traduzione per uno o più argomenti di un lavoro di traduzione, la **In corso** lo stato di traduzione di tutti gli argomenti rifiutati viene ripristinato al loro stato originale. Lo stato degli argomenti di cui si fa riferimento viene controllato e ripristinato in base allo stato di traduzione più recente. Inoltre, i file di traduzione creati nel progetto di destinazione non vengono eliminati anche se la traduzione viene rifiutata per essi.


## Passa l’etichetta della versione alla versione di destinazione

AEM Guide consente di passare l’etichetta del file di origine al file di destinazione. Questo ti aiuterà a identificare facilmente la versione di origine del file tradotto.

Per aggiungere l’etichetta della versione di origine nella copia di destinazione, l’amministratore di sistema deve selezionare l’opzione **Propagare le etichette della versione sorgente alla versione di destinazione** in **Traduzione** scheda in **Impostazioni editor**.

Ad esempio, se disponi di alcuni file di origine con l’etichetta della versione `Release 1.0` applicati a essi, puoi anche passare l&#39;etichetta sorgente \(`Release 1.0`\) al file tradotto.

![](images/translation-pass-source-label.png){width="650" align="left"}

>[!NOTE]
>
> L’etichetta sorgente viene associata a una sola versione di destinazione. Se sposti l’etichetta sorgente in un’altra versione, questa viene automaticamente riflessa nell’etichetta di destinazione più recente.

## Visualizza la differenza di versione per i file Out of Sync 

AEM Guide fornisce la funzione per controllare le differenze tra la versione selezionata e l’ultima versione sorgente tradotta degli argomenti. Puoi scegliere di tradurre il **Non sincronizzato** in base alle modifiche apportate.

![](images/translation-version-diff.png){width="800" align="left"}

Seleziona la **Mostra differenza** icona \(![](images/show-difference-icon.svg)\) per un argomento per vedere le differenze tra l&#39;ultima versione tradotta e la versione corrente del file selezionato.

>[!NOTE]
>
> **Mostra differenza** icona \(![](images/show-difference-icon.svg)\) viene visualizzato solo per i file DITA con lo stato di traduzione **Non sincronizzato**.

La **Differenza di versione** viene visualizzata la finestra di dialogo . Mostra la **Ultima versione tradotta** e **Versione selezionata** numero a sinistra. Nella finestra di anteprima vengono visualizzate le differenze tra l’ultima versione tradotta e la versione selezionata dell’argomento.

![](images/version-diff.png){width="650" align="left"}

## Ignora risorse fuori sincronia

Se apporti modifiche ad alcune risorse, queste diventano fuori sincronia. È possibile tradurre nuovamente le risorse modificate o scegliere di ignorare lo stato Out of Sync. Ad esempio, se hai apportato alcune modifiche molto minori che non hanno bisogno di una traduzione, puoi contrassegnarne lo stato in In Sync.

Per ignorare lo stato Out of Sync, effettua le seguenti operazioni:

1. Seleziona le risorse non sincronizzate per le quali vuoi modificare lo stato.
1. Seleziona la **Contrassegna in sincronia** pulsante \(![](images/translation-mark-in-sync-icon.svg)\) in alto. La **Contrassegna in sincronia** viene visualizzata la finestra di dialogo .

   ![](images/translation-mark-in-sync.png){width="550" align="left"}

1. Fai clic su **Forza sincronizzazione**. Imposta lo stato su In sincronizzato per le risorse non sincronizzate selezionate.

>[!NOTE]
>
> **Contrassegna in sincronia** pulsante \(![](images/translation-mark-in-sync-icon.svg)\) viene visualizzato solo per le risorse con lo stato di traduzione impostato su Non sincronizzato.

## Visualizza progetti di traduzione in corso per una mappa o un argomento

È possibile che alcuni riferimenti nel dashboard di traduzione siano in corso. Questi riferimenti hanno un **In corso** link sotto **Stato della traduzione** colonna. Quando fai clic sul collegamento, la **Progetti in corso** viene visualizzata la finestra di dialogo . Nella finestra di dialogo, puoi visualizzare l’elenco di tutti i progetti di traduzione in corso \(insieme alla lingua di destinazione\) che contengono il riferimento selezionato.

>[!NOTE]
>
> Puoi vedere il collegamento In corso per i progetti tradotti creati nella versione di AEM Guide as a Cloud Service di febbraio 2023 o successiva.

Fate clic sul nome del riferimento nella finestra di dialogo per aprirlo in modalità anteprima. Puoi anche fare clic sul progetto di traduzione per avviare la traduzione.

![](images/translation-in-progress.png){width="550" align="left"}

**Argomento principale:**[ Utilizzare l’editor Web](web-editor.md)
