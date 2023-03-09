---
title: FMPS e guide AEM
description: Pubblicazione con FMPS tramite AEM Guides
source-git-commit: 75e4d308f5298660a2d9006b43daf82416eb0822
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---



# FrameMaker Publishing Server (FMPS) e guide AEM

**L&#39;integrazione di AEM Guides con FrameMaker Publishing Server può rappresentare la soluzione ideale se si desidera una pubblicazione automatizzata di alta qualità.\
L’articolo seguente ti aiuterà a configurare ed eseguire FMPS con le guide AEM.**

## Compatibilità dell&#39;FMPS con le guide dell&#39;AEM :

- Compatibilità con il punto 4.1 delle guide AEM : [Collegamento](https://experienceleague.adobe.com/docs/experience-manager-guides-learn/tutorials/release-info/release-notes/on-prem-release-notes/release-notes-4.1.html?lang=en/#compatibility-matrix)

- Compatibilità con le guide AEM 4.0 : [Collegamento](https://helpx.adobe.com/xml-documentation-for-experience-manager/release-note/release-notes-xml-documentation-solution-4-0.html/#Compatibility%20matrix)

- Versione futura : [Collegamento](https://experienceleague.adobe.com/docs/experience-manager-guides-learn/tutorials/release-info/latest-release-info.html?lang=en)

## Installazione:

### Guide AEM:

Per informazioni sull&#39;installazione e la configurazione, vedere: [Collegamento](https://helpx.adobe.com/content/dam/help/en/xml-documentation-solution/4-1-2/Adobe-Experience-Manager-Guides_Installation-Configuration-Guide_EN.pdf)

### FMPS:

Per l&#39;installazione di FMPS è possibile fare riferimento a [Collegamento video](https://www.youtube.com/watch?v=2deelyM5VA8&amp;t) o [Documentazione](https://help.adobe.com/en_US/framemaker/server/index.html#t=fmps-user-guide%2Finstall_config_fmps.html%23install_config_fmps&amp;rhtocid=_2)

## Configurazioni richieste:

Il contenuto DITA può essere emesso utilizzando FrameMaker Publishing Server (FMPS). È possibile creare l&#39;output in qualsiasi formato supportato da FMPS.
Nella console web, modifica le seguenti proprietà del bundle com.adobe.fmdita.config.ConfigManager per configurare le guide AEM per l’utilizzo di FMPS.

Per aprire la console Web, vai all&#39;URL Accesso http://\&lt;server name=&quot;&quot;>:\&lt;port>/system/console/configMgr .

**Proprietà di configurazione e relativa descrizione:** [Collegamento](https://helpx.adobe.com/content/dam/help/en/xml-documentation-solution/4-1-2/Adobe-Experience-Manager-Guides_Installation-Configuration-Guide_EN.pdf#page=89)

## Test in esecuzione:

Utilizzando FMPS, puoi pubblicare automaticamente **PDF, Responsive HTML5**, e **Epub** per le risorse DITA e FM.

Dal menu &quot;Generate PDF using&quot; (Genera utilizzando), scegliete FrameMaker Publishing Server.

L’utente può fornire &quot;File delle impostazioni (.sts)&quot; e &quot;ditaval. Il filtraggio verrà eseguito utilizzando Ditaval in base alle condizioni specificate.

- **File di impostazione**: impostazione FrameMaker /FMPS Publish che contiene tutte le impostazioni che si desidera vengano rispettate da FMPS durante la pubblicazione Ad esempio: ,Generazione di output con modello personalizzato ,Generazione di indicatori e pagine al vivo (PDF) , Generazione di PDF con sommario , indice e così via .
- **FMPS presenti:** Combinazione predefinita di Ditaval e file delle impostazioni . Invece di fornire file Ditaval e delle impostazioni separati, l’utente può creare un predefinito FMPS che può essere riutilizzato per le esigenze di pubblicazione.

**Nota:**  Se non selezioni alcuna delle impostazioni o del predefinito FMPS, FMPS eseguirà la pubblicazione con le impostazioni di sistema predefinite.

Se hai selezionato il predefinito FMPS e hai fornito anche il file Settings/Ditaval da AEM, questo è in conflitto e il predefinito FMPS ha la precedenza sul file Settings/Ditaval personalizzato.

### Pubblicazione della linea di base tramite FMPS:

È possibile pubblicare le linee di base già create con FMPS2020.0.2 o versione successiva.

**File di esempio delle impostazioni FMPS (file .sts) per iniziare:** [Collegamento](https://acrobat.adobe.com/link/track?uri=urn:aaid:scds:US:ef750752-7a7e-4e51-923e-6b7d9861ed54) (decomprimi questo file)

## Domande frequenti e risoluzione dei problemi:

- ### La pubblicazione di FMPS non riesce con &quot;Eccezione di timeout&quot;

Controlla e aumenta il valore di &quot;Timeout FMPS&quot; (secondi) in /system/console/configMgr/com.adobe.fmdita.config.ConfigManager&quot;

- ### Impossibile ottenere il predefinito FMPS nel menu a discesa

Verificare che nel server sia stato creato un predefinito FMPS predefinito e che le impostazioni di connessione siano corrette.

- ### Ricevo Blank PDF durante la pubblicazione.

Se si utilizza UUID, assicurarsi di aver selezionato &quot;Usa riferimenti basati su UUID&quot; in FrameMaker EditPreferences e viceversa per le guide AEM non-UUID

- ### Le mie impostazioni/Ditaval non vengono applicate nell&#39;output pubblicato finale

Accertatevi di non selezionare contemporaneamente il file Setting/Ditaval e il predefinito FMPS.Verificate l&#39;output manualmente utilizzando FrameMaker

- ### La linea di base non viene pubblicata da FMPS

La pubblicazione della linea di base è compatibile con FMPS2020.0.2 o versione successiva.\
Assicurati che la linea di base sia stata creata correttamente, per verificare vai a Mappa mappa download argomenti dashboard e seleziona &quot;Usa linea di base&quot;.

- ### L&#39;operazione di pubblicazione da FMPS richiede più tempo rispetto ad altri motori.

Ci sarà un&#39;intestazione fissa ideale di circa 3-4 minuti solo durante la pubblicazione da FMPS rispetto ad altri motori . Se pensi che sia più di questo, verifica con il tuo amministratore FMPS o contatta il supporto Adobe.

## Altre risorse:

### [Formazione e supporto per FMPS](https://helpx.adobe.com/support/framemaker-publishing-server.html)

### [Informazioni e supporto per AEM](https://helpx.adobe.com/in/support/xml-documentation-for-experience-manager.html)

### [Community FrameMaker e FMPS](https://community.adobe.com/t5/framemaker/ct-p/ct-framemaker?page=1&amp;sort=latest_replies&amp;lang=all&amp;tabid=all)

### [Comunità delle guide dell’AEM](https://experienceleaguecommunities.adobe.com/t5/experience-manager-guides/ct-p/aem-xml-documentation)
