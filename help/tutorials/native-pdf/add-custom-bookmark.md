---
title: Funzione di pubblicazione nativa di PDF | Aggiungi un segnalibro personalizzato nell’output di PDF
description: Scopri come creare e utilizzare fogli di stile e creare stili per i contenuti.
source-git-commit: fb7ffbaefcdca4302e43d8369bc056c1f08a3ed6
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---


# Aggiungi un segnalibro personalizzato nell’output di PDF

In genere, il sommario in una mappa DITA viene replicato come segnalibri nell&#39;output finale di PDF. Questo sommario viene creato dai titoli degli argomenti o delle sezioni nella mappa DITA. A volte può essere utile aggiungere un segnalibro personalizzato su un particolare contenuto nell’output di PDF per facilitarne la navigazione. A questo scopo è possibile aggiungere un `outputclass` sull’elemento e applica il seguente attributo:

`bookmark-level: 3`

Qui, il `bookmark-level` è un attributo e un numero `3` è il valore che indica il livello nella gerarchia dei segnalibri in cui viene aggiunto il segnalibro. Nell&#39;esempio seguente, l&#39;argomento di primo livello &quot;Contatti&quot; ha una tabella, &quot;Elenco contatti&quot;, sulla quale abbiamo aggiunto un `outputclass` attributo con il valore di `custom-bookmark`.


<img src="./assets/custom-bookmark-attribute.png" width="500">

La seguente definizione di `custom-bookmark` La classe viene aggiunta nel file CSS:

```css
…
/*Adding a custom bookmark*/
.custom-bookmark{
    bookmark-level: 2
}
…
```

Nell’output di PDF, la variabile *Elenco contatti* La tabella viene aggiunta al secondo livello nell’elenco dei segnalibri di PDF, come illustrato di seguito:

<img src="./assets/custom-bookmark-in-pdf-output.png" width="500">

>[!NOTE]
>
>È necessario scegliere il livello corretto in cui viene aggiunto il segnalibro personalizzato. Se si specifica un numero inferiore al segnalibro dell&#39;argomento principale, il segnalibro personalizzato assume la posizione del segnalibro principale e tutti gli altri segnalibri vengono visualizzati come elementi secondari. Questo può portare a una struttura di segnalibri inaspettata.

