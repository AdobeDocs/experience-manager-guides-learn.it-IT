---
title: Come aggiungere [!DNL AEM Guides] al tuo [!DNL AEM as a Cloud Service] ambiente
description: Scopri come aggiungere [!DNL AEM Guides] al tuo [!DNL AEM as a Cloud Service] ambiente
exl-id: a1e020c2-360c-4d71-b5fd-8179d9ceacda
source-git-commit: b5e64512956f0a7f33c2021bc431d69239f2a088
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# [!DNL AEM Guides] Distribuzione as a Cloud Service

Scopri come aggiungere [!DNL Guides] al tuo [!DNL AEM as a Cloud Service] ambiente.

## Distribuzione manuale tramite pipeline Git di Cloud Manager

Se hai acquistato [!DNL AEM Guides] as a Cloud Service prima del 29 marzo 2022, segui queste istruzioni di distribuzione:

* Se stai iniziando da nuovo, puoi sostituire il codice generato automaticamente da [!UICONTROL Cloud Manager] con il codice del repository sottostante che ha il plugin XML già integrato: https://github.com/Adobe-TCS/XML-documentation-for-AEMaaCS

* Se hai già eseguito il check-in delle personalizzazioni in [!UICONTROL Cloud Manager] git repo, puoi fare riferimento al seguente repo per le istruzioni su come aggiungere il plugin XML nel codice esistente: https://github.com/Adobe-TCS/DoX-Installer-for-AEMaaCS

## Implementazione Tramite Cloud Manager

Se sei un cliente che ha acquistato [!DNL AEM Guides] as a Cloud Service il 29/03/2022 o dopo, segui queste istruzioni per aggiungere [!DNL Guides] al tuo [!DNL AEM as a Cloud Service] ambiente:

1. Accedi a [!UICONTROL Cloud Manager].

1. Modificare il programma per il quale si desidera configurare [!DNL AEM Guides].

1. Passa a **[!UICONTROL Soluzioni e componenti aggiuntivi]** scheda .

1. In **[!UICONTROL Soluzioni e componenti aggiuntivi]** tabella, fai clic su **[!UICONTROL Risorse]**.

1. Seleziona **[!UICONTROL Guide]** e seleziona **[!UICONTROL Salva]**.

Il programma è stato configurato correttamente per il provisioning automatico della soluzione Guide AEM.

![Configurazione AEM soluzione Guide](assets/addon-configuration.png)

>[!NOTE]
>
>Per installare [!DNL AEM Guides] in qualsiasi ambiente del programma integrato, è necessario eseguire la pipeline associata all’ambiente. Non è necessaria alcuna configurazione aggiuntiva nel codebase Git di CM per l’installazione [!DNL AEM Guides].
