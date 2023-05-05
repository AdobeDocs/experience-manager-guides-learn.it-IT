---
title: Creare un progetto DITA
description: Scopri come creare un progetto DITA
exl-id: 6dc88ac4-249a-4da2-9787-a58370e281ca
source-git-commit: 8823669fd29e8a40a41f9ca5d654b38fbea8e2fa
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# Creare un progetto DITA {#id1645HA00NM6}

AEM Guide fornisce un modello di progetto DITA che è possibile utilizzare per creare e gestire le attività di revisione.

È possibile creare un progetto DITA e quindi utilizzarlo per avviare le revisioni. Un progetto consente di definire una scadenza e di controllare le attività e i tempi necessari per completare l’attività di revisione per la quale è stato creato il progetto.

Puoi aggiungere membri del team a un progetto a cui possono quindi essere assegnati vari ruoli: Autori, Revisori e Editori.

Dopo aver creato il progetto DITA, è possibile avviare la revisione dall’Editor Web o dall’interfaccia utente Assets. Per ulteriori dettagli, consulta [Invia argomenti per la revisione](review-send-topics-for-review.md#).

Allo stesso modo, ogni volta che un autore avvia un flusso di lavoro di revisione, i membri selezionati del progetto ricevono una notifica e-mail. Per configurare le notifiche e-mail, vedi *Personalizzare i modelli e-mail* in Installare e configurare le guide di Adobe Experience Manager as a Cloud Service.

Esegui i seguenti passaggi per creare un progetto DITA:

1. Apri la console Progetti .

   Puoi anche accedere alla console Progetti utilizzando il seguente URL:

   ```http
   http://<server name>:<port>/projects.html
   ```

1. Fai clic su **Crea** \> **Progetto** per avviare la procedura guidata Crea progetto.

   ![](images/project-console-63.png){width="650" align="left"}

1. Nella pagina Crea progetto , seleziona la **Progetto DITA** modello e fai clic su **Successivo**.

1. Nella pagina Proprietà progetto , immetti i seguenti dettagli:

   Informazioni nella **Base** scheda:

   ![](images/create-project.png){width="650" align="left"}

   - Inserisci il **Titolo**, **Descrizione** e **Data di scadenza**.

   - Facoltativamente, puoi scegliere una miniatura per il progetto.

   - Per impostazione predefinita, sei il proprietario del progetto. Per aggiungere altri utenti a questo progetto:
   1. Inserisci o scegli un utente dalla **Utente** elenco a discesa.

   1. Scegli un tipo di utente: Autori, Revisori o Editori.

      >[!NOTE]
      >
      >Verranno visualizzati altri tipi di utenti in questo elenco a discesa, ma per un progetto DITA è consigliabile scegliere solo tra Autori, Revisori o Editori. Anche se si aggiunge un utente di un tipo diverso, tale utente non sarà in grado di accedere ad alcuna funzionalità specifica DITA disponibile nelle Guide AEM.

   1. Fai clic su **Aggiungi**.

      >[!NOTE]
      >
      >Se si utilizza AEM Guide versione 3.5 o precedente, viene visualizzata un&#39;opzione per selezionare un file di mappa DITA per risolvere i riferimenti chiave per i flussi di lavoro di modifica, anteprima e revisione degli argomenti. Nelle versioni 3.6 e successive, è possibile impostare la mappa principale tramite l&#39;editor Web. Per ulteriori informazioni, consulta la sezione [Preferenze utente](web-editor-features.md#id2087G0P40SB) nell&#39;editor Web. Un altro modo per impostare la mappa principale consiste nel configurarla nei profili globali o a livello di cartella. Per ulteriori dettagli, consulta *Configurare profili globali o a livello di cartella* nella Guida all&#39;installazione e alla configurazione.
   Informazioni nella **Avanzate** scheda:

   - Inserisci un nome per il progetto. Questo nome viene utilizzato per creare l&#39;URL per il progetto.



1. Fai clic su **Crea**.

   Viene visualizzata la finestra di dialogo Crea progetto .

1. Fai clic su **Apri** per aprire la pagina del progetto.


**Argomento principale:**[ Esamina argomenti o mappe](review.md)
