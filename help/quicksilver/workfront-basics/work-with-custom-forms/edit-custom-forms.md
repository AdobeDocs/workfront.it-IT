---
product-area: projects;user-management
keywords: modificare,moduli,rich,testo,speciale,formato,campi,personalizzati,informazioni,personalizzare,oggetti
navigation-topic: work-with-custom-forms
title: Modificare le informazioni nei campi modulo personalizzati
description: È possibile modificare le informazioni in un modulo personalizzato dopo che il modulo è stato associato a un oggetto. Per informazioni sull’aggiunta di moduli personalizzati agli oggetti, vedere Aggiunta di un modulo personalizzato a un oggetto.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 6580fec18982215dbc2535d5f2ab159fc32ac3f5
workflow-type: tm+mt
source-wordcount: '982'
ht-degree: 0%

---

# Modificare le informazioni nei campi modulo personalizzati

È possibile modificare le informazioni in un modulo personalizzato dopo che il modulo è stato associato a un oggetto. Per informazioni sull’aggiunta di moduli personalizzati agli oggetti, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>piano Adobe Workfront*</p> </td> 
   <td>Team o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licenze Adobe Workfront*</p> </td> 
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modificare l’accesso all’oggetto per il quale si desidera modificare il modulo personalizzato</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorizzazioni oggetto</p> </td> 
   <td> 
    <ul> 
     <li> <p>Autorizzazioni di Contribute o superiori per l'oggetto per il quale si desidera modificare il modulo personalizzato</p> </li> 
     <li>Visualizza le autorizzazioni per i campi da modificare. Per informazioni sulla condivisione delle autorizzazioni per i campi personalizzati, consulta <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configurare la condivisione per campi e widget personalizzati</a>.</li> 
     <li> <p>Modificare le autorizzazioni per le sezioni del modulo in cui si trovano i campi che si desidera modificare</p> </li> 
    </ul> <p>Per informazioni sulla richiesta di accesso aggiuntivo per gli oggetti, consulta <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

* L’amministratore di Workfront o un utente di Plan con accesso amministrativo ai moduli personalizzati deve creare moduli personalizzati nel proprio ambiente. Per ulteriori informazioni, consulta [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* A un oggetto è necessario associare moduli personalizzati.

   Per informazioni su come applicare moduli personalizzati a un oggetto, consultare [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Modifica delle informazioni su un modulo personalizzato

La modifica delle informazioni su un modulo personalizzato associato a un oggetto è identica per tutti gli oggetti. Per informazioni sugli oggetti che possono avere un modulo personalizzato, consultare [Panoramica sui moduli personalizzati](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. Passare a un oggetto per il quale si desidera modificare le informazioni sul modulo personalizzato.
1. Fai clic su **`<Object type>`Dettagli** nel pannello a sinistra.

   Ad esempio, quando modifichi informazioni su un modulo personalizzato di un progetto, fai clic su **Dettagli progetto**.

1. Scorri fino al modulo personalizzato. Quando all’oggetto è associato un modulo personalizzato, il nome del modulo viene visualizzato come area nella sezione Dettagli.
1. Se necessario, fai clic sulla freccia ![](assets/expand-arrow-right.png) a sinistra del nome del modulo personalizzato per espanderlo.
1. Fai clic sull’icona Modifica nell’angolo in alto a destra della pagina ![](assets/edit-icon.png).
1. Inizia a immettere informazioni in qualsiasi campo a cui hai accesso.

   ![](assets/click-in-field-to-edit-info-350x132.png)

   Oppure

   Se non sono state ancora inserite informazioni sul modulo, fare clic su **Aggiungi+** per qualsiasi campo a cui hai accesso e inizia a immettere informazioni.

   ![](assets/plus-add-to-edit-info-350x180.png)

   Se all’oggetto sono associati più moduli personalizzati, è possibile farlo per ogni modulo.

   A seconda del tipo di campo in cui si sta lavorando, considera quanto segue:

   * È possibile selezionare una sola opzione per i campi pulsante di scelta.
   * È possibile selezionare una o più opzioni in un campo casella di controllo, a seconda della configurazione del campo da parte dell’autore del modulo.
   * È possibile selezionare una o più opzioni in un campo a discesa a selezione multipla, a seconda della configurazione del campo da parte del creatore del modulo.
   * È possibile formattare i campi di testo (grassetto, corsivo o sottolineato) solo se l’utente che ha creato il modulo li ha impostati come Campo di testo con tipo di campo Formattazione. Impossibile formattare i campi di testo a riga singola e i campi di testo a paragrafo singolo.
   * È possibile aggiornare l’ora del giorno in un tipo di campo Data solo se l’utente che ha creato il modulo lo ha incluso durante la creazione del campo.

   Per informazioni su tutti i tipi di campo, vedi [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Fai clic su **Salva** Modifiche.

   >[!IMPORTANT]
   >
   >
   >
   ><!--   >
   ><p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is true in "Edit custom forms" but not in "Add a custom form to an object." This snippet is used in both articles. The whole snippet is conditioned for classic only in "Add" but not in "Edit." Don't remove the NWE conditioning in the snippet because it is needed in "Edit."</p>   >
   >-->   >
   >
   >È necessario completare tutti i campi obbligatori del modulo prima di poter salvare il modulo. Il nome di un campo obbligatorio è seguito da un asterisco.
   ![](assets/nwe-required-custom-field.png)   >

   Quando un utente modifica dati in un altro oggetto a cui fanno riferimento i campi personalizzati calcolati nell’oggetto, le modifiche non vengono applicate automaticamente all’oggetto. Per informazioni sull’aggiornamento manuale di tutti i campi personalizzati calcolati nell’oggetto, consulta [Ricalcolare tutti i campi personalizzati calcolati per un oggetto](#recalculate-all-calculated-custom-fields-for-an-object) in questo articolo.

   È inoltre possibile aggiornare manualmente tutti i campi personalizzati calcolati per un oggetto quando si modifica in massa l’oggetto insieme ad altri oggetti di un elenco. Per istruzioni, consulta [Ricalcolare tutti i campi personalizzati calcolati per più oggetti in un elenco durante la modifica degli oggetti](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) in questo articolo.

## Ricalcolare tutti i campi personalizzati calcolati per un oggetto  {#recalculate-all-calculated-custom-fields-for-an-object}

1. Passare alla pagina principale dell’oggetto di cui si desidera ricalcolare i campi personalizzati.
1. Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png) a destra del nome dell&#39;oggetto, quindi fare clic su **Ricalcola espressioni**.

   In questo modo vengono ricalcolati tutti i campi personalizzati nel modulo dell’oggetto.

## Ricalcolare tutti i campi personalizzati calcolati per più oggetti in un elenco durante la modifica degli oggetti {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

È possibile ricalcolare manualmente i campi personalizzati di più oggetti modificandoli in blocco da un elenco o da un rapporto.

1. Fare clic su un elenco di oggetti che contengono moduli personalizzati con campi calcolati.
1. Selezionare gli oggetti di cui si desidera aggiornare i campi personalizzati calcolati.
1. Fai clic sul pulsante **Icona Modifica**.
1. Fai clic su **Forms personalizzato** nel menu a sinistra, seleziona **Ricalcola espressioni personalizzate**.
1. Fai clic su **Salva** **Modifiche**.

   Workfront calcola tutti i campi personalizzati per tutti gli oggetti selezionati.

>[!TIP]
A seconda della complessità dei progetti, si consiglia di non selezionare un numero elevato di progetti quando si ricalcolano i campi personalizzati calcolati in blocco per garantire prestazioni ottimali. Alcuni elementi che potrebbero rendere un progetto troppo complesso potrebbero essere più dipendenze o assegnazioni o un numero elevato di campi personalizzati.
Per ricalcolare in blocco le espressioni personalizzate da un elenco di progetti:
1. Passa a un elenco di progetti o a un rapporto e seleziona uno o più progetti.
1. Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Ricalcola espressioni personalizzate**.
![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
Workfront calcola tutti i campi personalizzati per tutti i progetti selezionati.
