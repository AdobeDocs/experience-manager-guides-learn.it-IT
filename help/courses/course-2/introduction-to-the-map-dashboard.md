---
title: Introduzione al dashboard mappa
description: Introduzione al dashboard mappa
exl-id: c2efa073-15e7-42a0-aaa8-04859b0fdf62
source-git-commit: 1c4d278a05f2612bc55ce277efb5da2e6a0fa9a9
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Introduzione al dashboard mappa

Di seguito viene fornita una panoramica delle funzioni principali del dashboard mappa.

>[!VIDEO](https://video.tv.adobe.com/v/339040?quality=12&learn=on)

## Apri una mappa nel dashboard Mappa

1. In Vista archivio, seleziona l’icona Ellissi sulla mappa per aprire il menu Opzioni, quindi Apri dashboard mappa.
   ![images/ellipsis-map-dashboard.png](images/ellipsis-map-dashboard.png)

   Il dashboard mappa si apre in un&#39;altra scheda.

## Componenti della dashboard mappa

La dashboard di mappa contiene diverse schede, tra cui predefiniti di output, risultati di output, argomento utilizzato, linee di base e altro ancora.

### Predefiniti di output

La scheda Predefiniti di output visualizza i predefiniti per i diversi tipi di output: Sito AEM, PDF, HTML5, ePub e Personalizzato.

![images/output-presets.png](images/output-presets.png)

Puoi selezionare un predefinito di output per visualizzare i dettagli delle relative impostazioni, tra cui il nome della trasformazione, il percorso di destinazione, le linee di base e le condizioni applicate.

### Uscite

La scheda Output visualizza tutti gli output generati in precedenza e attualmente generatori.

![images/generated-outputs.png](images/generated-outputs.png)

Un cerchio verde sotto la colonna Impostazioni generazione indica che l&#39;output è stato generato correttamente. Il testo in questa colonna funge da collegamento ipertestuale attivo e puoi selezionarli per aprire l’output generato. Le voci della colonna Tipo indicano il tipo di output.
Qui vengono visualizzate anche altre informazioni sulla generazione dell’output, tra cui il nome dell’utente che ha generato l’output, la data e l’ora della generazione e il tempo necessario per la generazione. Se si verifica un errore durante la generazione, puoi selezionare la data e l’ora della generazione nella colonna Generated At per aprire e rivedere il registro degli errori.

### Argomenti

Nella scheda Argomenti viene visualizzato un elenco di tutti gli argomenti inclusi nella mappa.

![images/topics.png](images/topics.png)

La selezione della casella di controllo di un argomento consente di eseguire ulteriori azioni. È possibile modificarlo, rigenerarlo e mostrare, applicare o nascondere i relativi tag.

### Predefiniti condizione

La scheda Predefiniti condizione visualizza le impostazioni per il contenuto condizionale specifico da includere o escludere.

![images/condition-presets.png](images/condition-presets.png)

In questo caso, selezionando la casella di controllo per l’edizione Solo autore si otterrà un output che esclude tutto il contenuto con l’attributo &quot;pubblico&quot; che ha l’etichetta &quot;designer&quot; e include tutto il contenuto con l’etichetta &quot;scrittori&quot;.

### Linee di base

La scheda Linee di base consente di visualizzare le linee di base.

![images/baselines.png](images/baselines.png)

Le linee di base fungono da istantanee nel tempo e consentono di creare una versione degli argomenti e delle risorse da pubblicare. Ad esempio, una linea di base che acquisisce il contenuto in una data e in un’ora specifiche può utilizzare la versione 1.3 di un argomento e la versione 1.0 di un altro argomento, in base alle rispettive versioni all’epoca.
Se non è specificata alcuna linea di base, l’output viene generato con le versioni più recenti di tutto il contenuto.

### Rapporti

Nella scheda Rapporti viene visualizzato un riepilogo delle informazioni relative all’argomento, compreso il numero di argomenti totali in uso, gli elementi mancanti all’interno di tali argomenti e lo stato del documento.

![images/reports.png](images/reports.png)

Se manca un elemento in un argomento, puoi selezionare la freccia più a destra nella riga per espandere la voce e visualizzare i dettagli dell’errore.
