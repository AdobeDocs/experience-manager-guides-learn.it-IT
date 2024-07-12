---
title: Introduzione alla dashboard mappa
description: Introduzione alla dashboard mappa
exl-id: c2efa073-15e7-42a0-aaa8-04859b0fdf62
source-git-commit: 1c4d278a05f2612bc55ce277efb5da2e6a0fa9a9
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Introduzione alla dashboard mappa

Di seguito è riportata una panoramica delle funzioni principali del dashboard mappa.

>[!VIDEO](https://video.tv.adobe.com/v/339040?quality=12&learn=on)

## Apri una mappa nel dashboard Mappa

1. In Vista archivio, seleziona l’icona con i puntini di sospensione sulla mappa per aprire il menu Opzioni, quindi Apri dashboard mappa.
   ![images/ellipsis-map-dashboard.png](images/ellipsis-map-dashboard.png)

   Il quadro comandi Mappa (Map Dashboard) si apre in un’altra scheda.

## Componenti del dashboard mappa

Il dashboard Mappa contiene diverse schede, inclusi i predefiniti di output, i risultati di output, l’argomento utilizzato, le linee di base e altro ancora.

### Predefiniti di output

Nella scheda Predefiniti di output vengono visualizzati i predefiniti predefiniti per i diversi tipi di output: Sito AEM, PDF, HTML5, ePub e Personalizzato.

![images/output-presets.png](images/output-presets.png)

È possibile selezionare un predefinito di output per visualizzare i dettagli delle impostazioni, tra cui il nome della trasformazione, il percorso di destinazione, le linee di base e le condizioni applicate.

### Uscite

Nella scheda Output vengono visualizzati tutti gli output generati in precedenza e quelli attualmente in fase di generazione.

![images/generated-outputs.png](images/generated-outputs.png)

Un cerchio verde sotto la colonna Impostazioni di generazione indica che l’output è stato generato correttamente. Il testo di questa colonna funge da collegamento ipertestuale attivo ed è possibile selezionarlo per aprire l&#39;output generato. Le voci nella colonna Tipo indicano il tipo di output.
In questa pagina vengono visualizzate anche altre informazioni sulla generazione dell’output, tra cui il nome dell’utente che ha generato l’output, la data e l’ora della generazione e il tempo necessario per la generazione. Se si verifica un errore durante la generazione, è possibile selezionare la data e l&#39;ora di generazione nella colonna Generato alle per aprire e rivedere il registro degli errori.

### Argomenti

Nella scheda Argomenti viene visualizzato un elenco di tutti gli argomenti all&#39;interno della mappa.

![images/topics.png](images/topics.png)

La selezione della casella di controllo di un argomento consente di eseguire azioni aggiuntive. Puoi modificarlo, rigenerarlo e mostrarne, applicarne o nasconderne i tag.

### Predefiniti condizione

Nella scheda Predefiniti condizione vengono visualizzate le impostazioni per il contenuto condizionale specifico da includere o escludere.

![images/condition-presets.png](images/condition-presets.png)

In questo caso, selezionando la casella di controllo per l’edizione Solo autore, viene generato un output che esclude tutti i contenuti con l’attributo &quot;pubblico&quot; con l’etichetta &quot;designer&quot; e include tutti i contenuti con l’etichetta &quot;autori&quot;.

### Linee di base

La scheda Baseline consente di visualizzare le baseline.

![images/baselines.png](images/baselines.png)

Le baseline fungono da istantanee nel tempo e consentono di creare una versione degli argomenti e delle risorse da pubblicare. Ad esempio, una linea di base che acquisisce il contenuto in una data e in un&#39;ora specifiche può utilizzare la versione 1.3 di un argomento e la versione 1.0 di un altro argomento, in base alle rispettive versioni in quel momento.
Se non è specificata alcuna linea di base, l’output viene generato con le versioni più recenti di tutto il contenuto.

### Rapporti

Nella scheda Rapporti viene visualizzato un riepilogo delle informazioni sull&#39;argomento, incluso il numero di argomenti totali in uso, gli elementi mancanti all&#39;interno di tali argomenti e lo stato del documento.

![images/reports.png](images/reports.png)

Se in un argomento manca un elemento, è possibile selezionare la freccia più a destra nella riga per espandere la voce e visualizzare i dettagli dell&#39;errore.
