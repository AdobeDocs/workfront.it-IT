---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Gestione di moduli personalizzati associati agli oggetti
description: È possibile aggiornare l’ordine di visualizzazione, rimozione o modifica collettiva dei moduli personalizzati associati a un oggetto nel modo in cui i moduli personalizzati vengono visualizzati su più oggetti.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 23257f11b0795aa1f1e422923f6d596017c58126
workflow-type: tm+mt
source-wordcount: '1120'
ht-degree: 0%

---

# Gestione di moduli personalizzati associati agli oggetti

<span class="preview">Le informazioni evidenziate in questa pagina fanno riferimento a funzionalità non ancora disponibili al pubblico. È disponibile solo nell’ambiente Anteprima.</span>

È possibile aggiornare l’ordine di visualizzazione, rimozione o modifica collettiva dei moduli personalizzati associati a un oggetto nel modo in cui i moduli personalizzati vengono visualizzati su più oggetti.

## Requisiti di accesso

Per eseguire le azioni descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso agli oggetti per i quali si gestiscono moduli personalizzati</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute o superiori agli oggetti per i quali si gestiscono moduli personalizzati</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

* L’amministratore di Workfront o un utente di Plan con accesso amministrativo ai moduli personalizzati deve creare moduli personalizzati nel proprio ambiente. Per ulteriori informazioni, consulta [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* A un oggetto è necessario associare moduli personalizzati.

   Per informazioni su come applicare moduli personalizzati a un oggetto, consultare [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Riordinare più moduli personalizzati collegati a un oggetto {#reorder-multiple-custom-forms-attached-to-an-object}

1. Passare all’oggetto in cui si desidera modificare l’ordine dei moduli personalizzati aggiunti, quindi iniziare a modificare l’oggetto.

   **Esempio:** Ad esempio, per gestire i moduli personalizzati di un progetto, passa al progetto e fai clic sul pulsante **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Modifica** .

1. In **Forms personalizzato** per progetti, attività e problemi, fai clic sul pulsante ![](assets/move-icon---dots.png) accanto al nome di un modulo personalizzato. Per tutti gli altri oggetti, fare clic su **Gestione Forms**. Questa opzione viene visualizzata solo se all’oggetto è associato almeno un modulo personalizzato.
1. Trascina un modulo ![](assets/move-icon---dots.png) in una nuova posizione nell’elenco.
1. Per progetti, attività ed emette moduli personalizzati, fai clic su **Salva**.

   Per tutti gli altri oggetti, fare clic su **Ho finito di gestire** > **Salva modifiche**.

## Rimuovere un modulo personalizzato da un oggetto {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Quando si rimuove un modulo personalizzato da un oggetto, tutte le informazioni acquisite nei campi personalizzati del modulo vengono perse e non possono essere recuperate.

1. Passare all’oggetto in cui si desidera rimuovere il modulo personalizzato e iniziare a modificare l’oggetto.

   Ad esempio, passa a un progetto e fai clic sul pulsante **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Modifica** .

1. Fai clic su **Forms personalizzato**.
1. Per progetti, attività ed emette moduli personalizzati, fai clic sul pulsante **X** a destra di un modulo per rimuoverlo dall’oggetto.

   Per tutti gli altri oggetti, fare clic su **Gestione Forms**, quindi fai clic su **X** a destra di un modulo per rimuoverlo dall’oggetto.

1. Fai clic su **Salva** .

## Gestione di più moduli personalizzati contenenti gli stessi campi personalizzati

È possibile che lo stesso campo venga visualizzato in più moduli personalizzati collegati allo stesso oggetto. In questo caso, considera quanto segue:

* Il valore del campo è identico in tutti i moduli.

   Non è possibile avere valori diversi per gli stessi campi in diversi moduli collegati allo stesso oggetto.

* Se su due oggetti diversi sono presenti gli stessi campi calcolati, i relativi calcoli devono essere identici per evitare errori. Per informazioni sull’aggiunta di campi calcolati ai moduli personalizzati, compresi più moduli, vedere [Aggiungere dati calcolati a un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) .

## Gestione di più moduli personalizzati durante la modifica collettiva di oggetti

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
><span class="preview">Per informazioni sulla gestione di moduli personalizzati su progetti in blocco nell’ambiente di anteprima, vedere l’articolo [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md)</span>.

Quando si modificano in serie oggetti a cui sono applicati più moduli personalizzati, è possibile modificare la modalità di visualizzazione dei moduli personalizzati su tali oggetti, nonché modificare i campi comuni nei moduli personalizzati.

È possibile modificare in blocco solo i moduli personalizzati allegati a tutti gli oggetti selezionati.

Per modificare più moduli personalizzati durante la modifica collettiva di oggetti:

1. In un elenco di oggetti, selezionare gli oggetti a cui sono collegati i moduli personalizzati, quindi fare clic sul pulsante **Modifica** icona ![](assets/edit-icon.png).
1. Fai clic su **Forms personalizzato**.

   È possibile modificare solo i moduli personalizzati associati a tutti gli oggetti selezionati.

   I moduli personalizzati allegati solo ad alcuni oggetti non vengono visualizzati.

1. Inizia a modificare i campi nei moduli personalizzati.

   Quando i campi vengono modificati, nel campo viene visualizzato un indicatore visivo che indica che il campo è stato modificato.

   Se un campo è incluso in più moduli personalizzati, tutti i valori di tali campi vengono aggiornati in ciascun modulo quando si aggiorna il campo in uno dei moduli.

1. Fai clic sul pulsante **Selezione** menu a discesa e selezionare ulteriori moduli da aggiungere a tutti gli oggetti selezionati.

   Quando si applicano moduli aggiuntivi, tenere presente quanto segue:

   * Gli oggetti possono avere fino a 10 moduli personalizzati.
   * È possibile applicare i moduli solo se il modulo non è già applicato a nessuno degli oggetti che si stanno modificando. Un modulo già associato a uno degli oggetti non viene visualizzato nel menu a discesa.
   * Dopo aver applicato un modulo aggiuntivo, tutti i campi del modulo in comune con altri moduli vengono visualizzati nella **Campi comuni** e possono essere modificati.

1. (Facoltativo) Se sono stati aggiunti moduli personalizzati a tutti gli oggetti, ma non sono ancora stati salvati gli oggetti, è possibile modificare l’ordine in cui i moduli personalizzati vengono visualizzati sugli oggetti.

   Per ulteriori informazioni sulla modifica dell’ordine dei moduli, vedere [Riordinare più moduli personalizzati collegati a un oggetto](#reorder-multiple-custom-forms-attached-to-an-object) in questo articolo.

1. Fai clic su **Rimuovi modulo** per rimuovere un modulo personalizzato dagli oggetti.

   Per ulteriori informazioni sulla rimozione dei moduli personalizzati dagli oggetti, vedere [Rimuovere un modulo personalizzato da un oggetto](#remove-a-custom-form-from-an-object).

   Quando si rimuovono moduli in blocco da più oggetti, tenere presente quanto segue:

   * Se sono state apportate modifiche al modulo, la rimozione comporta la perdita delle modifiche e il recupero delle modifiche.
   * Dopo la rimozione di un modulo, tutti i campi del modulo presenti nel modulo **Campi comuni** Questa sezione viene rimossa e non può più essere modificata.

1. Fai clic su **Ripristina modulo** per ripristinare lo stato del modulo prima della modifica degli oggetti.
1. (Facoltativo) Fare clic sulla freccia di compressione accanto al nome del modulo per comprimere un modulo alla volta.

   Oppure

   Fai clic su **Comprimi Forms** per comprimere tutti i moduli contemporaneamente.

1. (Facoltativo) Fare clic sulla freccia di espansione accanto al nome del modulo per espandere un modulo alla volta.

   Oppure

   Fai clic su **Espandi Forms** espandere tutti i moduli contemporaneamente. 

1. Fai clic su **Salva modifiche**.
