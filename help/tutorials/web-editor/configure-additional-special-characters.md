---
title: Configurare caratteri speciali aggiuntivi nella barra degli strumenti dell’Editor web
description: Come configurare caratteri speciali aggiuntivi nella barra degli strumenti dell’Editor web
feature: Web Editor
role: User
exl-id: 0fbc05a5-a6b0-4f6b-bbc4-8fca03581d90
source-git-commit: b5e64512956f0a7f33c2021bc431d69239f2a088
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Come configurare caratteri speciali aggiuntivi nella barra degli strumenti dell’Editor web

Nella barra degli strumenti dell’editor web è presente un’opzione di scelta rapida che consente all’autore di inserire già i caratteri speciali.
Lo stesso si può vedere nella schermata sottostante:

![Caratteri speciali](assets/special-chars.png)


Questo elenco di caratteri è configurabile qui. Per aggiungere altri caratteri, effettua le seguenti operazioni:

+ Accedi a AEM e apri la modalità CRXDE Lite.

+ Crea il file simboli.json nella posizione seguente: &#39;/apps/fmdita/xmleditor/&#39; (Puoi copiare il valore predefinito da - &#39;/libs/fmdita/clientlibs/clientlibs/xmleditor/symbols.json&#39; posizione)

+ Aggiungi la definizione del carattere speciale nel file simboli.json come:

```
{
      "label": "Logical Symbols",
      "items": [
        {
          "name": "≥",
          "title": "Greater-Than or Equal To"
        },
        {
          "name": "≤",
          "title": "Smaller-Than or Equal To"
        }
      ]
}
```

La struttura del file simboli.json è spiegata di seguito:

+ &quot;label&quot;: &quot;Simboli logici&quot;: Specifica la categoria per i caratteri speciali. Nello snippet viene definita una categoria denominata &quot;Simbolo logico&quot;.

+ &quot;items&quot;: Definisce la raccolta di caratteri speciali nella categoria.

+ &quot;name&quot;: &quot; ≥&quot;, &quot;title&quot;: &quot;Maggiore o uguale a&quot;: Questa è la definizione del carattere speciale. Inizia con l&#39;etichetta &quot;name&quot;, che non deve essere modificata. Il nome è seguito dal carattere speciale. Il &quot;titolo&quot; è il nome o il titolo del carattere speciale visualizzato come descrizione del carattere speciale.

È possibile definire più definizioni di caratteri speciali all’interno di una categoria.

Verrà aggiunta un’altra categoria nella finestra di dialogo caratteri speciali:

![Categoria di simboli speciali](assets/special-char-category.png)

![Inserisci carattere speciale](assets/insert-special-char.png)

>[!MORELIKETHIS]
>
>+ [Guida all’installazione e alla configurazione](https://helpx.adobe.com/content/dam/help/en/xml-documentation-solution/3-6/XML-Documentation-for-Adobe-Experience-Manager_Installation-Configuration-Guide_EN.pdf)

