---
title: profilazione degli attributi condizionali
description: Scopri come eseguire il profiling dell’attributo condizionale
source-git-commit: 7cd719921e68ac1763d09d9665d912e3697e5849
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---


# profilazione degli attributi condizionali {#id1843I0HN0Y4}

A livello aziendale, è estremamente importante assicurarsi di disporre di un sistema di assegnazione tag standard. I tag o gli attributi condizionali possono essere associati alle risorse digitali nell’archivio, il che aiuta a pubblicare l’output in base alle condizioni scelte. Ad esempio, puoi creare un attributo condizionale per contenuti Windows e Mac. Quindi, aggiungi questi attributi al contenuto pertinente nei tuoi argomenti. Al momento della pubblicazione del contenuto, puoi scegliere se pubblicare solo il contenuto di Windows o Mac.

AEM Guide consente di creare e associare facilmente gli attributi condizionali utilizzando gli attributi DITA pertinenti. Puoi definire gli attributi condizionali a livello globale o a livello di cartella. Le condizioni definite a livello globale sono visibili in tutti i progetti e le condizioni specifiche delle cartelle sono visibili solo nei progetti creati all’interno della cartella specificata. Gli autori di contenuti possono utilizzare questi attributi condizionali per condizionare il contenuto dei loro argomenti o mappe DITA creati o utilizzati. Queste condizioni possono quindi essere utilizzate dall’editore per creare predefiniti condizionali. Utilizzando i predefiniti condizionali, l’editore può decidere quale condizione includere ed escludere dall’output pubblicato.

>[!NOTE]
>
> Puoi creare o modificare gli attributi condizionali in un profilo cartella a cui hai accesso. Se l’amministratore di sistema non ti ha concesso l’accesso a un profilo di cartella, non puoi creare o modificare gli attributi condizionali nel profilo cartella.

Per definire gli attributi condizionali, effettua le seguenti operazioni:

1. Fai clic sul collegamento Adobe Experience Manager in alto e scegli **Strumenti**.

1. Seleziona **Guide** dall&#39;elenco degli strumenti.

1. Fai clic sul pulsante **Profili cartella** e seleziona un profilo cartella.

   >[!NOTE]
   >
   > Non puoi modificare il profilo globale.

1. Fai clic sul pulsante **Attributi condizionali** e fai clic su **Modifica**.

   Viene visualizzata la tabella Attributi condizionali .

1. Fai clic su **Aggiungi**.

1. Inserisci il **Nome**, **Valore** e **Etichetta** per l&#39;attributo .

   Puoi salvare un profilo con solo il nome dell’attributo. Tuttavia, un attributo può essere utilizzato solo quando gli è stato specificato un valore. Se si specificano sia il valore che l&#39;etichetta per un attributo, nell&#39;Editor Web verrà comunque visualizzato solo il valore dell&#39;attributo. L’etichetta viene mostrata all’amministratore di pubblicazione al momento della creazione del predefinito condizionale.

   La schermata seguente mostra la definizione per `platform` attributo con valore di `unix` e un&#39;etichetta `Red Hat Linux`.

   ![](images/add-profile.png)

1. Se desideri aggiungere più valori per lo stesso attributo, fai clic sul pulsante **+** e immetti valore e etichetta aggiuntivi.

1. Per aggiungere altri attributi, fai clic su **Aggiungi**.

1. Fai clic su **Salva** per salvare le modifiche.


La `platform` l&#39;attributo è memorizzato nel sistema. Ogni volta che un autore decide di utilizzare il `platform` in un argomento DITA in una cartella, i valori verranno visualizzati nella scheda Proprietà nell&#39;editor Web.

![](images/properties-tab.png)

**Argomento principale:**[ Generazione di output](generate-output.md)

