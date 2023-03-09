---
title: FMPS e guide AEM
description: Pubblicazione con FMPS tramite AEM Guides
source-git-commit: 82f010a97d0ed0e3c6351e6411e5955c79e0b01f
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---


# FrameMaker Publishing Server (FMPS) e guide AEM

**L&#39;integrazione di AEM Guides con FrameMaker Publishing Server potrebbe essere la soluzione ideale per la pubblicazione automatizzata di alta qualità.\
L’articolo seguente ti aiuterà a configurare ed eseguire FMPS con le guide AEM.**

## Compatibilità di FMPS con le guide AEM:

- Compatibilità con il punto 4.1 delle guide AEM: [Collegamento](https://experienceleague.adobe.com/docs/experience-manager-guides-learn/tutorials/release-info/release-notes/on-prem-release-notes/release-notes-4.1.html?lang=en/#compatibility-matrix)
- Compatibilità con le guide AEM 4.0: [Collegamento](https://helpx.adobe.com/xml-documentation-for-experience-manager/release-note/release-notes-xml-documentation-solution-4-0.html/#Compatibility%20matrix)
- Versione futura: [Collegamento](https://experienceleague.adobe.com/docs/experience-manager-guides-learn/tutorials/release-info/latest-release-info.html?lang=en)

## Installazione:

### Guide AEM:

Per informazioni sull&#39;installazione e la configurazione, vedere: [Collegamento](https://helpx.adobe.com/content/dam/help/en/xml-documentation-solution/4-1-2/Adobe-Experience-Manager-Guides_Installation-Configuration-Guide_EN.pdf)

### FMPS:

Per l&#39;installazione di FMPS è possibile fare riferimento a [Collegamento video](https://www.youtube.com/watch?v=2deelyM5VA8&amp;t) o [Documentazione](https://help.adobe.com/en_US/framemaker/server/index.html#t=fmps-user-guide%2Finstall_config_fmps.html%23install_config_fmps&amp;rhtocid=_2)

## Configurazioni richieste:

Il contenuto DITA può essere emesso utilizzando FrameMaker Publishing Server (FMPS). È possibile creare l&#39;output in qualsiasi formato supportato da FMPS. Nella console web, modifica le seguenti proprietà del bundle com.adobe.fmdita.config.ConfigManager per configurare le guide AEM per l’utilizzo di FMPS.

Per aprire la console Web, vai all&#39;URL Accesso http://\&lt;server name=&quot;&quot;>:\&lt;port>/system/console/configMgr.

**Proprietà di configurazione e relativa descrizione:** [Collegamento](https://helpx.adobe.com/content/dam/help/en/xml-documentation-solution/4-1-2/Adobe-Experience-Manager-Guides_Installation-Configuration-Guide_EN.pdf#page=89)

## Test in esecuzione:

Utilizzando FMPS, puoi pubblicare automaticamente **PDF, Responsive HTML5**, e **Epub** per le risorse DITA e FM.

Dal menu &quot;Generate PDF using&quot; (Genera utilizzando), scegliete FrameMaker Publishing Server.

L’utente può fornire &quot;settings File(.sts)&quot; e &quot;ditaval. Il filtro verrà eseguito utilizzando ditaval in base alle condizioni specificate.

- **file di impostazione**: impostazione FrameMaker /FMPS Publish che contiene tutte le impostazioni che si desidera vengano rispettate da FMPS durante la pubblicazione. Ad esempio: generazione dell&#39;output con il modello personalizzato, generazione di indicatori e pagine al vivo (PDF), generazione di PDF con sommario, indice e così via.
- **Predefinito FMPS:** Combinazione predefinita di file ditaval e impostazioni. Anziché fornire file ditaval e impostazioni separati, l’utente può precreare un predefinito FMPS che può essere riutilizzato per le esigenze di pubblicazione.

**Nota:** Se non si seleziona nessuna delle impostazioni o del predefinito FMPS, FMPS verrà pubblicato con le impostazioni di sistema predefinite.

Se hai selezionato il predefinito FMPS e hai fornito anche un file di impostazioni/ditaval da AEM, questo entrerà in conflitto e il predefinito FMPS avrà la precedenza su impostazioni personalizzate/file ditaval.

### Pubblicazione della linea di base tramite FMPS:

È possibile pubblicare le linee di base già create con FMPS2020.0.2 o versione successiva.

**File di esempio delle impostazioni FMPS (file .sts) per iniziare:** [Collegamento](https://acrobat.adobe.com/link/track?uri=urn:aaid:scds:US:ef750752-7a7e-4e51-923e-6b7d9861ed54) (decomprimi questo file)

## Domande frequenti e risoluzione dei problemi:

- La pubblicazione FMPS non riesce con &quot;Timeout Exception&quot;.

Controlla e aumenta il valore di &quot;Timeout FMPS&quot; (secondi) in /system/console/configMgr/com.adobe.fmdita.config.ConfigManager&quot;

- Impossibile ottenere il predefinito FMPS nel menu a discesa.

Verificare che sul server sia stato creato un predefinito FMPS predefinito e che le impostazioni di connessione siano corrette.

- Ricevo PDF vuoti durante la pubblicazione.

Se si utilizza UUID, assicurarsi di aver selezionato &quot;Usa riferimenti basati su UUID&quot; in Preferenze di modifica di FrameMaker e viceversa per le guide AEM non UUID.

- Le mie impostazioni/ditaval non vengono applicate nell&#39;output pubblicato finale.

Accertatevi di non selezionare contemporaneamente il file di impostazione/ditaval e il predefinito FMPS. Verificare l&#39;output manualmente utilizzando FrameMaker.

- La linea di base non viene pubblicata da FMPS.

La pubblicazione della linea di base è compatibile con FMPS2020.0.2 o versione successiva.\
Assicurati che la linea di base sia stata creata correttamente, per verificare vai a Mappa mappa download argomento dashboard e seleziona &quot;Usa linea di base&quot;.

- La pubblicazione delle attività da FMPS richiede più tempo rispetto ad altri motori.

Ci sarà un&#39;intestazione fissa ideale di circa 3-4 minuti solo durante la pubblicazione da FMPS rispetto ad altri motori, se pensi che sia più di questo, verifica con il tuo amministratore FMPS o contatta il supporto Adobe.

## Altre risorse:

[Formazione e supporto per FMPS](https://helpx.adobe.com/support/framemaker-publishing-server.html)

[Informazioni e supporto per AEM](https://helpx.adobe.com/in/support/xml-documentation-for-experience-manager.html)

[Community FrameMaker e FMPS](https://community.adobe.com/t5/framemaker/ct-p/ct-framemaker?page=1&amp;sort=latest_replies&amp;lang=all&amp;tabid=all)

[Community delle guide dell’AEM](https://experienceleaguecommunities.adobe.com/t5/experience-manager-guides/ct-p/aem-xml-documentation)
