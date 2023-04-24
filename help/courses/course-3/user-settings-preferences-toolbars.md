---
title: Preferenze utente, Impostazioni editor e Barre degli strumenti Editor
description: Modifica delle preferenze utente e delle impostazioni dell’editor in AEM Guide
exl-id: 8cb099e4-d985-4eeb-b1a5-0e372b04d218
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '1169'
ht-degree: 2%

---

# Preferenze utente, impostazioni editor e barre degli strumenti dell’editor

L’editor dispone di un’interfaccia altamente configurabile. La combinazione di Preferenze utente, Impostazioni editor e Profili cartelle consente di personalizzare quasi ogni aspetto del proprio ambiente di lavoro specifico.

>[!VIDEO](https://video.tv.adobe.com/v/342769?quality=12&learn=on)

## Mostrare o nascondere i tag degli elementi

I tag sono segnali visivi che indicano i limiti di un elemento. Un bordo dell’elemento indica l’inizio e la fine di un elemento. È quindi possibile utilizzare questi bordi come spunta visiva per posizionare il punto di inserimento o selezionare il testo all&#39;interno di un bordo.

1. Fai clic sul pulsante [!UICONTROL **Attiva/Disattiva visualizzazione tag**] sulla barra degli strumenti secondaria.

   ![Attiva/Disattiva tag](images/lesson-2/tags-on-icon.png)

   I tag vengono visualizzati all’interno dell’argomento. Con la Vista tag puoi effettuare le seguenti operazioni:

   - Seleziona il contenuto di un elemento facendo clic sul tag di apertura o chiusura.

   - Espandi o comprimi i tag facendo clic sul segno + o - nel tag .

   - Utilizza il menu di scelta rapida per tagliare, copiare o superare l’elemento selezionato.

   - Trascina gli elementi selezionando il tag e rilasciando l’elemento in una posizione valida.

1. Fai clic sul pulsante [!UICONTROL **Attiva/Disattiva visualizzazione tag**] per nascondere i tag.

I tag scompaiono e consentono di concentrarsi sul testo.

## Bloccare le risorse in uso

Il blocco (o il ritiro) di un file consente all’utente di accedere in scrittura al file. Quando il file viene sbloccato (o archiviato), le modifiche vengono salvate nella versione corrente del file.

1. Fai clic sul pulsante [!UICONTROL **Blocca**] sulla barra degli strumenti secondaria.

   ![Pagamento](images/lesson-2/checkout-icon.png)

   Il file è stato estratto e viene visualizzata un’icona Blocca accanto al nome del file nell’archivio.

1. Fai clic sul pulsante [!UICONTROL **Sblocca**] icona.

   ![Registra](images/lesson-2/check-in-icon.png)

Il Repository si aggiorna per mostrare che il file è stato archiviato.

## Inserisci caratteri speciali

1. Fai clic sul pulsante [!UICONTROL **Inserisci caratteri speciali**] sulla barra degli strumenti secondaria.

   ![Speciale](images/lesson-2/special-icon.png)

1. Nella finestra di dialogo Inserisci carattere speciale digitare il nome del carattere nella barra di ricerca.

   In alternativa, utilizza il menu a discesa Seleziona categoria per visualizzare tutti i caratteri in una categoria specifica.

1. Seleziona il carattere desiderato.

1. Fai clic su [!UICONTROL **Inserisci**].

Il carattere speciale è inserito nel testo.

## Passa dalle modalità Autore, Origine e Anteprima

La barra degli strumenti in alto a destra dello schermo consente di passare da una visualizzazione all’altra.

![Modalità](images/lesson-2/modes.png)

- Seleziona **Autore** per visualizzare la struttura e il contenuto mentre si lavora con un argomento.

- Seleziona **Origine** per visualizzare il codice XML sottostante che costituisce l&#39;argomento.

- Seleziona **Anteprima** per mostrare come verrà visualizzato un argomento quando un utente lo visualizza nel proprio browser.

## Modifica il tema con Preferenze utente

Puoi scegliere tra i temi chiari o scuri per l&#39;editor. Utilizzando il tema Luce, le barre degli strumenti e i pannelli utilizzano uno sfondo grigio chiaro. Utilizzando il tema Scuro, le barre degli strumenti e i pannelli utilizzano uno sfondo nero. In entrambi i temi, l’area di modifica dei contenuti viene visualizzata con uno sfondo bianco.

1. Fai clic sul pulsante [!UICONTROL **Preferenze utente**] nella barra degli strumenti superiore.

   ![Preferenze utente](images/reuse/user-prefs-icon.png)

1. Nella finestra di dialogo Preferenze utente, fai clic sul pulsante [!UICONTROL **Tema**] a discesa.

1. Scegli tra le opzioni disponibili.

   ![Temi](images/lesson-2/themes.png)

1. Fai clic su [!UICONTROL **Salva**].

L’editor viene aggiornato per visualizzare il tema desiderato.

## Aggiornare il percorso di base con le preferenze utente

È possibile aggiornare il percorso di base in modo che la visualizzazione archivio mostri il contenuto da una posizione specifica non appena si avvia l&#39;Editor. Questo riduce il tempo necessario per accedere ai file di lavoro.

1. Fai clic sul pulsante [!UICONTROL **Preferenze utente**] nella barra degli strumenti superiore.

   ![Preferenze utente](images/reuse/user-prefs-icon.png)

1. Nella finestra di dialogo Preferenze utente, fai clic sul pulsante [!UICONTROL **Cartella**] accanto al percorso di base.

   ![Percorso cartella di base](images/lesson-2/base-path-folder-icon.png)

1. Nella finestra di dialogo Seleziona percorso , fai clic sulla casella di controllo accanto a una cartella specifica.

1. Fai clic su [!UICONTROL **Seleziona**].

Al successivo avvio dell&#39;Editor, il Repository visualizzerà i file specificati nel Percorso di base.

## Assegnare un nuovo profilo cartella

Il profilo globale è un valore predefinito del sistema. Gli amministratori possono creare ulteriori profili cartella tra cui scegliere.

1. Fai clic sul pulsante [!UICONTROL **Preferenze utente**] nella barra degli strumenti superiore.

   ![Preferenze utente](images/reuse/user-prefs-icon.png)

1. Nella finestra di dialogo Preferenze utente, fai clic sul pulsante [!UICONTROL **Profili cartella**] a discesa.

   ![Elenco profili](images/lesson-2/folder-profiles-dropdown.png)

1. Scegli un profilo dalle opzioni disponibili.

1. Fai clic su [!UICONTROL **Salva**].

Ora viene assegnato il nuovo profilo cartella . Nel pannello a sinistra sono state modificate le opzioni della barra degli strumenti, le modalità di visualizzazione, le condizioni e gli snippet. Può anche modificare l’aspetto visivo del contenuto nell’editor.

## Modifica il dizionario con le impostazioni dell’editor

Le impostazioni dell’editor sono disponibili per gli utenti amministratori. Queste preferenze consentono di configurare una serie di impostazioni, una delle quali è il dizionario utilizzato dall’Editor per il controllo ortografia.

1. Fai clic sul pulsante [!UICONTROL **Impostazioni editor**] nella barra degli strumenti superiore.

   ![Impostazioni editor](images/lesson-2/editor-settings-icon.png)

1. Nella finestra di dialogo Impostazioni editor, fai clic sul pulsante [!UICONTROL **Generale**] scheda .

1. Selezionare il dizionario da utilizzare.

1. Fai clic su [!UICONTROL **Salva**].

Il dizionario viene aggiornato. Il passaggio a Controllo ortografia AEM consente di utilizzare un elenco di parole personalizzato.

## Mostrare e nascondere i pannelli con le impostazioni dell’editor

Una delle funzioni che è possibile personalizzare con Impostazioni editor è Panels. In particolare, è possibile selezionare i pannelli che vengono visualizzati o nascosti nell’Editor.

1. Fai clic sul pulsante [!UICONTROL **Impostazioni editor**] nella barra degli strumenti superiore.

   ![Impostazioni editor](images/lesson-2/editor-settings-icon.png)

1. Nella finestra di dialogo Impostazioni editor, fai clic sul pulsante [!UICONTROL **Pannelli**] scheda .

1. Passa i pannelli disponibili da Mostra o Nascondi come necessario.

   ![Attiva/disattiva pannello](images/lesson-2/toggle-panels.png)

1. Fai clic su [!UICONTROL **Salva**].

Il pannello a sinistra è ora configurato per mostrare solo i pannelli attivati come Mostra.

## Elementi di nome ed etichetta nelle impostazioni dell’editor

L’elenco Elementi ti consente di assegnare un nome a un elemento specifico e assegnargli un’etichetta più intuitiva. Il nome dell&#39;elemento deve essere uno degli elementi DITA. L&#39;etichetta può essere di qualsiasi stringa.

1. Fai clic sul pulsante [!UICONTROL **Impostazioni editor**] nella barra degli strumenti superiore.

   ![Impostazioni editor](images/lesson-2/editor-settings-icon.png)

1. Nella finestra di dialogo Impostazioni editor, fai clic sul pulsante [!UICONTROL **Elenco elementi**] scheda .

1. Digita un **Nome elemento** e **Etichetta** nei rispettivi campi.

1. Fai clic sul pulsante [!UICONTROL **Plus**] per aggiungere altri elementi all’elenco.

   ![Elenco elementi](images/lesson-2/elements-list.png)

1. Fai clic su [!UICONTROL **Salva**].

Puoi vedere immediatamente la modifica all’elenco Elementi nei tag esistenti nell’editor. Puoi visualizzarli anche nelle opzioni fornite quando aggiungi un nuovo elemento.

## Attributi di nome ed etichetta nelle impostazioni dell’editor

L’elenco Attributi funziona in modo simile all’elenco Elementi. Da Impostazioni editor, puoi controllare l’elenco degli attributi e i relativi nomi visualizzati.

1. Fai clic sul pulsante [!UICONTROL **Impostazioni editor**] nella barra degli strumenti superiore.

   ![Impostazioni editor](images/lesson-2/editor-settings-icon.png)

1. Nella finestra di dialogo Impostazioni editor, fai clic sul pulsante [!UICONTROL **Elenco attributi**] scheda .

1. Digita un **Nome attributo** e **Etichetta** nei rispettivi campi.

1. Fai clic sul pulsante [!UICONTROL **Plus**] per aggiungere altri attributi all’elenco.

## Configurare le condizioni in Impostazioni editor

La scheda Condizione consente di configurare diverse proprietà.

1. Fai clic sul pulsante [!UICONTROL **Impostazioni editor**] nella barra degli strumenti superiore.

   ![Impostazioni editor](images/lesson-2/editor-settings-icon.png)

1. Nella finestra di dialogo Impostazioni editor, fai clic sul pulsante [!UICONTROL **Condizione**] scheda .

1. Selezionare le caselle di controllo delle condizioni da applicare.

   ![Scheda Condizione](images/lesson-2/condition.png)

1. Fai clic su [!UICONTROL **Salva**].

## Creare un profilo di pubblicazione in Impostazioni editor

I profili di pubblicazione possono essere utilizzati per pubblicare la knowledge base. Ad esempio, Salesforce utilizza un’app configurata con una chiave del consumatore e un segreto del consumatore. Queste informazioni possono essere utilizzate per creare un profilo di pubblicazione Salesforce.

1. Fai clic sul pulsante [!UICONTROL **Impostazioni editor**] nella barra degli strumenti superiore.

   ![Impostazioni editor](images/lesson-2/editor-settings-icon.png)

1. Nella finestra di dialogo Impostazioni editor, fai clic sul pulsante [!UICONTROL **Profili**] scheda .

1. Fai clic sul pulsante [!UICONTROL **Plus**] accanto a Profili .

1. Compilare i campi come richiesto.

1. Fai clic su [!UICONTROL **Salva**].

È stato creato un profilo di pubblicazione.
