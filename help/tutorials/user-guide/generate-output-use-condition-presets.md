---
title: Utilizzare i predefiniti per le condizioni
description: Scopri come utilizzare i predefiniti per le condizioni
exl-id: cd8f8196-ba03-4a4b-9ce8-2651de4e5cc2
source-git-commit: 8073716bccacbe8d6a158b44d5106b083e3a5dcd
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 2%

---

# Utilizzare i predefiniti per le condizioni {#id1825FL004PN}

È possibile definire gli attributi negli argomenti DITA e utilizzare il predefinito di condizione per specificare cosa accade con l&#39;attributo nell&#39;output finale. Ad esempio, puoi aggiungere nel contenuto attributi come versione 1.0 e versione 2.0 e utilizzare un predefinito di condizione per includere la versione 1.0 per la versione 1.0 ed escludere la versione 2.0. Allo stesso modo, è possibile aggiungere al contenuto attributi come OS Windows e OS Linux e quindi includere o escludere il contenuto rilevante per l&#39;output finale in base al sistema operativo.

## Creare un predefinito di condizione

Per creare un predefinito di condizione, effettua le seguenti operazioni:

1. Clic **Predefiniti condizione** nella console delle mappe DITA.
1. Clic **Crea** pulsante.
1. Immettete un nome per il predefinito in **Condizione nome**.
1. Seleziona una delle seguenti azioni predefinite da **Imposta azione predefinita su** elenco a discesa:

   - Includi
   - Escludi
   - Passthrough
   - Flag L’azione è impostata come azione predefinita per tutti gli attributi, a prescindere che vengano aggiunti o meno al predefinito della condizione.

   Ad esempio, nel documento sono presenti 15 attributi di condizione, quattro dei quali sono stati inclusi nel predefinito di condizione. Se si seleziona **escludi** come azione predefinita, viene applicata a tutti e 15 gli attributi.

1. Per aggiungere gli attributi, effettuate una delle seguenti operazioni:
   - Clic **Aggiungi** a un attributo del predefinito di condizione. Puoi ripetere questo passaggio per aggiungere altri attributi.
   - Clic **Aggiungi tutto** per aggiungere tutti gli attributi al predefinito di condizione.
1. \(Facoltativo\) Se necessario, è possibile sostituire l&#39;azione predefinita applicata agli attributi nel passaggio 4. Effettua una delle operazioni seguenti:
   - Seleziona più attributi, scegli un’azione da **Imposta l&#39;azione per le condizioni selezionate su** e fai clic su **Applica**.
   - Selezionare un&#39;azione per un attributo da **Azione** a discesa.
1. Fai clic su **Salva**.

## Modificare un predefinito di condizione

È possibile apportare modifiche a un predefinito di condizione esistente per modificare le azioni applicate agli attributi nel predefinito di condizione. Per modificare un predefinito di condizione, effettua le seguenti operazioni:

1. Clic **Predefiniti condizione** nella console delle mappe DITA.
1. Clic **Modifica** pulsante.
1. Apporta le modifiche necessarie per tutti gli attributi nel predefinito di condizione.
1. Fai clic su **Salva**.

## Creare una copia di un predefinito di condizione

È possibile creare una copia di un predefinito di condizione e quindi modificarlo in base alle proprie esigenze. Per creare una copia di un predefinito di condizione, effettua le seguenti operazioni:

1. Clic **Predefiniti condizione** nella console delle mappe DITA.
1. Clic **Duplica** pulsante.

   >[!NOTE]
   >
   > Il nome predefinito è `<selected condition preset name>_Duplicate`

   Puoi modificare il nome in base alle tue esigenze.

1. \(Facoltativo\) Apportare le modifiche necessarie per tutti gli attributi nel predefinito di condizione.
1. Fai clic su **Salva**.

## Elimina predefinito condizione

È possibile eliminare uno o più predefiniti di condizione dal **Predefinito condizione** della console delle mappe DITA. Per eliminare i predefiniti di condizione, effettua le seguenti operazioni:

1. Clic **Predefiniti condizione** nella console delle mappe DITA.
1. Seleziona il predefinito di condizione\(s\) da eliminare.
1. Clic **Rimuovi** pulsante.
1. Clic **Rimuovi** per confermare l’azione.

**Argomento padre:**[ Generazione di output](generate-output.md)
