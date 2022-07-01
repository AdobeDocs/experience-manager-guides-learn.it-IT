---
title: Escludere dalla traduzione i paragrafi all’interno di un argomento
description: Come escludere i paragrafi all’interno di un argomento dalla traduzione
feature: Translation
role: User
exl-id: 21e41bb4-52f3-4352-92d9-4a60f636de99
source-git-commit: b5e64512956f0a7f33c2021bc431d69239f2a088
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---

# Come escludere i paragrafi all’interno di un argomento dalla traduzione

Il modo più semplice è quello di utilizzare l&#39;attributo translation=no.

+ Gli autori possono inserire l’attributo aggiuntivo come **translation=no** sui paragrafi che non vogliono tradurre. Il fornitore di traduzione deve essere informato e può eseguire la configurazione al termine del processo per ignorare il testo con questo attributo.
+ La traduzione automatica OOTB (con il connettore di traduzione Microsoft di prova) mostra lo stesso comportamento.
+ Test con Microsoft Translation : se definisci **translate=no** a livello di paragrafo, non traduce il paragrafo completo. Questo attributo può essere definito in qualsiasi elemento e il contenuto all’interno di tale elemento non verrà tradotto.


Ecco alcune schermate che spiegano ulteriormente questo:

**Contenuto sorgente**

![Contenuto sorgente](assets/source-content.jpg)

**Contenuto tradotto in spagnolo**

![Contenuto tradotto in spagnolo](assets/trans-content.jpg)
