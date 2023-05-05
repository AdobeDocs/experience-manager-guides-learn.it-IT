---
title: Rapporto Riutilizzo contenuto
description: Scopri come utilizzare i rapporti di riutilizzo dei contenuti
exl-id: 658ae0fd-9032-4480-b9e4-fe4fec261e72
source-git-commit: c74badebbcb4733fb9caa79c646b1d1e5c8bfe8e
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Rapporto Riutilizzo contenuto {#id205BB900OQD}

Un altro utile rapporto che puoi generare è il Rapporto di riutilizzo dei contenuti . Questo rapporto calcola la percentuale media di utilizzo del contenuto, molto utile per i responsabili di progetto e per i proprietari business per vedere la quantità di contenuto che viene riutilizzato.

>[!TIP]
>
> Per garantire il corretto funzionamento del rapporto di riutilizzo dei contenuti, devi abilitare il flusso di lavoro di post-elaborazione. Contatta l’amministratore di sistema per abilitare i flussi di lavoro di post-elaborazione.

Per visualizzare il rapporto sul riutilizzo dei contenuti, effettua le seguenti operazioni:

1. Fai clic sul collegamento Adobe Experience Manager in alto e scegli **Strumenti**.

1. Seleziona **Guide** dall&#39;elenco degli strumenti.

1. Fai clic sul pulsante **Rapporto Riutilizzo contenuto** piastrelle.

1. Fai clic su **Sfoglia** per scegliere un percorso in cui risiedano gli argomenti o inserire manualmente il percorso.

   Il rapporto viene generato effettuando la scansione del contenuto delle cartelle principali e secondarie.

1. Fai clic su **Genera report** per ottenere il rapporto sul riutilizzo dei contenuti.

   ![](images/content-reuse-uuid.png){width="800" align="left"}

   La pagina del rapporto è divisa in due parti:

   - **Riepilogo del rapporto:**

      Elenca il riutilizzo medio dei contenuti, calcolato come istanze di riutilizzo dei contenuti/conteggio totale degli argomenti. Questo rapporto tiene conto di tutti i riferimenti diretti al contenuto di primo livello e dei riferimenti agli argomenti da calcolare. Le istanze di riutilizzo dei contenuti vengono calcolate come la somma totale dei valori nel campo Numero di volte riutilizzati . L’argomento che viene maggiormente riutilizzato è inoltre elencato in Riepilogo rapporto. Facendo clic sul collegamento dell’argomento nell’argomento più riutilizzato viene visualizzata l’anteprima dell’argomento.

   - **Dettagli:**

      La sezione Dettagli contiene le colonne seguenti:

      - **Titolo**: Titolo dell&#39;argomento. Facendo clic sul collegamento del titolo dell’argomento si apre l’anteprima dell’argomento.

      - **UUID**: Identificatore univoco universale \(UID\) del file.

      - **Dimensione**: Dimensione dei file in byte.

      - **Stato**: Lo stato corrente del documento: Bozza, In-Review o Revisione.

      - **Numero di volte riutilizzati**: Numero di volte in cui l’argomento corrispondente è stato riutilizzato. Viene calcolato come somma totale delle voci nelle colonne con riferimento meno 1.

      - **A cui fa riferimento**: Argomenti a cui è stato fatto riferimento l&#39;argomento corrispondente. In questo caso, vengono considerati solo i riferimenti diretti \(primo livello\). Gli argomenti multipli sono separati da virgole. L&#39;UUID del file a cui si fa riferimento è menzionato anche tra parentesi.Facendo clic sul collegamento del titolo dell&#39;argomento si apre l&#39;anteprima dell&#39;argomento.


>[!NOTE]
>
> Puoi anche esportare il rapporto di riutilizzo dei contenuti in formato CSV. A questo scopo, fai clic sul collegamento Esporta in CSV nell’angolo in alto a sinistra dello schermo e scegli una posizione in cui salvare il file CSV. Puoi quindi aprire questo file CSV in qualsiasi editor CSV.

**Argomento principale:**[ Rapporti](reports-intro.md)
