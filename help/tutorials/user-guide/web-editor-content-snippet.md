---
title: Inserire uno snippet di contenuto dall'origine dati
description: Scopri come inserire uno snippet di contenuto dall’origine dati
source-git-commit: e4fcf6c7b7e69d83edb91e25081dae6e7cf1ae89
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---


# Inserire uno snippet di contenuto dall&#39;origine dati

Le guide AEM forniscono la funzione di connessione all’origine dati. Puoi recuperare i dati, inserirli negli argomenti e modificarli. Puoi creare facilmente un frammento di contenuto utilizzando il generatore di frammenti di contenuto e riutilizzarlo all’interno degli argomenti.

Per creare uno snippet di contenuto utilizzando il generatore di snippet di contenuto e inserirlo nell’argomento, effettua le seguenti operazioni:

1. Seleziona **Origini dati** ![](images/data-source-icon.svg)   nel pannello a sinistra per visualizzare le origini dati collegate. Viene visualizzato il pannello Origini dati (Data Sources), in cui sono visualizzate tutte le origini dati collegate. Per ulteriori dettagli, vedi [Configurare un connettore di origine dati](../cs-install-guide/conf-data-source-connector.md).
   >[!NOTE]
   >
   > Verranno visualizzate le origini dati per le quali l’amministratore ha configurato il connettore.

1. Selezionare un&#39;origine dati per visualizzare i generatori di frammenti di contenuto disponibili per l&#39;origine dati selezionata.
   ![](images/code-snippet-generator.png){width="300" align="left"}
1. Seleziona **Aggiungi** per aggiungere un nuovo generatore di frammenti di contenuto. Il **Aggiungi generatore frammenti di contenuto** viene visualizzato il pannello.

1. Immettere la query nella casella di testo Query dati.
1. Seleziona il modello da mappare con l&#39;origine dati dall&#39; **Modello di mappatura dati** a discesa.
I modelli predefiniti per l’origine dati selezionata vengono visualizzati nel menu a discesa. Ad esempio, è possibile visualizzare il modello &quot;sql-table&quot; per l&#39;origine dati denominata &quot;PostgreSQL&quot;.

   >[!NOTE]
   >  
   > Se l’amministratore ha configurato dei modelli personalizzati, questi vengono visualizzati anche nell’elenco a discesa (in base alle configurazioni del percorso del modello eseguite dall’amministratore).

1. Clic **Recupera** per recuperare i dati dall&#39;origine dati e applicare il modello ai dati risultanti dalla query SQL.
1. È possibile visualizzare i dati nell&#39;anteprima o nella vista origine DITA.

   1. L’anteprima mostra come verranno visualizzati i dati quando vengono inseriti nel contenuto. Nell&#39;anteprima viene visualizzata una piccola frazione di dati nel formato del modello selezionato.
Ad esempio:
      * Se è stato selezionato il modello di tabella SQL, è possibile visualizzare i dati SQL in formato tabulare.
      * Se hai selezionato il modello di elenco jira ordinato, puoi visualizzare un elenco ordinato per i problemi Jira.

   1. La vista origine mostra i dati nella vista origine DITA.
      ![](images/add-content-snippet-generator.png){width="800" align="left"}
1. Per salvare i risultati della query, immettere il nome del generatore, quindi fare clic su **AGGIUNGI**.   All’elenco viene aggiunto un nuovo generatore di frammenti di contenuto.

   >[!NOTE]
   >
   > Devi seguire la convenzione di denominazione dei file per il nome del nuovo generatore di contenuti. Il nome del generatore di frammenti di contenuto non può contenere spazi. Inoltre, non è possibile salvare un nuovo generatore di contenuti con il nome di un generatore di contenuti esistente. Si verifica un errore.

## Opzioni per un generatore di frammenti di contenuto

Fai clic con il pulsante destro del mouse su un generatore di frammenti di contenuto per aprire Opzioni. Utilizzando le opzioni, potete effettuare le seguenti operazioni:
* **Inserisci**: utilizza questa opzione per inserire lo snippet di contenuto selezionato nell’argomento aperto per la modifica nell’editor web. Poiché i dati vengono inseriti come frammento, è anche possibile modificare i dati all&#39;interno dell&#39;argomento nell&#39;Editor Web.

  >[!NOTE]
  > 
  > L&#39;opzione Inserisci viene visualizzata solo durante la modifica di un argomento.

* **Modifica**: utilizza questa opzione per apportare modifiche al generatore di frammenti di contenuto e salvarlo.
* **Elimina**: utilizza questa opzione per eliminare il generatore di frammenti di contenuto selezionato.
* **Duplica**: utilizza questa opzione per creare un duplicato o una copia del generatore di frammenti di contenuto selezionato. Per impostazione predefinita, il duplicato viene creato con un suffisso (come generator_1).

### Inserire uno snippet di query

È inoltre possibile utilizzare **Inserisci frammento di query** ![](images/data-source-icon.svg)   dalla barra degli strumenti principale per inserire lo snippet di dati negli argomenti.  Puoi selezionare un generatore dal menu a discesa, modificare la query o modificare il modello e inserire i dati nell’argomento.

![](images/insert-content-snippet.png){width="800" align="left"}




