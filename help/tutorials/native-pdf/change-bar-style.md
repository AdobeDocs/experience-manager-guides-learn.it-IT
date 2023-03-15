---
title: Funzione di pubblicazione nativa di PDF | Utilizzare stili di barre di modifica personalizzati
description: Scopri come applicare gli stili sulle barre di modifica.
source-git-commit: 79de97e667bffae8d120deee68a0a82011047cf5
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Operazioni con gli stili delle barre di modifica personalizzati

Una barra di modifica è una linea verticale che identifica visivamente il contenuto nuovo o rivisto. AEM guide ti consente di visualizzare una barra di modifica a sinistra del contenuto modificato all’interno degli argomenti e anche degli argomenti modificati nel sommario dell’output di PDF.

Per ulteriori dettagli sulla visualizzazione della barra delle modifiche, consulta *Crea PDF con barra di modifica tra le versioni pubblicate* impostazione
[Pubblica output PDF](../web-editor/native-pdf-web-editor.md).

## Contenuto modificato negli argomenti

La barra delle modifiche viene visualizzata a sinistra del contenuto negli argomenti inseriti, modificati o eliminati.

È possibile modificare i seguenti stili per mostrare il contenuto modificato e tra di essi con le barre di modifica.


>[!NOTE]
>
>Questi stili fanno parte di `layout.css` e puoi modificarli come necessario.

Ad esempio, puoi utilizzare l’attributo colore nella `.inserted-block` per definire la modalità di visualizzazione del contenuto inserito nell’output di PDF pubblicato.


```css
...
.inserted-block { 
  color: #2ECC40; 
  display: inline; 
  -ro-comment-content: " "; 
  -ro-comment-style: underline; 
  -ro-comment-title: "Inserted"; 
  -ro-comment-date: attr(data-time); 
  -ro-comment-dateformat: "yyyy/dd/MM HH:mm:ss"; 
} 
...
```

Allo stesso modo, puoi utilizzare la `.deleted-block` per definire la modalità di visualizzazione del contenuto eliminato nell’output di PDF pubblicato.

```css
...
.deleted-block { 
  display: inline; 
  color: #FF6961; 
  text-decoration: line-through; 
  -ro-comment-content: " "; 
  -ro-comment-style: strikeout; 
  -ro-comment-title: "Deleted"; 
  -ro-comment-date: attr(data-time); 
  -ro-comment-dateformat: "yyyy/dd/MM HH:mm:ss"; 
} 
...
```

È possibile utilizzare `.inserted-change-bar` e `.deleted-change-bar` per modificare l’aspetto delle barre di modifica visualizzate a sinistra del contenuto aggiornato.

Ad esempio, puoi utilizzare `-ro-change-bar-color` attributo in `.inserted-change-bar` stile per mostrare la barra di modifica inserita in verde. È inoltre possibile utilizzare `-ro-change-bar-color` attributo in `.deleted-change-bar` stile per mostrare la barra di modifica eliminata in rosso.

```css
...
.inserted-change-bar { 
  -ro-change-bar-color: #2ECC40; 
} 

.deleted-change-bar { 
  -ro-change-bar-color: #FF6961; 
  } 
...
```

<img src="./assets/changed-bar-content.png" alt="Contenuto dell’argomento della barra modificato" width="500">

## Argomento modificato nel sommario (sommario)

È inoltre possibile aggiungere una barra di modifica a sinistra degli argomenti modificati nel sommario dell’output di PDF. È possibile utilizzare `-ro-change-bar-color` nella `.changed-topic` stile per aggiungere una barra di modifica nel colore desiderato per gli argomenti aggiornati nell’elenco sommario.

Ad esempio, puoi aggiungere una barra di modifica del colore verde.

```css
...
.changed-topic { 
 -ro-change-bar-color: #2ECC40; 
}  
...
```


Viene visualizzata una barra di modifica verde per tutti gli argomenti nel sommario in cui sono stati eseguiti alcuni aggiornamenti. Puoi fare clic sull’argomento modificato nel sommario e visualizzare le modifiche dettagliate.

<img src="./assets/changed-bar-TOC.png" alt="TOC a barre modificato" width="500">
