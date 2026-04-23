---
product-area: requests
navigation-topic: create-requests
title: Creare e gestire le viste nell’area Richieste
description: Se utilizzi la nuova esperienza di richiesta, puoi creare e salvare viste per l’area Richieste.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 058abefdf7bcee16b9cee7f28e10337886c7fb05
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 9%

---


# Creare e gestire le viste nell’area Richieste

<!--

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

Se utilizzi la nuova esperienza di richiesta in Adobe Workfront, puoi creare e salvare viste per l’area Richieste. Queste visualizzazioni includono filtri, disposizione delle colonne e raggruppamenti.

>[!IMPORTANT]
>
>* Questa funzionalità è disponibile solo nella nuova esperienza di richiesta nell’area Richieste.
>* Le impostazioni di visualizzazione sono disponibili anche nel widget Richieste personali nella Home. Tuttavia, le viste dall’area Richieste sono separate da quelle del widget Richieste personali.
>* L’elenco delle richieste nell’area Richieste e nel widget Il mio lavoro utilizza l’elenco avanzato in Workfront. Per ulteriori informazioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workfront o flusso di lavoro</p>
   <p>Qualsiasi licenza di Workfront Planning, per visualizzare le richieste di Workfront Planning negli elenchi delle richieste</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Collaboratore o successiva</p>
   <p>Richiedente o successiva</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p>  <p>Per aggiungere visualizzazioni ai modelli di layout è necessario essere un amministratore Workfront</td> 
  </tr> 
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzazioni di sistema per le richieste

>[!WARNING]
>
>Le visualizzazioni di sistema documentate in questa sezione non sono ancora disponibili. Saranno disponibili dopo il 16 aprile 2026.

Oltre alle viste che è possibile creare autonomamente, Workfront offre le seguenti viste di sistema per l&#39;area Richieste e il widget Richieste personali nella Home:

* **Tutte le richieste**: tutte le richieste inviate da te o da altri utenti in code o aree di lavoro per cui disponi delle autorizzazioni di visualizzazione. Questo non è disponibile per il widget Richieste personali.
* **Richieste personali**: richieste inviate, indipendentemente dallo stato.
* **Richieste aperte**: richieste inviate e ancora aperte.
* **Le mie bozze**: bozze delle tue missioni che non sono ancora state inviate.
* **Richieste aperte**: richieste inviate da te o da altri utenti in code o per aree di lavoro per le quali disponi delle autorizzazioni di visualizzazione e ancora aperte. Questo non è disponibile per il widget Richieste personali.

Non è possibile modificare le viste di sistema. Puoi modificarne gli elementi, quindi copiare la vista e modificare o condividere la copia.

## Creare una visualizzazione per le richieste

Puoi creare una visualizzazione nell’area Richieste di Workfront quando utilizzi la nuova esperienza Richieste. Dopo l’abilitazione e la nuova esperienza di richieste, puoi anche creare visualizzazioni per il widget Richieste personali nella Home.

1. Per accedere all&#39;elenco **Richieste**:

   {{step1-to-requests}}

   1. Verificare che l&#39;impostazione **Usa nuova esperienza** sia attivata.

1. Per accedere al widget **Richieste personali** nella home:

   {{step1-to-home}}

   1. Aggiungi o vai al widget **Richieste personali**.

1. Nell&#39;elenco delle richieste fare clic sul menu a discesa **Visualizzazioni** ![Visualizzazioni](assets/view-icon-requests.png) e quindi su **Nuova visualizzazione**.

   <!-- 
   
   replace the screen shot with release
   ![New view](assets/create-new-view.png)

   -->

1. Immettere un nome per la nuova visualizzazione e fare clic su **Crea**.
1. Continua con [Modifica una visualizzazione per le richieste](#edit-a-view-for-requests).

## Modificare una visualizzazione per le richieste

Puoi modificare le viste esistenti, comprese quelle appena create nell’area Richieste o il widget Richieste personali nella Home.

Modificando una vista, è possibile modificare i seguenti elementi della vista:

* Nome
* Filtri
* Colonne
* Raggruppamento
* Formatta celle
* Altezza riga

Per ulteriori informazioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!-- 
hide these details - all the information is in "Use enhanced lists" - we need one point of messaging for this feature: 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to edit from the **Views** dropdown menu ![Views dropdown](assets/view-icon-requests.png).

1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and click the three-dot menu next to the view, select **Rename**, then type in the new name for the view.
1. Press Enter to save the new name. 
1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and select the view you want to edit.
1. To add a field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list. 

   The **Column manager** opens.
1. Click the plus icon next to the field that you want to add as a column to the view, then click **Save**.

   Fields associated with the objects in the list are available to add as columns. <!-keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future->

   >[!TIP]
   >
   >Fields you add to the columns must exist before they are available in the **Column manager**.

1. (Optional) Click **Columns** to open the **Fields visibility and order** box. 
1. Turn on the setting for each field  you want to show in the list, turn it off to hide it, or drag and drop the fields in a different order.

1. (Optional) Click **Filters** and start adding conditions for what requests you want to view. 

    You can filter by the following request fields:  

    * **Workspace**: The workspace the request form is associated with.
    * **Object type**: The record type the request form is associated with.
    * **Entry date**: The date when the request was submitted.
    * **Request form**: The name of the request form used to submit the request.
    * **Status**: The status of the request.
    * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.

    You can also filter by any fields that have been added to the view for any object visible in the view.

    You can have multiple filters joined by either **And** or **Or**.
    The request list is filtered automatically, as you add the filter conditions. 
-->

<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Le modifiche alle viste vengono salvate automaticamente.
> * Le modifiche apportate alle viste sono visibili a tutti gli utenti che utilizzano la vista solo quando si condivide una nuova copia della vista dopo averla modificata.
> * Utilizza il carattere jolly del filtro **Me (utente connesso)** in qualsiasi campo il cui valore è utenti.

## Aggiungere la vista richieste a un modello di layout

Un amministratore di Workfront può aggiungere o rimuovere una nuova visualizzazione o una visualizzazione di sistema ai modelli di layout per l’area Richieste.

Per istruzioni, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Condividere una visualizzazione

Puoi condividere le viste create con altri utenti, team, gruppi o aziende.

Dopo aver condiviso una vista, gli altri utenti possono visualizzare gli elementi di vista aggiornati modificati per la vista prima di condividerla.

Se la vista viene aggiornata, le modifiche apportate non saranno visibili agli altri utenti, a meno che non creino una copia della stessa vista e non mantengano le modifiche prima di condividere la copia.

Per ulteriori informazioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!--
Let's just redirect to Use enhanced lists so we avoid duplicating information. 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to share.
1. Hover over the view that you want to share, then click on the three-dot menu to the right of the view name, then click  **Share**.
1. In the **Share** box, enter the people, teams, roles, groups, or companies that you want to share the view with, then select them from the list when they appear.
1. Click **Save**.

   The view is shared with the entities you indicate. 
-->