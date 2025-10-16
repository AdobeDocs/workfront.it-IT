---
product-area: projects;user-management
keywords: modifica,moduli,RTF,testo,speciale,formato,campi,personalizzato,informazioni,personalizza,oggetti
navigation-topic: work-with-custom-forms
title: Modificare le informazioni nei campi modulo personalizzati
description: È possibile modificare le informazioni di un modulo personalizzato dopo che il modulo è stato allegato a un oggetto. Per informazioni sull'aggiunta di moduli personalizzati agli oggetti, vedere Aggiungere un modulo personalizzato a un oggetto.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 0%

---

# Modificare le informazioni nei campi modulo personalizzati

<!--Audited: 10/2025-->

È possibile modificare le informazioni di un modulo personalizzato dopo che il modulo è stato allegato a un oggetto. Per informazioni sull&#39;aggiunta di moduli personalizzati agli oggetti, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Pacchetto Adobe Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licenza Adobe Workfront</p> </td> 
   <td> <p>Collaboratore o versione successiva</p> 
   <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso all’oggetto per il quale si desidera modificare il modulo personalizzato</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorizzazioni oggetto</p> </td> 
   <td> 
    <ul> 
     <li> <p>Autorizzazioni Contribute o superiori per l'oggetto per il quale si desidera modificare il modulo personalizzato</p> </li> 
     <li><p>Visualizzare le autorizzazioni per i campi che si desidera modificare.</p></li> 
     <li><p>Autorizzazioni di modifica per le sezioni del modulo in cui si trovano i campi da modificare</p></li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Team or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront licenses*</p> </td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to the object for which you want to edit the custom form</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute or higher permissions on the object for which you want to edit the custom form</p> </li> 
     <li>View permissions on the fields you want to edit. For information about sharing permissions for custom fields, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</li> 
     <li> <p>Edit permissions for the sections on the form where the fields you want to edit are located</p> </li> 
    </ul> <p>For information on requesting additional access for objects, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Prerequisiti

* L’amministratore di Workfront o un utente con accesso amministrativo ai moduli personalizzati deve creare moduli personalizzati nel tuo ambiente. Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* A un oggetto devono essere allegati moduli personalizzati.

  Per informazioni su come applicare moduli personalizzati a un oggetto, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Modificare le informazioni in un modulo personalizzato

La modifica delle informazioni in un modulo personalizzato associato a un oggetto è identica per tutti gli oggetti. Per informazioni sugli oggetti che possono avere un modulo personalizzato, vedere [Panoramica moduli personalizzati](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. Passare a un oggetto per il quale si desidera modificare le informazioni nel modulo personalizzato.
1. Fai clic su **`<Object type>`Dettagli** nel pannello a sinistra.

   Ad esempio, durante la modifica delle informazioni in un modulo personalizzato del progetto, fai clic su **Dettagli progetto**.

1. Scorri fino al modulo personalizzato. Se all&#39;oggetto è allegato un modulo personalizzato, il nome del modulo viene visualizzato come area nella sezione Dettagli.
1. Se necessario, fare clic sulla freccia ![](assets/expand-arrow-right.png) a sinistra del nome del modulo personalizzato per espanderlo.
1. Fare clic sull&#39;icona Modifica ![](assets/edit-icon.png) nell&#39;angolo superiore destro della pagina.
1. Inizia a immettere informazioni in qualsiasi campo a cui hai accesso.

   ![](assets/click-in-field-to-edit-info-350x132.png)

   Oppure

   Se nel modulo non sono ancora state immesse informazioni, fare clic su **Aggiungi+** per qualsiasi campo a cui si ha accesso e iniziare a immettere le informazioni.

   ![](assets/plus-add-to-edit-info-350x180.png)

   Se all’oggetto sono allegati più moduli personalizzati, è possibile eseguire questa operazione per ogni modulo.

   A seconda del tipo di campo in cui si sta lavorando, considerare quanto segue:

   * È possibile selezionare una sola opzione per i campi pulsante di opzione.
   * Puoi selezionare una o più opzioni in un campo casella di controllo, a seconda di come il creatore del modulo ha configurato il campo.
   * Puoi selezionare una o più opzioni in un campo a discesa a selezione multipla, a seconda di come il creatore del modulo ha configurato il campo.
   * È possibile formattare i campi di testo (grassetto, corsivo o sottolineato) solo se l&#39;utente che ha creato il modulo li ha impostati come campo di testo con tipo di campo Formattazione. Impossibile formattare i campi di testo a riga singola e i campi di testo a paragrafo.
   * È possibile aggiornare l&#39;ora del giorno in un tipo di campo Data solo se l&#39;utente che ha creato il modulo lo ha incluso durante la creazione del campo.

   Per informazioni su tutti i tipi di campo, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Fai clic su **Salva modifiche**.

   >[!IMPORTANT]
   >
   >Per salvare il modulo è necessario compilare tutti i campi obbligatori del modulo. Il nome di un campo obbligatorio è seguito da un asterisco.
   >
   >![](assets/nwe-required-custom-field.png)

   Quando qualcuno modifica i dati in un altro oggetto a cui fanno riferimento i campi personalizzati calcolati nell&#39;oggetto, le modifiche non vengono applicate automaticamente nell&#39;oggetto. Per informazioni sull&#39;aggiornamento manuale di tutti i campi personalizzati calcolati nell&#39;oggetto, vedere [Ricalcolare tutti i campi personalizzati calcolati per un oggetto](#recalculate-all-calculated-custom-fields-for-an-object) in questo articolo.

   Quando i campi dipendenti della pagina vengono modificati, i campi calcolati del modulo personalizzato vengono ricalcolati in tempo reale in modo dinamico. È possibile visualizzare il nuovo valore del campo calcolato senza salvare il modulo, ma non viene effettivamente applicato al modulo e all&#39;oggetto fino a quando non si salvano le modifiche. Ciò si applica ai campi calcolati nei moduli predefiniti e nei moduli personalizzati.

   È inoltre possibile aggiornare manualmente tutti i campi personalizzati calcolati per un oggetto quando si modifica in blocco l&#39;oggetto insieme ad altri oggetti in un elenco. Per istruzioni, vedere [Ricalcolare tutti i campi personalizzati calcolati per più oggetti in un elenco durante la modifica degli oggetti](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) in questo articolo.

## Ricalcolare tutti i campi personalizzati calcolati per un oggetto  {#recalculate-all-calculated-custom-fields-for-an-object}

1. Passare alla pagina principale dell&#39;oggetto di cui si desidera ricalcolare i campi personalizzati.
1. Fai clic sul menu **Altro** ![](assets/more-icon.png) a destra del nome dell&#39;oggetto, quindi fai clic su **Ricalcola espressioni**.

   In questo modo vengono ricalcolati tutti i campi personalizzati nel modulo dell&#39;oggetto.

## Ricalcolare tutti i campi personalizzati calcolati per più oggetti in un elenco durante la modifica degli oggetti {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

È possibile ricalcolare manualmente i campi personalizzati di più oggetti modificandoli in blocco da un elenco o da un report.

1. Consente di passare a un elenco di oggetti che contengono moduli personalizzati con campi calcolati.
1. Selezionare gli oggetti di cui si desidera aggiornare i campi personalizzati calcolati.
1. Fai clic sull&#39;icona **Modifica**.
1. Fai clic su **Forms personalizzato** nel menu a sinistra, quindi seleziona **Ricalcola espressioni personalizzate**.
1. Fai clic su **Salva** **Modifiche**.

   Workfront calcola tutti i campi personalizzati per tutti gli oggetti selezionati.

>[!TIP]
>
>È inoltre possibile ricalcolare le espressioni personalizzate da un elenco di oggetti. Ad esempio, per ricalcolare espressioni personalizzate in blocco da un elenco di progetti:
>
>1. Passare a un elenco o a un report di progetti e selezionare uno o più progetti.
>1. Fai clic sul menu **Altro** ![](assets/more-icon.png), quindi fai clic su **Ricalcola espressioni personalizzate**.
>
>![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
>
>Workfront calcola tutti i campi personalizzati per tutti i progetti selezionati.
>>Non tutti gli elenchi di tutti gli oggetti dispongono di questa funzionalità.
>
>A seconda della complessità dei progetti, è consigliabile non selezionare un numero elevato di progetti durante il ricalcolo in blocco dei campi personalizzati calcolati per garantire prestazioni ottimali. Alcuni elementi che potrebbero rendere un progetto troppo complesso potrebbero essere più dipendenze o assegnazioni o un numero elevato di campi personalizzati.

