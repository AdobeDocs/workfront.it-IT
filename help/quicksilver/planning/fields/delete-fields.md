---
title: Elimina campi
description: In Adobe Workfront Planning è possibile eliminare i campi personalizzati che non sono più rilevanti.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Planning, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Elimina campi

{{planning-important-intro}}

In Adobe Workfront Planning è possibile creare campi personalizzati per memorizzare informazioni sui record.

Per informazioni sulla creazione di campi personalizzati in Workfront Planning, vedere [Creare campi](/help/quicksilver/planning/fields/create-fields.md).

È possibile eliminare i campi di Workfront Planning che non sono più rilevanti.

## Considerazioni sull&#39;eliminazione dei campi di Workfront Planning:

* È possibile eliminare un campo solo nella vista tabella del tipo di record.
* Impossibile eliminare il campo principale di un record.
* Tutte le informazioni memorizzate nel campo vengono eliminate e non possono essere recuperate.
* Quando si elimina un campo record connesso, vengono eliminati anche tutti i campi di ricerca connessi dal tipo di record da cui ci si connette. I campi dei record connessi dei tipi di record a cui ci si connette vengono eliminati anche dal record a cui ci si connette.

  Ad esempio, quando si collegano le campagne a un altro tipo di record denominato prodotto e si eliminano dalla campagna il campo connesso al prodotto e il campo di ricerca Stato del prodotto, vengono eliminati i seguenti elementi:

   * Il campo Prodotto connesso dalla campagna
   * Il campo di ricerca Stato prodotto dalla campagna
   * Il campo Campaign connesso dal prodotto.

  Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>L'organizzazione deve essere iscritta alla fase di accesso anticipato per Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Nuovo: Standard</p>
   <p>Corrente: Piano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Nessun controllo del livello di accesso per Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere l'area Planning nel modello di layout. Per informazioni, vedere <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica dell'accesso</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
</td>
  </tr>
 </tbody>
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Elimina campi

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera eliminare i campi record.

   Viene aperto il workspace e vengono visualizzati i tipi di record.

1. Fare clic sulla scheda di un tipo di record.

1. (Condizionale) Se non è già selezionata, fare clic sulla scheda di una **visualizzazione tabella** nella pagina del tipo di record.

   Tutti i record esistenti associati al tipo di record vengono visualizzati nelle righe della vista tabella.

1. Individuare il campo da eliminare nelle intestazioni di colonna, posizionare il puntatore del mouse sull&#39;intestazione di colonna e fare clic sulla freccia rivolta verso il basso dopo il nome del campo.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Fai clic su **Elimina**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Fai clic su **Elimina** per confermare.

   Il campo viene eliminato, non può essere recuperato e non può più essere associato ad alcun record.
