---
title: Controllo ortografia e ricerca/sostituzione
description: Utilizzo del controllo ortografico e ricerca/sostituzione nelle guide AEM
exl-id: 5f39618d-a919-4d3c-a4de-2896f2d1bf20
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Controllo ortografico e ricerca/sostituzione

L’Editor AEM Guide dispone di potenti funzionalità di controllo ortografico e Trova e Sostituisci .

>[!VIDEO](https://video.tv.adobe.com/v/342768?quality=12&learn=on)

Correggere un errore di ortografia

1. Individua un errore in un argomento aperto, mostrato con una sottolineatura rossa.

1. Premi e tieni premuto Ctrl + clic sul pulsante secondario del mouse all’interno della parola.

1. Scegli l’ortografia corretta dai suggerimenti.

Se non viene suggerita l’ortografia corretta, è sempre possibile modificarla manualmente.

## Passa al controllo ortografia AEM

È possibile utilizzare uno strumento di controllo ortografico diverso dal dizionario predefinito del browser.

1. Passa a **Impostazioni editor**.

1. Seleziona la **Generale** scheda impostazioni.

   ![Configurazione controllo ortografia](images/lesson-11/configure-dictionary.png)

1. Sono disponibili due opzioni:

   - **Controllo ortografia del browser** — l&#39;impostazione predefinita in cui il controllo ortografia utilizza il dizionario incorporato del browser.

   - **Controllo ortografia AEM** — utilizza questo per creare un elenco di parole personalizzato utilizzando AEM dizionario personalizzato.

1. Scegli **Controllo ortografia AEM**.

1. Fai clic su [!UICONTROL **Salva**].

Configurare un dizionario personalizzato

L’amministratore può modificare le impostazioni in modo che il dizionario AEM riconosca parole personalizzate come i nomi aziendali.

1. Passa a **Strumenti** riquadro.

1. Accedi a **CRXDE Lite**.

   ![Icona CRXDE Lite dell’interfaccia AEM](images/lesson-11/crxde-lite.png)

1. Passa a **_/apps/fmdita/config node_**.

   ![Nodo di configurazione di CRXDE Lite](images/lesson-11/config-node.png)

1. Crea un nuovo file.

   a) Fai clic con il pulsante destro del mouse sulla cartella di configurazione.

   b) Scegli **Crea > Crea file**.

   ![Creazione di nuovi file dizionario](images/lesson-11/new-dictionary-file.png)

   c. Denominare il file _**user_Dictionary.txt**_.

   ![Testo del dizionario utente](images/lesson-11/user-dictionary.png)

   d. Fai clic su [!UICONTROL **OK**].

1. Apri il file .

1. Aggiungi un elenco di parole da includere nel dizionario personalizzato.

1. Fai clic su [!UICONTROL **Salva tutto**].

1. Chiudi il file.

Per ottenere l&#39;elenco di parole personalizzate aggiornato nel dizionario AEM, potrebbe essere necessario riavviare la sessione dell&#39;editor Web.

## Trova e sostituisci in un singolo file

1. Fare clic sull’icona Trova e sostituisci nella barra degli strumenti superiore.

   ![Trova icona Sostituisci](images/lesson-11/find-replace-icon.png)

1. Nella barra degli strumenti inferiore, digitare una parola o una frase.

1. Fai clic su [!UICONTROL **Trova**].

1. Se necessario, digitare una parola per sostituire la parola trovata.

1. Fai clic su [!UICONTROL **Sostituisci**].

## Trova e sostituisci nell’archivio

1. Passa a **Archivio**.

1. Fai clic sul pulsante [!UICONTROL **Trova e sostituisci**] in basso a sinistra dello schermo.

1. Fai clic sul pulsante [!UICONTROL **Mostra impostazioni**] icona.

1. Scegli una

   - **File di estrazione prima della sostituzione** — se abilitato da un amministratore, il file viene estratto automaticamente prima di sostituire i termini di ricerca.

   - **Solo parola intera** — limita la ricerca a restituire solo la parola o la frase esatta inserita.

   ![Trova sostituisci nel repository](images/lesson-11/repository-find-replace.png)

1. Fai clic sul pulsante [!UICONTROL **Applica filtro**] per selezionare il percorso nel repository in cui si desidera eseguire la ricerca.

1. Inserire i termini Trova e sostituisci.

1. Se necessario, seleziona **Crea nuova versione dopo la sostituzione**.

1. Fai clic su [!UICONTROL **Trova**].

1. Apri il file desiderato e utilizza le frecce per passare da un risultato trovato all’altro.

   ![Trova/sostituisci interfaccia di navigazione](images/lesson-11/find-replace-navigation.png)
