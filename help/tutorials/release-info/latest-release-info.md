---
title: Versioni delle guide AEM
description: Versioni più recenti AEM Guide e versioni AEM preliminari necessarie
exl-id: 780697a9-bdc6-40c2-b258-64639fe30f88
source-git-commit: f836ad2178524b1ddfb89fdfa728a8b06cb02c2c
workflow-type: tm+mt
source-wordcount: '1188'
ht-degree: 0%

---

# [!DNL AEM Guides] Indicazione estesa delle versioni

[!DNL Adobe Experience Manager Guides] è un&#39;applicazione distribuita in AEM. Si tratta di una potente soluzione di gestione dei contenuti per componenti di livello enterprise (CCMS) che consente il supporto DITA nativo in Adobe Experience Manager, consentendo AEM gestire la creazione e la distribuzione di contenuti basati su DITA.

I pacchetti AEM Guide sono disponibili in due varianti: build UID e build non UUID.

## Build UUID e non UUID

Le differenze chiave tra le build UUID e non UUID sono le seguenti:

|  | Build non UUID | Build UUID |
|---|---|---|
| **Identificazione della risorsa** | Tutte le risorse vengono identificate utilizzando il percorso della risorsa nell’archivio. | Tutte le risorse vengono identificate utilizzando il loro UUID (ID univoco generato dal sistema al momento del primo caricamento della risorsa). |
| **Creazione di riferimenti** | Tutti i riferimenti al contenuto vengono creati in base ai relativi percorsi. | Tutti i riferimenti di contenuto vengono creati in base al loro UUID. |

### Vantaggi della build UID

* L’installazione di UUID è più performante:
   * I riferimenti sono indipendenti dal percorso: Il sistema di gestione dei riferimenti è consapevole dei collegamenti in quanto i riferimenti vengono creati in base agli UUID e non ai percorsi.
   * Le operazioni di spostamento/aggiornamento sono efficienti: Gli UUID rimangono uguali anche se le risorse si spostano in un altro percorso nell’archivio. Pertanto, non è necessaria alcuna elaborazione per applicare una patch ai riferimenti tra le risorse durante le operazioni di spostamento/aggiornamento.
* La build UUID è lungimirante, in quanto utilizziamo questo framework anche per la configurazione cloud delle guide AEM.


### Scegli tra le due build

* Se sei un nuovo cliente, ti consigliamo di utilizzare la build UUID.
* Se sei un cliente esistente, puoi scegliere di passare alla build UUID, poiché è ora possibile effettuare la migrazione dalla build Non-UUID alla build UUID. Per ulteriori dettagli, consulta la sezione *Migrazione dei contenuti non UUID a UUID* nella sezione **Installa e configura le guide di Adobe Experience Manager.**

>[!NOTE]
>
>* I clienti dovranno scegliere tra la modalità UUID e non UUID al momento della prima configurazione (se hai bisogno di aiuto, contatta Customer Success Manager per aiutarti a prendere la decisione in base al tuo utilizzo).
>* Durante l’aggiornamento da una versione di AEM Guide a una versione più recente, i clienti dovranno assicurarsi di scegliere la stessa modalità (UUID / non-UUID) per corrispondere alla modalità esistente. Una build non UUID non deve essere aggiornata direttamente a una build UUID. Il passaggio dalla build non UUID alla build UUID richiede la migrazione dei contenuti.


**Aggiornamento delle build**

Quando esegui l’aggiornamento da una versione precedente a una versione più recente di [!DNL AEM Guides], potrebbe essere necessario eseguire script di migrazione. Per istruzioni sull’aggiornamento, consulta Note sulla versione e documentazione specifica sulla versione .

Non tutti i percorsi di aggiornamento sono supportati direttamente. Ad esempio, l&#39;aggiornamento diretto alla versione 4.0 è possibile solo dalla versione 3.8. Se utilizzi una versione precedente alla versione 3.8, consulta la documentazione specifica della versione per le istruzioni di aggiornamento [Archiviazione della Guida](https://helpx.adobe.com/xml-documentation-for-experience-manager/archive.html).
Rivolgiti al tuo responsabile di successo cliente per convalidare il percorso di aggiornamento.

**[!DNL AEM Guides]Build**

L&#39;elenco seguente contiene l&#39;ultima [!DNL AEM Guides] pacchetti disponibili per l&#39;installazione su AMS o On-Prem, versioni AEM corrispondenti (prerequisiti), collegamenti per il download di pacchetti e altre informazioni utili. È consigliabile utilizzare solo la build più recente di [!DNL AEM Guides]. Se per qualche motivo hai bisogno di accedere a build precedenti, connettiti con Customer Success Manager del tuo account.

>[!NOTE]
>
>Rivolgiti al tuo Customer Success Manager per accedere a [!DNL AEM Guides] build per AEM as a Cloud Service.

| [!DNL AEM Guides]Versione  | Note sulla versione | AEM | Creare collegamenti di download |
|---|---|---|---|
| **Guide AEM 4.2** | [Note sulla versione 4.2](https://experienceleague.adobe.com/docs/experience-manager-guides-learn/tutorials/release-info/release-notes/on-prem-release-notes/release-notes-4.2.html) | **Non UID e UUID 4.2**<br><br> AEM 6.5 SP15, SP14, SP13 o SP12 <br><br>Java: 11 o 8<br><br> | **Non UID**: <br> **AEM 6.5** <br>[4.2.](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Faemdox%2F4-2%2F4-2-non-uuid%2Fcom.adobe.fmdita-6.5-4.2.229.zip)<br><br> **UUID** <br>**AEM 6.5** <br>[4.2.](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Faemdox%2F4-2%2F4-2-uuid%2Fcom.adobe.fmdita-6.5-uuid-4.2.229.zip)<br> |
| **Guide AEM 4.1** | [Note sulla versione 4.1.x](https://experienceleague.adobe.com/docs/experience-manager-guides-learn/tutorials/release-info/release-notes/on-prem-release-notes/release-notes-4.1.html) | **Non UUID e UUID 4.1.2**<br><br> AEM 6.5 SP13, SP12, SP11 o SP10 <br>Java: 11 o 8 <br><br>**Non UUID e UUID 4.1**<br><br> AEM 6.5 SP13, SP12, SP11 o SP10 | **Non UID**: <br> **AEM 6.5** <br>[4.1.](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Faemdox%2F4-1%2F4-1-non-uuid%2Fcom.adobe.fmdita-6.5-4.1.159.zip)<br>[4.1.2.](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Faemdox%2F4-1-2%2F4-1-2-non-uuid%2Fcom.adobe.fmdita-6.5-sp-4.1.2.11.zip)<br>[4.1.3.](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Faemdox%2F4-1-3%2F4-1-3-non-uuid%2Fcom.adobe.fmdita-6.5-sp-4.1.3.2.zip)<br><br> **UUID** <br>**AEM 6.5** <br>[4.1.](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Faemdox%2F4-1%2F4-1-uuid%2Fcom.adobe.fmdita-6.5-uuid-4.1.159.zip)<br>[4.1.2.](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Faemdox%2F4-1-2%2F4-1-2-uuid%2Fcom.adobe.fmdita.uuid-6.5-sp-4.1.2.11.zip)<br>[4.1.3.](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Faemdox%2F4-1-3%2F4-1-3-uuid%2Fcom.adobe.fmdita.uuid-6.5-sp-4.1.3.2.zip) |
| **Guide AEM 4.0** | [Note sulla versione 4.0.x](https://helpx.adobe.com/xml-documentation-for-experience-manager/release-note/release-notes-xml-documentation-solution-4-0.html) | **UUID e UUID 4.0.3 non UUID**<br> AEM 6.5 SP12, SP11, SP10 o SP9 <br>Java: 11 o 8 <br><br> <br>**Non UUID e UUID 4.0.2** <br> AEM 6.5 SP12, SP11, SP10 o SP9 <br>Java: 11 o 8 <br><br> **UUID e UUID 4.0 non UUID** <br> AEM 6.5 SP11, SP10 o SP9 | **Non UID**: <br> **AEM 6.5** <br>[4.0.3](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Faemdox%2F4-0-3%2F4-0-2-non-uuid%2Fcom.adobe.fmdita-6.5-hotfix-4.0.3.1.zip)<br>[4.0.2](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Faemdox%2F4-0-2%2F4-0-2-non-uuid%2Fcom.adobe.fmdita-6.5-sp-4.0.2.10.zip)  <br> [4.0](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/aemdox/4-0/4-0-non-uuid/com.adobe.fmdita-6.5-4.0.70.zip)  <br><br> **UUID** <br>**AEM 6.5**  <br>[4.0.3](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Faemdox%2F4-0-3%2F4-0-3-uuid%2Fcom.adobe.fmdita.uuid-6.5-hotfix-4.0.3.1.zip) <br>[4.0.2](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Faemdox%2F4-0-2%2F4-0-2-uuid%2Fcom.adobe.fmdita.uuid-6.5-sp-4.0.2.10.zip)<br> [4.0](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/aemdox/4-0/4-0-uuid/com.adobe.fmdita-6.5-uuid-4.0.70.zip) |
| **Guide AEM 3.8.5** <br> 3.8.5 è una versione di SP in aggiunta alla versione 3.8. <br>La versione 3.8 non deve essere installata autonomamente in quanto la versione 3.8.5 SP contiene una correzione critica. <br>I clienti devono prima installare 3.8 e poi SP 3.8.5. | [Note sulla versione 3.8.x](https://helpx.adobe.com/xml-documentation-for-experience-manager/release-note/release-notes-xml-documentation-solution-3-8.html) | **Non UID** <br> AEM 6.5 SP9 o SP8 <br> AEM 6.4 SP8 <br> AEM 6.3 SP3 <br><br> **UUID** <br> AEM 6.5 SP9 o SP8 | **Non UID**: <br> **AEM 6.5** <br> [3.8.5 SP](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/aemdox/3-8-5/com.adobe.fmdita-6.5-hotfix-3.8.5.2.zip) <br>[3,8](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/aemdox/3-8/com.adobe.fmdita-6.5-3.8.166.zip)<br> **AEM 6.4**<br> [3.8.5 SP](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/aemdox/3-8-5/com.adobe.fmdita-6.4-hotfix-3.8.5.1.zip) <br>[3,8](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/aemdox/3-8/com.adobe.fmdita-6.4-3.8.166.zip) <br> **AEM 6.3** <br> [3.8.5 SP](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/aemdox/3-8-5/com.adobe.fmdita-6.3-hotfix-3.8.5.1.zip) <br>[3,8](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/aemdox/3-8/com.adobe.fmdita-6.3-3.8.166.zip) <br><br> **UUID** <br>**AEM 6.5** <br> [3.8.5 SP](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/aemdox/3-8-5uuid/com.adobe.fmdita.uuid-6.5-hotfix-3.8.5.2.zip) <br> [3.8](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/aemdox/3-8uuid/com.adobe.fmdita.uuid-6.5-3.8.168.zip) |
