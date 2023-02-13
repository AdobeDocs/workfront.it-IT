---
content-type: reference
product-area: reporting
keywords: audit,trail,personalizzato,campo
navigation-topic: calculate-custom-data-reports
title: "Esempio di campo personalizzato calcolato: visualizzare la cronologia delle modifiche di un campo"
description: Se gli utenti aggiornano regolarmente i campi personalizzati e si desidera acquisire un registro di tutte le modifiche apportate a un campo e una data in cui le modifiche vengono apportate, è possibile acquisire tali informazioni in un campo personalizzato calcolato.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# Esempio di campo personalizzato calcolato: visualizzare la cronologia delle modifiche di un campo

Se gli utenti aggiornano regolarmente i campi personalizzati e si desidera acquisire un registro di tutte le modifiche apportate a un campo e una data in cui le modifiche vengono apportate, è possibile acquisire tali informazioni in un campo personalizzato calcolato.

L’esempio seguente illustra come generare il *Istruzioni Modifica cronologia* campo calcolato per acquisire tutte le modifiche apportate a un campo di testo a riga singola denominato *Istruzioni*.

>[!TIP]
>
>È possibile seguire questo esempio per tutti i tipi di campi personalizzati, non solo per i campi di testo a riga singola.

Questo esegue le seguenti operazioni: 

* Limiti *Istruzioni Modifica cronologia* fino ai 2000 caratteri più recenti per rimanere entro il limite del database Workfront.
* Controlla se il valore corrente del *Istruzioni* corrisponde al fronte del *Istruzioni Modifica cronologia* valore; presuppone che sia vuoto e, in caso contrario, esegue le seguenti operazioni: 

   * Se corrispondono, lascia il *Istruzioni Modifica cronologia* così come è;
   * Se non corrispondono, sostituisce il *Istruzioni Modifica cronologia* con il valore più recente nel *Istruzioni* seguito dalla data corrente tra parentesi, da una barra verticale e dalla data precedente *Istruzioni Modifica cronologia*, che conserva i valori precedenti e le date in cui sono stati immessi.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l'amministratore Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td> <p>Licenza Workfront*</p> </td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Accesso amministrativo a Custom Forms</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Gestione delle autorizzazioni sui moduli personalizzati </p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Condivisione di un modulo personalizzato</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti

Per aggiungere a un modulo personalizzato un campo calcolato in cui è visualizzata la cronologia delle modifiche di un campo, è necessario innanzitutto:

* Creare il modulo personalizzato
* Aggiungere al modulo personalizzato il campo di cui si desidera acquisire la cronologia

## Visualizzare la cronologia delle modifiche di un campo

1. Passare a un modulo personalizzato in cui si desidera aggiungere il campo calcolato.

1. Per creare un campo personalizzato di testo a riga singola, ad esempio, eseguire le operazioni seguenti:

   1. Fai clic su **Campo di testo a riga singola**.
   1. Specifica una **Etichetta** per il campo personalizzato, ad esempio *Istruzioni*.
   1. Fai clic su **Applique**.

1. Seleziona **Aggiungi un campo**, quindi seleziona **Calcolato** per aggiungere al modulo un campo personalizzato calcolato.
1. Specifica una **Etichetta** per il campo personalizzato calcolato, ad esempio *Istruzioni Modifica cronologia*.

   Questo è il campo che acquisirà le modifiche apportate al primo campo creato (*Istruzioni*).

1. Fai clic su **Salva e chiudi**.
1. Fare clic sul nome del modulo in cui sono stati aggiunti due campi per riaprirlo.
1. Fai clic sul campo personalizzato calcolato *Istruzioni Modifica cronologia,* quindi copia e incolla quanto segue nella casella Calcolo:
1. In **Calcolo** specifica il seguente calcolo per il campo personalizzato:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Consigliato) Incolla lo stesso calcolo nel **Istruzioni** sul campo calcolato del modulo.
1. Assicurati che  **Testo** è selezionato in **Formato** per formattare il campo personalizzato calcolato come testo.

   Questa è l’impostazione predefinita.

1. Fai clic su **Salva e chiudi**.

   Ora, quando si allega il modulo personalizzato a un oggetto e quindi un utente modifica le informazioni nel *Istruzioni* Il campo *Istruzioni Modifica cronologia&quot; visualizza il valore più recente, seguito dalla data corrente tra parentesi e da una barra verticale. Se vengono apportate ulteriori modifiche, queste vengono aggiunte a queste informazioni nello stesso modo.

   Nel calcolo di cui sopra, è possibile sostituire *Istruzioni* con il nome esatto del campo di testo a riga singola di cui si desidera tenere traccia e *Istruzioni Modifica cronologia* con il nome esatto del campo calcolato.
