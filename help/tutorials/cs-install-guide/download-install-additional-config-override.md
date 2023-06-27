---
title: Sostituzioni configurazione
description: Scopri come eseguire le sostituzioni della configurazione
source-git-commit: 6051181e243cf71919901093c1b5590f21832545
workflow-type: tm+mt
source-wordcount: '92'
ht-degree: 0%

---


# Sostituzioni configurazione {#id216IFC003XA}

Per apportare qualsiasi aggiornamento alla configurazione, si deve utilizzare il seguente approccio generico:

1. Accedi all’archivio Git di Cloud Manager.

1. Crea un nuovo file JSON nella posizione seguente:

   src/main/content/jcr\_root/apps/fmditaCustom/config/

1. Denomina il file nel formato seguente:

   $\{PID\}.cfg.json

   In questo caso, il PID è l’ID processo della configurazione.

1. Aggiungi le proprietà nel file JSON utilizzando il seguente formato:

   ```
   {
      "aem.adminuname": "updatedUserjson",
      "valid.characters": "[-a-zA-Z0-9_@$]",
      "dita.serialization": true
   }
   ```

1. Apporta le modifiche ed esegui la pipeline di Cloud Manager per distribuire la configurazione aggiornata.


**Argomento padre:**[ Scarica e installa](download-install.md)

