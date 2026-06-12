---
title: Controllo ortografico e ricerca/sostituzione
description: Utilizzo del controllo ortografico e della funzione Trova/Sostituisci in AEM Guides
exl-id: 5f39618d-a919-4d3c-a4de-2896f2d1bf20
TQID: https://experienceleague.adobe.com/cSdhulSc30KrwsGh1ldB2yn-8eSLccHBpyD-0S1x1M0
product_v2:
  - id: fae5e35a-80c9-4b94-9352-1a060a6aab1d
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 27ffc636d63300fb2e99903d92cab12f0cfcbb25
workflow-type: tm+mt
source-wordcount: 443
ht-degree: 0%

---

# Controllo ortografico e ricerca/sostituzione

L’editor di AEM Guides dispone di potenti funzionalità di controllo ortografico e di Trova e sostituisci.

>[!VIDEO](https://video.tv.adobe.com/v/342768?quality=12&learn=on)

Correggere un errore ortografico

1. Individua un errore in un argomento aperto, mostrato con una sottolineatura rossa.

1. Tenere premuto Ctrl + fare clic sul pulsante secondario del mouse all&#39;interno della parola.

1. Scegli l’ortografia corretta tra i suggerimenti.

Se non viene suggerita l&#39;ortografia corretta, è sempre possibile modificare manualmente la parola.

## Passa a controllo ortografia AEM

È possibile utilizzare uno strumento di controllo ortografico diverso dal dizionario predefinito del browser.

1. Passa a **Impostazioni editor**.

1. Selezionare la scheda Impostazioni **Generali**.

   ![Configurazione controllo ortografico](images/lesson-11/configure-dictionary.png)

1. Sono disponibili due opzioni:

   - **Controllo ortografia browser**: impostazione predefinita in cui il controllo ortografico utilizza il dizionario incorporato del browser.

   - **Controllo ortografico AEM**. Utilizzarlo per creare un elenco di parole personalizzato utilizzando il dizionario personalizzato di AEM.

1. Scegli **Controllo ortografia AEM**.

1. Fai clic su [!UICONTROL **Salva**].

Configurare un dizionario personalizzato

L&#39;amministratore può modificare le impostazioni in modo che il dizionario AEM riconosca parole personalizzate, ad esempio i nomi delle società.

1. Passa al riquadro **Strumenti**.

1. Accedi a **CRXDE Lite**.

   ![Icona CRXDE Lite dell&#39;interfaccia utente di AEM](images/lesson-11/crxde-lite.png)

1. Passare al nodo **_/apps/fmdita/config_**.

   ![Nodo di configurazione CRXDE Lite](images/lesson-11/config-node.png)

1. Crea un nuovo file.

   a. Fai clic con il pulsante destro del mouse sulla cartella di configurazione.

   b. Scegliere **Crea > Crea file**.

   ![Creazione di un nuovo file del dizionario](images/lesson-11/new-dictionary-file.png)

   c. Denomina il file _&#x200B;**user_dictionary.txt**&#x200B;_.

   ![Testo dizionario utente](images/lesson-11/user-dictionary.png)

   d. Fai clic su [!UICONTROL **OK**].

1. Apri il file.

1. Aggiungere un elenco di parole da includere nel dizionario personalizzato.

1. Fare clic su [!UICONTROL **Salva tutto**].

1. Chiudete il file.

Per ottenere l&#39;elenco di parole personalizzato aggiornato nel dizionario AEM, potrebbe essere necessario riavviare la sessione dell&#39;editor Web.

## Trova e sostituisci in un singolo file

1. Fai clic sull’icona Trova e sostituisci nella barra degli strumenti superiore.

   ![Trova icona Sostituisci](images/lesson-11/find-replace-icon.png)

1. Nella barra degli strumenti inferiore digitare una parola o una frase.

1. Fare clic su [!UICONTROL **Trova**].

1. Se necessario, digitare una parola per sostituire la parola trovata.

1. Fare clic su [!UICONTROL **Sostituisci**].

## Trova e sostituisci nell’archivio

1. Passare all&#39;**archivio**.

1. Fai clic sull&#39;icona [!UICONTROL **Trova e sostituisci**] in basso a sinistra nella schermata.

1. Fai clic sull&#39;icona [!UICONTROL **Mostra impostazioni**].

1. Scegli una delle seguenti opzioni

   - **Estrai il file prima di sostituirlo**. Se attivato da un amministratore, il file verrà estratto automaticamente prima di sostituire i termini di ricerca.

   - **Solo parola intera** — limita la ricerca in modo che restituisca solo la parola o la frase esatta immessa.

   ![Trova sostituto nell&#39;archivio](images/lesson-11/repository-find-replace.png)

1. Fai clic sull&#39;icona [!UICONTROL **Applica filtro**] per selezionare il percorso nell&#39;archivio in cui desideri eseguire la ricerca.

1. Inserire i termini da trovare e sostituire.

1. Se necessario, selezionare **Crea nuova versione dopo la sostituzione**.

1. Fare clic su [!UICONTROL **Trova**].

1. Apri il file desiderato e utilizza le frecce per passare da un risultato trovato all’altro.

   ![Trova Interfaccia Sostituisci Navigazione](images/lesson-11/find-replace-navigation.png)
