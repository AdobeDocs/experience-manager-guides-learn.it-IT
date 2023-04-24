---
title: Traduci argomenti modificati
description: Scopri come tradurre gli argomenti modificati
source-git-commit: 7cd719921e68ac1763d09d9665d912e3697e5849
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# Traduci argomenti modificati {#id16A5A0B6072}

Se apporti modifiche ad alcuni argomenti, questi richiedono una nuova traduzione. È possibile tenere traccia degli argomenti modificati dalla mappa DITA. Dalla cartella copia lingua di origine, fare clic sul file mappa DITA e fare clic sulla scheda Traduzione. Puoi visualizzare lo stato di ogni argomento, sia che esso richieda o meno una nuova traduzione.

Esegui i seguenti passaggi per inviare un argomento modificato per la ritraduzione:

1. Fare clic sul file di mappa DITA dalla cartella di copia della lingua di origine.

1. Fai clic sul pulsante **Traduzione** scheda .

1. In **Filtro** a sinistra, seleziona il **Traduci lingue** per controllare lo stato e fare clic su **Fine**.

   Puoi visualizzare lo stato di traduzione di ogni argomento. Gli argomenti che presentano un’altra revisione dell’argomento disponibile rispetto a quello inviato per la traduzione, mostrano un **Obsoleto** stato.

   >[!NOTE]
   >
   > Il flusso di lavoro di traduzione confronta l’ultima revisione salvata del file argomento nella cartella della lingua di origine con la versione tradotta.

   Se fai clic sulla freccia per visualizzare ulteriori dettagli. puoi vedere la copia in lingua particolare non aggiornata.

   ![](images/out-of-sync-uuid.png)

1. Fai clic sulla casella di controllo per selezionare gli argomenti da inviare per la riconversione.

   Quando selezioni una data non sincronizzata, la **Creare/aggiornare copie per lingua** nel pannello Riferimenti e nella **Ignora stato di sincronizzazione non disponibile** sopra il pulsante **Filtro** icona.

   È possibile utilizzare **Disattivare la sincronizzazione fuori sincronia** pulsante per ignorare lo stato Out of Date per gli argomenti nella mappa DITA. Ad esempio, se hai apportato alcune modifiche nella versione inglese dell’argomento che non richiedono la traduzione, puoi utilizzare questo pulsante e modificare lo stato Non aggiornato per l’argomento selezionato.

   >[!NOTE]
   >
   > Se fai clic sul pulsante **Ignora stato di sincronizzazione non disponibile** imposta lo stato dell&#39;argomento su Up to Date per gli argomenti non aggiornati selezionati.

1. Fai clic su **Aggiorna copie per lingua** e configura il processo di traduzione.

1. Puoi scegliere di creare un nuovo progetto di traduzione o di aggiungere argomenti a un progetto di traduzione esistente. Fornisci i dettagli richiesti per configurare il progetto di traduzione.

1. Fai clic su **Inizio**.

   Viene visualizzato un messaggio di conferma che indica che l’argomento è stato inviato per la traduzione.

1. Passa al progetto di traduzione nella console Progetto . Nella cartella viene creata una nuova scheda del processo di traduzione. Fai clic sui puntini di sospensione per visualizzare le risorse della cartella.

   ![](images/incremental-job.PNG)

1. Per avviare la traduzione, fare clic sulla freccia sulla scheda del processo di traduzione e selezionare **Inizio** dall&#39;elenco. Un messaggio notifica che il processo è iniziato.

   Puoi anche visualizzare lo stato dell’argomento tradotto quando fai clic sull’ellissi nella parte inferiore della scheda del lavoro di traduzione.

   >[!NOTE]
   >
   > Se utilizzi il servizio di traduzione umana, devi esportare il contenuto per la traduzione. Una volta che hai tradotto il contenuto, devi importarlo nuovamente nel progetto di traduzione.

1. Al termine della traduzione, lo stato cambia in **Pronto per la revisione**. Fai clic sull’ellissi per visualizzare i dettagli dell’argomento ed effettua una delle seguenti operazioni dalla barra degli strumenti:

   - Fai clic su **Mostra in Assets** per vedere e verificare la traduzione.

   - Fai clic su **Accetta traduzione** se ritieni che le modifiche siano state tradotte correttamente. Viene visualizzato un messaggio di conferma.

   - Fai clic su **Rifiuta traduzione** se pensi che il lavoro debba essere rifatto. Viene visualizzato un messaggio di rifiuto.
   >[!NOTE]
   >
   > È importante accettare o rifiutare la risorsa tradotta, altrimenti il file rimane nella posizione temporanea e non viene copiato in DAM.

1. Torna al file di mappa DITA nella cartella della lingua di origine nell’interfaccia utente Assets. Gli argomenti tradotti sono ora sincronizzati.


**Argomento principale:**[ Tradurre il contenuto](translation.md)

