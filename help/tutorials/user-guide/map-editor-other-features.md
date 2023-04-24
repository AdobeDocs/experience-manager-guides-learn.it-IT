---
title: Altre funzioni nell’editor mappa
description: Scopri come aggiungere altre funzioni negli editor mappa
source-git-commit: 7cd719921e68ac1763d09d9665d912e3697e5849
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---


# Altre funzioni nell’editor mappa {#id1942D0T0HUI}

Alcune funzioni comuni degli editor di mappe di base e avanzate sono:

## Risolvere i riferimenti chiave {#id176GD01H05Z}

Un riferimento a una chiave di contenuto DITA, oppure `conkeyref` è un meccanismo per inserire una parte del contenuto da un argomento all’altro. Questo meccanismo utilizza la chiave per individuare il contenuto da riutilizzare anziché il meccanismo di riferimento diretto del contenuto. Per ulteriori informazioni sui riferimenti diretti e indiretti in DITA, vedere *Indirizzamento DITA* in OASIS DITA Language Specification.

Se all&#39;argomento DITA sono associati riferimenti chiave, è necessario risolverli prima di visualizzare l&#39;anteprima, modificare o rivedere un argomento.

I riferimenti chiave vengono risolti in base alla mappa radice impostata nel seguente ordine di priorità:

1. Preferenze utente
1. Pannello Vista mappa
1. Profilo cartella

La mappa principale selezionata in Preferenze utente ha la precedenza più alta per risolvere i riferimenti chiave seguiti dal pannello Visualizza mappa e dalla mappa principale del profilo della cartella. Pertanto, se non è impostata alcuna mappa nelle Preferenze utente, viene utilizzata la mappa aperta nel pannello Visualizza mappa . Se nel pannello Visualizzazione mappa non viene aperta alcuna mappa, per risolvere i riferimenti chiave viene utilizzato il set di mappe in Profili cartella .

I riferimenti chiave possono essere memorizzati in un file di mappa DITA o in un file DITA separato. In Guide AEM è possibile specificare riferimenti chiave a livello di progetto o di sessione. Se una mappa principale è già definita per la sessione utente, viene utilizzata per risolvere le chiavi. In caso contrario, viene utilizzata la mappa principale predefinita per quella cartella. Se una mappa principale predefinita non è configurata, all&#39;utente vengono evidenziati i riferimenti chiave mancanti.

Esistono diversi modi per risolvere i riferimenti chiave in un argomento DITA definendo la mappa DITA da utilizzare nelle posizioni seguenti:

**Proprietà del progetto** - È possibile definire una mappa principale per la risoluzione dei riferimenti chiave durante la creazione di un progetto nella sezione Proprietà progetto .

Questa mappa radice sarà applicabile per tutte le risorse \(cartelle e sottocartelle\) associate a quel progetto. Per i contenuti a cui si fa riferimento in più progetti, viene mantenuto un elenco alfabetico di progetti e viene utilizzata la mappa principale predefinita associata al primo progetto. È inoltre possibile scegliere la mappa DITA da utilizzare nell&#39;elenco per la risoluzione dei riferimenti chiave.

**Anteprima argomento** - In modalità anteprima argomento, fare clic sull&#39;icona Risoluzione chiave nella barra degli strumenti e selezionare il file DITA da utilizzare per i riferimenti chiave.

**Vista modifica argomento** - Fare clic sull&#39;icona Risoluzione chiave durante la modifica di un argomento DITA e selezionare il file DITA da utilizzare per la risoluzione dei riferimenti chiave.

**Argomento principale:**[ Utilizzare l’Editor mappa](map-editor.md)

