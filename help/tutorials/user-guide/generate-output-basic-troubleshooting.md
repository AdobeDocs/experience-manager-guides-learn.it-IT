---
title: Risoluzione dei problemi di base
description: Scopri come risolvere i problemi di base
source-git-commit: 7cd719921e68ac1763d09d9665d912e3697e5849
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---


# Risoluzione dei problemi di base {#id1821I0Y0G0A}

Durante l&#39;utilizzo delle AEM guide, è possibile che si verifichino errori durante la pubblicazione o l&#39;apertura del documento. Tali errori potrebbero essere nella mappa DITA, nell&#39;argomento o nel processo AEM Guide stesso. Questa sezione fornisce informazioni su come accedere e analizzare le informazioni nel file di registro di generazione dell&#39;output. Inoltre, se l&#39;argomento DITA è troppo grande, è possibile che venga visualizzato l&#39;errore di compilazione JSP. Questa sezione fornisce anche informazioni su come risolvere l&#39;errore di compilazione JSP.

## Visualizza e controlla il file di registro {#id1822G0P0CHS}

Esegui i seguenti passaggi per visualizzare e controllare il file di registro della generazione dell&#39;output:

1. Dopo aver avviato il processo di generazione dell&#39;output, fai clic su **Uscite** nella console mappa DITA.

   La **Generale** della colonna **Uscite generate** mostra le icone per fornire un&#39;indicazione visiva del successo o del fallimento della generazione dell&#39;output.

   ![](images/output-general-settings.png)

   Nella schermata precedente, la prima e la terza icona mostrano la generazione di output non riuscita. La seconda icona mostra una generazione di output di successo ma con i messaggi. L’ultima è una generazione di output di successo senza alcun messaggio.

1. Fai clic sul collegamento nel **Generato a** al termine del processo.

   Il file di registro si apre in una nuova scheda.

   ![](images/log-file.png)

1. Applica i seguenti filtri per evidenziare il testo nel file di log:
   - Fatale: Evidenzia gli errori fatali nel file di log con colore rosa.
   - Errore: Evidenzia gli errori nel file di log con colore arancione.
   - Avviso: Evidenzia le avvertenze nel file di log con colore viola.
   - Informazioni: Evidenzia i messaggi informativi nel file di registro con colore blu.
   - Eccezione: Evidenzia le eccezioni nel file di log con colore giallo.
1. Utilizza i pulsanti di navigazione su e giù per passare al testo evidenziato nel file di registro.

   In alternativa, scorri il file di registro e controlla i messaggi.


## Copia e controlla il file di registro in un editor di testo

Esegui i seguenti passaggi per copiare e controllare il file di registro della generazione di output in un editor di testo:

1. Dopo aver avviato il processo di generazione dell&#39;output, fai clic su **Uscite** nella console mappa DITA.

1. Fai clic sul collegamento nel **Generato a** al termine del processo.

   Il file di registro si apre in una nuova scheda.

1. Fai clic su **Copia registro** pulsante . Il file di registro viene copiato negli Appunti.
1. Apri un editor di testo e incolla il file di registro nell’editor.

1. Scorri il file di registro e controlla i messaggi.

   Le seguenti informazioni sono utili per determinare se si verifica un errore nel file DITA o nel processo Guide AEM:

   - *Errore relativo al file mappa DITA*: Nel caso in cui si verifichi un errore nel file di mappa DITA o in qualsiasi altro file contenuto nella mappa DITA, il file di registro conterrà una stringa &quot;BUILD FAILED&quot;. Puoi controllare le informazioni fornite nel file di registro per individuare il file errato e risolvere il problema.

      Nel seguente frammento di file di registro di esempio, puoi vedere il `BUILD FAILED` insieme al motivo dell’errore.

      ![](images/dita-error-in-log-file.png)

      - *Errore relativo alle AEM*: L’altro tipo di errore che è possibile identificare nel file di registro è relativo al processo Guide AEM. In questo caso, il file di mappa DITA viene analizzato correttamente, ma il processo di generazione dell&#39;output non riesce a causa di qualche errore interno nelle guide AEM. Per questo tipo di errori, è necessario chiedere aiuto al team di supporto tecnico.

         Nel seguente frammento di file di registro di esempio, puoi vedere il `BUILD SUCCESSFUL` , seguito da un altro errore tecnico.

         ![](images/process-error-in-log-file.png)


## Risoluzione dell&#39;errore di compilazione JSP

Se l&#39;argomento DITA è troppo grande, è possibile che venga visualizzato l&#39;errore di compilazione JSP \(`org.apache.sling.api.request.TooManyCallsException`\) nel browser. Questo errore potrebbe essere visualizzato quando si apre un argomento per la modifica, la revisione o la pubblicazione.

Esegui i seguenti passaggi per risolvere il problema:

1. In Navigazione globale, selezionare Strumenti e scegliere Operazioni \> Console Web.

   Viene visualizzata la pagina Configurazione della console Web di Adobe Experience Manager.

1. Cerca e fai clic su *Servlet principale Apache Sling* componente.

   Vengono visualizzate le opzioni configurabili per il servlet principale Apache Sling.

1. Aumenta il valore per *Numero di chiamate per richiesta* in base alle tue esigenze.


**Argomento principale:**[ Generazione di output](generate-output.md)

