---
title: Modificare gli argomenti nell'editor Web
description: Scopri come modificare gli argomenti nell’editor Web
source-git-commit: cc0fbca257d82cc82db5b5da8d263309fd71de55
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---


# Modificare gli argomenti nell&#39;editor Web {#id2056B040VUI}

L’editor web include una serie di funzioni di modifica che consentono di creare o modificare facilmente i file degli argomenti. In linea generale, per modificare un argomento nell&#39;editor Web è necessario eseguire i seguenti passaggi.

>[!IMPORTANT]
>
> Se si verifica un errore dell&#39;applicazione durante l&#39;utilizzo dell&#39;editor Web, aggiornare la pagina per continuare a funzionare.

1. Per apportare modifiche all’argomento, fai clic all’interno del bordo del testo dell’elemento richiesto e inizia a apportare modifiche.

1. Per inserire un elemento specifico, fai clic su alla fine dell’elemento dopo il quale desideri inserire il nuovo elemento e fai clic sull’icona dell’elemento richiesta nella barra degli strumenti. È inoltre possibile utilizzare le scelte rapide da tastiera `Alt+Enter` per invocare **Inserisci elemento** popup.

   Viene visualizzato un elenco di elementi che possono essere utilizzati nell’argomento. AEM Guide effettua un posizionamento intelligente degli elementi in base alla loro posizione valida nell’argomento.

   >[!NOTE]
   >
   > Puoi anche scegliere quale icona visualizzare nella barra degli strumenti configurando la `ui_config.json` file situato a - `/etc/designs/fmdita/clientlibs/xmleditor/`. Per ulteriori informazioni sulla personalizzazione delle funzioni, contattare l’amministratore di sistema.

1. Una volta completata la modifica del documento, fai clic su **Salva**.

   >[!NOTE]
   >
   > Se non desideri eseguire il commit delle modifiche AEM archivio, fai clic su **Chiudi**, quindi fai clic su **Chiudi senza salvataggio** nella finestra di dialogo Modifiche non salvate .

   **Aggiorna il browser durante la modifica dei file**
AEM Guide fornisce il supporto per aggiornare il browser durante la modifica del contenuto nell’editor Web. Questa funzione consente di continuare a modificare il contenuto in caso di errore dell’applicazione durante il lavoro. Se premi l’aggiornamento del browser quando si aprono per la modifica uno o più file con modifiche non salvate, ti viene comunicato che le modifiche non salvate potrebbero andare perse. Puoi annullare l’operazione di aggiornamento e salvare i file per mantenere le modifiche.

   Anche quando si aggiorna il browser, le visualizzazioni del pannello di sinistra e di destra vengono mantenute nell’Editor web. Ad esempio, l’argomento attivo nel pannello Archivio viene riaperto. Il pannello mappa viene mantenuto insieme alla mappa precedentemente aperta.

   L’argomento attivo o la mappa DITA viene riaperta nell’area di modifica del contenuto.

   Anche il pannello di destra viene riaperto e visualizza la stessa visualizzazione di prima dell’aggiornamento.

   **Indicatore della copia di lavoro**
AEM Guide fornisce l&#39;indicatore della copia di lavoro che mostra se l&#39;attuale \(copia di lavoro\) del file è sincronizzato o meno con la versione salvata. Se hai apportato delle modifiche alla copia corrente e non hai salvato il file, compare un segno \* insieme al titolo nella scheda del file dell’argomento. Questo indicatore funge da promemoria per salvare le modifiche e scompare quando salvi il file.

   ![](images/working-copy-text-update-indicator.png){width="550" align="left"}

   AEM Guide indica anche se l&#39;ultima copia salvata \(working\) del file è sincronizzata o meno con la versione salvata. Se sono presenti alcune modifiche non salvate tra la copia di lavoro e l’ultima versione salvata, viene visualizzato un segno \* insieme alle informazioni sulla versione visualizzate nell’angolo superiore destro della scheda file dell’argomento. Questo indicatore funge da promemoria per salvare e creare una versione dalla copia corrente \(working\) del file.

   ![](images/version-update-indicator.png){width="550" align="left"}


**Argomento principale:**[ Utilizzare l’editor Web](web-editor.md)

