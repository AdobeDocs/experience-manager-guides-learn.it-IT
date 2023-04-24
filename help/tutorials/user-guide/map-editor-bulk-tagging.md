---
title: Assegnazione di tag in blocco al contenuto DITA
description: Scopri come assegnare tag in blocco al contenuto DITA
source-git-commit: 528dd5d33f38c29809e7e7dafd77d860daaba8db
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---


# Assegnazione di tag in blocco al contenuto DITA {#id179SG0TN05Z}

I tag consentono di raggruppare o classificare il contenuto all’interno dell’archivio dei contenuti e anche nell’output pubblicato. Se sul contenuto sono stati applicati tag, è possibile trovare facilmente argomenti correlati all’interno di una mappa DITA che possono essere utili per la creazione di contenuto. Con l’output pubblicato, gli utenti finali saranno in grado di individuare più rapidamente il contenuto corretto con i tag appropriati.

AEM Guide consente di assegnare tag al contenuto DITA in pochi clic. È possibile utilizzare la funzione di assegnazione tag in blocco per applicare più tag su più argomenti, su una mappa DITA o su una mappa secondaria. Oppure, puoi anche applicare tag a un singolo argomento. L’assegnazione tag è la funzione nativa di AEM. Ulteriori informazioni sulla creazione e la gestione dei tag sono disponibili nella sezione [Amministrazione dei tag](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/sites/authoring/features/tags.html?lang=en) nella documentazione AEM.

Per impostazione predefinita, AEM Guide non consente l’accesso in lettura a nessun utente della cartella in cui sono archiviati tutti i tag nell’archivio AEM. Per utilizzare i tag definiti nell&#39;archivio AEM, è necessario chiedere all&#39;amministratore di sistema di concedere l&#39;accesso alla cartella in cui sono memorizzati i tag.

## Applicare tag in blocco

Utilizza la funzione di assegnazione tag in blocco per applicare più tag contemporaneamente. Esegui i seguenti passaggi per applicare tag agli argomenti in una mappa DITA:

1. Nell’interfaccia utente Assets, individua e fai clic sul file di mappa DITA.

   Viene visualizzata la console mappa DITA che mostra l’elenco dei predefiniti di output disponibili per generare l’output.

1. Fai clic su **Argomenti**.

   Viene visualizzato un elenco di argomenti disponibili nella mappa DITA. Gli UUID degli argomenti’ sono visualizzati sotto il titolo dell’argomento.

1. Seleziona gli argomenti o la mappa secondaria a cui applicare i tag.

   ![](images/apply-tags-uuid.png)


   >[!NOTE]
   >
   > La schermata precedente mostra una mappa secondaria selezionata ed espansa. Quando si seleziona la mappa secondaria, vengono selezionati anche tutti gli argomenti della mappa secondaria.

1. Fai clic su **Applica tag**.

   Viene visualizzata la finestra di dialogo Seleziona tag .

1. Seleziona uno o più tag da applicare agli argomenti selezionati.

1. Conferma la selezione.

   I tag selezionati vengono applicati agli argomenti e visualizzati accanto al titolo dell’argomento.

   >[!NOTE]
   >
   > Dopo aver aggiunto i tag agli argomenti, se si sposta o si elimina un argomento, vengono rimossi anche i tag di tali argomenti. Tuttavia, tale argomento rimane nella mappa fino a quando non viene rimosso.


## Applicare tag a un singolo argomento

Per applicare i tag a un singolo argomento, effettua le seguenti operazioni:

1. Nell’interfaccia utente Assets, individua e seleziona il file dell’argomento a cui applicare i tag.

1. Nella barra degli strumenti, fai clic su **Proprietà**.

   Viene visualizzata la pagina delle proprietà dell&#39;argomento.

1. Nella scheda Base, fai clic sull’icona Sfoglia accanto alla **Tag** campo .

1. Seleziona uno o più tag da applicare all’argomento selezionato.

1. Conferma la selezione.

1. Fai clic su **Applica tag**.

   I tag selezionati vengono applicati all’argomento e visualizzati nel campo Tag .

1. Fai clic su **Salva e chiudi**.


## Rimuovi tag

In base alle esigenze aziendali, è possibile modificare le informazioni sui tag per qualsiasi argomento DITA. È possibile rimuovere facilmente tutti i tag contemporaneamente o rimuovere solo i tag non validi nell’argomento.

Esegui i seguenti passaggi per rimuovere tutti i tag da uno o più argomenti:

1. Nell’interfaccia utente Assets, individua e fai clic sul file di mappa DITA.

   Viene visualizzata la console mappa DITA che mostra l’elenco dei predefiniti di output disponibili per generare l’output.

1. Fai clic su **Argomenti**.

   Viene visualizzato un elenco di argomenti disponibili nella mappa DITA.

1. Selezionare gli argomenti da cui si desidera rimuovere i tag.

1. Fai clic su **Rimuovi tag**.

   >[!NOTE]
   >
   > Se l’icona Elimina tag non è visibile, accertati di non aver attivato la funzione Nascondi tag .

1. Nella finestra di dialogo Conferma eliminazione, fai clic su **OK** per rimuovere i tag dagli argomenti selezionati.


## Mostrare o nascondere i tag

Se hai un lungo elenco di tag applicati ai tuoi argomenti, allora potresti trovarti un po&#39; complicato navigare. Per nascondere facilmente i tag nella vista della console mappa DITA, fai clic sull’icona Nascondi tag . Allo stesso modo, quando i tag non sono visibili, facendo clic su Mostra tag vengono visualizzati tutti i tag.

**Argomento principale:**[ Gestire i metadati](manage-metadata.md)

