---
title: Note sulla versione | Guide Adobe Experience Manager as a Cloud Service, versione di aprile 2022
description: Rilascio di aprile delle guide di Adobe Experience Manager as a Cloud Service
exl-id: c735ba24-a803-454b-8723-57dacf90061b
source-git-commit: b5e64512956f0a7f33c2021bc431d69239f2a088
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 3%

---

# Rilascio di aprile delle guide di Adobe Experience Manager as a Cloud Service

## Aggiornamento alla versione di aprile

Aggiorna il tuo [!DNL Adobe Experience Manager Guides] as a Cloud Service (successivamente indicato come *[!DNL AEM Guides]as a Cloud Service*) eseguendo le seguenti operazioni:
1. Controlla il codice Git dei Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
2. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file dei tuoi Cloud Services Codice Git a 2022.4.133.
3. Conferma le modifiche ed esegui la pipeline dei Cloud Services per eseguire l’aggiornamento alla versione di aprile di [!DNL AEM Guides] as a Cloud Service.

## Matrice di compatibilità

In questa sezione viene elencata la matrice di compatibilità per le applicazioni software supportate da [!DNL AEM Guides] Versione as a Cloud Service di aprile 2022.

### FrameMaker e FrameMaker Publishing Server

| FMPS | FrameMaker |
| --- | --- |
| Non compatibile | Aggiornamento 4 e superiore del 2020 |
|  |  |


### Connettore dell&#39;ossigeno

| Versione di AEM Guide Cloud | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno |
| --- | --- | --- |
| 2022.4.0 | 2.5.6 | 2.5.6 |
|  |  |  |

*La linea di base e le condizioni create in AEM sono supportate nelle versioni FMPS a partire dal 2020.2.

## Nuove funzioni e miglioramenti

Sono stati aggiunti molti miglioramenti e nuove funzioni nell’editor web:

### Risoluzione dei tasti migliorata

Un riferimento a una chiave di contenuto DITA inserisce una parte di contenuto da un argomento all’altro. Utilizza una chiave per individuare il contenuto. È necessario risolvere i riferimenti chiave associati a un argomento DITA. La mappa radice selezionata ha la precedenza più alta per risolvere i riferimenti chiave.

![finestra di dialogo delle preferenze utente](assets/user-preferences.png)

Ora i riferimenti chiave vengono risolti in base alla mappa radice impostata nel seguente ordine di priorità:

1. Preferenze utente
2. Pannello Vista mappa
3. Profilo cartella

Per ulteriori dettagli, consulta *Risolvere i riferimenti chiave* nella guida utente.

### Aggiungi un pannello personalizzato nel pannello a sinistra

Ora è possibile aggiungere un pannello personalizzato nel pannello di sinistra dell’Editor Web. Puoi utilizzare un pannello personalizzato per vari scopi, ad esempio per fornire aiuto o eseguire i test per un progetto. Se è stato configurato un pannello personalizzato, questo viene visualizzato anche nell’elenco dei pannelli all’interno della **Impostazioni editor**. Puoi attivare o disattivare l’opzione per visualizzare o nascondere il pannello personalizzato.

### Possibilità di modificare lo stato del documento degli argomenti in una mappa DITA

Ora è possibile modificare facilmente lo stato del documento degli argomenti selezionati all&#39;interno di una mappa DITA. È inoltre possibile aprire e modificare le proprietà degli argomenti selezionati in una mappa DITA dalla **Altre opzioni** nella parte inferiore del pannello Visualizza mappa.

![proprietà argomento selezionate](assets/map-view-properties.png)

### Informazioni sulla versione visualizzate in modalità Anteprima

L’editor Web consente di gestire le versioni. Ora è anche possibile visualizzare la versione dell&#39;argomento attivo o la mappa DITA nell&#39;angolo in alto a destra della scheda file dell&#39;argomento in modalità Anteprima di un argomento.

![versione di anteprima](assets/preview-version.png)

## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

* Le nuove etichette non vengono riportate automaticamente nel menu a discesa Aggiungi/Rimuovi etichetta, ma è necessario aggiornare la linea di base. (9249)
* Impossibile modificare il titolo della linea di base se una linea di base viene creata da criteri di etichetta. (9171)
* Se lo stato della linea di base diventa &quot;non riuscito&quot;, il processo di pubblicazione che utilizza una linea di base si blocca in stato di &quot;attesa&quot;. (9194)
* La rimozione delle etichette sui riferimenti diretti rimuove anche le etichette dai riferimenti indiretti. (9257)
* La ricerca durante la digitazione causa richieste di ricerca indesiderate nella vista Archivio. (9307)
* Si verificano problemi quando una parola chiave viene utilizzata nel titolo della scheda . (9318)
* La linea di base non riesce quando si aggiunge un&#39;etichetta con spazi. (9362)
* AEM&#39;output del sito non visualizza correttamente l&#39;elemento glossusage. (8936)
* Errore della console all&#39;apertura **Uscita** nell&#39;editor Web. (8715)
* Il messaggio di errore visualizzato durante la pubblicazione di un tipo di record manuale tramite Salesforce non è intuitivo. (8952)
* L’impostazione Convalida con attributi di condizione non viene aperta immediatamente, ma l’utente deve riaprire il file per visualizzare le convalide. (9300)
* I metadati non possono essere rimossi una volta pubblicata una mappa DITA con metadati.  (9178)
* Il pannello di traduzione è visibile anche all’apertura della mappa DITA nell’Editor mappa. (9053)
* La DTD personalizzata definita dall&#39;utente non ha la precedenza rispetto alla DTD DITA standard incorporata in DITA-OT. (9104)
* Nella funzione PDF nativa, il caricamento nei modelli non riesce per i file non DITA e non-image. (9070)
* Il meccanismo di autorizzazione esegue due query invece di una, in alcuni scenari specializzati. (9221)
* La pubblicazione dell&#39;output del sito AEM non riesce quando si utilizza la DTD personalizzata. (9243)
* La nota a piè di pagina utilizzata per riferimento non scorre fino alla sezione a piè di pagina nell&#39;output AEM sito. (9234)

## Problemi noti

L&#39;Adobe ha identificato il seguente problema noto nel [!DNL AEM Guides] Versione as a Cloud Service di aprile.

* L&#39;editor Web non segnala un errore quando due o più linee di base vengono create con lo stesso nome ma con differenze di spazio o di maiuscole/minuscole. Ad esempio, &quot;adobe&quot; e &quot;Adobe &quot; o &quot;Adobe&quot;.
* Il connettore dell&#39;ossigeno si blocca in modo intermittente durante l&#39;esecuzione di login o logout frequenti o il passaggio tra diversi tipi di autenticazione.
