---
title: Imposta DITA-OT personalizzato in [!DNL AEM Guides]
description: Scopri come impostare DITA-OT personalizzato in [!DNL Adobe Experience Manager Guides]
role: Admin
exl-id: f479c2cf-5b8b-4517-be97-81303468007a
source-git-commit: b5e64512956f0a7f33c2021bc431d69239f2a088
workflow-type: tm+mt
source-wordcount: '153'
ht-degree: 0%

---

# Imposta DITA-OT personalizzato in [!DNL AEM Guides] per AEM

I passaggi per aggiungere un DITA-OT personalizzato sono documentati nella sezione . _Utilizzare plug-in DITA-OT personalizzati_ del _Guida all’installazione e alla configurazione_.

Ad alto livello i passaggi sono i seguenti:

+ Ottenere la DITA-OT di base
   + Se si desidera ottenere una copia di DITA-OT preconfigurato da [!DNL AEM Guides], scaricalo dal percorso `/etc/fmdita/dita_resources/DITA-OT.zip`
   + Se desideri ottenere una versione diversa, puoi scaricare da [repo dita-to](https://www.dita-ot.org/download)
+ Apporta modifiche a DITA-OT come [aggiunta di un nuovo plug-in](https://www.dita-ot.org/dev/topics/plugins-installing.html), o personalizzazione dei plug-in esistenti (consulta l’esempio nella sezione link correlati di seguito)
+ Carica `DITA-OT.zip` ricevuto `/apps/<project-folder>/dita_resources` (si consiglia di creare una cartella di progetto personalizzata)
+ Aggiungi profilo DITA tramite **[!UICONTROL Strumenti]** > **[!UICONTROL Guide]** > **[!UICONTROL Profili DITA]** (utilizza il percorso DITA-OT in cui viene caricato il DITA-OT personalizzato, fai riferimento alla schermata seguente)
   ![Profili DITA](assets/dita-profile.png)

>[!MORELIKETHIS]
>
>+ [Personalizzazione degli esempi di plug-in DITA-OT](https://www.dita-ot.org/dev/topics/pdf-customization.html)
