---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Gestire i moduli personalizzati allegati agli oggetti
description: È possibile aggiornare l'ordine di visualizzazione dei moduli personalizzati allegati a un oggetto, rimuoverli o modificare in blocco la modalità di visualizzazione dei moduli personalizzati su più oggetti.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: b3534cccd4a06b8c5b8b7e742f63eeb898bd5b99
workflow-type: tm+mt
source-wordcount: '1147'
ht-degree: 0%

---

# Gestire i moduli personalizzati allegati agli oggetti

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile per tutti i clienti nell&#39;ambiente di anteprima e per un gruppo selezionato di clienti nell&#39;ambiente di produzione.</span>

È possibile aggiornare l&#39;ordine di visualizzazione dei moduli personalizzati allegati a un oggetto, rimuoverli o modificare in blocco la modalità di visualizzazione dei moduli personalizzati su più oggetti.

## Requisiti di accesso

Per eseguire le azioni descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso agli oggetti per i quali si gestiscono i moduli personalizzati</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute o superiori per gli oggetti per i quali si gestiscono i moduli personalizzati</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Prerequisiti

* L’amministratore di Workfront o un utente con accesso amministrativo ai moduli personalizzati deve creare moduli personalizzati nel tuo ambiente. Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* A un oggetto devono essere allegati moduli personalizzati.

  Per informazioni su come applicare moduli personalizzati a un oggetto, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Riordinare più moduli personalizzati allegati a un oggetto {#reorder-multiple-custom-forms-attached-to-an-object}

1. Passare all&#39;oggetto in cui si desidera modificare l&#39;ordine dei moduli personalizzati aggiunti, quindi iniziare a modificare l&#39;oggetto.

   **Esempio:** Ad esempio, per gestire i moduli personalizzati di un progetto, accedi al progetto, fai clic sul menu **Altro** ![](assets/more-icon.png), quindi fai clic su **Modifica** .

1. Nella sezione **Forms** personalizzato per progetti, attività e problemi, fai clic sull&#39;icona ![](assets/move-icon---dots.png) accanto al nome di un modulo personalizzato. Per tutti gli altri oggetti, fare clic su **Gestisci Forms**. Questa opzione viene visualizzata solo se all’oggetto è allegato almeno un modulo personalizzato.
1. Trascinare un modulo ![](assets/move-icon---dots.png) in una nuova posizione nell&#39;elenco.
1. Per progetti, attività e problemi moduli personalizzati, fai clic su **Salva**.

   Per tutti gli altri oggetti, fai clic su **Gestione completata** > **Salva modifiche**.

## Rimuovere un modulo personalizzato da un oggetto {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Quando si rimuove un modulo personalizzato da un oggetto, tutte le informazioni acquisite nei campi personalizzati del modulo vengono perse e non possono essere recuperate.

1. Passare all&#39;oggetto in cui si desidera rimuovere il modulo personalizzato e iniziare a modificare l&#39;oggetto.

   Ad esempio, vai a un progetto, fai clic sul menu **Altro** ![](assets/more-icon.png), quindi fai clic su **Modifica** .

1. Fare clic su **Forms personalizzato**.
1. Per progetti, attività e problemi di moduli personalizzati, fai clic sull&#39;icona **X** a destra di un modulo per rimuoverlo dall&#39;oggetto.

   Per tutti gli altri oggetti, fare clic su **Gestisci Forms**, quindi fare clic sull&#39;icona **X** a destra di un modulo per rimuoverlo dall&#39;oggetto.

1. <span class="preview">Nella finestra di dialogo visualizzata, fare clic su **Rimuovi**.</span>

1. Fai clic su **Salva**.

## Gestire più moduli personalizzati contenenti gli stessi campi personalizzati

È possibile che lo stesso campo venga visualizzato in più moduli personalizzati associati allo stesso oggetto. In questo caso, considera quanto segue:

* Il valore del campo è identico in tutti i moduli.

  Non è possibile avere valori diversi per gli stessi campi su moduli diversi associati allo stesso oggetto.

* Se si dispone degli stessi campi calcolati su due oggetti diversi, i relativi calcoli devono essere identici per evitare errori. Per informazioni sull&#39;aggiunta di campi calcolati ai moduli personalizzati, inclusi più moduli, vedere [Aggiungere campi calcolati a un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Gestire più moduli personalizzati durante la modifica in blocco di oggetti

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>La gestione dei moduli personalizzati in oggetti è identica per tutti gli oggetti ad eccezione dei progetti.
>
>Per informazioni sull&#39;aggiunta di moduli personalizzati a progetti in blocco, vedere l&#39;articolo [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).

Quando si modificano in blocco oggetti a cui sono applicati più moduli personalizzati, è possibile modificare la modalità di visualizzazione dei moduli personalizzati su tali oggetti e i campi comuni tra i moduli personalizzati.

Solo i moduli personalizzati allegati a tutti gli oggetti selezionati possono essere modificati in modalità collettiva.

Per modificare più moduli personalizzati durante la modifica di oggetti in blocco:

1. In un elenco oggetti, selezionare gli oggetti a cui sono allegati i moduli personalizzati, quindi fare clic sull&#39;icona **Modifica** ![](assets/edit-icon.png).
1. Fare clic su **Forms personalizzato**.

   È possibile modificare solo i moduli personalizzati allegati a tutti gli oggetti selezionati.

   I moduli personalizzati allegati solo ad alcuni oggetti non vengono visualizzati.

1. Inizia a modificare i campi nei moduli personalizzati.

   Quando si modificano i campi, nel campo viene visualizzato un indicatore visivo che indica che il campo è stato modificato.

   Se un campo è incluso in più moduli personalizzati, tutti i valori di tali campi vengono aggiornati in ogni modulo quando si aggiorna il campo in uno dei moduli.

1. Fare clic sul menu a discesa **Effettua una selezione** e selezionare ulteriori moduli da aggiungere a tutti gli oggetti selezionati.

   Quando si applicano moduli aggiuntivi, considera quanto segue:

   * Gli oggetti possono avere fino a 10 moduli personalizzati.
   * È possibile applicare i moduli solo se il modulo non è già applicato a nessuno degli oggetti che si stanno modificando. Un modulo già associato a uno degli oggetti non viene visualizzato nel menu a discesa.
   * Dopo aver applicato un modulo aggiuntivo, tutti i campi che il modulo ha in comune con altri moduli vengono visualizzati nella sezione **Campi comuni** e possono essere modificati.

1. (Facoltativo) Se sono stati aggiunti moduli personalizzati a tutti gli oggetti, ma gli oggetti non sono ancora stati salvati, è possibile modificare l&#39;ordine di visualizzazione dei moduli personalizzati sugli oggetti.

   Per ulteriori informazioni sulla modifica dell&#39;ordine dei moduli, vedere [Riordinare più moduli personalizzati allegati a un oggetto](#reorder-multiple-custom-forms-attached-to-an-object) in questo articolo.

1. Fare clic su **Rimuovi modulo** per rimuovere un modulo personalizzato dagli oggetti.

   Per ulteriori informazioni sulla rimozione di moduli personalizzati dagli oggetti, vedere [Rimuovere un modulo personalizzato da un oggetto](#remove-a-custom-form-from-an-object).

   Quando si rimuovono moduli in blocco da più oggetti, tenere presente quanto segue:

   * Se sono state apportate modifiche al modulo, la rimozione di quest&#39;ultimo comporta la perdita delle modifiche e l&#39;impossibilità di recuperarle.
   * Dopo aver rimosso un modulo, tutti i campi del modulo presenti nella sezione **Campi comuni** verranno rimossi da questa sezione e non potranno più essere modificati qui.

1. Fare clic su **Ripristina modulo** per ripristinare lo stato del modulo precedente alla modifica degli oggetti.
1. (Facoltativo) Fare clic sulla freccia di compressione accanto al nome del modulo per comprimere un modulo alla volta.

   Oppure

   Fare clic su **Comprimi Forms** per comprimere tutti i moduli contemporaneamente.

1. (Facoltativo) Fare clic sulla freccia di espansione accanto al nome del modulo per espandere un modulo alla volta.

   Oppure

   Fare clic su **Espandi Forms** per espandere tutti i moduli contemporaneamente. 

1. Fai clic su **Salva modifiche**.
