---
title: Aggiungere stili personalizzati all’editor Web Guide
description: Scopri come aggiungere stili personalizzati per modificare l’aspetto dell’editor web Guide.
source-git-commit: 9e7d5bb4c8f6c6ebe21bfcebdd7d2e13971b8df2
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# Aggiungere stili personalizzati all’editor Web Guide

In questo articolo impareremo come aggiungere stili personalizzati per modificare l’aspetto predefinito del webeditor.

Ciò comporta i seguenti passaggi:
- Aggiunta di stili personalizzati tramite Configurazione dell’editor XML del profilo cartella
- Scelta del rispettivo profilo di cartella in webeditor e verifica le modifiche


## Implementazione tramite un esempio

Comprendiamo questo con un esempio in cui vogliamo mostrare la breve descrizione e il titolo come blocco separato con alcuni aspetti di stile nell’editor.

![Anteprima dell’editor web con stili personalizzati](../../../assets/authoring/webeditor-customstyles-preview.png)


## Implementazione


### Aggiunta di CSS personalizzati al profilo della cartella

Utilizza i profili di cartella per controllare il *css_layout.css* nella scheda &quot;Configurazione editor XML&quot; e aggiungi il CSS con stili personalizzati

[utilizza questo collegamento per ulteriori informazioni sul profilo cartella e sulla configurazione del layout del modello CSS](https://experienceleague.adobe.com/docs/experience-manager-guides-learn/videos/advanced-user-guide/editor-configuration.html?lang=en#customize-the-css-template-layout)

Utilizza quanto segue per impostare lo stile precedente nel tuo editor web:
- Utilizzo [css_layout.css](../../../assets/authoring/webeditor-customstyles-css_layout.css) e caricarlo nel profilo della cartella desiderato
- Installa il pacchetto allegato [webeditor-style-resources.zip](../../../assets/authoring/webeditor-styles-resources.zip) utilizzo di AEM gestione pacchetti per installare le risorse utilizzate nel file CSS di cui sopra

```
This will install the resources at path "/content/dam/resources" which will include sub-folders "fonts" and "images"
```


### Test

- Apri editor web
- In Preferenze utente scegli il profilo della cartella in cui hai aggiunto gli stili personalizzati. Se l’hai aggiunto al Profilo globale, probabilmente lo stai già utilizzando.
- Apri un argomento, noterai che l’area di modifica deve avere un’interfaccia utente personalizzata

```
Please note this is compatible to AEM Guides version 4.2 and AEM Guides cloud version 2303 (March)
```


## Riferimenti

Potresti anche essere interessato alla sessione esperta sulle configurazioni del webeditor e la personalizzazione coperta in [Sessione esperta su webeditor](https://experienceleague.adobe.com/docs/experience-manager-guides-learn/tutorials/knowledge-base/expert-session/webbased-authoring-jan2023.html?lang=en)