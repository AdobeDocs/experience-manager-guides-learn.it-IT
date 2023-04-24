---
title: Plug-in di ossigeno per le guide di Adobe Experience Manager
description: Scopri come utilizzare il plug-in Oxygen per le guide Adobe Experience Manager per creare e gestire i contenuti.
hide: true
hidefromtoc: true
source-git-commit: 96347fed96979eb735dc55c32fcda90cc70ddcb4
workflow-type: tm+mt
source-wordcount: '5762'
ht-degree: 0%

---


# Plug-in di ossigeno per le guide di Adobe Experience Manager {#id1645H6010Q5}

Il plug-in Oxygen per le guide Adobe Experience Manager \(più avanti indicato come plugin Oxygen per le guide AEM nella guida\) consente di collegare l&#39;autore XML Oxygen con l&#39;archivio Adobe Experience Manager \(AEM\) per l&#39;authoring e la gestione dei contenuti. È possibile utilizzare il plug-in per sfogliare, cercare e aprire i file; file di check-out e check-in; carica cartelle e file AEM archivio. Il pannello Guide AEM nell&#39;applicazione desktop consente di contrassegnare le cartelle desiderate \(da AEM repository\) all&#39;elenco delle cartelle preferite per un accesso rapido. Inoltre, è possibile installare un pacchetto in AEM interfaccia Web e aprire i file DITA in Oxygen XML Author direttamente dall&#39;interfaccia Web AEM.

## Scarica e installa {#id1826M0L0PUI}

Il plugin Oxygen per le guide AEM è reso disponibile tramite il portale di distribuzione software di Adobe. Cerca &quot;ossigeno&quot; nella scheda Experience Manager e poi scarica il programma di installazione del plugin dal tuo [Portale di distribuzione software di Adobe](https://experience.adobe.com/#/downloads/content/software-distribution/en/general.html).

>[!NOTE]
>
>Controlla la compatibilità della versione del connettore ossigeno dalle note sulla versione per le specifiche guide di Adobe Experience Manager.

Una volta installato il programma di installazione, installalo sul computer locale in cui è installato l&#39;autore XML Oxygen. Prima di iniziare il processo di installazione, è necessario assicurarsi che il sistema soddisfi i requisiti tecnici per installare il plugin Oxygen per AEM Guide.

### Requisiti tecnici

- Oxygen XML Author versione 24.1

- Guide di Adobe Experience Manager versione 3.4 o successiva

- Adobe Experience Manager versione 6.5 con Service Pack 10, 11, 12 e 13

- Sistema operativo supportato da Oxygen XML Author versione 24.1

- Kit di sviluppo Java
   - Oracle SE 8 JRE 1.8

### Installa il plug-in su Windows

>[!IMPORTANT]
>
>Se nel sistema è installata una versione precedente del plug-in, assicurarsi di disinstallarla prima di avviare il processo di installazione. Consulta la sezione **Disinstallazione dei pacchetti** nella sezione [Come lavorare con i pacchetti](https://helpx.adobe.com/it/experience-manager/6-4/sites/administering/using/package-manager.html) articolo per le istruzioni di disinstallazione.

Esegui i seguenti passaggi sul sistema in cui è installato Oxygen XML Author:

1. Avvia il programma di installazione di `.exe` file.

   Viene visualizzata la schermata di benvenuto della procedura guidata di installazione.

1. Fai clic su **Successivo** e cercare il percorso in cui è disponibile il file .exe dell&#39;autore XML di Oxygen.

1. Selezionare il file e fare clic su **Apri**.

   Il percorso del file selezionato viene aggiunto nella procedura guidata di installazione.

1. Fai clic su **Avanti**.

1. Fai clic su **Installa**.

1. Fai clic su **Fine** per chiudere la procedura guidata di installazione.
1. Avvia Oxygen XML Author.

   Il pannello Guide AEM viene visualizzato in Oxygen XML Author.

   ![](images/oxygen-aem-connector.png)

   >[!NOTE]
   >
   >Se il pannello Guide AEM non viene visualizzato, vedere le soluzioni alternative nella sezione Risoluzione dei problemi—[Pannello Guide AEM mancanti](#id192BH200ZAX).


### Installare il plug-in su Mac

>[!IMPORTANT]
>
>Se nel sistema è installata una versione precedente del plug-in, assicurarsi di disinstallarla prima di avviare il processo di installazione. Consulta la sezione **Disinstallazione dei pacchetti** nella sezione [Come lavorare con i pacchetti](https://helpx.adobe.com/it/experience-manager/6-4/sites/administering/using/package-manager.html) istruzioni per la disinstallazione dell’articolo.

Esegui i seguenti passaggi sul sistema in cui è installato Oxygen XML Author:

1. Individua il file .dmg del plugin sul tuo sistema.

1. Fai doppio clic sul file .dmg per aprire il contenuto del file.

   Il file .dmg contiene una cartella aem-connector-x.x e un file di configurazione aem-connector-x.x.

   >[!NOTE]
   >
   >x.x nei nomi dei file è il numero di versione del plug-in.

1. Copia la cartella aem-connector-x.x nella cartella plugins di Oxygen XML Author.
1. Fai doppio clic sul file di installazione di aem-connector-x.x per avviare il programma di installazione.

1. Avvia Oxygen XML Author.

   Il pannello Guide AEM viene visualizzato in Oxygen XML Author.

   ![](images/oxygen-aem-connector-mac.png)

   >[!NOTE]
   >
   >Se il pannello Guide AEM non viene visualizzato, vedere le soluzioni alternative nella sezione Risoluzione dei problemi—[Pannello Guide AEM mancanti](#id192BH200ZAX).


### Installa il pacchetto per abilitare la funzionalità di modifica dei documenti da AEM&#39;interfaccia Web {#id182CE0Q0TY4}

In qualità di autore, è possibile aprire e modificare le mappe DITA o gli argomenti in Oxygen XML Author direttamente dall&#39;interfaccia Web AEM. Per abilitare questa funzione nell’interfaccia Web AEM, l’amministratore AEM deve installare un pacchetto nell’istanza di authoring di AEM.

In qualità di amministratore AEM, esegui i seguenti passaggi per installare il pacchetto:

1. Scarica il file .zip del pacchetto dal tuo team IT.
1. Accedi alla tua istanza AEM *\(in qualità di amministratore\)* e passa a Gestione pacchetti CRX. L’URL predefinito per accedere al gestore dei pacchetti è

   `http://<server name>:<port>/crx/packmgr/index.jsp`

   Gestione pacchetti gestisce i pacchetti nell’installazione AEM locale. Per ulteriori informazioni sull&#39;utilizzo di Gestione pacchetti, vedi [Come lavorare con i pacchetti](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developer-tools/package-manager.html?lang=en) nella documentazione AEM.

   ![](images/package-manager.png)

1. Per caricare il pacchetto Oxygen, fai clic su **Carica pacchetto**.
1. Nella finestra di dialogo Carica pacchetto, accedi al file del pacchetto Ossigeno scaricato al passaggio 1 e fai clic su OK.

   Il pacchetto viene caricato sulla tua istanza AEM.

1. Per avviare il processo di installazione, fare clic su **Installa**.

   ![](images/oxygen-package.png)

1. Nella finestra di dialogo Installa pacchetto , fai clic su **Installa**.
1. Al termine dell&#39;installazione, fai clic sul pulsante Home nell&#39;angolo superiore sinistro di CRX Package Manager.
1. Seleziona un file DITA nella cartella delle risorse.

   **Modifica in ossigeno** è disponibile nella barra degli strumenti. Per ulteriori informazioni sull’utilizzo di questa opzione, consulta [Apri argomento DITA in Oxygen XML Author da AEM interfaccia web](#id182CE0I905Z).

   >[!NOTE]
   >
   >La **Modifica in ossigeno** è visibile quando si seleziona un argomento DITA. Se selezioni più argomenti, l’opzione non sarà visibile.


## Configurare il plugin di ossigeno per le guide AEM {#id1826KF00AHS}

Dopo aver scaricato e installato il plug-in, è necessario configurare quanto segue per funzionare con il plug-in:

- **Impostazioni di autenticazione web**: Impostazioni per l&#39;autenticazione SSO nel plug-in per AEM Guide.
- **Impostazioni generali**: Impostazioni di connessione per il plug-in, ad esempio AEM URL del server, dettagli di accesso e così via.
- **Preferenza per la personalizzazione degli attributi di profiling**: Questa configurazione è necessaria per gli schemi di attributi di profiling per i set di documentazione.

### Impostazioni di autenticazione web

JxBrowser viene utilizzato per l&#39;autenticazione SSO dal plugin del connettore Oxygen. È un browser basato sul cromo. Per Java 9+ è necessario l&#39;accesso alle API non pubbliche e devi concedere esplicitamente questo accesso a JxBrowser. Per ulteriori dettagli, consulta [Risoluzione dei problemi JxBrowser](https://jxbrowser-support.teamdev.com/docs/guides/troubleshooting/issues.html).

Aggiorna i file specificati per configurare le impostazioni di autenticazione web nel plugin Oxygen per AEM Guide:

>[!NOTE]
>
>Esegui un backup del file prima di aggiornarlo.

**Per Mac e Ossigeno 24.1**

Aggiungi le seguenti righe in env.sh

```java
--illegal-access=permit\
--add-opens=java.desktop/javax.swing.plaf.basic=ALL-UNNAMED\
--add-exports=javafx.controls/com.sun.javafx.scene.control=ALL-UNNAMED\
--add-exports=javafx.graphics/com.sun.javafx.stage=ALL-UNNAMED\
--add-exports=javafx.graphics/com.sun.javafx.scene=ALL-UNNAMED\
--add-exports=javafx.graphics/com.sun.javafx.scene.traversal=ALL-UNNAMED\
--add-exports=javafx.graphics/com.sun.javafx.tk=ALL-UNNAMED\
--add-exports=javafx.graphics/com.sun.glass.ui=ALL-UNNAMED\
--add-opens=javafx.graphics/com.sun.glass.ui=ALL-UNNAMED\
--add-opens=javafx.graphics/javafx.stage=ALL-UNNAMED\
--add-opens=javafx.graphics/com.sun.javafx.tk.quantum=ALL-UNNAMED\
--add-exports=java.desktop/sun.awt=ALL-UNNAMED\
--add-opens javafx.swing/javafx.embed.swing=ALL-UNNAMED
```

Aggiungi le seguenti righe in ossigenoAuthor.sh

```java
-Djdk.module.illegalAccess=permit\-Djava.ipc.external=true\
```

**Per Windows e Ossigeno 24.1**

Aggiungi le seguenti righe in env.bat

```java
--illegal-access=permit --add-opens=java.desktop/javax.swing.plaf.basic=ALL-UNNAMED --add-exports=javafx.controls/com.sun.javafx.scene.control=ALL-UNNAMED --add-exports=javafx.graphics/com.sun.javafx.stage=ALL-UNNAMED --add-exports=javafx.graphics/com.sun.javafx.scene=ALL-UNNAMED --add-exports=javafx.graphics/com.sun.javafx.scene.traversal=ALL-UNNAMED --add-exports=javafx.graphics/com.sun.javafx.tk=ALL-UNNAMED --add-exports=javafx.graphics/com.sun.glass.ui=ALL-UNNAMED --add-opens=javafx.graphics/com.sun.glass.ui=ALL-UNNAMED --add-opens=javafx.graphics/javafx.stage=ALL-UNNAMED --add-opens=javafx.graphics/com.sun.javafx.tk.quantum=ALL-UNNAMED --add-exports=java.desktop/sun.awt=ALL-UNNAMED --add-opens javafx.swing/javafx.embed.swing=ALL-UNNAMED
```

Aggiungi le seguenti righe in ossigenoAuthor.bat

```java
-Djdk.module.illegalAccess=permit -Djava.ipc.external=true
```

>[!NOTE]
>
>È necessario eseguire l&#39;ossigeno da ossigenoAuthor.sh per Mac e ossigenoAuthor.bat per Windows come amministratore.

### Impostazioni generali

Esegui i seguenti passaggi per configurare le impostazioni di connessione nel plugin Oxygen per le guide Adobe Experience Manager:

1. Nel pannello Guide AEM, fai clic sull’icona delle impostazioni, quindi seleziona **Impostazioni**.

   ![](images/settings.png)

1. Specifica i seguenti dettagli:
   - **URL server**: URL del server AEM, ad esempio:

      ```http
      http[s]://<host>:<port>
      ```

      Nell&#39;URL di cui sopra, specifica il nome host e la porta del server in cui viene distribuito AEM server.

      >[!IMPORTANT]
      >
      >Se il server AEM è distribuito sulle porte 80 o 443, non è necessario specificarlo nell’URL.

   - **Autenticazione:** Scegli tra **Base \(Nome utente/Password\)** o **Autenticazione web**. Nel caso in cui selezioni **Base** autenticazione necessaria per immettere **Nome utente** e **Password** nella finestra di dialogo Preferenze.

      Se si seleziona Autenticazione Web, viene visualizzata la schermata Accesso AEM. Immetti le credenziali di accesso e fai clic sul pulsante **Accesso** pulsante . Una volta effettuato l’accesso, la schermata di accesso AEM viene chiusa e il pannello Guide AEM visualizza l’elenco dei file dal server AEM.

   - **Timeout connessione**: Specifica il tempo in secondi in cui il client attenderà una risposta dal server AEM. Se non viene ricevuta alcuna risposta dal server entro il tempo specificato, la richiesta viene terminata. Il valore predefinito è 20 secondi.

   - **Cartella locale**: Posizione nel computer locale in cui i file AEM archivio vengono memorizzati dopo il pagamento. Se si specifica una posizione che non esiste sull&#39;unità, il plug-in crea tale posizione.
   - **Apri file quando estratto**: Se selezionato, apre i file al momento del pagamento.
   - **Chiudi file durante l&#39;archiviazione**: Se selezionato, chiude i file al momento del check-in. Prima di chiudere il file, viene visualizzato un pop-up in cui è possibile specificare i commenti sulla versione.
   - **Mostra finestra di dialogo di archiviazione nel file di chiusura**: Se selezionato, alla chiusura di un file viene visualizzato un pop-up. Dal pop-up, è possibile scegliere di archiviare il file o di chiuderlo senza eseguire il check-in.
   - **File di estrazione automatica all’apertura**: Se selezionato, facendo doppio clic su un file viene automaticamente estratto e aperto per la modifica. Nel caso in cui il file sia già stato estratto, viene semplicemente aperto per la modifica. Se questa opzione non è selezionata, l&#39;apertura di un file su cui non è presente un blocco lo apre in modalità di sola lettura.
1. Fai clic su **OK**.

### Preferenza per la personalizzazione degli attributi di profiling {#id1827K0D0OHT}

È necessario configurare le preferenze in Oxygen XML Author per utilizzare l&#39;attributo di profilazione associato agli argomenti DITA nell&#39;archivio AEM.

Esegui i seguenti passaggi per configurare gli attributi di profiling:

1. In Oxygen XML Author, fai clic su **Opzioni** \> **Preferenze**.
1. In **Associazione del tipo di documento** scheda , seleziona **DITA**, quindi fai clic su **Estendi**.

   ![](images/document_type_association.png)

1. In **Classpath** , seleziona com.adobe.o2.connector nel **Utilizzare il caricatore di classe padre dal plug-in con ID** a discesa.

   ![](images/dita-extension.png)

1. In **Estensioni** , apporta le seguenti modifiche:
1. 
   - Fai clic su **Scegli** accanto al **Listener di stato dell&#39;estensione dell&#39;autore** sotto **Estensioni singole** e seleziona CustomAuthorExtensionStateListener - com.adobe.o2.framework.extn nel **Classe** elenco. Fai clic su **OK**.
- Fai clic su **Scegli** accanto al **Editor valore attributo personalizzato autore** sotto **Estensioni singole** e seleziona CustomValueEditor - com.adobe.o2.framework.extn nel **Classe** elenco. Fai clic su **OK**.
La schermata seguente mostra il **Estensione** scheda per argomenti DITA:

   ![](images/dita-topic-extension-tab.png)

1. Fai clic su **OK** in tutte le finestre di dialogo per salvare le modifiche.

### Configura estensione mappa DITA

La configurazione dell&#39;estensione della mappa DITA è necessaria per abilitare l&#39;apertura dei file della mappa in Oxygen XML Author direttamente dall&#39;interfaccia Web AEM. Queste configurazioni sono simili alle configurazioni per gli attributi di profiling eseguite nella procedura precedente.

Esegui i seguenti passaggi per configurare l’estensione mappa DITA:

1. In Oxygen XML Author, fai clic su **Opzioni** \> **Preferenze**.
1. In **Associazione del tipo di documento** scheda , seleziona **Mappa DITA**, quindi fai clic su **Estendi**.
1. In **Classpath** , seleziona com.adobe.o2.connector nel **Utilizzare il caricatore di classe padre dal plug-in con ID** a discesa.
1. In **Estensioni** , apporta le seguenti modifiche:
1. 
   - Fai clic su **Scegli** accanto al **Listener di stato dell&#39;estensione dell&#39;autore** sotto **Estensioni singole** e seleziona CustomDITAMapAuthorExtensionStateListener - com.adobe.o2.framework.extn nel **Classe** elenco. Fai clic su **OK**.
- Fai clic su **Scegli** accanto al **Editor valore attributo personalizzato autore** sotto **Estensioni singole** e seleziona CustomValueEditor - com.adobe.o2.framework.extn nel **Classe** elenco. Fai clic su **OK**.
- *\(Facoltativo\)* Se non si desidera risolvere i riferimenti durante l&#39;apertura di un file di mappa, è necessario eseguire la seguente configurazione aggiuntiva:

   Fai clic su **Scegli** accanto al **Referente** sotto **Estensioni singole** e seleziona CustomDITAMapReferenceResolver - com.adobe.o2.framework.extn nel **Classe** elenco. Fai clic su **OK**.

   La schermata seguente mostra il **Estensione** scheda:

   ![](images/dita-map-extension-tab.png)

1. Fai clic su **OK** in tutte le finestre di dialogo per salvare le modifiche.

## Utilizzare il plugin di ossigeno per le guide AEM {#id1826JG00WY4}

### Pannello Guide AEM

La schermata seguente mostra il pannello Guide AEM.

![](images/connector-panel.png)

**A**\) Mostra la barra di ricerca.

**B**\) Mostra la cartella Preferiti. Per impostazione predefinita è vuoto. È possibile aggiungere cartelle dall&#39;archivio AEM come preferito, le cartelle preferite vengono quindi mostrate qui.

**C**\) La cartella DAM mostra l&#39;archivio AEM. È possibile espandere e comprimere la visualizzazione cartelle.

**D**\) L&#39;icona Impostazioni \(ingranaggio\) con le seguenti opzioni:

- **Connetti**: Selezionare questa opzione per connettersi al server AEM. L&#39;opzione è disabilitata quando l&#39;autore XML Oxygen è connesso al server AEM.
- **Aggiorna**: Selezionare questa opzione per ottenere lo stato più recente dei file e della cartella dal repository AEM.

   >[!NOTE]
   >
   >Assicurati di salvare i file prima di aggiornarli. Quando selezioni **Aggiorna** viene visualizzato un avviso per salvare i file prima di aggiornarli. Se i file non sono stati salvati, puoi fare clic su **Annulla** e salvateli.

- **Impostazioni**: Puoi utilizzare questa opzione per aprire la finestra di dialogo Preferenze generali del plugin.
- **Logout**: Selezionare questa opzione per chiudere la connessione AEM server. Questa opzione è disponibile solo se si utilizza la modalità di autenticazione Web.

### Funzioni del menu di scelta rapida

Le funzioni del plugin Oxygen per AEM Guide sono disponibili facendo clic con il pulsante destro del mouse su una cartella o un file nell&#39;archivio AEM. Le funzioni disponibili per le cartelle sono diverse dai file. Ecco un elenco completo delle funzioni nel menu di scelta rapida Oxygen Plugin for AEM Guide :

- **Apri**: Apre il file selezionato o espande la cartella selezionata.
- **Apri in**: È possibile scegliere di aprire il file selezionato in Editor Web AEM Guide, Dashboard mappa o Editor mappa. Per ulteriori informazioni su queste opzioni, consulta [Apri file nell’editor AEM guide](#id195GH0V30KX).
- **Check-out**: Esegue il Check-Out di un file AEM repository. Per ulteriori dettagli, consulta [File di estrazione](#id195HC020TS4).
- **Check-out con dipendenti**: Esegue il Check-Out di un file con i relativi riferimenti diretti. Per ulteriori dettagli, consulta [File di estrazione](#id195HC020TS4).
- **Check-out con dipendenti di sola lettura**: Esegue il Check-Out del file selezionato insieme ai relativi dipendenti. Non è possibile apportare alcuna modifica ai file dipendenti. Per ulteriori dettagli, consulta [File di estrazione](#id195HC020TS4).
- **Annulla estrazione**: Annulla il file estratto, chiude il file dall’editor e ripristina le modifiche all’ultima versione del file salvato sul server.
- **Aggiorna**: In caso di un file, recupera la copia più recente del file dall’archivio AEM. Per una cartella, recupera la struttura della cartella e lo stato del file. Questo significa che viene aggiunto un file che verrà quindi mostrato nella vista AEM guide. Inoltre, se un file viene estratto AEM server, facendo un aggiornamento in Oxygen Autore mostrerà il file come estratto. Tuttavia, questo non aggiorna l’elenco dei file nel *File estratti nelle guide AEM* Visualizza.
- **Aggiorna file estratti**: Aggiorna l’elenco dei file estratti nella *File estratti nelle guide AEM* Visualizza. Se un file viene estratto AEM server, l&#39;esecuzione di un aggiornamento aggiornerà l&#39;elenco dei file estratti nel *File estratti nelle guide AEM* Visualizza. Tuttavia, se è stato aggiunto un nuovo file o lo stato di un file è stato modificato, non lo aggiorna nella vista ad albero AEM Guide. Per aggiornare lo stato dei file in AEM, è necessario eseguire un aggiornamento.
- **Check-in**: Archivia i file estratti. Per ulteriori dettagli, consulta [Archiviare un file](#id182CF0J0FHS).
- **Check-in con dipendenti**: Se hai estratto file con dipendenti, questa opzione controlla nel file principale insieme ai relativi dipendenti. Per ulteriori dettagli, consulta [Archiviare un file](#id182CF0J0FHS).
- **Crea cartella**: Crea una cartella nel repository AEM. Questa opzione è disponibile solo a livello di cartella.
- **Carica file\(s\)**: Carica uno o più file. Per ulteriori dettagli, consulta [Caricare file e cartelle](#id195HC03F03J).
- **Carica con dipendenti**: Carica i file DITA \(XML, DITA, Book map o DITA map\) con i relativi dipendenti. Per ulteriori dettagli, consulta [Caricare file e cartelle](#id195HC03F03J).
- **Carica cartella**: Carica una cartella sull&#39;archivio AEM. Per ulteriori dettagli, consulta [Caricare file e cartelle](#id195HC03F03J).
- **Aggiungi ai preferiti**: Aggiunge una cartella al *Preferiti* nel pannello Guide AEM. Si consiglia di aggiungere qui la cartella di lavoro, che rende più facile sincronizzare i file e lo stato del file da AEM.
- **Rimuovi dai preferiti**: Rimuove una cartella da *Preferiti*. Per ulteriori dettagli, consulta [Aggiungere o rimuovere i Preferiti](#id195HC04405P).
- **Visualizza metadati**: Mostra i metadati quali Classe DITA, Titolo del documento, Tipo, UUID e altre informazioni associate a un file. Per ulteriori dettagli, consulta [Visualizzare i metadati di un file](#id195GHN0H05C).
- **Visualizza versioni**: Mostra la cronologia delle versioni di un file. Per ulteriori dettagli, consulta [Visualizzare la cronologia delle versioni di un file](#id195GI000D5Q).

### Apri un file in Oxygen XML Author {#id195GHJ0A0UB}

Dopo aver effettuato la connessione all&#39;archivio AEM, è possibile aprire i file per la modifica nell&#39;autore XML Oxygen. Esegui i seguenti passaggi per aprire un file da modificare nell&#39;autore XML di Ossigeno:

1. Fate clic con il pulsante destro del mouse su un file nel pannello Guide AEM che desiderate aprire per la modifica.

1. Seleziona **Apri** dal menu di scelta rapida.

   Il file viene aperto nell&#39;editor di Oxygen XML Author.

   ![](images/guid-in-file-tab.png)

   Quando passi il puntatore del mouse sulla scheda di un file, viene visualizzato il percorso del server insieme al relativo UUID. Nella schermata precedente, viene evidenziato l’UUID del documento.


Se hai selezionato la **File di estrazione automatica all’apertura** l&#39;opzione \(nella finestra di dialogo Preferenze\), quindi all&#39;apertura di un file, il file viene estratto automaticamente ed è disponibile per la modifica. Per aprire un file, è possibile fare doppio clic sul nome di un file oppure fare clic con il pulsante destro del mouse sul nome del file e scegliere **Apri** dal menu di scelta rapida. Se questa opzione non è selezionata, il file viene aperto in modalità di sola lettura.

>[!NOTE]
>
>È inoltre possibile fare doppio clic su un file per aprirlo.

### Apri file nell’editor AEM guide {#id195GH0V30KX}

Per utilizzare gli editor disponibili in AEM guide, seleziona l’opzione richiesta dal menu di scelta rapida. Esegui i seguenti passaggi per utilizzare l&#39;editor AEM Guide al posto dell&#39;editor di Oxygen XML Author:

1. Fate clic con il pulsante destro del mouse su un file nel pannello Guide AEM che desiderate aprire per la modifica.

1. Seleziona **Apri in** dal menu di scelta rapida e scegli tra le seguenti opzioni:

   - **Editor argomenti web**: Se il file che si sta aprendo è un file .xml o .dita, è possibile aprirlo per la modifica nell&#39;Editor Web. Scegli la **Editor argomenti web** per aprire il file selezionato per la modifica nell&#39;editor Web.

   - **Dashboard mappa**: Puoi scegliere di modificare un file .ditamap nel dashboard mappa in cui puoi eseguire varie operazioni sul file mappa. Queste operazioni dipendono dal ruolo/gruppo a cui appartieni.

   - **Editor mappa DITA Web**: Se desideri aprire il file .ditamap da modificare nell’Editor mappa, scegli questa opzione. Utilizzando l&#39;opzione Editor mappa DITA è possibile aggiungere o rimuovere argomenti, aggiungere tabelle di relazioni ed eseguire altre operazioni sulla mappa.


### File di estrazione {#id195HC020TS4}

Quando estrai un file, questo viene memorizzato localmente sul tuo sistema e bloccato per la modifica nell&#39;archivio AEM. Esegui i seguenti passaggi per estrarre un file:

1. Fate clic con il pulsante destro del mouse su un file nel pannello Guide AEM.
1. Selezionare una delle opzioni seguenti:
   - **Check-out:** Esegue il Check-Out di un file AEM archivio e lo rende disponibile per la modifica.
   - **Check-out con dipendenti**: Esegue il Check-Out di un file con i relativi riferimenti diretti. Questa opzione consente di apportare modifiche alle pagine padre e figlio. Plug-in di ossigeno per AEM Guide supporta il check-out di un livello di dipendenti. Ad esempio, Mappa A fa riferimento all&#39;argomento A e l&#39;argomento A fa riferimento all&#39;argomento B. Quando si esegue il check-out della mappa A, l&#39;argomento A verrà estratto indipendentemente dal livello nella gerarchia del sommario. Tuttavia, non estrae l&#39;argomento B perché non è collegato direttamente dalla mappa A.
   - **Check-out con dipendenti di sola lettura**: Esegue il Check-Out di un file e ne scarica i dipendenti nel computer locale come copie di sola lettura. Non è possibile apportare alcuna modifica ai file dipendenti.

Se hai selezionato la **Apri file in estrazione** opzione \(nella finestra di dialogo Preferenze\), quindi dopo aver estratto un file, il file viene aperto automaticamente per la modifica.

Se hai selezionato la **File di estrazione automatica all’apertura** opzione \(nella finestra di dialogo Preferenze\), quindi all&#39;apertura del file il file viene estratto automaticamente e reso disponibile per la modifica. Per aprire un file, è possibile fare doppio clic sul nome di un file oppure fare clic con il pulsante destro del mouse sul nome del file e scegliere **Apri** dal menu di scelta rapida.

Quando un file viene estratto, l&#39;icona del file cambia per mostrare il relativo stato bloccato.

![](images/check-out-file.png)

Nella schermata precedente, un file estratto da un altro utente viene mostrato con un&#39;icona a forma di lucchetto nero \(A\). Il file estratto dall&#39;utente corrente viene visualizzato con un blocco di colore verde \(B\).

>[!NOTE]
>
>Se il file estratto viene eliminato o spostato in un&#39;altra cartella di AEM, viene visualizzato un messaggio di errore al momento dell&#39;archiviazione del file. Assicurati che il file estratto non venga spostato o eliminato utilizzando l&#39;interfaccia Web AEM.

### Archiviare un file {#id182CF0J0FHS}

Quando si archivia un file, la copia locale dal sistema viene memorizzata nell&#39;archivio AEM e il blocco sul file viene rimosso. Esegui i seguenti passaggi per archiviare un file:

1. Salva il file facendo clic su **File** \> **Salva**.

1. Fai clic con il pulsante destro del mouse su un file estratto e scegli una delle due opzioni seguenti:

   - **Consegna**: Archivia il file selezionato dal sistema locale in AEM archivio.
   - **Consegna con dipendenti:** Se hai estratto un file insieme ai relativi dipendenti, utilizza questa opzione per archiviare tutti i file dipendenti in un’unica operazione. Quando selezioni questa opzione, viene visualizzata la finestra di dialogo Archivia con tutti i file dipendenti. Fare clic su OK per archiviare tutti i file contemporaneamente.

   Se non hai estratto i file dipendenti e poi scegli questa opzione, verranno archiviati solo i file dipendenti estratti da \(separatamente\). Verrà visualizzato un elenco di file che non è stato possibile archiviare:

   ![](images/check-in-error.png)

   Si consiglia vivamente di non spostare un file estratto. Tuttavia, se un file estratto viene spostato in un percorso diverso, è necessario annullare il pagamento relativo a quel file. Se si desidera apportare aggiornamenti a quel file, quindi estrarre di nuovo il file, apportare modifiche e quindi archiviarlo nuovamente. Se tenti di archiviare un file che è stato spostato dalla posizione originale, riceverai un errore.

   Se un file dipendente viene estratto in AEM, il file dipendente non verrà visualizzato in Check-In con dipendenti nella finestra di dialogo Archivia. Per ottenere un elenco dei file dipendenti estratti in AEM, è necessario eseguire un aggiornamento della cartella.

   Allo stesso modo, se hai archiviato un file dipendente tramite AEM, l&#39;elenco dei file non viene aggiornato in Oxygen Author finché non esegui un aggiornamento e un aggiornamento della cartella File estratti-out. Se effettui un Check-in con Dipendenti con alcuni file sottoposti a Check-In tramite AEM, riceverai un errore nell’elenco dei file che non è stato possibile archiviare.

1. \(Facoltativo\) Nella finestra di dialogo Consegna, aggiungi un commento in **Commenti sulla versione** casella di testo.

   >[!NOTE]
   >
   >Questo commento viene visualizzato nella cronologia delle versioni AEM del file.

1. Fai clic su **OK**.

>[!NOTE]
>
>Se il file estratto viene eliminato o spostato in un&#39;altra cartella di AEM, viene visualizzato un messaggio di errore al momento dell&#39;archiviazione del file. Assicurati che il file estratto non venga spostato o eliminato utilizzando l&#39;interfaccia Web AEM.

### File estratti nella visualizzazione AEM guide

Quando si dispone in più cartelle, allora non è facile scoprire quanti file vengono estratti in un&#39;unica visualizzazione. AEM Guide fornisce i file estratti nella visualizzazione delle guide AEM che forniscono un&#39;istantanea completa dei file attualmente estratti. Utilizzando questa visualizzazione, è possibile individuare facilmente quali file sono stati controllati AEM repository utilizzando AEM Guide. Esegui i seguenti passaggi per accedere e lavorare con questa visualizzazione:

1. Fai clic su **Finestra** \> **Mostra visualizzazione** \> **File estratti nelle guide AEM**.

   Viene visualizzata la vista File estratti AEM visualizzazione Guide .

   ![](images/files-checkedout-view.png)

1. Fai clic con il pulsante destro del mouse su un file in questa visualizzazione per ottenere le seguenti opzioni:

   - [Apri](#id195GH0V30KX)
   - [Apri in](#id195GH0V30KX)
   - Annulla estrazione
   - [Consegna](#id182CF0J0FHS)
   - [Consegna con dipendenti](#id182CF0J0FHS)
   - [Visualizza metadati](#id195GHN0H05C)
   - [Visualizza versioni](#id195GI000D5Q)

**Note sui file estratti nella visualizzazione AEM guide:**

- La *File estratti nelle guide AEM* Visualizza mantiene le sessioni dell&#39;utente. Ciò significa che i file estratti dall&#39;utente corrente vengono memorizzati e mantenuti nella visualizzazione nelle stesse sessioni dell&#39;utente \(o cache\).

- Se l&#39;utente modifica le credenziali di accesso o il server AEM, i dati \(o cache\) del file estratto nella visualizzazione vengono reimpostati. L&#39;utente deve eseguire manualmente un *Aggiorna file estratti* su ogni cartella da cui i file sono stati precedentemente estratti. Per semplificare, è consigliabile aggiungere le cartelle di lavoro a *Preferiti* da dove puoi eseguire rapidamente un aggiornamento della cartella.

- È possibile ordinare l’elenco dei file in base ai nomi dei file, al titolo o al percorso. Se un nuovo file viene estratto, il file viene visualizzato in ordine ordinato nella visualizzazione.


### Caricare file e cartelle {#id195HC03F03J}

Esegui i seguenti passaggi per caricare file o cartelle:

1. Fate clic con il pulsante destro del mouse su una cartella nel pannello Guide AEM.
1. Selezionare una delle opzioni seguenti:
   - **Carica file\(s\)**: Seleziona questa opzione per caricare uno o più file nella cartella selezionata nell’archivio AEM. Nella finestra di dialogo Seleziona file \(s\) da caricare, seleziona i file e fai clic su **Apri**.
   - **Carica con dipendenti**: Selezionare questa opzione per caricare un file DITA con i relativi dipendenti. Nella finestra di dialogo Seleziona file da caricare, seleziona i file e fai clic su **Apri**.
   - **Carica cartella**: Seleziona questa opzione per caricare una cartella nell’archivio AEM. Nella finestra di dialogo Scegli , seleziona la cartella e fai clic su **Scegli**.

**Note aggiuntive sull’utilizzo dei file basati su UUID**:

Durante lo spostamento o la copia del contenuto dal sistema locale a AEM archivio, è necessario considerare i seguenti punti:

- Quando si caricano uno o più file, viene generato un nuovo UID per i file che non hanno alcun UUID. Questo UUID viene aggiunto nel `topic id` di un file DITA.

- Quando si copia una cartella, i riferimenti ai file \(all&#39;interno della cartella\) vengono aggiornati automaticamente in tutte le mappe DITA che fanno riferimento ai file in tale cartella.

- Quando si copia un file di mappa DITA, i riferimenti UUID all’interno del file di mappa non vengono modificati.

- Se un file o una cartella presenta un conflitto o un duplicato, viene generato un nome di file univoco per il nuovo file da copiare o spostare.

- Due file non possono avere lo stesso UUID. Un UUID univoco viene assegnato a tutti i nuovi file.

- Se un file viene caricato contemporaneamente da due utenti diversi, il file elaborato successivamente sovrascrive il file precedente. Tuttavia, tale pratica dovrebbe essere evitata.

- Quando estrai contenuto AEM archivio e apporti modifiche al sistema locale, assicurati che il nome del file non venga modificato al momento del caricamento del file.


### Aggiungere o rimuovere i Preferiti {#id195HC04405P}

Per aggiungere o rimuovere una cartella nella cartella Preferiti nel pannello Guide AEM, effettua le seguenti operazioni:

- Fai clic con il pulsante destro del mouse su una cartella e seleziona **Aggiungi ai preferiti**. È possibile aggiungere una cartella ai preferiti se non si trova nei Preferiti.
- È possibile rimuovere una cartella dai preferiti nei modi seguenti:
   - Fai clic con il pulsante destro del mouse su una cartella nel **Preferiti** e seleziona **Rimuovi dai preferiti**.
   - Fai clic con il pulsante destro del mouse su una cartella nell’archivio AEM in **DAM** cartella già aggiunta come preferita e seleziona **Rimuovi dai preferiti**.

### Visualizzare la cronologia delle versioni di un file {#id195GI000D5Q}

Esegui i seguenti passaggi per visualizzare la cronologia delle versioni di un file:

1. Fate clic con il pulsante destro del mouse su un file nel pannello Guide AEM.

1. Seleziona **Visualizza versioni** dal menu di scelta rapida.

   La cronologia delle versioni del file viene visualizzata nella finestra di dialogo Versioni.

   ![](images/version-history.png)


### Visualizzare i metadati di un file {#id195GHN0H05C}

Per visualizzare i metadati di un file, effettua le seguenti operazioni:

1. Fate clic con il pulsante destro del mouse su un file nel pannello Guide AEM.

1. Seleziona **Visualizza metadati** dal menu di scelta rapida.

   I metadati del file, quali Classe DITA, Stato documento, data di modifica, dimensione, Titolo e UUID, vengono visualizzati nella finestra di dialogo Metadati.

   ![](images/metadata.png)


## Cerca un argomento nell’archivio AEM {#id1826J20405Z}

Puoi cercare argomenti nell’archivio AEM utilizzando la barra di ricerca nel pannello Guide AEM. È possibile cercare nell’intera cartella DAM oppure selezionare una cartella e quindi cercare un argomento in tale cartella. Il risultato della ricerca mostra gli argomenti con testo corrispondente alla query di ricerca.

Esegui i seguenti passaggi per cercare gli argomenti:

1. Selezionare una cartella nell&#39;archivio AEM in cui si desidera cercare un argomento.
1. Inserisci la query di ricerca \(ad esempio, `introduction`\) nella barra di ricerca del plugin di ossigeno per le guide AEM.
1. Fare clic sul pulsante di ricerca o premere Invio.

   Il risultato viene visualizzato nella scheda Risultati ricerca come un elenco con il percorso del file. Se non vi sono risultati corrispondenti per la query di ricerca, nessun risultato trovato in &lt;path of=&quot;&quot; the=&quot;&quot; selected=&quot;&quot; folder=&quot;&quot;> viene visualizzato il messaggio.

   ![](images/search.png)

1. \(Facoltativo\) Fare doppio clic su un file nel risultato della ricerca per aprirlo in Oxygen XML Author.
1. Per tornare alla vista Archivio AEM, effettuare una delle seguenti operazioni:
   - Per visualizzare la vista Archivio AEM senza cancellare i risultati della ricerca, fare clic su **Sfoglia** scheda .
   - Per cancellare i risultati della ricerca e visualizzare l&#39;archivio AEM, fare clic sull&#39;icona Elimina ricerca.

## Apri argomento DITA in Oxygen XML Author da AEM interfaccia web {#id182CE0I905Z}

È possibile aprire e modificare l&#39;argomento DITA in Oxygen XML Author dall&#39;interfaccia Web AEM. Per abilitare questa opzione è necessario installare un pacchetto in AEM. Per ulteriori informazioni sull&#39;installazione del pacchetto, vedi [Installa il pacchetto per abilitare la funzionalità di modifica dei documenti da AEM&#39;interfaccia Web](#id182CE0Q0TY4).

>[!NOTE]
>
>La **Modifica in ossigeno** è accessibile da varie posizioni in AEM: quando viene selezionato un argomento, quando viene visualizzato un argomento in anteprima o dalla scheda Argomenti e rapporti della console mappa DITA. Se selezioni più argomenti, l’opzione non è visibile nella barra degli strumenti.

**Apri un argomento DITA**

Esegui i seguenti passaggi per aprire un argomento DITA in Oxygen XML Author:

1. Seleziona un argomento nelle risorse e fai clic su **Modifica in ossigeno** nella barra degli strumenti.

   >[!NOTE]
   >
   >Se l’argomento non è estratto, viene prima estratto e poi aperto in Ossigeno in modalità di modifica.

1. Seleziona autore XML ossigeno *&lt;version>* in **Applicazione Launch** finestra di messaggio. È possibile selezionare **Ricorda la mia scelta per i collegamenti AEM** per salvare la preferenza.

**Modificare un argomento DITA**

Esegui i seguenti passaggi per modificare un argomento DITA in Oxygen XML Author:

1. Seleziona ed effettua il check-out di un argomento nelle risorse.
1. Fai clic su **Modifica in ossigeno** nella barra degli strumenti.

   >[!NOTE]
   >
   >Se l’argomento non è estratto, viene prima estratto e poi aperto in Ossigeno in modalità di modifica.

1. Seleziona autore XML ossigeno *&lt;version>* in **Applicazione Launch** finestra di messaggio. È possibile selezionare **Ricorda la mia scelta per i collegamenti AEM** per salvare la preferenza.
1. Modifica l&#39;argomento in Oxygen XML Author.
1. Controlla l&#39;argomento dal plugin di Ossigeno per le Guide AEM.

   Per ulteriori informazioni sul check-in di un argomento che utilizza il plugin Oxygen per AEM Guide, vedi [Archiviare un file](#id182CF0J0FHS).

   >[!NOTE]
   >
   >Assicurati di archiviare l&#39;argomento utilizzando il plugin Oxygen per AEM Guide, se effettui il check-in dall&#39;interfaccia web AEM, le modifiche apportate in Oxygen XML Author non vengono salvate nella versione archiviata dell&#39;argomento.


## Utilizzare i profili di attributi {#id1827JA002YK}

AEM Guide consente di creare e associare facilmente gli attributi condizionali utilizzando gli attributi DITA pertinenti. Puoi definire gli attributi condizionali a livello globale o a livello di cartella. Le condizioni definite a livello globale sono visibili in tutti i progetti e le condizioni a livello di cartella sono visibili solo nei progetti creati all’interno della cartella specificata. Gli autori di contenuti possono utilizzare questi attributi condizionali per condizionare il contenuto dei loro argomenti o mappe DITA creati o utilizzati. Per ulteriori informazioni su come creare attributi condizionali in AEM utilizzando le Guide AEM, consulta *Configurare gli attributi condizionali per i profili globali o a livello di cartella* in Installare e configurare le guide di Adobe Experience Manager.

>[!NOTE]
>
>Assicurati di aver aggiunto gli attributi condizionali in AEM e di aver impostato [Preferenza per la personalizzazione degli attributi di profiling](#id1827K0D0OHT) prima di aggiungere attributi condizionali al contenuto.

Esegui i seguenti passaggi per aggiungere attributi condizionali al contenuto in Oxygen XML Author:

1. Estrai e apri un argomento dal *Plug-in di ossigeno per AEM guide*.
1. Seleziona la parte del contenuto in cui desideri applicare gli attributi condizionali.
1. Fare doppio clic sull&#39;attributo condizionale nel pannello Attributi dell&#39;autore XML di ossigeno.

   ![](images/attribute-panel.png)

1. In **Disponibile** nella colonna della finestra di dialogo Modifica attributo, seleziona gli attributi\(s\) e fai clic su **Aggiungi**.

   Viene visualizzata la seguente schermata `audience` attributi.

   ![](images/edit-attributes.png)

1. Fai clic su **OK**.

   Gli attributi vengono aggiunti al contenuto.


## Risoluzione dei problemi comuni {#id188ABC00RY4}

Questo argomento tratta alcuni dei problemi più comuni che potresti riscontrare durante l’utilizzo del plugin, insieme alle relative soluzioni.

### Pannello Guide AEM mancanti {#id192BH200ZAX}

**Problema** - Se il pannello Guide AEM non viene visualizzato in Oxygen XML Author, prova le seguenti soluzioni:

Soluzione 1:

1. In Oxygen XML Author, abilita il plug-in.

   Fai clic su **Opzioni** \> **Preferenze** \> **Plug-in** e seleziona **Plug-in di ossigeno per le guide di Adobe Experience Manager.**

1. Riavvia L&#39;Autore XML Dell&#39;Ossigeno.


Soluzione 2:

1. Se il pannello Guide AEM non viene ancora visualizzato, abilitare la finestra Guide AEM.

   Nell&#39;Autore XML Di Ossigeno, Fai Clic Su **Finestra** \> **Mostra visualizzazione** \> **Guide AEM**.

Soluzione 3:

1. Disinstalla e reinstalla il plug-in Oxygen per le guide Adobe Experience Manager.

   - Su Windows, disinstalla il plug-in da **Aggiungere o rimuovere programmi** elenco. Quindi, reinstalla il plug-in.

   - Su Mac, accedi alla cartella aem-connector-x.x nella cartella plugins di Oxygen XML Author e spostala in **Cestino**. Quindi, svuota il **Cestino** cartella.


### Configura la porta per la trasformazione DITA-OT

**Problema** - Quando si esegue una trasformazione DITA-OT su file elaborati dal plugin, la trasformazione non riesce con il seguente errore:

![](images/proxy-server-path-error-new.png)

**Soluzione** - Questo problema è stato risolto aggiungendo un server proxy tra DITA-OT e il plugin. Questo server proxy elabora e condivide tutti i file richiesti da DITA-OT per le trasformazioni. La porta predefinita su cui è stato configurato il server è: `5972`. Se si utilizza questa porta per un altro server, è possibile specificare una porta diversa per il server proxy.

Esegui i seguenti passaggi per modificare la porta predefinita del server proxy:

1. Individua la directory principale \(user&#39;s\).
1. Crea un file denominato aem\_connector\_proxy.
1. Apri il file in qualsiasi editor di testo e aggiungi un numero di porta disponibile nella prima riga del file.
1. Salva e chiudi il file 
1. Riavvia l&#39;autore XML dell&#39;ossigeno ed esegui la trasformazione DITA-OT.


### AEM pannello Guide non sfoglia il percorso del file aperto

Problema: Quando si sceglie di aprire un file per la modifica in Oxygen XML Author da AEM server, il file viene aperto per la modifica in Oxygen XML Author. Tuttavia, AEM pannello Guide non mostra la posizione del file nella struttura di navigazione.

Soluzione: Questo problema è stato osservato in scenari in cui il percorso del file contiene /content/dam due volte in esso. Per impostazione predefinita, tutte le risorse in AEM sono memorizzate nella cartella /content/dam. Se carichi o crei una struttura di cartelle che contiene anche /content/dam, questo problema viene osservato. È possibile eseguire tutte le operazioni normali su tali file, tuttavia la loro posizione all’interno della struttura di navigazione non viene visualizzata per impostazione predefinita. Per accedere a tale file nella struttura di navigazione, è necessario individuare manualmente la posizione del file. Nella struttura di navigazione il percorso /content/dam duplicato viene sostituito con /content/assets.

### Configurare la registrazione

Problema: Per impostazione predefinita, il plugin Oxygen per le guide AEM non genera alcun log, il che rende difficile il debug di qualsiasi scenario di errore.

Soluzione: Esegui i seguenti passaggi per abilitare la funzione di generazione dei registri nel plugin:

1. Individua il percorso di installazione dell&#39;autore XML Oxygen.

1. Apri il file ossigenoAuthor19.1.vmoptions in un editor di testo.

   >[!NOTE]
   >
   >Il numero di versione del file potrebbe variare in base al numero di versione dell&#39;applicazione installata sul sistema.

1. Aggiungi la seguente riga nel file :

   ```java
   -Djava.util.logging.config.file=./log.properties
   ```

1. Salva e chiudi il file 

1. Nella stessa posizione, crea un file denominato log.properties con il seguente contenuto:

   ```java
   handlers=java.util.logging.FileHandler
   java.util.logging.FileHandler.level = DEBUG
   java.util.logging.FileHandler.limit = 1048576
   java.util.logging.FileHandler.count = 5
   java.util.logging.FileHandler.pattern = %h/aem-plugin%g.log
   java.util.logging.FileHandler.formatter = java.util.logging.SimpleFormatter
   java.util.logging.FileHandler.format=[%1$tF %1$tT] [%4$s] %5$s %n
   ```

1. Salva e chiudi il file 
1. Avvia l&#39;autore XML dell&#39;ossigeno.


Il plug-in ora crea i registri nella home directory dell&#39;utente con il nome file aem-pluginX.log \(*dove X indica il numero di rotazione*\).