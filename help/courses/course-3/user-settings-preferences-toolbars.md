---
title: Preferenze utente, impostazioni editor e barre degli strumenti editor
description: Modifica delle preferenze utente e delle impostazioni dell’editor nelle guide AEM
exl-id: 8cb099e4-d985-4eeb-b1a5-0e372b04d218
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '1169'
ht-degree: 2%

---

# Preferenze utente, Impostazioni editor e Barre degli strumenti dell&#39;editor

L’editor dispone di un’interfaccia altamente configurabile. La combinazione di Preferenze utente, Impostazioni editor e Profili cartella consente di personalizzare quasi ogni aspetto dell’ambiente di lavoro specifico.

>[!VIDEO](https://video.tv.adobe.com/v/342769?quality=12&learn=on)

## Mostrare o nascondere i tag degli elementi

I tag sono segnali visivi che indicano i limiti di un elemento. Un limite di elemento contrassegna l&#39;inizio e la fine di un elemento. È quindi possibile utilizzare questi limiti come spunto visivo per posizionare il punto di inserimento o selezionare il testo all&#39;interno di un limite.

1. Fai clic su [!UICONTROL **Attiva/Disattiva visualizzazione tag**] sulla barra degli strumenti secondaria.

   ![Attiva/Disattiva tag](images/lesson-2/tags-on-icon.png)

   I tag vengono visualizzati all&#39;interno dell&#39;argomento. Con la visualizzazione Tag su puoi:

   - Seleziona il contenuto di un elemento facendo clic sul tag di apertura o chiusura.

   - Espandi o comprimi i tag facendo clic sul segno + o - nel tag.

   - Utilizza il menu di scelta rapida per tagliare, copiare o oltrepassare l’elemento selezionato.

   - Trascina e rilascia gli elementi selezionando il tag e rilasciando l’elemento in una posizione valida.

1. Fai clic su [!UICONTROL **Attiva/Disattiva visualizzazione tag**] per nascondere i tag.

I tag scompaiono consentendo di concentrarsi sul testo.

## Blocca le risorse quando in uso

Il blocco (o l&#39;estrazione) di un file consente all&#39;utente l&#39;accesso in scrittura esclusivo sul file. Quando il file viene sbloccato (o archiviato), le modifiche vengono salvate nella versione corrente del file.

1. Fai clic su [!UICONTROL **Blocca**] sulla barra degli strumenti secondaria.

   ![Pagamento](images/lesson-2/checkout-icon.png)

   Il file è stato estratto e accanto al nome del file nel repository viene visualizzata un&#39;icona Blocca.

1. Fai clic su [!UICONTROL **Sblocca**] icona.

   ![Registra](images/lesson-2/check-in-icon.png)

L’archivio viene aggiornato per mostrare che il file è stato archiviato.

## Inserisci caratteri speciali

1. Fai clic su [!UICONTROL **Inserisci caratteri speciali**] sulla barra degli strumenti secondaria.

   ![Speciale](images/lesson-2/special-icon.png)

1. Nella finestra di dialogo Inserisci carattere speciale digitare il nome del carattere nella barra di ricerca.

   In alternativa, utilizza il menu a discesa Seleziona categoria per visualizzare tutti i caratteri in una categoria specifica.

1. Seleziona il carattere desiderato.

1. Clic [!UICONTROL **Inserisci**].

Il carattere speciale viene inserito nel testo.

## Passa dalla modalità Autore alla modalità Origine e Anteprima

La barra degli strumenti in alto a destra dello schermo consente di passare da una visualizzazione all’altra.

![Modalità](images/lesson-2/modes.png)

- Seleziona **Autore** per visualizzare la struttura e il contenuto mentre si lavora con un argomento.

- Seleziona **Sorgente** per visualizzare il codice XML sottostante che costituisce l&#39;argomento.

- Seleziona **Anteprima** per mostrare come verrà visualizzato un argomento quando viene visualizzato da un utente nel browser.

## Modificare il tema con Preferenze utente

Puoi scegliere tra i temi Chiaro o Scuro per l’editor. Utilizzando il tema Luce, le barre degli strumenti e i pannelli utilizzano uno sfondo grigio chiaro. Utilizzando il tema Scuro, le barre degli strumenti e i pannelli utilizzano uno sfondo nero. In entrambi i temi, l&#39;area di modifica dei contenuti viene visualizzata con uno sfondo bianco.

1. Fai clic su [!UICONTROL **Preferenze utente**] nella barra degli strumenti superiore.

   ![Preferenze utente](images/reuse/user-prefs-icon.png)

1. Nella finestra di dialogo Preferenze utente, fai clic su [!UICONTROL **Tema**] a discesa.

1. Scegli tra le opzioni disponibili.

   ![Temi](images/lesson-2/themes.png)

1. Fai clic su [!UICONTROL **Salva**].

L’editor viene aggiornato per visualizzare il tema preferito.

## Aggiornare il percorso di base con le preferenze utente

È possibile aggiornare il Percorso base in modo che la Vista archivio mostri il contenuto da una posizione specifica non appena si avvia l’Editor. Questo riduce il tempo necessario per accedere ai file di lavoro.

1. Fai clic su [!UICONTROL **Preferenze utente**] nella barra degli strumenti superiore.

   ![Preferenze utente](images/reuse/user-prefs-icon.png)

1. Nella finestra di dialogo Preferenze utente, fai clic su [!UICONTROL **Cartella**] accanto al Percorso base.

   ![Percorso cartella base](images/lesson-2/base-path-folder-icon.png)

1. Nella finestra di dialogo Seleziona percorso, fai clic sulla casella di controllo accanto a una cartella specifica.

1. Clic [!UICONTROL **Seleziona**].

Al successivo avvio dell&#39;editor, nel repository verranno visualizzati i file specificati nel Percorso base.

## Assegna un nuovo profilo cartella

Il Profilo globale è un&#39;impostazione predefinita del sistema. Gli amministratori possono creare ulteriori profili cartella tra cui scegliere.

1. Fai clic su [!UICONTROL **Preferenze utente**] nella barra degli strumenti superiore.

   ![Preferenze utente](images/reuse/user-prefs-icon.png)

1. Nella finestra di dialogo Preferenze utente, fai clic su [!UICONTROL **Profili cartella**] a discesa.

   ![Elenco profili](images/lesson-2/folder-profiles-dropdown.png)

1. Scegli un profilo tra le opzioni disponibili.

1. Fai clic su [!UICONTROL **Salva**].

Il nuovo Profilo cartella è ora assegnato. Sono state modificate le opzioni della barra degli strumenti, le modalità di visualizzazione e Condizioni e snippet nel pannello a sinistra. Può anche modificare l’aspetto visivo del contenuto nell’Editor.

## Modificare il dizionario con le impostazioni dell&#39;editor

Le impostazioni dell&#39;editor sono disponibili per gli utenti amministratori. Queste preferenze consentono di configurare una serie di impostazioni, tra cui il dizionario utilizzato dall&#39;editor per il controllo ortografico.

1. Fai clic su [!UICONTROL **Impostazioni editor**] nella barra degli strumenti superiore.

   ![Impostazioni editor](images/lesson-2/editor-settings-icon.png)

1. Nella finestra di dialogo Impostazioni editor, fai clic su [!UICONTROL **Generale**] scheda.

1. Selezionare il dizionario che si desidera utilizzare.

1. Fai clic su [!UICONTROL **Salva**].

Il dizionario viene aggiornato. Il passaggio al controllo ortografico dell’AEM consente di utilizzare un elenco di parole personalizzato.

## Mostrare e nascondere i pannelli con le impostazioni dell’editor

Una delle funzioni personalizzabili con Impostazioni editor è Pannelli. In particolare, puoi selezionare quali pannelli visualizzare o nascondere nell’Editor.

1. Fai clic su [!UICONTROL **Impostazioni editor**] nella barra degli strumenti superiore.

   ![Impostazioni editor](images/lesson-2/editor-settings-icon.png)

1. Nella finestra di dialogo Impostazioni editor, fai clic su [!UICONTROL **Pannelli**] scheda.

1. Attiva Mostra o Nascondi i pannelli disponibili in base alle esigenze.

   ![Attiva/Disattiva pannello](images/lesson-2/toggle-panels.png)

1. Fai clic su [!UICONTROL **Salva**].

Il pannello sinistro è ora configurato per mostrare solo i pannelli attivati Mostra.

## Elementi nome ed etichetta nelle impostazioni dell’editor

L’elenco Elementi consente di denominare un elemento specifico e assegnargli un’etichetta più semplice da usare. Il nome elemento deve essere uno degli elementi DITA. L’etichetta può essere qualsiasi stringa.

1. Fai clic su [!UICONTROL **Impostazioni editor**] nella barra degli strumenti superiore.

   ![Impostazioni editor](images/lesson-2/editor-settings-icon.png)

1. Nella finestra di dialogo Impostazioni editor, fai clic su [!UICONTROL **Elenco elementi**] scheda.

1. Digita un **Nome elemento** e un **Etichetta** nei rispettivi campi.

1. Fai clic su [!UICONTROL **Più**] per aggiungere altri elementi all’elenco.

   ![Elenco elementi](images/lesson-2/elements-list.png)

1. Fai clic su [!UICONTROL **Salva**].

Puoi vedere immediatamente la modifica all’Elenco elementi nei tag esistenti nell’Editor. Puoi anche visualizzarli nelle opzioni fornite quando aggiungi un nuovo elemento.

## Attributi di nome ed etichetta nelle impostazioni dell’editor

L&#39;elenco Attributi funziona in modo simile all&#39;elenco Elementi. In Impostazioni editor è possibile controllare l&#39;elenco degli attributi e i relativi nomi visualizzati.

1. Fai clic su [!UICONTROL **Impostazioni editor**] nella barra degli strumenti superiore.

   ![Impostazioni editor](images/lesson-2/editor-settings-icon.png)

1. Nella finestra di dialogo Impostazioni editor, fai clic su [!UICONTROL **Lista Attributi**] scheda.

1. Digita un **Nome attributo** e un **Etichetta** nei rispettivi campi.

1. Fai clic su [!UICONTROL **Più**] per aggiungere altri attributi all&#39;elenco.

## Configurare le condizioni nelle impostazioni dell’editor

La scheda Condizione consente di configurare diverse proprietà.

1. Fai clic su [!UICONTROL **Impostazioni editor**] nella barra degli strumenti superiore.

   ![Impostazioni editor](images/lesson-2/editor-settings-icon.png)

1. Nella finestra di dialogo Impostazioni editor, fai clic su [!UICONTROL **Condizione**] scheda.

1. Selezionare le caselle di controllo delle condizioni da applicare.

   ![Scheda Condizione](images/lesson-2/condition.png)

1. Fai clic su [!UICONTROL **Salva**].

## Creare un profilo di pubblicazione nelle impostazioni dell’editor

I profili di pubblicazione possono essere utilizzati per pubblicare la knowledge base. Ad esempio, Salesforce utilizza un’app configurata con una chiave consumer e un segreto consumer. Queste informazioni possono essere utilizzate per creare un profilo di pubblicazione Salesforce.

1. Fai clic su [!UICONTROL **Impostazioni editor**] nella barra degli strumenti superiore.

   ![Impostazioni editor](images/lesson-2/editor-settings-icon.png)

1. Nella finestra di dialogo Impostazioni editor, fai clic su [!UICONTROL **Profili**] scheda.

1. Fai clic su [!UICONTROL **Più**] accanto a Profili.

1. Compila i campi come richiesto.

1. Fai clic su [!UICONTROL **Salva**].

È stato creato un profilo di pubblicazione.
