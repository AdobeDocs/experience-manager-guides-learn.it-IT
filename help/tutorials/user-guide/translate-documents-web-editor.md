---
title: Traduci documenti dall'editor Web
description: Scopri come tradurre i documenti dall’editor web
exl-id: 02fc2b51-5b9a-4ad6-9e2e-726ab7602514
source-git-commit: 3bca42f0954afc2362ab24f369e698113324dbc3
workflow-type: tm+mt
source-wordcount: '1517'
ht-degree: 0%

---

# Traduci documenti dall&#39;editor Web {#id21BKF0Z0YZF}

>[!TIP]
>
> Si consiglia di utilizzare questa funzione di traduzione dall’editor web se è stato effettuato l’aggiornamento alla versione di febbraio 2022 o successiva delle guide AEM as a Cloud Service.

Le guide AEM sono dotate di una potente funzione nell’editor web che consente di tradurre i contenuti in più lingue. Puoi creare un nuovo progetto di traduzione e successivamente aggiungerlo al progetto esistente. Puoi anche creare un progetto di traduzione multilingue che include processi di traduzione per tutte le lingue selezionate.

>[!NOTE]
>
> L’amministratore può configurare la scheda Gestisci \(utilizzata per la traduzione\) nell’editor web. Per ulteriori dettagli, consulta *Configurare la funzione di traduzione nell’editor web* nella sezione Installare e configurare Adobe Experience Manager Guides as a Cloud Service.

## Prima di iniziare

Prima di eseguire i passaggi descritti in questa procedura, verificare di aver creato le cartelle principali e di destinazione della lingua richieste

1. Crea una cartella principale per archiviare il contenuto sorgente. La cartella principale deve essere creata con il nome della lingua \(ad esempio Inglese\) o il codice della lingua \(en\).
1. Crea le cartelle di destinazione in cui desideri tradurre il contenuto. Ad esempio, se desideri tradurre il contenuto in tedesco o francese, devi creare una cartella denominata -de \(per tedesco\) o -fr \(per francese\).

>[!NOTE]
>
> La cartella principale e le cartelle di destinazione devono essere create allo stesso livello.

## Crea un progetto di traduzione

1. Nel pannello Repository, aprire il file mappa DITA in visualizzazione mappa.
1. Fai clic su **Gestisci** scheda. Il pannello Traduzione visualizza il titolo del collegamento ipertestuale della mappa DITA insieme al **Lingue** elenco.
1. Dalla sezione **Lingue** , seleziona la lingua in cui desideri tradurre il progetto. Puoi selezionare **Tutti** per tradurre il progetto in tutte le lingue disponibili.

   >[!NOTE]
   >
   > L&#39;elenco contiene le cartelle della lingua insieme ai relativi codici di lingua. Ad esempio, francese \(fr\) e tedesco \(de\).

   >[!IMPORTANT]
   >
   > Lingua mostra solo le lingue per le quali viene creata una cartella della lingua parallela alla lingua di origine. Non viene visualizzata neanche una cartella della lingua creata a qualsiasi altro livello, ad esempio a un livello inferiore rispetto alla cartella della lingua di origine. Assicurati di creare tutte le cartelle della lingua di destinazione allo stesso livello della cartella della lingua di origine.

   ![](images/translation-languages.png){width="350" align="left"}

1. È inoltre possibile utilizzare le seguenti opzioni:

   **Usa baseline:** Puoi selezionare una previsione per tradurre il progetto. Fate clic su Usa baseline (Use Baseline) e scegliete una baseline creata sulla mappa. Tutti i file che fanno parte della baseline selezionata vengono visualizzati nella pagina Traduzione. Una volta tradotti i contenuti, puoi esportare la linea di base tradotta. Per ulteriori dettagli sull&#39;esportazione della linea di base tradotta, vedi [Esporta previsione tradotta](generate-output-use-baseline-for-publishing.md#id196SE600GHS).

   **Usa ultima versione come**: scegli di filtrare la versione degli argomenti in base alla data e all’ora di creazione. Quando si seleziona una data e un&#39;ora, viene visualizzata solo la versione più recente dei file creati in corrispondenza o prima della data e dell&#39;ora selezionate.

1. Clic **Applica**. Viene visualizzato un elenco con i dettagli degli argomenti e delle risorse associate.
1. Seleziona gli argomenti da inviare per la traduzione.

   Puoi anche utilizzare le seguenti opzioni di filtro per argomenti:

   - **Titolo**: titolo del file di origine
   - **Nome file**: nome del file di origine
   - **Tipo di file**: tipo del file di origine. Le opzioni disponibili sono Mappa, Argomento e Immagine.
   - **Tipo di riferimento**: riferimenti diretti o indiretti
   - **Versione**: numero di versione del file di origine
   - **Etichetta versione**: etichetta per la versione selezionata del file di origine
   - **Versione di destinazione**: numero di versione del file di destinazione
   - **Stato documento**: stato del file di origine. Le opzioni disponibili sono Bozza, In revisione e Rivisto.
   - **Lingua di destinazione**: lingua in cui desideri tradurre il file di origine
   - **Stato traduzione**: le opzioni disponibili sono: Non sincronizzato, Copia mancante, In corso e In sincronia.
   - **Etichetta destinazione**: etichetta per la versione selezionata del file di destinazione
1. Clic **Invia per traduzione** nell&#39;angolo in alto a destra.

   ![](images/translation-send.png){width="800" align="left"}

1. Dal menu a discesa, seleziona **Crea un nuovo progetto di traduzione**.

   ![](images/translation-project-types.png){width="350" align="left"}

   Oltre a un nuovo progetto di traduzione, puoi selezionare tra le seguenti opzioni:

   - Puoi scegliere di **Creare una struttura** solo per il progetto di traduzione.
   - Puoi selezionare **Crea un nuovo progetto di traduzione multilingue** che includerà i processi di traduzione per tutte le lingue selezionate per la traduzione. Ad esempio, se hai selezionato francese, tedesco e spagnolo, verrà creato un progetto che contiene processi di traduzione per tutte e tre le lingue.
   - Se disponi già di un progetto di traduzione, puoi aggiungere argomenti a tale progetto. Seleziona Aggiungi a **Progetto di traduzione esistente** dall’elenco Progetto e scegli un progetto dall’elenco Progetto di traduzione esistente. Puoi ordinare questi progetti in base all’ordine più recente, crescente o decrescente.

      >[!NOTE]
      >
      > Se il progetto esistente è un progetto con ambito, al suo nome viene aggiunto &quot;\(Ambito\)&quot;.

   - Per creare l’ambito di un progetto da tradurre, puoi selezionare **Crea un nuovo progetto di traduzione ambito**. Questo non invierà le copie per la traduzione e lo stato di traduzione originale dei file viene mantenuto. Non vi è alcun impatto sulla copia nella lingua di destinazione degli argomenti trattati che vengono inviati per l’ambito.
1. Nel campo **Titolo progetto**, inserisci un titolo.
1. Clic **Crea** per creare un nuovo progetto di traduzione.

   Viene creato un nuovo progetto di traduzione con la versione selezionata degli argomenti. In questo momento, viene visualizzato un messaggio pop-up che conferma la creazione del progetto di traduzione. Una volta che tutte le copie per lingua di destinazione sono disponibili nel progetto di traduzione, si riceve una notifica nella casella in entrata. Una volta che le copie per lingua di destinazione sono disponibili nel progetto di traduzione, puoi procedere e avviare il processo di traduzione. Per maggiori dettagli, vedere [Avvia il processo di traduzione](translation-first-time.md#id225IK030OE8).

   >[!NOTE]
   >
   > Se rifiuti la traduzione per uno o più argomenti in un processo di traduzione, il **In corso** lo stato di traduzione di tutti gli argomenti rifiutati ritorna allo stato originale. Lo stato degli argomenti indicati viene controllato e ripristinato in base all’ultimo stato di traduzione. Inoltre, i file di traduzione creati nel progetto di destinazione non vengono eliminati anche se la traduzione viene rifiutata per essi.


## Passa l’etichetta della versione alla versione di destinazione

Le guide AEM consentono di passare l&#39;etichetta del file di origine al file di destinazione. Questo ti aiuterà a identificare facilmente la versione sorgente del file tradotto.

Per aggiungere l’etichetta della versione di origine nella copia di destinazione, l’amministratore di sistema deve selezionare l’opzione **Propaga le etichette della versione di origine alla versione di destinazione** sotto **Traduzione** scheda in **Impostazioni editor**.

Ad esempio, se disponi di alcuni file di origine con l’etichetta della versione `Release 1.0` applicate, è possibile passare anche l&#39;etichetta di origine \(`Release 1.0`\) al file tradotto.

![](images/translation-pass-source-label.png){width="650" align="left"}

>[!NOTE]
>
> L’etichetta di origine è associata a una sola versione di destinazione. Se sposti l’etichetta di origine in un’altra versione, questa si riflette automaticamente nell’etichetta di destinazione più recente.

## Visualizza differenza di versione per file non sincronizzati 

Le guide AEM consentono di verificare le differenze tra la versione selezionata e l&#39;ultima versione di origine tradotta degli argomenti. Puoi scegliere di tradurre la **Non sincronizzato** file in base alle modifiche apportate.

![](images/translation-version-diff.png){width="800" align="left"}

Seleziona la **Mostra differenza** icona \(![](images/show-difference-icon.svg)\) affinché un argomento visualizzi le differenze tra l&#39;ultima versione tradotta e la versione corrente del file selezionato.

>[!NOTE]
>
> **Mostra differenza** icona \(![](images/show-difference-icon.svg)\) viene visualizzato solo per i file DITA con stato di traduzione **Non sincronizzato**.

Il **Differenza di versione** viene visualizzata. Mostra la **Ultima versione tradotta** e **Versione selezionata** numero a sinistra. Nella finestra di anteprima vengono visualizzate le differenze tra l&#39;ultima versione tradotta e la versione selezionata dell&#39;argomento.

![](images/version-diff.png){width="650" align="left"}

## Ignora risorse non sincronizzate

Se apporti modifiche ad alcune delle risorse, queste diventano non sincronizzate. Puoi tradurre nuovamente le risorse modificate o scegliere di ignorare lo stato Non sincronizzato. Ad esempio, se hai apportato alcune modifiche molto piccole che non richiedono alcuna traduzione, puoi contrassegnarne lo stato su In sincronia.

Per ignorare lo stato Non sincronizzato, effettuare le seguenti operazioni:

1. Seleziona le risorse non sincronizzate per le quali desideri modificare lo stato.
1. Seleziona la **Segna in sincronia** button \(![](images/translation-mark-in-sync-icon.svg)\) in alto. Il **Segna in sincronia** viene visualizzata.

   ![](images/translation-mark-in-sync.png){width="550" align="left"}

1. Clic **Forza sincronizzazione**. Imposta lo stato su In sincronia per le risorse non sincronizzate selezionate.

>[!NOTE]
>
> **Segna in sincronia** button \(![](images/translation-mark-in-sync-icon.svg)\) viene visualizzato solo per le risorse con stato di traduzione Non sincronizzato.

## Visualizza progetti di traduzione in corso per una mappa o un argomento

Alcuni dei riferimenti nel dashboard di traduzione potrebbero essere in stato di avanzamento. Questi riferimenti hanno un **In corso** collega in **Stato traduzione** colonna. Quando fai clic sul collegamento, il **Progetti in corso** viene visualizzata una finestra di dialogo. Nella finestra di dialogo, puoi visualizzare l’elenco di tutti i progetti di traduzione In corso \(insieme alla lingua di destinazione\) che contengono il riferimento selezionato.

>[!NOTE]
>
> Puoi visualizzare il collegamento In corso per i progetti tradotti creati nella versione di febbraio 2023 o successiva delle guide dell’AEM as a Cloud Service.

Fate clic sul nome del riferimento nella finestra di dialogo per aprirlo in modalità anteprima. Puoi anche fare clic sul progetto di traduzione per avviare la traduzione.

![](images/translation-in-progress.png){width="550" align="left"}

**Argomento padre:**[ Utilizzare l’editor web](web-editor.md)
