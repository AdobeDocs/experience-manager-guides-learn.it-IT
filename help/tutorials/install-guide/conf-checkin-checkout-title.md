---
title: Configurare il titolo per le icone Check-In e Check-Out
description: Scopri come configurare il titolo per le icone di check-in e check-out
source-git-commit: bb4b875864b31197437a944ded5862bbf937bc29
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Configurare il titolo per le icone Archivia ed Estrai

Le guide AEM consentono di configurare il titolo per le icone Check-In e Check-Out nell&#39;editor Web. Per configurare il titolo per le icone di check-in e check-out, effettuare le seguenti operazioni:

1. Scarica il file di configurazione dell’interfaccia utente accedendo ad Adobe Experience Manager come amministratore.
1. Fai clic sul collegamento Adobe Experience Manager in alto e scegli **Strumenti**.
1. Seleziona **Guide** dall&#39;elenco degli strumenti e fare clic su **Profili cartella**.
1. Fai clic sul pulsante **Profilo globale** affiancare.
1. Seleziona la **Configurazione editor XML** e fai clic sul pulsante **Modifica** nella parte superiore.
1. In **Configurazione interfaccia utente editor XML** , fare clic sul pulsante **Scarica** per scaricare `ui_config.json` sul sistema locale.
1. In `ui_config.json` , modificare il titolo nella sezione &quot;topbar&quot;. È possibile modificare i seguenti valori:

   ```json
   //Change title to "Check out" instead of "Lock"
           "title": "Check out"
   
   //Change title to "Check in" instead of "@checkOutBy
            "title": "Check in"
   ```

1. Salva il file e caricalo.

