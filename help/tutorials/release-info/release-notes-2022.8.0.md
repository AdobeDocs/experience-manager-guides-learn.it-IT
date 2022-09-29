---
title: Note sulla versione | Guide Adobe Experience Manager as a Cloud Service, agosto 2022
description: Rilascio di agosto delle guide di Adobe Experience Manager as a Cloud Service
source-git-commit: d49ccb3f654dede0c0447849d89ecbab333a1055
workflow-type: tm+mt
source-wordcount: '1156'
ht-degree: 2%

---

# Rilascio di agosto delle guide di Adobe Experience Manager as a Cloud Service

## Aggiornamento alla versione di agosto

Aggiorna le guide correnti di Adobe Experience Manager as a Cloud Service (in seguito denominate *Guide AEM as a Cloud Service*) eseguendo le seguenti operazioni:
1. Controlla il codice Git dei Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
2. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file dei tuoi Cloud Services Codice Git a 2022.8.167.
3. Conferma le modifiche ed esegui la pipeline dei Cloud Services per eseguire l’aggiornamento alla versione di agosto di AEM Guide as a Cloud Service.

## Matrice di compatibilità

In questa sezione viene elencata la matrice di compatibilità per le applicazioni software supportate dalle AEM Guide as a Cloud Service nella versione di agosto 2022.

### FrameMaker e FrameMaker Publishing Server

| FMPS | FrameMaker |
| --- | --- |
| Non compatibile | Aggiornamento 4 e superiore del 2020 |
|  |  |

*La linea di base e le condizioni create in AEM sono supportate nelle versioni FMPS a partire dal 2020.2.

### Connettore dell&#39;ossigeno

| AEM guide as a Cloud Release | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno |
| --- | --- | --- |
| 2022.8.0 | 2,7,5 | 2,7,5 |
|  |  |  |


## Nuove funzioni e miglioramenti

AEM guide as a Cloud Service offre numerosi miglioramenti e nuove funzioni nella versione di agosto:

### Visualizzazione Layout nell’Editor mappa

Ora è possibile visualizzare il layout completo di una mappa DITA nell&#39;Editor mappa. Quando apri una mappa per la modifica, viene aperta la **Layout** vista dell’Editor mappa. In questa visualizzazione è possibile visualizzare la gerarchia delle mappe in una vista ad albero e organizzare o strutturare gli argomenti in una mappa.

![visualizzazione layout](assets/layout-view-map.png)

La visualizzazione Layout contiene una barra degli strumenti separata che consente di eseguire molte attività sugli argomenti presenti in una mappa.
È possibile inserire riferimenti ad argomenti, gruppi di argomenti, definizioni di chiavi in una mappa. È possibile riorganizzare gli argomenti presenti in una mappa spostandoli verso l’alto, verso il basso, verso sinistra o verso destra. Puoi anche trascinare gli argomenti per spostarli in una mappa. L’Editor mappa fornisce inoltre le icone per bloccare o sbloccare i file, controllare la cronologia delle versioni e eseguire una gestione delle etichette delle versioni.


La vista Layout fornisce anche la **Opzioni di visualizzazione** per visualizzare o nascondere il numero di riga, mostrare o nascondere la casella di controllo o mostrare il nome o il titolo del file per gli argomenti in una mappa.


![view-options](assets/view-options.png)

Puoi anche visualizzare gli argomenti in base ai filtri condizionali applicati.

Oltre a organizzare gli argomenti nel file di mappa, è anche possibile aggiungere, spostare, copiare, incollare o eliminare riferimenti utilizzando il **Opzioni** menu disponibile per un elemento nella vista Layout. Puoi anche trascinare un argomento o una mappa dal pannello archivio alla mappa aperta nell’Editor mappa.

Il pannello a destra visualizza le proprietà del contenuto e le proprietà della mappa nella vista Layout dell’Editor mappa. Gli Attributi in linea definiti per l’argomento selezionato vengono visualizzati rispetto all’argomento nella vista Layout. Ad esempio, puoi trovare rapidamente tutti gli argomenti con l’attributo platform definito come `IOS`.

Ora è anche possibile impostare le informazioni sui metadati per gli argomenti o la mappa. Puoi definire il Titolo della barra di navigazione, Testo collegamento, Descrizione breve e Parole chiave per l’argomento o la mappa selezionati.

![pannello a destra della visualizzazione layout](assets/layout-inline-attributes.png)

Per ulteriori dettagli, consulta *Visualizzazione Layout* in Utilizzo delle guide di Adobe Experience Manager as a Cloud Service.

### Attributi in linea nelle impostazioni dell’editor

AEM Guide consente ora la configurazione di **Attributi in linea** da parte dell&#39;amministratore **Impostazioni editor**. Puoi anche aggiungere nuovi attributi in linea o eliminare quelli esistenti dal **Attributi in linea** in Impostazioni editor.
Gli Attributi in linea configurati per un argomento vengono visualizzati rispetto all’argomento nella visualizzazione Layout.

![Impostazioni editor](assets/editor-settings-inline-attributes.png)


### Filtri aggiuntivi nella vista Archivio

Ora la ricerca del filtro nella visualizzazione archivio è stata resa più efficace. Due nuovi criteri di ricerca, **Ultima modifica** e **Tag** sono stati aggiunti per filtrare i file e limitare la ricerca nell’archivio AEM:
* **Ultima modifica**: È possibile cercare i file che sono stati modificati per l’ultima volta dopo una data selezionata ma prima di una data selezionata. È inoltre possibile utilizzare i criteri predefiniti e cercare i file modificati per l’ultima volta nelle ultime 2 ore, la settimana scorsa, il mese scorso o l’anno scorso.
* **Tag**: Puoi anche cercare i file a cui sono stati applicati tag specifici. Puoi digitare il tag o selezionarlo dall’elenco a discesa.

![Filtri per la visualizzazione archivio](assets/repo-filter-search.png)


## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

* L&#39;indice Lucene obsoleto viene utilizzato in /core/article-publish/src/main/java/com/adobe/dxml/article/publish/util/DoxUtils.java (9291)
* Node.js aggiornato non viene utilizzato per la pubblicazione. (9835)
* L&#39;argomento DITA non viene aggiornato automaticamente con le modifiche apportate al **Proprietà** pagina. (8745)
* L&#39;elemento Frontsubject aggiunto a una libreria DITA non funziona correttamente. (9507)
* PDF nativo | Viene generato un PDF vuoto utilizzando **Generazione rapida** per più file quando viene selezionato un elemento vuoto. (9822)
* PDF nativo | L&#39;appendice è pubblicata come capitolo nell&#39;output PDF. (9829)
* PDF nativo | Quando un’immagine di SVG viene modificata, non viene visualizzata aggiornata nel layout di pagina. (9069)
* Un carattere trattino normale viene inserito quando viene inserito un `Nonbreaking Hyphen` viene inserito utilizzando **Inserisci carattere speciale** finestra di dialogo. (8919)
* XML Editor non mostra le immagini aggiornate negli argomenti se sono state modificate. (9500)
* Durante la pubblicazione dell’output tramite l’editor, i predefiniti non possono essere eliminati dal **Uscita** scheda . (9100)
* Le mappe secondarie di una mappa DITA non vengono estratte utilizzando la **Seleziona tutto** dal menu dei puntini di sospensione. (9814)
* Impossibile trascinare la mappa o i modelli di argomento dal **Modelli** al modello di mappa personalizzato nell&#39;editor Web. (9846)
* Impossibile creare un nuovo argomento o un modello di mappa nella sottocartella di una mappa o di un modello di argomento. (9888)
* Non è presente alcuna opzione per sfogliare gli argomenti o le mappe presenti nelle sottocartelle di una mappa o di un modello di argomento. (9889)
* Quando un file Schematron viene aggiornato e salvato insieme al file DITA, il pannello di destra non viene visualizzato (se il file DITA interrompe le convalide presenti nel file Schematron). (9986)
* È possibile creare un nuovo predefinito di output duplicato se il nome è lo stesso di un predefinito esistente. (9997)
* Le immagini di SVG vengono danneggiate e non vengono pubblicate correttamente durante la generazione dell&#39;output di HTML. (9949)


## Problemi noti

Adobe ha identificato i seguenti problemi noti per la versione di AEM Guide as a Cloud Service nell’agosto 2022.

### Problemi noti con la soluzione alternativa

Utilizza la soluzione alternativa indicata per i seguenti problemi noti:

* La visualizzazione Layout non è visibile nell’Editor mappa.

   **Soluzione alternativa**: Aggiorna il file ui_config.json nel profilo della cartella.

* Il problema 8919 si verifica.

   **Soluzione alternativa**: L’aggiornamento di simboli.json deve essere unito a simboli.json con override.

### Altri problemi noti

* Se sono selezionati più file dalla sezione dei risultati visualizzata durante l&#39;esecuzione di una ricerca nell&#39;archivio e quindi trascinati nella visualizzazione dell&#39;autore, viene aggiunto solo un file singolo.
