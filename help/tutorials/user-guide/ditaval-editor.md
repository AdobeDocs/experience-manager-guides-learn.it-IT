---
title: Usa editor DIAVAL
description: Scopri come utilizzare l’editor DITAVAL
source-git-commit: 7cd719921e68ac1763d09d9665d912e3697e5849
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---


# Editor DITAVAL {#id17C5E0U0OQE}

I file DITAVAL vengono utilizzati per generare l’output condizionale. In un singolo argomento, puoi aggiungere condizioni utilizzando gli attributi degli elementi per condizionalizzare il contenuto. Quindi, crei un file DITAVAL in cui specifichi le condizioni da prendere per generare contenuto e quale condizione deve essere esclusa dall’output finale.

AEM Guide consente di creare e modificare facilmente i file DIAVAL utilizzando l’editor DITAVAL. L&#39;editor DITAVAL recupera gli attributi \(o tags\) definiti nel tuo sistema ed è possibile usarli per creare o modificare file DITAVAL. Per ulteriori dettagli sulla creazione e la gestione dei tag in AEM, consulta [Amministrazione dei tag](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/sites/authoring/features/tags.html?lang=en) nella documentazione AEM.

## Crea file DIAVAL

Esegui i seguenti passaggi per creare un file DITAVAL:

1. Nell’interfaccia utente Assets, individua il percorso in cui desideri creare il file DITAVAL.

1. Fai clic su **Crea** \> **Argomento DITA**.

1. Nella pagina Blueprint, seleziona il modello di file DITAVAL e fai clic su **Successivo**.

1. Nella pagina Proprietà , specifica l’ **Titolo** e **Nome** per il file DITAVAL.

   >[!NOTE]
   >
   > Il nome viene suggerito automaticamente in base al Titolo del file. Se si desidera specificare manualmente il nome del file, assicurarsi che il Nome non contenga spazi, apostrofo o parentesi graffe e termini con .ditaval.

1. Fai clic su **Crea**. Viene visualizzato il messaggio Argomento creato.

   È possibile scegliere di aprire il file DITAVAL per la modifica nell&#39;editor DITAVAL o salvare il file argomento nell&#39;archivio AEM.


## Modifica file DIAVAL

Esegui i seguenti passaggi per modificare un file DITAVAL:

1. Nell’interfaccia utente Assets, individua il file DIAVAL da modificare.

1. Per bloccare il file in modo esclusivo, selezionarlo e fare clic su **Estrai**.

1. Seleziona il file e fai clic su **Modifica** per aprire il file nell’editor AEM Guide DIAVAL.

   L&#39;editor DITAVAL ti consente di eseguire le seguenti attività:

   R: Attiva/Disattiva pannello a sinistra : Attiva/disattiva la visualizzazione del pannello a sinistra. Se il file DITAVAL è stato aperto tramite la mappa DITA, la mappa e il repository sono visualizzati in questo pannello. Per ulteriori informazioni sull&#39;apertura di un file tramite mappa DITA, vedere [Modifica argomenti tramite mappa DITA](map-editor-advanced-map-editor.md#id17ACJ0F0FHS).

   B: Salva : Salva le modifiche apportate nel file. Tutte le modifiche vengono salvate nella versione corrente del file.

   C: Aggiungi proprietà : Aggiungi una singola proprietà nel file DITAVAL.

       ![](images/ditaval-editor-props.png)
       
       Il primo elenco a discesa elenca gli attributi DITA consentiti che è possibile utilizzare nel file DITAVAL. Sono supportati cinque attributi: `audience`, `platform`, `product`, `props` e `otherprops`.
   
   : Il secondo elenco a discesa mostra i valori configurati per l&#39;attributo selezionato. Quindi, l’elenco a discesa successivo mostra le azioni che puoi configurare sull’attributo selezionato. I valori consentiti nel menu a discesa delle azioni sono: `include`, `exclude`, `passthrough`e `flag`. Per ulteriori informazioni su questi valori, consulta la definizione di [prop](http://docs.oasis-open.org/dita/dita/v1.3/errata01/os/complete/part3-all-inclusive/langRef/ditaval/ditaval-prop.html#ditaval-prop) elemento nella documentazione DITA OASIS

   D: Aggiungi tutte le proprietà : Se desideri aggiungere con un solo clic tutte le proprietà o gli attributi condizionali definiti nel sistema, utilizza la funzione Aggiungi tutte le proprietà .

>[!NOTE]
>
> Se nel file DITAVAL sono già presenti tutte le proprietà condizionali definite, non è possibile aggiungere altre proprietà. Viene visualizzato un messaggio di errore in questo scenario.

    ![](images/ditaval-all-props.png)

1. Una volta completata la modifica del file DITAVAL, fai clic su **Salva**.

   >[!NOTE]
   >
   > Se chiudi il file senza salvarlo, le modifiche andranno perse. Se non desideri eseguire il commit delle modifiche AEM archivio, fai clic su **Chiudi**, quindi fai clic su **Chiudi senza salvataggio** in **Modifiche non salvate** finestra di dialogo.


## Visualizzazioni dell&#39;editor DITAVAL

L&#39;editor DITAVAL di AEM Guide supporta la visualizzazione di file DITAVAL in due modalità o viste diverse:

Autore : Questa è una tipica visualizzazione What You Get \(WYSISYG\) dell&#39;editor DITAVAL. È possibile aggiungere o rimuovere proprietà utilizzando la semplice interfaccia utente, che presenta le proprietà, i valori e le azioni nell’elenco a discesa. Nella visualizzazione Autore sono disponibili le opzioni per inserire una singola proprietà e inserire tutte le proprietà con un solo clic.

: Puoi anche trovare la versione del file DITAVAL su cui stai lavorando passando il puntatore del mouse sul nome del file.

Origine : Nella visualizzazione Origine viene visualizzato il codice XML sottostante che costituisce il file DITAVAL. Oltre a apportare modifiche regolari al testo in questa visualizzazione, un autore può anche aggiungere o modificare proprietà utilizzando lo Smart Catalog.

    Per richiamare il Catalogo avanzato, posiziona il cursore alla fine di qualsiasi definizione di proprietà e immetti &quot;&lt;&quot;. L&#39;editor mostrerà un elenco di tutti gli elementi XML validi che è possibile inserire in tale posizione.
    
    ![](images/ditaval-source-view.png)

