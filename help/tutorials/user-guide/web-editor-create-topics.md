---
title: Creazione di argomenti
description: Scopri come creare argomenti
source-git-commit: cc0fbca257d82cc82db5b5da8d263309fd71de55
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---


# Creazione di argomenti {#id2056AL00O5Z}

AEM Guide consente di creare argomenti DITA di tipo: argomento, attività, concetto, riferimento, glossario, DITAVAL e altro ancora. Oltre a creare argomenti basati sui modelli predefiniti, puoi anche definire modelli personalizzati. Per ulteriori informazioni sull&#39;utilizzo dei modelli DITA personalizzati, vedere *Configurare modelli e tag per la creazione* in Installare e configurare le guide di Adobe Experience Manager as a Cloud Service.

Esegui i seguenti passaggi per creare un argomento:

1. Nell’interfaccia utente Assets, individua il percorso in cui desideri creare l’argomento.

1. Per creare un nuovo argomento, fai clic su **Crea** \> **Argomento DITA**.

1. Nella pagina Blueprint selezionare il tipo di documento DITA che si desidera creare e fare clic su **Successivo**.

   ![](images/create_dita_topic.png){width="800" align="left"}

   Per impostazione predefinita, AEM Guide fornisce i modelli di argomenti DITA più comunemente utilizzati. Puoi configurare più modelli di argomento in base ai requisiti organizzativi, vedi *Configurare modelli e tag per la creazione* in Installare e configurare le guide di Adobe Experience Manager as a Cloud Service.

   >[!NOTE]
   >
   > Nella vista a elenco dell’interfaccia utente Assets, il tipo di argomento DITA viene visualizzato nella colonna Tipo come Argomento, Attività, Concetto, Riferimento, Glossentry o DITAVAL. La mappa DITA viene visualizzata come mappa.

1. Nella pagina Proprietà, specifica il documento **Titolo**.

1. \(Facoltativo\) Specificare il file **Nome**.

   Se l’amministratore ha configurato il nome file automatico in base all’impostazione UID, non verrà visualizzata l’opzione per specificare il nome file. Al file viene assegnato automaticamente un nome di file basato su UUID.

   Se l’opzione di denominazione del file è disponibile, viene suggerito automaticamente anche il nome in base alla **Titolo** del documento. Se si desidera specificare manualmente il nome del documento, assicurarsi che il **Nome** non contiene spazi, apostrofo o parentesi graffe e termina con .xml o.dita. Per impostazione predefinita, AEM Guide sostituisce tutti i caratteri speciali con i trattini. Per le best practice relative alla denominazione dei file DITA, consulta la sezione Filenames nella guida Best practice .

1. Fai clic su **Crea**. Viene visualizzato il messaggio Argomento creato.

   È possibile scegliere di aprire l&#39;argomento per la modifica nell&#39;editor Web o salvare il file dell&#39;argomento nell&#39;archivio AEM.

   Ogni nuovo argomento creato dall’interfaccia utente Assets **Crea** \> **Argomento DITA** oppure all’Editor web viene assegnato un ID argomento univoco. Il valore di questo ID è il nome del file stesso. Inoltre, un nuovo documento viene salvato come ultima copia di lavoro dell’argomento in DAM. Fino a quando non si salva una revisione di un argomento appena creato, non verrà visualizzato alcun numero di versione nella cronologia delle versioni. Se apri l’argomento per la modifica, le informazioni sulla versione vengono visualizzate nell’angolo superiore destro della scheda del file dell’argomento:

   ![](images/topic-version-none_cs.png){width="550" align="left"}

   Le informazioni sulla versione di un argomento appena creato vengono visualizzate come *nessuno*. Quando si salva una nuova versione, viene assegnato un numero di versione pari a 1.0. Per ulteriori informazioni sul salvataggio di una nuova versione, vedere [Salva come nuova versione](web-editor-features.md#save-as-new-version-id209ME400GXA).


>[!NOTE]
>
> Se l&#39;amministratore ha configurato l&#39;editor Web per estrarre i file prima della modifica, non sarà possibile modificare un file finché non lo si estrae. Analogamente, se configurato, vi verrà chiesto di archiviare qualsiasi file estratto prima di chiuderlo.

>[!IMPORTANT]
>
> Dopo aver creato l&#39;argomento DITA, continua a salvare le modifiche nella copia di lavoro e crea una nuova versione dopo aver completato gli aggiornamenti all&#39;argomento.

**Argomento principale:**[ Creazione e visualizzazione in anteprima degli argomenti](create-preview-topics.md)

