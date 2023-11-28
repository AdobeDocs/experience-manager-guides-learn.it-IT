---
sidebar_position: 3
source-git-commit: 42052b37724f97e34ab007db4cc3d9f9524ad3a2
workflow-type: tm+mt
source-wordcount: '62'
ht-degree: 0%

---


# Campo di testo e area di testo

Per prendere il testo come input, usiamo i componenti, il campo di testo e l’area di testo.
Il componente area di testo in JUI rappresenta un html `<textarea/>`.

```js title="textArea.js"
const textAreaJSON =  {
    "component": "textarea", //tells the component name
    "id": "input_name", // can be used to give a unique identifier to a component
    "data": "@name", // the variable storing the inputted text
    "on-keyup": {
        "name": "submitName",
        "eventArgs": {
            "keys": [
            "ENTER"
            ]
        }
    },
},
```

Qui, `on-keyup` è la sintassi per richiamare i comandi nei controller.
Verrà generato un textArea in cui premendo INVIO verrà chiamato l&#39;evento `submitName`

L’area di testo di cui è stato eseguito il rendering sarà simile alla seguente:

![area di testo](./imgs/text_area.png "Area di testo")
