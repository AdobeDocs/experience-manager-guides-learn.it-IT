---
title: Guide alla pubblicazione di benchmark su AEMaaCS
description: Comprendere i limiti di sistema per la pubblicazione su AEM Cloud.
source-git-commit: e64430bb968b18090c3981cc2d21ebe6593ba933
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 7%

---


# Guide AEM per la pubblicazione di benchmark su AEMaaCS

Attualmente il servizio cloud Guide AEM ha alcuni limiti sulla pubblicazione delle dimensioni delle mappe che il team Guide sta attivamente lavorando per risolvere.

Il team Guide ha già introdotto una [Pubblicazione di Microsoft Service](publish-microservice-architecture-and-performance.md) per supportare mappe di grandi dimensioni e più pubblicazioni simultanee. Per il momento, questo microservizio supporta un sottoinsieme di tipi di output e altri tipi sono in fase di sviluppo attivo.

Per configurare il nuovo servizio di pubblicazione per qualsiasi ambiente cloud AEM consulta [Configurare una nuova pubblicazione basata su microservizi](configure-microservices.md)

## Ambiente di esecuzione

    Versione AEM: 2023.5.11983.20230511T173830Z
    Versione Del Componente Aggiuntivo Della Guida: 2023.6.0
    Modello per sito AEM: modello OOTB delle guide AEM
    Versione DITA-OT: 3.5.4
    Tipo di flusso di lavoro di pubblicazione: Dividi flusso di lavoro di pubblicazione
    Output supportato dal microservizio: Native PDF, PDF (Dita-OT)

## Numeri di generazione output

| Tipo di output | Dimensione mappa (riferimenti argomento) | Tempo di esecuzione (in secondi) | Pubblicazione di Microsoft Service |
|---------------|------------------------------|----------------------------|-----------------------|
| Sito AEM | 3500 | 5220 | No |
| Native PDF | 3500 | 780 | Sì |
| PDF (DITA-OT) | 11000 | 960 | Sì |
| HTML5 | 3500 | 240 | No |
| Personalizzati | 300 | 300 | No |

## Punti chiave da ricordare

- Il sito AEM crea molti nodi cq:Page e li appiattisce eseguendo il rendering singolarmente durante la generazione. Per questo motivo, è consigliabile evitare di eseguire più pubblicazioni simultanee di grandi dimensioni del sito AEM, in quanto ciò potrebbe sovraccaricare il sistema.
- Il tempo di generazione del sito AEM dipende dal modello utilizzato. Il tempo di esecuzione può aumentare se si utilizza un modello complesso.
- Il tempo di esecuzione della pubblicazione personalizzata si riferisce a un output personalizzato di esempio. Il tempo di pubblicazione personalizzato dipende esclusivamente dalla logica di trasformazione del cliente.
