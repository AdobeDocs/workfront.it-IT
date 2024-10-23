---
content-type: reference
product-area: reporting
keywords: audit,trail,personalizzato,campo
navigation-topic: calculate-custom-data-reports
title: "Esempio di campo personalizzato calcolato: visualizzazione della cronologia di modifica di un campo"
description: Se gli utenti aggiornano regolarmente i campi personalizzati e desideri acquisire un registro di tutte le modifiche apportate a un campo nonché una data in cui tali modifiche vengono apportate, puoi acquisire queste informazioni in un campo personalizzato calcolato.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Esempio di campo personalizzato calcolato: visualizzazione della cronologia di modifica di un campo

Se gli utenti aggiornano regolarmente i campi personalizzati e desideri acquisire un registro di tutte le modifiche apportate a un campo nonché una data in cui tali modifiche vengono apportate, puoi acquisire queste informazioni in un campo personalizzato calcolato.

Nell&#39;esempio seguente viene illustrato come creare il campo calcolato Cronologia modifica istruzioni per acquisire tutte le modifiche apportate a un campo di testo a riga singola denominato Istruzioni.

>[!TIP]
>
>Puoi seguire questo esempio per tutti i tipi di campi personalizzati, non solo per i campi di testo a riga singola.

Questa operazione consente di:

* Limita il campo Cronologia modifica istruzioni ai 2.000 caratteri più recenti, in modo che non superi il limite del database di Workfront.
* Controlla se il valore corrente del campo Istruzioni corrisponde alla parte anteriore del valore Cronologia di modifica delle istruzioni. Presuppone che sia vuoto e, in caso contrario, esegue le operazioni seguenti:

   * Se corrispondono, lascia invariata la cronologia di modifica delle istruzioni;
   * Se non corrispondono, sostituisce la cronologia di modifica delle istruzioni con il valore più recente nel campo Istruzioni, seguito dalla data corrente tra parentesi, da una barra verticale e dalla cronologia di modifica delle istruzioni precedenti, che mantiene i valori precedenti e le date in cui sono stati immessi.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Per informazioni sulla pianificazione, il tipo di licenza o l'accesso disponibili, contattare l'amministratore Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td> <p>Licenza Workfront*</p> </td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurazioni del livello di accesso*</strong> </td> 
   <td> <p>Accesso amministrativo a Forms personalizzato</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Gestire le autorizzazioni sui moduli personalizzati </p> <p>Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Condividi modulo personalizzato</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti

Per aggiungere un campo calcolato che visualizza la cronologia di modifica di un campo in un modulo personalizzato, è necessario innanzitutto:

* Creare il modulo personalizzato
* Aggiungi al modulo personalizzato il campo di cui desideri acquisire la cronologia

## Visualizzare la cronologia di modifica di un campo

1. Passare a un modulo personalizzato in cui si desidera aggiungere il campo calcolato.

1. Per creare il campo personalizzato di testo a riga singola, ad esempio, eseguire le operazioni seguenti:

   1. Fare clic su **Testo su riga singola**.
   1. Specifica un **etichetta** per il campo personalizzato. Ad esempio, puoi denominarlo &quot;Istruzioni&quot;.
   1. Fare clic su **Applica**.

1. Fare clic su **Calcolato** per aggiungere al modulo un campo personalizzato calcolato.
1. Specifica un **etichetta** per il campo personalizzato calcolato. Ad esempio, è possibile denominarlo &quot;Istruzioni Modifica cronologia&quot;.

   Questo è il campo che acquisirà eventuali modifiche apportate al primo campo creato (&quot;Istruzioni&quot;).

1. Fare clic su **Salva e chiudi**.
1. Fare clic sul nome del modulo in cui sono stati aggiunti due campi per riaprirlo.
1. Fai clic sul campo personalizzato calcolato **Istruzioni Modifica cronologia**, quindi copia e incolla quanto segue nella casella **Calcolo**:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Consigliato) Incolla lo stesso calcolo nel campo **Istruzioni** del campo calcolato del modulo.
1. Assicurati che **Testo** sia selezionato nel campo **Formato** per formattare il campo personalizzato calcolato come testo.

   Questa è l&#39;impostazione predefinita.

1. Fare clic su **Salva e chiudi**.

   Ora, quando si allega il modulo personalizzato a un oggetto e successivamente qualcuno modifica le informazioni nel campo **Istruzioni**, il campo **Cronologia modifiche istruzioni** visualizza il valore più recente, seguito dalla data corrente tra parentesi e da una barra verticale. Se vengono apportate ulteriori modifiche, queste vengono aggiunte a queste informazioni nello stesso modo.

   Nel calcolo riportato sopra è possibile sostituire *Istruzioni* con il nome esatto del campo di testo a riga singola di cui si desidera tenere traccia della cronologia e **Istruzioni Modifica cronologia** con il nome esatto del campo calcolato.
