---
title: Visualizza lo stato dell'attività di generazione dell'output
description: Scopri come visualizzare lo stato dell’attività di generazione dell’output
source-git-commit: 7cd719921e68ac1763d09d9665d912e3697e5849
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---


# Visualizza lo stato dell&#39;attività di generazione dell&#39;output {#viewing_output_history}

Dopo aver avviato l&#39;attività di generazione dell&#39;output per un documento FrameMaker, AEM Guide invia questa attività alla coda di generazione dell&#39;output. Questa coda viene aggiornata in tempo reale, mostrando lo stato di ogni attività di generazione dell&#39;output nella coda.

Esegui i seguenti passaggi per visualizzare la coda di generazione dell’output:

1. Nell&#39;interfaccia utente Assets, passare al documento FrameMaker di cui si desidera controllare lo stato di generazione dell&#39;output e fare clic su di esso.

1. Fare clic su Output.

   ![](images/output-queued-fm.png)

1. La pagina Output è divisa in due parti:

   - **Uscite in coda:**

      Elenca gli output in attesa di generazione o in fase di generazione. È inoltre possibile trovare l&#39;impostazione di generazione dell&#39;output o il predefinito utilizzato per l&#39;attività in coda, il tipo, l&#39;utente che ha avviato l&#39;attività, l&#39;ora dal momento in cui l&#39;attività viene messa in coda e lo stato corrente.

   - **Uscite generate**

      Elenca le attività di output completate. Anche in questo caso, le informazioni visualizzate in questo documento sono simili alla sezione Uscite in coda, con l&#39;unica differenza nel tempo di generazione dell&#39;output.

      In questo elenco è possibile che le attività eseguite correttamente o le attività non siano riuscite. Per le attività completate correttamente, il processo di pubblicazione crea un file di registro \(logs.txt\) a cui è possibile accedere facendo clic sul collegamento nella colonna Generated At (A generato).


**Argomento principale:**[ Genera output di documenti FrameMaker](fm-output-generatation.md)

