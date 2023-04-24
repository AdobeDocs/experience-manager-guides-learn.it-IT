---
title: Gestione delle attività di pubblicazione tramite il dashboard di pubblicazione
description: Scopri come gestire le attività di pubblicazione utilizzando il dashboard di pubblicazione
source-git-commit: 8b6294425c6e60d1c5b37d98e99114014a104ee6
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---


# Gestione delle attività di pubblicazione tramite il dashboard di pubblicazione {#id205CC08305Z}

Quando nel sistema è in esecuzione un insieme di attività di pubblicazione di grandi dimensioni, diventa praticamente impossibile controllare ogni mappa DITA singolarmente per monitorare l&#39;attività di pubblicazione. AEM Guide offre agli amministratori e agli editori una visualizzazione unificata di tutte le attività di pubblicazione in esecuzione nel sistema. Un elenco di tutte le attività di pubblicazione attive è disponibile nel dashboard di pubblicazione.

La dashboard di pubblicazione offre una panoramica completa di tutte le attività di pubblicazione attualmente in esecuzione nel sistema.

![](images/publish-dashboard.png)

Il dashboard di pubblicazione contiene i seguenti dettagli:

- **Titolo mappa** - Il titolo di un file mappa attualmente pubblicato o nella coda di pubblicazione.

- **Nome file** - Il nome file della mappa DITA.

- **Predefinito di output** - Nome del predefinito di output utilizzato per generare l&#39;output.

- **Iniziato da** - Nome utente dell&#39;utente che ha avviato l&#39;attività di pubblicazione.

- **Avviato** - Data e ora di inizio dell&#39;attività di pubblicazione.

- **Tempo trascorso** - Ora dal momento in cui l’attività di pubblicazione è in esecuzione nel sistema.

- **Icona Elimina** - Annullare o terminare un&#39;attività di pubblicazione.

Il pannello a sinistra nel dashboard di pubblicazione fornisce le seguenti opzioni di filtro:

- **Predefinito di output** - Seleziona uno o più predefiniti di output per i quali visualizzare le attività di pubblicazione attualmente attive. Nella schermata seguente, le attività di pubblicazione vengono filtrate per mostrare solo le attività che utilizzano il predefinito di output AEM sito:

![](images/publish-dashboard-preset-filter.png)

- **Iniziato da** - Seleziona un nome utente dall’elenco per visualizzare le attività di pubblicazione avviate dall’utente selezionato.

- **Mappa** - Seleziona un file di mappa dall’elenco per visualizzare le attività di pubblicazione in esecuzione per la mappa selezionata.

## Accedere al dashboard di pubblicazione {#id205CC100DY4}

Esegui le seguenti operazioni per accedere al dashboard di pubblicazione:

>[!NOTE]
>
> Solo un amministratore o un editore può accedere al dashboard di pubblicazione.

1. Fai clic sul collegamento Adobe Experience Manager in alto e scegli **Strumenti**.

1. Seleziona **Guide** dall&#39;elenco degli strumenti.

1. Fai clic sul pulsante **Pubblica dashboard** piastrelle.

   Viene visualizzato il Dashboard di pubblicazione con un elenco di tutte le attività di pubblicazione attive nel sistema.

   Se si fa clic sul collegamento Nome file, viene visualizzata la console Mappa DITA della mappa selezionata.

   ![](images/publish-dashboard-click-filename-link.png)


>[!NOTE]
>
> Puoi anche accedere al Dashboard di pubblicazione dalla scheda Output mentre generi l&#39;output dal dashboard della mappa. Per ulteriori dettagli, consulta [Visualizza lo stato dell&#39;attività di generazione dell&#39;output](generate-output-for-a-dita-map.md#viewing_output_history).

## Annullare un’attività di pubblicazione

Esegui i seguenti passaggi per annullare un’attività di generazione dell’output dal dashboard di pubblicazione:

1. [Accedere al dashboard di pubblicazione](#id205CC100DY4).

1. Nell’elenco delle attività di pubblicazione attive, fare clic sull’icona Elimina di un’attività da annullare.

   ![](images/publish-dashboard-cancel-task.png)

1. Fai clic su **Sì** al prompt dei messaggi Conferma annullamento.

   Il comando Annulla viene accettato e viene eseguito un tentativo di annullamento finché l&#39;attività rimane attiva. Quando l&#39;attività viene terminata, viene rimossa dall&#39;elenco attività attualmente attivo. Lo stato dell&#39;attività viene aggiornato anche nella console mappa DITA come Annullato. Nella schermata seguente, il *HTML5* L&#39;attività viene annullata dal Dashboard di pubblicazione e il relativo stato viene modificato anche nella console mappa DITA.

   ![](images/cancelled-output-task.png)


**Argomento principale:**[ Generazione di output](generate-output.md)

