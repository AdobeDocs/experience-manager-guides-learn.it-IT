---
title: Utilizzare i predefiniti condizione
description: Scopri come utilizzare i predefiniti delle condizioni
source-git-commit: 6eb8d29e71301581e8dbb5b6a4252194c5a89f96
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 2%

---


# Utilizzare i predefiniti condizione {#id1825FL004PN}

È possibile definire gli attributi negli argomenti DITA e utilizzare il predefinito di condizione per specificare cosa succede con l&#39;attributo nell&#39;output finale. Ad esempio, è possibile aggiungere attributi come versione 1.0 e versione 2.0 nel contenuto e utilizzare un predefinito per condizioni che includa la versione 1.0 per la versione 1.0 ed escluda la versione 2.0. Analogamente, è possibile aggiungere attributi come OS Windows e OS Linux al contenuto e quindi includere o escludere il contenuto pertinente per l&#39;output finale in base al sistema operativo.

## Creare un predefinito di condizione

Per creare un predefinito di condizione, effettua le seguenti operazioni:

1. Fai clic su **Predefiniti condizione** nella console mappa DITA.
1. Fai clic su **Crea** pulsante .
1. Immetti un nome per il predefinito in **Condizione nome**.
1. Seleziona una delle seguenti azioni predefinite da **Imposta l&#39;azione predefinita su** a discesa:

   - Includi
   - Escludi
   - Passaggio
   - Flag L’azione è impostata come azione predefinita per tutti gli attributi, siano essi aggiunti o meno al predefinito di condizione.

   Ad esempio, hai 15 attributi di condizione nel documento e ne hai inclusi quattro nel predefinito di condizione. Se si seleziona **escludere** come azione predefinita, viene applicata a tutti e 15 gli attributi.

1. Effettua una delle seguenti operazioni per aggiungere gli attributi:
   - Fai clic su **Aggiungi** a un attributo del predefinito di condizione. Puoi ripetere questo passaggio per aggiungere altri attributi.
   - Fai clic su **Aggiungi tutto** per aggiungere tutti gli attributi al predefinito di condizione.
1. \(Facoltativo\) Se necessario, è possibile ignorare l&#39;azione predefinita applicata agli attributi nel passaggio 4. Effettua una delle operazioni seguenti:
   - Seleziona più attributi, scegli un’azione da **Imposta l&#39;azione per le condizioni selezionate su** e fai clic su **Applica**.
   - Seleziona un&#39;azione per un attributo dal **Azione** a discesa.
1. Fai clic su **Salva**.

## Modificare un predefinito di condizione

Puoi apportare modifiche in un predefinito di condizione esistente per modificare le azioni applicate agli attributi nel predefinito di condizione. Per modificare un predefinito di condizione, effettua le seguenti operazioni:

1. Fai clic su **Predefiniti condizione** nella console mappa DITA.
1. Fai clic su **Modifica** pulsante .
1. Apporta le modifiche necessarie per tutti gli attributi nel predefinito per condizioni.
1. Fai clic su **Salva**.

## Creare una copia di un predefinito per condizioni

Puoi creare una copia di un predefinito per condizioni e quindi modificarlo in base alle tue esigenze. Per creare una copia di un predefinito per condizioni, effettua le seguenti operazioni:

1. Fai clic su **Predefiniti condizione** nella console mappa DITA.
1. Fai clic su **Duplica** pulsante .

   >[!NOTE]
   >
   > Il nome predefinito del predefinito è `<selected condition preset name>_Duplicate`

   Puoi modificare il nome in base alle tue esigenze.

1. \(Facoltativo\) Apporta le modifiche necessarie per tutti gli attributi nel predefinito per condizioni.
1. Fai clic su **Salva**.

## Elimina predefinito di condizione

È possibile eliminare uno o più predefiniti di condizioni dal **Predefinito condizione** scheda della console mappa DITA. Esegui i seguenti passaggi per eliminare i predefiniti condizione:

1. Fai clic su **Predefiniti condizione** nella console mappa DITA.
1. Seleziona il predefinito/i della condizione da eliminare.
1. Fai clic su **Rimuovi** pulsante .
1. Fai clic su **Rimuovi** per confermare l’azione.

**Argomento principale:**[ Generazione di output](generate-output.md)

