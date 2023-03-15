---
title: Funzione di pubblicazione nativa di PDF | Usa stili personalizzati nelle note a piè di pagina
description: Scopri come applicare lo stile ai numeri nelle note a piè di pagina.
source-git-commit: ef562c43f5b70d3fe425427108ad8277e1456f24
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Usa stili personalizzati nelle note a piè di pagina

Le note a piè di pagina sono note posizionate nella parte inferiore di una pagina che contengono commenti o citano un riferimento per una parte specifica del testo.

È possibile assegnare uno stile ai numeri nella chiamata a piè di pagina presente nel contenuto dell’argomento e al marcatore a piè di pagina presente nella parte inferiore della pagina. Ad esempio, è possibile aggiungere parentesi intorno al numero o modificarne il colore. Questi stili consentono di identificare facilmente le note a piè di pagina nel documento.

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

* Aggiungi il prefisso &quot;(&quot; e il suffisso &quot;)&quot; utilizzando l’attributo di contenuto nel `footnote-call` stile che aggiungerà le parentesi intorno al numero della nota a piè di pagina nel contenuto dell’argomento.
* Aggiungi il prefisso &quot;(&quot; e il suffisso &quot;)&quot; utilizzando l’attributo di contenuto nel `footnote-marker` stile che aggiunge le parentesi quadre intorno al numero di nota nella parte inferiore della pagina.

<img src="./assets/pdf-output-footer-numbers.png" alt="Piè di pagina nell’output di PDF" width="500">
