---
product-area: projects;user-management
keywords: modifica,moduli,RTF,testo,speciale,formato,campi,personalizzato,informazioni,personalizza,oggetti
navigation-topic: work-with-custom-forms
title: Modificare le informazioni nei campi modulo personalizzati
description: È possibile modificare le informazioni di un modulo personalizzato dopo che il modulo è stato allegato a un oggetto. Per informazioni sull'aggiunta di moduli personalizzati agli oggetti, vedere Aggiungere un modulo personalizzato a un oggetto.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 456310e460bae44183de390efc4be919fda3f36d
workflow-type: tm+mt
source-wordcount: '1034'
ht-degree: 0%

---

# Modificare le informazioni nei campi modulo personalizzati

È possibile modificare le informazioni di un modulo personalizzato dopo che il modulo è stato allegato a un oggetto. Per informazioni sull&#39;aggiunta di moduli personalizzati agli oggetti, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Piano Adobe Workfront*</p> </td> 
   <td>Team o versione successiva</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licenze Adobe Workfront*</p> </td> 
   <td> <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modificare l’accesso all’oggetto per il quale si desidera modificare il modulo personalizzato</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorizzazioni oggetto</p> </td> 
   <td> 
    <ul> 
     <li> <p>Autorizzazioni Contribute o superiori per l’oggetto per il quale desideri modificare il modulo personalizzato</p> </li> 
     <li>Visualizzare le autorizzazioni per i campi che si desidera modificare. Per informazioni sulle autorizzazioni di condivisione per i campi personalizzati, vedere <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configurare la condivisione per i campi e i widget personalizzati</a>.</li> 
     <li> <p>Autorizzazioni di modifica per le sezioni del modulo in cui si trovano i campi da modificare</p> </li> 
    </ul> <p>Per informazioni sulla richiesta di accesso aggiuntivo per gli oggetti, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Prerequisiti

* L’amministratore di Workfront o un utente con accesso amministrativo ai moduli personalizzati deve creare moduli personalizzati nel tuo ambiente. Per ulteriori informazioni, vedere [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
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

   Per informazioni su tutti i tipi di campo, vedere [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

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
>A seconda della complessità dei progetti, è consigliabile non selezionare un numero elevato di progetti durante il ricalcolo in blocco dei campi personalizzati calcolati per garantire prestazioni ottimali. Alcuni elementi che potrebbero rendere un progetto troppo complesso potrebbero essere più dipendenze o assegnazioni o un numero elevato di campi personalizzati.
>
>Per ricalcolare espressioni personalizzate in blocco da un elenco di progetti:
>
>1. Passare a un elenco o a un report di progetti e selezionare uno o più progetti.
>1. Fai clic sul menu **Altro** ![](assets/more-icon.png), quindi fai clic su **Ricalcola espressioni personalizzate**.
>
>![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
>
>Workfront calcola tutti i campi personalizzati per tutti i progetti selezionati.
