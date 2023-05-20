---
title: Funzione di pubblicazione nativa di PDF | Usa stili personalizzati nelle note a piè di pagina
description: Scopri come applicare lo stile ai numeri nelle note a piè di pagina.
exl-id: f1068f2f-2ace-4bdb-b5a4-46b03d4e43d6
source-git-commit: 7b48633ef2418fa7c91842a8d2c2a4177017ef58
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Usa stili personalizzati nelle note a piè di pagina

Le note a piè di pagina sono note posizionate nella parte inferiore di una pagina che commenta o cita un riferimento per una parte designata del testo.

È possibile applicare uno stile ai numeri nella chiamata a piè di pagina presenti nel contenuto dell&#39;argomento e al contrassegno della nota a piè di pagina presente nella parte inferiore della pagina. Ad esempio, è possibile aggiungere parentesi quadre attorno al numero o modificarne il colore. Questi stili consentono di identificare facilmente le note a piè di pagina nel documento.

```css
...
.footnote::footnote-call { 
content: "(" counter(footnote, decimal) ")"; 
} 

.footnote::footnote-marker { 
content: "(" counter(footnote, decimal) ")"; 
} 

...
```

Nell’esempio in questione, viene aggiunta una parentesi prima e dopo la chiamata e il marcatore della nota a piè di pagina:

* Aggiungi il prefisso &quot;(&quot; e il suffisso &quot;)&quot; utilizzando l’attributo content nel `footnote-call` stile che consente di aggiungere le parentesi quadre attorno al numero della nota a piè di pagina nel contenuto dell&#39;argomento.
* Aggiungi il prefisso &quot;(&quot; e il suffisso &quot;)&quot; utilizzando l’attributo content nel `footnote-marker` che aggiungerà le parentesi quadre attorno al numero della nota a piè di pagina nella parte inferiore della pagina.

<img src="./assets/pdf-output-footer-numbers.png" alt="Piè di pagina nell’output di PDF" width="500">
