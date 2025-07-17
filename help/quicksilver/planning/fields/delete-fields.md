---
title: Elimina campi
description: In Adobe Workfront Planning è possibile eliminare i campi personalizzati che non sono più rilevanti.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 1%

---



# Elimina campi

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

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

+++ Espandere per visualizzare i requisiti di accesso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestire le autorizzazioni per un'area di lavoro e il tipo di record </a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p></td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Elimina campi

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera eliminare i campi record.

   Viene aperto il workspace e vengono visualizzati i tipi di record.

1. Fare clic sulla scheda di un tipo di record.

1. (Condizionale) Se non è già selezionata, fare clic sulla scheda di una **visualizzazione tabella** nella pagina del tipo di record.

   Tutti i record esistenti associati al tipo di record vengono visualizzati nelle righe della vista tabella.

1. Individuare il campo da eliminare nelle intestazioni di colonna, posizionare il puntatore del mouse sull&#39;intestazione di colonna e fare clic sulla freccia rivolta verso il basso dopo il nome del campo.

   ![Menu freccia dopo il nome del campo nell&#39;intestazione della tabella evidenziato](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Fai clic su **Elimina**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Fai clic su **Elimina** per confermare.

   Il campo viene eliminato, non può essere recuperato e non può più essere associato ad alcun record.
