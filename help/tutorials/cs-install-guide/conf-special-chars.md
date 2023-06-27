---
title: Configurare i caratteri speciali consentiti
description: Scopri come configurare i caratteri speciali consentiti
source-git-commit: 6051181e243cf71919901093c1b5590f21832545
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---


# Configurare i caratteri speciali consentiti {#id20CIL600035}

L’editor web consente di inserire caratteri speciali pronti all’uso. Tuttavia, è possibile personalizzare l&#39;elenco dei caratteri speciali che gli autori possono inserire nei propri documenti. Se personalizzi l’elenco dei caratteri speciali, questo sovrascrive il set predefinito di caratteri speciali. Solo i caratteri speciali aggiunti nella configurazione vengono resi disponibili agli autori.

Per sovrascrivere l’elenco predefinito di caratteri speciali, effettua le seguenti operazioni:

1. Crea `symbols.json` nella seguente posizione nell’archivio Git di Cloud Manager:

   ```
   /apps/fmdita/xmleditor/
   ```

1. Aggiungi la definizione del carattere speciale nel `symbols.json` file come:

   ```
   {"symbols": [{"label": "Arrows",
      "items": [
      {   "name": "←",   "title": "Left Arrow"   } 
      ,   
      {   "name": "↑",   "title": "Up Arrow"      } 
      ]   
      }   ]   }
   ```


La struttura del `symbols.json` Il file è spiegato di seguito:

- `"label": "Arrows"`: specifica la categoria dei caratteri speciali. Nel frammento, una categoria con il nome `"Arrows"` è definito.
- `"items"`: definisce la raccolta di caratteri speciali nella categoria.
- `"name": "←", "title": "Left Arrow"`: questa è la definizione del carattere speciale. Inizia con `"name"` etichetta, che non deve essere modificata. Il nome è seguito dal carattere speciale. Il `"title"` è il nome o il titolo del carattere speciale visualizzato come descrizione comando per il carattere speciale.

  All’interno di una categoria è possibile definire più definizioni di caratteri speciali.


**Argomento padre:**[ Personalizza editor web](conf-web-editor.md)
