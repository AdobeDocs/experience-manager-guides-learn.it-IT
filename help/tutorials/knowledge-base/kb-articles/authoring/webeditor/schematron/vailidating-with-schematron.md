---
title: Supporto di Schematron in webeditor
description: Utilizzo di Schematron nell'editor web
source-git-commit: 2a036ec628424f0dedfdb69a5e860906ca100cc6
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---


# Controllo della qualità dei contenuti all’interno dell’editor web

Questo articolo offre una panoramica delle possibilità di convalida all’interno dell’editor web AEM Guide .
Mediante la progettazione dell&#39;editor web sfrutta la configurazione dello schema DITA nel sistema per imporre agli utenti di creare contenuto compatibile con DITA. In questo modo, tutto il contenuto memorizzato nel sistema è strutturato, riutilizzabile e valido contenuto DITA.

Oltre al supporto per le regole DITA, l&#39;editor web supporta anche la convalida del contenuto basato su &quot;*Schematro*&quot; regole.

&quot;*Schematro*&quot; si riferisce a un linguaggio di convalida basato su regole utilizzato per definire i test per un file XML. È possibile importare i file Schematron e modificarli in Web Editor. Utilizzando un file &quot;Schematron&quot; è possibile definire determinate regole e quindi convalidarle per un argomento DITA o una mappa. Le regole dello schema possono garantire la coerenza della struttura XML imponendo restrizioni definite come regole. Tali restrizioni sono guidate dalle PMI che possiedono la qualità e la coerenza dei contenuti.

    NOTA: L’editor web supporta lo schema ISO.


## Sapere come funziona &quot;Schematron&quot; nell&#39;editor web

### Configurazione delle regole di Schematron

Fare riferimento alla sezione &quot;Supporto per i file Schematron&quot; nella sezione [Guida utente](https://helpx.adobe.com/content/dam/help/en/xml-documentation-solution/4-2/Adobe-Experience-Manager-Guides_UUID_User-Guide_EN.pdf#page=148)


### Applica regole di convalida al salvataggio dei file

Le impostazioni di Webeditor consentono agli utenti di configurare le regole/file di Schematron che verranno eseguiti ogni volta che un utente aggiorna il contenuto. Per ulteriori dettagli consulta la sezione &quot;Convalida&quot; in [Guida utente](https://helpx.adobe.com/content/dam/help/en/xml-documentation-solution/4-2/Adobe-Experience-Manager-Guides_UUID_User-Guide_EN.pdf#page=58)

![Impostare le regole dalle impostazioni dell&#39;editor web](../../../assets/authoring/schematron-editorsettings-validation-tab.png)


### È possibile eseguire la convalida manualmente?

Sì, in qualità di autore/utente durante la creazione di contenuti puoi utilizzare il pannello Schematron nell’editor web per caricare un file di schema ed eseguire convalide sul file aperto nell’editor.

    Affinché ciò funzioni, l’amministratore del profilo di cartella deve consentire a tutti gli utenti di aggiungere file di schema nel pannello Convalida. Vedi le impostazioni dell&#39;editor (schermata precedente)

![Scegliere il file Schematron](../../../assets/authoring/schematron-rightpanel-validation-addsch.png)
![Esegui convalida](../../../assets/authoring/schematron-rightpanel-validation-runsch.png)


### Regole supportate

La versione corrente di AEM Guide supporta la convalida solo utilizzando regole basate su &quot;Assertion&quot;. (vedi [risorsa e rapporto](https://schematron.com/document/205.html)) Eventuali regole basate su &quot;Report&quot; non sono ancora supportate.


### Esempi e ulteriori informazioni sulle regole di Schematron

#### Casi di utilizzo di esempio

- Controlla se un collegamento è esterno e se ha ambito &quot;esterno&quot;

   ```
   <sch:pattern>
       <sch:rule context="xref[contains(@href, 'http') or contains(@href, 'https')]">
           <sch:assert test="@scope = 'external' and @format = 'html'">
               All external xref links must be with scope='external' and format='html'
           </sch:assert>
       </sch:rule>
   </sch:pattern>
   ```

- Controlla se c&#39;è almeno un &quot;topicref&quot; in una mappa o almeno un &quot;li&quot; sotto un &quot;ul&quot;

   ```
   <sch:pattern>
       <sch:rule context="map">
           <sch:assert test="count(topicref) > 0">
               There should be atleast one topicref in map
           </sch:assert>
       </sch:rule>
   
       <sch:rule context="ul">
           <sch:assert test="count(li) > 1" >
               A list must have more than one item.
           </sch:assert>
       </sch:rule>
   </sch:pattern>
   ```

- L&#39;elemento &quot;indexterm&quot; deve essere sempre presente in un &quot;prolog&quot;

   ```
   <sch:pattern>
       <sch:rule context="*[contains(@class, ' topic/indexterm ')]">
           <sch:assert test="ancestor::node()/local-name() = 'prolog'">
               The indexterm element should be in a prolog.
           </sch:assert>
       </sch:rule>
   </sch:pattern>
   ```

#### Riferimenti

- Comprensione  [Nozioni di base sullo schema](https://da2022.xatapult.com/#what-is-schematron)
- Ulteriori informazioni [Regole di asserzione in Schematron](https://www.xml.com/pub/a/2003/11/12/schematron.html#Assertions)
- [Esempio di file di schema](../../../assets/authoring/sample_schematron.sch)