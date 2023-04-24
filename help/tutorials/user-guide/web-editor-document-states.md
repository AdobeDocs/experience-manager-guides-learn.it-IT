---
title: Stato del documento
description: Scopri come documentare lo stato
source-git-commit: 13106cd1c7f6d38fecb67dd93eef66263eb29bae
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---


# Stato del documento {#id1821HC00URO}

Per gestire la preparazione dei documenti, in AEM Guide è disponibile una proprietà dello stato del documento che indica lo stato corrente del documento. Gli stati del documento consentono di verificare rapidamente se un documento è nuovo, in fase di revisione o di revisione dello stato completato.

## Tipi di stati del documento

Un documento può avere uno qualsiasi degli stati del documento definiti nel profilo Stato documento. Ad esempio, un documento può avere uno dei seguenti stati del documento:

- Bozza - Indica che il documento viene creato e salvato con nuove modifiche.
- In-Review - Indica che è stato avviato un flusso di lavoro di revisione per il documento.
- Rivisto - Indica che il documento è stato rivisto dagli utenti a cui è destinato.

Questi stati vengono impostati manualmente o automaticamente in base alle impostazioni del profilo Stati documento. Ad esempio, se il profilo Stato documento è configurato con stato iniziale come Bozza e lo stato In-Review è definito per i documenti in esame. Quindi, quando si crea un documento, lo stato del documento viene impostato su *Bozza*. Se si avvia un&#39;attività di revisione, lo stato del documento viene modificato in In-Review.

È inoltre possibile modificare manualmente lo stato del documento per uno o più documenti. Tuttavia, se si sceglie di modificare lo stato del documento per più documenti, lo stato consentito è determinato dagli stati comuni consentiti per i documenti selezionati. Ad esempio, supponiamo che gli stati del documento siano stati definiti come Bozza, In-Review, Rivisto e Pronto per la pubblicazione, nello stesso ordine. In document one.dita lo stato è impostato su *Bozza* e sul documento due.dita, lo stato è impostato su Reviewed. Quando si selezionano entrambi—one.dita e two.dita, lo stato del documento consentito sarà *Pronto per la pubblicazione*. Poiché two.dita è in *Rivisto* stato, lo stato successivo possibile per due.dita è solo *Pronto per la pubblicazione*, che viene visualizzato quando si selezionano entrambi i documenti.

>[!NOTE]
>
> Un documento può esistere in un solo stato alla volta.

## Cambia stato del documento

Per modificare lo stato di un documento, eseguire le operazioni seguenti:

1. Nell’interfaccia utente Assets, seleziona uno o più documenti per i quali vuoi modificare lo stato del documento.
1. Nella barra degli strumenti principale, fai clic su **Proprietà**.
1. Seleziona il nuovo stato dal **Stato del documento** a discesa. È possibile selezionare solo gli stati del documento consentiti nella sezione Transizione stato del profilo Stato documento.

   >[!NOTE]
   >
   >Gli amministratori possono visualizzare tutti gli stati del documento e modificare il documento in qualsiasi stato possibile.

1. Fai clic su **Salva e chiudi**.

## Visualizza stato documento

La vista a schede dell’interfaccia utente Assets mostra lo stato corrente insieme alla data di creazione e alle dimensioni del rispettivo argomento DITA o mappa DITA.

![](images/document_state.png){width="800" align="left"}

## Usa stati del documento in DLC

Gli stati dei documenti svolgono un ruolo importante nella gestione del ciclo di vita dei documenti in DLC. Se la tua organizzazione rispetta rigorosamente il DLC, diventa essenziale disporre di un meccanismo per controllare la modifica dei documenti in base al loro stato. Ad esempio, è possibile modificare i documenti quando si trovano in *Bozza* o *In-review* stati. Tuttavia, una volta che un documento è rivisto e pronto per la pubblicazione, dovrebbe esserci un modo per impedire ulteriori modifiche dei documenti.

AEM Guide fornisce un flusso di lavoro di approvazione dei documenti che consente di controllare il ciclo di vita del processo di sviluppo dei documenti. Quando un documento è pronto per la pubblicazione o ha raggiunto il penultimo stato, è possibile contrassegnarlo come approvato. Una volta approvato un documento, AEM Guide crea una nuova versione del documento e lo rende di sola lettura. È quindi possibile spostare il documento per la pubblicazione o creare una baseline per un&#39;ulteriore elaborazione.

Per avviare una nuova versione dai documenti contrassegnati come approvati, un autore deve avviare una nuova versione. Quando si avvia una nuova versione, lo stato del documento viene modificato in *Bozza* di nuovo. Modificando lo stato del documento in *Bozza*, il documento viene nuovamente reso modificabile e puoi continuare a lavorare alla versione successiva.

Per utilizzare la funzione di approvazione del documento, eseguire le operazioni seguenti:

>[!NOTE]
>
> La funzionalità del flusso di lavoro di approvazione deve essere abilitata dall’amministratore. Per ulteriori dettagli, consulta *Abilita flusso di lavoro di approvazione* in Installazione e configurazione delle guide Adobe Experience Manager as a Cloud Service.

1. Nell&#39;editor Web aprire il documento da contrassegnare per l&#39;approvazione.

1. Fai clic sul pulsante **Contrassegna approvato**![](images/mark_approve_icon.svg) icona.

1. Se il documento è nello stato da contrassegnare come approvato, viene visualizzata la seguente finestra di dialogo:

   ![](images/mark-approved-correct-state.png){width="550" align="left"}

   Se il documento non può essere contrassegnato come approvato, viene visualizzato il seguente messaggio:

   ![](images/mark-approved-incorrect-state.png){width="550" align="left"}

1. Se il documento è pronto per essere contrassegnato come approvato, seleziona un’etichetta dall’elenco a discesa e fai clic su **Approva**.

   >[!NOTE]
   >
   > Se l’amministratore non ha configurato un elenco predefinito di etichette, viene visualizzato un campo di testo a forma libera per immettere un’etichetta.

1. Una volta che il documento è stato contrassegnato correttamente come approvato, un **Anteprima** del documento viene visualizzato in modalità di sola lettura.

   ![](images/approved-doc-read-only.png){width="650" align="left"}

   >[!NOTE]
   >
   > Nella modalità Anteprima tutte le opzioni di modifica vengono rimosse dalla barra degli strumenti. Inoltre, la visualizzazione Autore e Origine del documento è stata rimossa anche dalla navigazione superiore.


Una volta che un documento viene contrassegnato come approvato, non è più disponibile per la modifica. Se desideri utilizzare il documento per la versione successiva, devi riportarlo alla pagina *Bozza* stato. Per modificare lo stato del documento di un documento approvato in *Bozza* , esegui i seguenti passaggi:

1. In un documento approvato, fai clic sul pulsante **Avvia una nuova versione** Icona ![](images/approved-restart-draft-mode-icon.svg).

   Viene visualizzato il messaggio Avvia nuova versione .

1. Fai clic su **Conferma**.

   Lo stato del documento viene modificato in Bozza e il documento viene aperto nell&#39;Editor Web in modalità di modifica.


**Argomento principale:**[ Utilizzare l’editor Web](web-editor.md)

