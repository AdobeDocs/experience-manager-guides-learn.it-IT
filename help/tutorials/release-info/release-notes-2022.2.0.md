---
title: Note sulla versione per [!DNL AEM Guides], versione di febbraio 2022
description: Versione di febbraio di [!DNL Adobe Experience Manager Guides] as a Cloud Service
exl-id: eb7ff475-bb5b-4d32-b291-024147fbfed1
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 3%

---

# Versione di febbraio di [!DNL Adobe Experience Manager Guides] as a Cloud Service

## Aggiornamento alla versione di febbraio

Aggiorna il tuo [!DNL Adobe Experience Manager Guides] as a Cloud Service (successivamente indicato come [!DNL AEM Guides] as a Cloud Service) eseguendo le seguenti operazioni:
1. Controlla il codice Git dei Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
1. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file dei tuoi Cloud Services Codice Git a 2022.2.114.
1. Conferma le modifiche ed esegui la pipeline dei Cloud Services per eseguire l’aggiornamento alla versione di febbraio di [!DNL AEM Guides] as a Cloud Service.

## Matrice di compatibilità

In questa sezione viene elencata la matrice di compatibilità per le applicazioni software supportate da [!DNL AEM Guides] Versione as a Cloud Service di febbraio 2022.

### FrameMaker e FrameMaker Publishing Server

| FMPS | FrameMaker |
| --- | --- |
| Non compatibile | Aggiornamento 4 e superiore del 2020 |
|  |  |


### Connettore dell&#39;ossigeno

| [!DNL AEM Guides] Versione cloud | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno |
| --- | --- | --- |
| 2022.2.0 | 2.4.0 | 2.4.0 |
|  |  |  |


## Nuove funzioni e miglioramenti

### Pubblicazione nativa di PDF

Nella versione di febbraio di [!DNL AEM Guides] as a Cloud Service. È stato introdotto un nuovo motore di pubblicazione con le seguenti funzioni:
* Creare un modello CSS
* Creare diversi modelli di pagina
* Modelli Design PDF che includono CSS e modelli di pagina
* Pubblicare contenuti mappa e argomento in formato PDF

### Supporto per il percorso del sito della knowledge base nella pubblicazione basata su articoli

[!DNL AEM Guides] as a Cloud Service fornisce la funzione di pubblicazione basata sugli articoli per generare in modo incrementale un output di uno o più argomenti o pubblicare i contenuti in una piattaforma knowledgebase. Con la versione di febbraio, hai un’opzione aggiuntiva per scegliere il percorso del sito della Knowledge Base al quale l’argomento/mappa deve essere pubblicato. Una volta selezionato il percorso, l&#39;output viene generato nel percorso specificato.

### Miglioramenti all’editor web

Sono stati aggiunti molti miglioramenti e nuove funzioni nell’editor web:

* **Finestra di dialogo migliorata alla chiusura del file**

[!DNL AEM Guides] Viene richiesto di salvare le modifiche e sbloccare i file bloccati quando si tenta di chiudere un file aperto nell&#39;Editor Web. I prompt vengono visualizzati in base al **Chiedi il check-in alla chiusura** e **Chiedi nuova versione alla chiusura** impostazioni configurate dall&#39;amministratore.

In base alla configurazione, è possibile salvare le modifiche e creare una nuova versione del documento. Oppure, puoi anche archiviare il file e salvare le modifiche alla versione corrente.

![File chiuso](assets/file-close-save-changes-unlock.png)

Per ulteriori dettagli, consulta *Scenari di chiusura e salvataggio dei file* nella Guida utente.

* Al pallet di caratteri è stato aggiunto uno spazio unificatore.  A **ininterrotto** lo spazio impedisce l’interruzione automatica della riga in un particolare punto di un documento HTML. L’editor Web supporta uno spazio unificatore sia per l’output AEM sito che per HTML5.

* Quando carichi un’immagine dall’Editor web, viene visualizzata una finestra di dialogo di conferma se esiste già un’immagine con lo stesso nome. È possibile mantenere entrambi i file, esistenti e nuovi, oppure sovrascrivere il file esistente e salvare solo il nuovo file.

* Se un utente ha bloccato qualsiasi file per le modifiche, un amministratore può rilasciare il blocco e archiviare il file. Questa funzione è utile quando alcuni file devono essere modificati ma sono stati bloccati da utenti che non sono disponibili per il check-in del file

### Dashboard mappa

Quando si seleziona per scaricare la mappa DITA, la richiesta viene messa in coda e si riceve una notifica una volta che la mappa è pronta per il download. Puoi scegliere di scaricare il file mappa immediatamente o scaricarlo in un secondo momento dal collegamento fornito nella casella in entrata della notifica AEM.

![Download mappa](assets/download-map-prompt.png)

### Recensione

È possibile citare i dettagli nel campo di descrizione dell&#39;attività di revisione, che viene visualizzato nell&#39;e-mail inviata al revisore.

## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

### Pubblicazione basata su articoli

* La pubblicazione basata su articoli non pubblica gli articoli in base alla linea di base selezionata. (8771)
* I file DITAVAL non vengono rispettati nella pubblicazione basata su articoli. (8770)
* Impossibile eseguire la pubblicazione basata sugli articoli per il profilo Salesforce quando il tipo di record è FAQ e il contenuto del campo articolo è Domanda. (8448)
* Impossibile eseguire la pubblicazione basata su articolo per il profilo Salesforce quando il tipo di record è Manuale. (8447)

### Editor web

* Il trascinamento e il rilascio di una condizione non funziona sugli argomenti DITA. (8761)
* Non sono disponibili attributi per l&#39;aggiunta di un capitolo nella libreria tramite trascinamento dalla vista Preferiti. (8746)
* La modifica delle proprietà di un&#39;immagine (altezza, larghezza) causa un errore dell&#39;applicazione. (8722)
* I collegamenti interrotti non vengono visualizzati nel pannello Struttura nella vista sorgente. (8590)
* L&#39;editor XML rimuove il tag di nuova riga nel blocco di codice. (8522)
* L’utilizzo del glossario viene visualizzato come Nota quando viene creata una voce Glossario. (8384)
* xref non può essere inserito anche in posizioni valide. (8354)
* L’elenco degli elementi (Alt+Invio) viene visualizzato in grigio nel tema scuro/scuro. (7913)
* L’elenco dei modelli mappa in **Crea** l&#39;opzione (menu ellissi) del pannello Archivio non corrisponde a **Profilo cartella** in Preferenze utente. (5918)
* Gli ID elemento non vengono generati automaticamente per gli elementi aggiunti dalla funzione Riutilizza contenuto della barra degli strumenti principale. (5826)

### Interfaccia utente Assets

* La modifica delle immagini non funziona come previsto sul server cloud. (8768)
* Nel pannello della cronologia delle versioni, la sezione della versione corrente mostra una marca temporale errata e viene modificata dalle informazioni. (8765)
* Il caricamento di file DITAVAL sul server cloud non riesce quando viene utilizzato lo strumento desktop AEM. (8707)
* Impossibile aggiungere il secondo utente amministratore come primo utente amministratore a una cartella. (8430)
* Le proprietà non univoche di una risorsa non vengono copiate quando la risorsa viene copiata e incollata. (8241)

### Modifiche all&#39;usabilità

* Nel pannello Revisione dell&#39;Editor Web, se un nome utente è lungo, le icone da accettare/rifiutare non vengono visualizzate chiaramente. (8793)
* In **Trova e sostituisci** , viene visualizzata un’icona indesiderata al passaggio del mouse nella sezione dei risultati. (8775)
* L’icona Personalizzato non viene selezionata dalla proprietà, ma viene visualizzata l’icona predefinita per i rapporti generati utilizzando il pulsante Genera report . (8573)
