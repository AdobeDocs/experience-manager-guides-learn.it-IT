---
title: Configurare il salvataggio automatico dei file nell’editor web
description: Scopri come configurare il salvataggio automatico dei file nell’editor web
source-git-commit: 801c306fa120e7889d4b9428fd5bee2849bf1956
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 1%

---


# Configurare il salvataggio automatico dei file nell’editor web {#id199CC0J0M5Z}

Una delle funzioni più comuni nell’editor basato su browser è la possibilità di salvare i dati dopo un periodo di tempo specifico. L&#39;editor Web delle guide AEM supporta inoltre il salvataggio automatico dei file argomento e mappa nell&#39;intervallo di tempo specificato. Quando questa funzione viene attivata, viene salvata la copia di lavoro dell&#39;argomento o della mappa. Non è stata creata una nuova versione dell&#39;argomento o della mappa. Per creare una nuova versione, è necessario fare clic sull&#39;icona Salva revisione nella barra degli strumenti dell&#39;editor Web.

La funzione di salvataggio automatico non è attivata per impostazione predefinita ed è necessario attivarla da configMgr. Per abilitare la funzione di salvataggio automatico nell’editor Web, effettua le seguenti operazioni:

1. Apri la pagina Configurazione della console web Adobe Experience Manager.

   L&#39;URL predefinito per accedere alla pagina di configurazione è:

   ```http
   http://<server name>:<port>/system/console/configMgr
   ```

1. Cerca e fai clic su **com.adobe.fmdita.xmleditor.config.XmlEditorConfig** pacchetto.

1. In *XmlEditorConfig* , selezionare la **Salvataggio automatico** opzione.

1. In **Intervallo salvataggio automatico** , specificare l&#39;intervallo di tempo in secondi per attivare la funzione di salvataggio automatico.

1. Fai clic su **Salva**.


**Argomento padre:**[ Personalizza editor web](conf-web-editor.md)

