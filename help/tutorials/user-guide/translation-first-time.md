---
title: Best practice per la traduzione dei contenuti
description: Scopri le best practice per la traduzione dei contenuti
source-git-commit: 7cd719921e68ac1763d09d9665d912e3697e5849
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 1%

---


# Best practice per la traduzione dei contenuti {#id1678G0S702F}

Considera il seguente punto per la traduzione dei contenuti:

- I nomi delle cartelle e dei file devono essere conformi agli standard di denominazione dei file, ad esempio: non devono essere presenti spazi, apostrofo, parentesi graffe, segno uguale, caratteri speciali o non ASCII.

- Se traduci contenuti in lingue diverse, devi creare cartelle corrispondenti a ciascuna lingua. Ognuna di queste cartelle linguistiche conterrà il contenuto corrispondente a tale lingua. Ad esempio, è possibile creare cartelle utilizzando il designatore di lingua come `de` per il tedesco, `fr` per il francese, e così via. In alternativa, è possibile creare cartelle utilizzando designatori di lingua e regione come `fr-FR` per il francese utilizzato in Francia o `fr-CA` per il francese utilizzato in Canada.
- Nella lingua di destinazione devono essere selezionate anche le impostazioni internazionali effettive in base alle cartelle della lingua di destinazione nella relativa istanza.
- La configurazione cloud deve corrispondere a quella della cartella di origine e deve essere presente una sola configurazione cloud in una cartella. Puoi creare più cartelle in /conf, se desideri utilizzare più connettori di traduzione.
- Una cartella non deve contenere più di 1000 file.
- Assicurati che l&#39;utente incaricato di avviare il processo di traduzione disponga delle autorizzazioni di lettura, modifica, creazione ed eliminazione per le cartelle della lingua di origine e di destinazione.
- Poiché la traduzione dei contenuti richiede la creazione di un progetto di traduzione, l’utente deve disporre dell’accesso per creare un progetto in AEM.
- Per utilizzare i predefiniti condizionali con la mappa, è necessario crearli prima di avviare il processo di traduzione. Poiché anche i predefiniti condizionali sono raggruppati nella versione tradotta della mappa, la creazione dei predefiniti prima di avviare il processo di traduzione garantisce che siano disponibili nella versione tradotta.
- Il processo di traduzione del contenuto deve essere avviato dalla console mappa DITA e non dall’interfaccia utente AEM Assets.
- Il flusso di lavoro di traduzione DITA basato su componenti non deve essere utilizzato se si traduce il contenuto tramite traduzione umana. Tuttavia, questa opzione deve essere utilizzata per la traduzione automatica.
- I contenuti e i contenuti utilizzati a livello globale che non richiedono la localizzazione devono essere esclusi dalle copie in lingua.
- Tutti i contenuti comuni da localizzare devono essere conservati in una cartella comune all’interno della cartella della lingua.

L’illustrazione seguente mostra un esempio di struttura di cartelle in AEM quando sono stati utilizzati globalmente contenuti e tre copie in lingua.

![](images/aem-directory_structure.png)

## Configurare il servizio di traduzione

Esegui i seguenti passaggi per configurare il servizio di traduzione umana o automatica da utilizzare:

1. Nell’interfaccia utente Assets, seleziona la cartella della lingua di origine.

1. Apri le proprietà della cartella e vai a **Cloud Services** scheda .

1. In **Cloud Services** configura il servizio di traduzione che desideri utilizzare.

   Puoi configurare la traduzione automatica o umana.

   Assicurati che ci sia una sola configurazione per il connettore di traduzione in un’unica cartella. Se sono presenti più connettori di traduzione, è possibile creare più cartelle in /conf. Prima di avviare il processo di traduzione, nella cartella della lingua di origine deve essere selezionata una configurazione cloud.

   >[!NOTE]
   >
   > Vedi [Configurazione del framework di integrazione della traduzione](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/sites/administering/reusing-content/translation/integration-framework.html?lang=en) nella documentazione AEM per informazioni dettagliate sull’integrazione con i servizi di traduzione di terze parti.

1. Fai clic su **Salva e chiudi** per salvare le proprietà della cartella aggiornate.


>[!TIP]
>
> Consulta la sezione *Traduzione* nella guida alle best practice per le best practice relative alla traduzione dei contenuti.

## Crea un nuovo progetto di traduzione

Esegui i seguenti passaggi per creare un progetto di traduzione:

>[!NOTE]
>
> Prima di eseguire i passaggi descritti in questa procedura, assicurati di aver creato le cartelle principali e di destinazione della lingua richieste come descritto in [Best practice per la traduzione dei contenuti](#id1678G0S702F).

1. Nell’interfaccia utente Assets, fai clic sul file di mappa DITA.

1. Fai clic sul pulsante **Traduzione** scheda .

1. Da **Lingue di destinazione** seleziona le impostazioni internazionali in cui tradurre il progetto e fai clic su **Fine**.

   Viene visualizzato un riepilogo e i dettagli degli argomenti e delle risorse associate.

   >[!IMPORTANT]
   >
   > La **Lingue di destinazione** mostrare solo le lingue per le quali viene creata una cartella di lingua parallela alla lingua di origine. Non viene visualizzata anche una cartella di lingua creata a un altro livello, ad esempio un livello inferiore dalla cartella della lingua di origine. Assicurati di creare tutte le cartelle della lingua di destinazione allo stesso livello della cartella della lingua di origine.

1. Seleziona gli argomenti da inviare per la traduzione.

   Puoi anche utilizzare le seguenti opzioni di filtro degli argomenti:

   >[!NOTE]
   >
   > Dopo aver applicato il filtro richiesto, fai clic su **Fine** nel pannello Filtro per filtrare gli argomenti in base alla selezione.

   - **Stato della traduzione**: Scegli di filtrare gli argomenti in base al loro stato di traduzione. Le opzioni disponibili sono: Out of Sync, missing Copy, In Progress e In Sync.
   - **Ricerca**: Immettere uno o più termini da cercare nei titoli degli argomenti.
   - **Tipo di origine**: Scegli di filtrare gli argomenti in base ai loro tipi di file. Le opzioni disponibili sono: Tutto, DITA, Mappa DITA, Risorsa.
   - **Versione sorgente modificata dopo**: Scegli di filtrare l’argomento in base alla data e all’ora di modifica. Tutti gli argomenti modificati dopo la data e l’ora specificate vengono visualizzati nell’elenco.
   - **Linea**: Fare clic su Usa linea di base e scegliere una linea di base creata sulla mappa. Tutti i file che fanno parte della baseline selezionata vengono visualizzati nella pagina Traduzione. Puoi scegliere i file desiderati dalla linea di base e procedere con il processo di traduzione. Una volta tradotto il contenuto, puoi esportare la baseline tradotta. Per ulteriori dettagli sull&#39;esportazione della linea di base tradotta, vedi [Esporta linea di base tradotta](generate-output-use-baseline-for-publishing.md#id196SE600GHS).
1. Fai clic su **Creare/aggiornare copie per lingua** nella parte inferiore del pannello Filtro.

1. Da **Progetto** elenco, selezionare **Creare un nuovo progetto di traduzione**.

   >[!NOTE]
   >
   > Se disponi già di un progetto di traduzione, puoi aggiungere argomenti a tale progetto. Seleziona **Aggiungi a progetto di traduzione esistente** dall&#39;opzione **Progetto** seleziona un progetto dall’elenco **Progetto di traduzione esistente** elenco.

1. Nel campo **Titolo progetto**, inserisci un titolo.

1. Seleziona la **Includi mappa DITA** per inviare la mappa per la traduzione.
1. Fai clic su **Inizio** per creare un nuovo progetto di traduzione.

   Viene creato un nuovo progetto di traduzione con la versione selezionata degli argomenti. Al momento, viene visualizzato un messaggio pop-up di conferma della creazione del progetto di traduzione. Una volta che tutte le copie della lingua di destinazione sono disponibili nel progetto di traduzione, viene visualizzata una notifica nella casella in entrata. Una volta che l’area copie in lingua di destinazione è disponibile nel progetto di traduzione, puoi procedere e avviare il lavoro di traduzione.


## Avvia il processo di traduzione {#id225IK030OE8}

Esegui i seguenti passaggi per avviare il processo di traduzione:

1. In **Progetti** console, passa alla cartella di progetto creata per la localizzazione.

1. Fai clic sul progetto di localizzazione per aprire la pagina dei dettagli.

1. Fai clic sulla freccia **Processo di traduzione** e seleziona **Inizio** dall’elenco per avviare il flusso di lavoro di traduzione.

   >[!NOTE]
   >
   > Se utilizzi il servizio di traduzione umana, devi esportare il contenuto per la traduzione. Una volta che hai tradotto il contenuto, devi importarlo nuovamente nel progetto di traduzione.

1. Per visualizzare lo stato del processo di traduzione, fai clic sui puntini di sospensione nella parte inferiore del **Processo di traduzione** piastrelle.


Al termine della traduzione, lo stato del processo di traduzione cambia in *Pronto per la revisione*. Per completare il processo di traduzione, devi accettare la copia tradotta e i metadati delle risorse dal riquadro Processo di traduzione nella console Progetto.

>[!NOTE]
>
> Se si rifiuta la traduzione per uno o più argomenti di un lavoro di traduzione, la **In corso** lo stato di traduzione di tutti gli argomenti rifiutati viene ripristinato al loro stato originale. Lo stato degli argomenti di cui si fa riferimento viene controllato e ripristinato in base allo stato di traduzione più recente. Inoltre, i file di traduzione creati nel progetto di destinazione non vengono eliminati anche se la traduzione viene rifiutata per essi.

**Argomento principale:**[ Tradurre il contenuto](translation.md)

