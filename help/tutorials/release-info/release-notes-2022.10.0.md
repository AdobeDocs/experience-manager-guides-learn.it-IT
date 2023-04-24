---
title: Note sulla versione | Guide Adobe Experience Manager as a Cloud Service, ottobre 2022
description: Rilascio di ottobre delle guide di Adobe Experience Manager as a Cloud Service
exl-id: 38638080-625c-49c3-9e54-56cc23831546
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 4%

---

# Rilascio di ottobre delle guide di Adobe Experience Manager as a Cloud Service

## Aggiornamento alla versione di ottobre

Aggiorna le guide correnti di Adobe Experience Manager as a Cloud Service (in seguito denominate *Guide AEM as a Cloud Service*) eseguendo le seguenti operazioni:
1. Controlla il codice Git dei Cloud Services e passa al ramo configurato nella pipeline dei Cloud Services corrispondente all’ambiente da aggiornare.
1. Aggiorna `<dox.version>` proprietà in `/dox/dox.installer/pom.xml` file dei tuoi Cloud Services Codice Git a 2022.10.183.
1. Conferma le modifiche ed esegui la pipeline dei Cloud Services per eseguire l’aggiornamento alla versione di ottobre di AEM Guide as a Cloud Service.

## Matrice di compatibilità

In questa sezione viene elencata la matrice di compatibilità per le applicazioni software supportate AEM Guide as a Cloud Service versione di ottobre 2022.

### FrameMaker e FrameMaker Publishing Server

| FMPS | FrameMaker |
| --- | --- |
| Non compatibile | Aggiornamento 4 e superiore del 2020 |
|  |  |

*La linea di base e le condizioni create in AEM sono supportate nelle versioni FMPS a partire dal 2020.2.

### Connettore dell&#39;ossigeno

| AEM guide as a Cloud Release | Finestre del connettore dell&#39;ossigeno | Mac connettore ossigeno | Modifica in Windows Ossigeno | Modifica in Oxygen Mac |
| --- | --- | --- | --- | --- |
| 2022.10.0 | 2.7.13 | 2.7.13 | 2.3 | 2.3 |
|  |  |  |  |


## Nuove funzioni e miglioramenti

AEM Guide as a Cloud Service fornisce miglioramenti e nuove funzioni nella versione di ottobre:


### Pannello Quick Generate

Ora AEM Guide fornisce **Generazione rapida** pannello che consente di generare e visualizzare rapidamente l’output dei predefiniti creati per la mappa DITA.

![Icona Genera rapida](assets/quick-generate-icon.png)

In **Generazione rapida** è possibile visualizzare l&#39;elenco di tutti i predefiniti di output creati per la mappa DITA.

![Pannello Quick Generate](assets/quick-generate-panel.png)

Seleziona uno o più predefiniti e genera rapidamente l’output. Puoi anche visualizzare rapidamente l’output generato per i predefiniti. Viene visualizzato un messaggio di successo sulla generazione dell&#39;output. Viene visualizzato un messaggio di errore se la generazione dell’output non riesce. Puoi anche visualizzare il registro degli errori per visualizzare i dettagli dell’errore che si è verificato nel processo di generazione.


## Problemi risolti

I bug corretti in varie aree sono elencati di seguito:

* PDF nativo | Si verifica un errore nella rimozione degli argomenti relativi solo alle risorse dall’output di PDF. (10554)
* PDF nativo | Nell&#39;output di PDF vengono visualizzati i Keyrefs vuoti. (10553)
* PDF nativo | `navtitle` per `topichead` non è onorato. (10509)
* PDF nativo | Supporto necessario per amd64 sapori JDK. (10465)
* PDF nativo | Impossibile nascondere gli argomenti relativi alla questione anteriore dal sommario. (10355)
* PDF nativo | Il riavvio del numero di pagina nel layout del capitolo avvia in modo casuale la numerazione dalla fine del capitolo precedente. (10154)
* Browser Chrome | Lo schermo viene lasciato vuoto quando si trascina e rilascia qualsiasi elemento dall’interfaccia utente. Ad esempio, quando trascini una condizione dal pannello Condizioni. (10524)
* Le proprietà del nodo vengono rimosse dopo l’operazione di copia e incolla di una risorsa. (10053)
* Al clic  **Chiudi** gli utenti venivano reindirizzati alle risorse : l’esperienza è stata corretta per indirizzare gli utenti alla home page di AEM. (9654)
