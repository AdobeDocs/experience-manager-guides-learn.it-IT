---
title: Note sulla versione per [!DNL AEM Guides], versione di marzo 2022
description: Rilascio di marzo [!DNL Adobe Experience Manager Guides] as a Cloud Service
exl-id: 885edbb5-dfe4-4bdc-bb66-0df64addb094
source-git-commit: b5e64512956f0a7f33c2021bc431d69239f2a088
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 2%

---

# Rilascio di marzo [!DNL Adobe Experience Manager Guides] as a Cloud Service

## Aggiornamento alla versione di marzo

Aggiorna il tuo [!DNL Adobe Experience Manager Guides] as a Cloud Service (successivamente indicato come *[!DNL AEM Guides]as a Cloud Service*) eseguendo le seguenti operazioni:
1. Controlla il codice Git dei Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
2. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file dei tuoi Cloud Services Codice Git a 2022.3.123.
3. Conferma le modifiche ed esegui la pipeline dei Cloud Services per eseguire l’aggiornamento alla versione di marzo di [!DNL AEM Guides] as a Cloud Service.

## Matrice di compatibilità

In questa sezione viene elencata la matrice di compatibilità per le applicazioni software supportate da [!DNL AEM Guides] Versione as a Cloud Service di marzo 2022.

### FrameMaker e FrameMaker Publishing Server

| FMPS | FrameMaker |
| --- | --- |
| Non compatibile | Aggiornamento 4 e superiore del 2020 |
|  |  |


### Connettore dell&#39;ossigeno

| [!DNL AEM Guides] Versione cloud | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno |
| --- | --- | --- |
| 2022.3.0 | 2.4.0 | 2.4.0 |
|  |  |  |

*La linea di base e le condizioni create in AEM sono supportate nelle versioni FMPS a partire dal 2020.2.

## Nuove funzioni e miglioramenti

### Nuovo dashboard della linea di base

[!DNL AEM Guides] La versione di marzo as a Cloud Service fornisce la funzione Linea di base integrata all’interno dell’editor web. È ora possibile creare linee di base dall’editor Web e utilizzarle per pubblicare o tradurre argomenti di versioni diverse.

Nota: Per il sistema aggiornato, aggiornare **ui_config.json** per Profilo cartella.

Utilizza questa funzione per creare una baseline con una versione specifica degli argomenti disponibili in una data e in un&#39;ora specifiche. Inoltre, ottieni il supporto API per creare o aggiornare una linea di base con un’etichetta definita per una versione di argomenti.

![scheda gestione linea di base](assets/baseline-manage.png)

È possibile cercare i file in base ai nomi dei file o alla posizione del file. Puoi anche filtrare gli argomenti da visualizzare nella finestra di modifica della linea di base e ordinarli in base a colonne specifiche.

![scheda gestione linea di base](assets/baseline-filter.png)

Le prestazioni del processo di creazione della linea di base sono state ulteriormente migliorate. Il processo di creazione delle linee di base è asincrono, pertanto puoi continuare a modificare altri file nell’Editor web durante la creazione della linea di base. Per ulteriori dettagli, consulta *Creare e gestire le linee di base dall’editor web* nella Guida utente.

Nota: La scheda Linea di base nel dashboard della mappa è nascosta per impostazione predefinita. L’amministratore può abilitare la scheda Linea di base nel dashboard della mappa.

### Comportamento di aggiornamento migliorato dell’Editor Web

I seguenti miglioramenti sono ora disponibili con l’operazione di aggiornamento del browser nell’editor Web:

* Ora è disponibile il supporto per aggiornare il browser mentre si modifica il contenuto nell&#39;editor Web. Se si preme l&#39;icona di aggiornamento del browser quando si aprono per la modifica uno o più file con modifiche non salvate, viene richiesto di salvare i file o annullare l&#39;azione di aggiornamento.

* Anche quando si aggiorna il browser, vengono mantenute le viste del pannello di sinistra e del pannello di destra.

* L’argomento attivo o la mappa DITA viene riaperta nell’area di modifica del contenuto.

### Miglioramenti alla pubblicazione

Il processo di pubblicazione è stato ulteriormente migliorato con la versione di marzo di [!DNL AEM Guides] as a Cloud Service:

* Le linee di base sono state rispettate per i metadati dell&#39;output AEM sito. È inoltre possibile elaborare le proprietà di una versione della linea di base come metadati. Se non viene definita alcuna linea di base, le proprietà della versione più recente vengono elaborate come metadati.

* La **Nome file** e **Argomenti della riga di comando DITA-OT** sono state aggiunte opzioni per i predefiniti di output HTML5, EPUB e Personalizzato. Ora è possibile specificare il nome del file con cui si desidera salvare l&#39;output. È inoltre possibile specificare gli argomenti aggiuntivi da elaborare durante la generazione dell&#39;output.

## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

* Impossibile aggiungere elementi di sfondo in una libreria utilizzando la visualizzazione Autore dell&#39;editor Web. (7652)
* La struttura dei riferimenti si interrompe dopo la rimozione di un argomento e l&#39;esecuzione di un&#39;operazione Sposta. (8804)
* Viene ricevuta un’eccezione alla visualizzazione del contenuto dopo il caricamento di una risorsa. (3638)
* L&#39;errore si verifica quando i file la cui cartella padre contiene caratteri speciali nel nome file, vengono aperti in Ossigeno (utilizzando **Modifica in ossigeno** ). (8918)
* La **Individua nell’archivio** l&#39;opzione non individua ed evidenzia la mappa DITA in XML Editor. (8796)
* Il filtro non mostra i risultati appropriati quando al contenuto in XML Editor vengono aggiunti più attributi. (8795)
* Si verifica un errore durante l’aggiunta di un utente come amministratore nel profilo della cartella quando l’ID utente è numerico. (8908)

## Problemi noti

L&#39;Adobe ha identificato il seguente problema noto nel [!DNL AEM Guides] Versione as a Cloud Service di marzo.

* La rimozione delle etichette sui riferimenti diretti rimuove anche le etichette dai riferimenti indiretti.

* Impossibile riflettere il titolo della linea di base aggiornato senza aggiornare manualmente il pannello della linea di base.

* La funzione di anteprima della versione nel pannello Cronologia versioni non mostra l’anteprima di un argomento selezionato.
