---
title: Controllo ortografico e ricerca/sostituzione
description: Utilizzo del controllo ortografico e ricerca/sostituzione nelle guide AEM
exl-id: 5f39618d-a919-4d3c-a4de-2896f2d1bf20
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Controllo ortografico e ricerca/sostituzione

L’editor di guide dell’AEM dispone di potenti funzionalità di controllo ortografico e di Trova e sostituisci.

>[!VIDEO](https://video.tv.adobe.com/v/342768?quality=12&learn=on)

Correggere un errore ortografico

1. Individua un errore in un argomento aperto, mostrato con una sottolineatura rossa.

1. Tenere premuto Ctrl + fare clic sul pulsante secondario del mouse all&#39;interno della parola.

1. Scegli l’ortografia corretta tra i suggerimenti.

Se non viene suggerita l&#39;ortografia corretta, è sempre possibile modificare manualmente la parola.

## Passa al controllo ortografico AEM

È possibile utilizzare uno strumento di controllo ortografico diverso dal dizionario predefinito del browser.

1. Accedi a **Impostazioni editor**.

1. Seleziona la **Generale** impostazioni.

   ![Configurazione controllo ortografia](images/lesson-11/configure-dictionary.png)

1. Sono disponibili due opzioni:

   - **Controllo ortografia browser** — l&#39;impostazione predefinita in cui il controllo ortografico utilizza il dizionario incorporato del browser.

   - **Controllo ortografia AEM** — utilizzare questa proprietà per creare un elenco di parole personalizzato utilizzando il dizionario personalizzato AEM.

1. Scegli **Controllo ortografia AEM**.

1. Fai clic su [!UICONTROL **Salva**].

Configurare un dizionario personalizzato

L&#39;amministratore può modificare le impostazioni in modo che il dizionario AEM riconosca parole personalizzate come i nomi delle società.

1. Accedi a **Strumenti** riquadro.

1. Accedi a **CRXDE Lite**.

   ![Icona CRXDE Lite dell’interfaccia utente AEM](images/lesson-11/crxde-lite.png)

1. Accedi a **_/apps/fmdita/config nodo_**.

   ![Nodo configurazione CRXDE Lite](images/lesson-11/config-node.png)

1. Crea un nuovo file.

   a. Fai clic con il pulsante destro del mouse sulla cartella di configurazione.

   b. Scegli **Crea > Crea file**.

   ![Creazione di un nuovo file del dizionario](images/lesson-11/new-dictionary-file.png)

   c. Denomina il file _**user_dictionary.txt**_.

   ![Testo dizionario utente](images/lesson-11/user-dictionary.png)

   d. Fai clic su [!UICONTROL **OK**].

1. Apri il file.

1. Aggiungere un elenco di parole da includere nel dizionario personalizzato.

1. Clic [!UICONTROL **Salva tutto**].

1. Chiudete il file.

Per ottenere l&#39;elenco di parole personalizzato aggiornato nel dizionario AEM, potrebbe essere necessario riavviare la sessione dell&#39;editor Web.

## Trova e sostituisci in un singolo file

1. Fai clic sull’icona Trova e sostituisci nella barra degli strumenti superiore.

   ![Icona Trova Sostituisci](images/lesson-11/find-replace-icon.png)

1. Nella barra degli strumenti inferiore digitare una parola o una frase.

1. Clic [!UICONTROL **Trova**].

1. Se necessario, digitare una parola per sostituire la parola trovata.

1. Clic [!UICONTROL **Sostituisci**].

## Trova e sostituisci nell’archivio

1. Accedi a **Archivio**.

1. Fai clic su [!UICONTROL **Trova e sostituisci**] in basso a sinistra.

1. Fai clic su [!UICONTROL **Mostra impostazioni**] icona.

1. Scegli una delle seguenti opzioni

   - **Estrai il file prima della sostituzione** — se attivato da un amministratore, il file viene estratto automaticamente prima della sostituzione dei termini di ricerca.

   - **Solo parola intera** — limita la ricerca in modo che restituisca solo la parola o la frase esatta immessa.

   ![Trova sostituisci nel repository](images/lesson-11/repository-find-replace.png)

1. Fai clic su [!UICONTROL **Applica filtro**] per selezionare il percorso nel repository in cui eseguire la ricerca.

1. Inserire i termini da trovare e sostituire.

1. Se necessario, seleziona **Crea nuova versione dopo la sostituzione**.

1. Clic [!UICONTROL **Trova**].

1. Apri il file desiderato e utilizza le frecce per passare da un risultato trovato all’altro.

   ![Interfaccia utente di navigazione di Sostituisci](images/lesson-11/find-replace-navigation.png)
