---
product-area: projects
navigation-topic: use-the-home-area
title: Utilizzare il widget Le mie richieste
description: È possibile inviare richieste nel widget Richieste personali. Puoi anche personalizzare il widget con filtri e colonne.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: a6c2bc4127a52fad209004995ea2262fa64c240d
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 7%

---

# Utilizzare il widget Le mie richieste

<!--
remove Preview and Production references at Production release April 15, 2026

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>Questo articolo descrive il nuovo widget Richieste personali. Per visualizzare il nuovo widget, è necessario che sia abilitata la nuova esperienza di richiesta.
>Puoi abilitare la nuova esperienza di richiesta nell’area Richieste.

Il widget Richieste personali visualizza le richieste inviate. Puoi filtrare le richieste, cercare richieste specifiche o regolare l’ordine e la visibilità delle colonne. Puoi anche creare una nuova richiesta dal widget Richieste personali.

>[!NOTE]
>
>* Quando viene caricato, il widget Richieste personali visualizza fino a 50 richieste. Per visualizzare altre richieste, scorri l’elenco verso il basso.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Qualsiasi pacchetto Workfront o flusso di lavoro</p>
   <p>Qualsiasi pacchetto di Workfront Planning per accedere alle richieste di Workfront Planning e ai relativi oggetti creati</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza</strong></td> 
   <td> <p>Collaboratore o successiva</p>
   <p>Richiedente o successiva</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>Configurazione del livello di accesso</strong></td> 
   <td> <p>Accesso di visualizzazione o accesso successivo a qualsiasi oggetto per il quale si è taggati in una conversazione o per il quale è necessario risolvere un'approvazione (progetti, attività, problemi, documenti)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni sugli oggetti</strong></td> 
   <td> <p>Autorizzazioni di [!UICONTROL View] o superiori per progetti, attività, problemi e documenti a cui vengono assegnati tag in una conversazione o in cui è necessario risolvere un'approvazione</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una richiesta

È possibile creare una richiesta direttamente dal widget Richieste personali.

Per istruzioni, vedere la sezione [Creare una richiesta](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request) nell&#39;articolo [Creare elementi di lavoro e progetti dall&#39;area Home](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Copiare una richiesta

È possibile copiare una richiesta nel widget Richieste personali, modificarla e inviarla come nuova richiesta.

Per istruzioni, consulta [Copiare e inviare richieste](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Gestire le informazioni nell&#39;elenco delle richieste nel widget Richieste personali

<!--
This is similar to what we document in Enhanced lists, so we will link to that to avoid documentation duplication:
The My Requests widget features a customizable filter that allows you to control which requests appear in the widget. You can configure this filter for different fields and values, and can stack conditions using AND and OR operators.

To configure the filter in the My Requests widget:
-->

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Per aggiungere il widget **Richieste personali** alla schermata iniziale. Fai clic su **Personalizza** e trova **Le mie richieste**, quindi fai clic su di esso per aggiungerlo alla **Home**.
1. (Facoltativo) Per gestire la modalità di visualizzazione delle informazioni nell’elenco delle richieste, crea o aggiorna i seguenti elementi di visualizzazione per l’elenco:

   * Visualizzazione
   * Filtro
   * Colonne
   * Raggruppamento
   * Formatta celle
   * Altezza riga

   Per ulteriori informazioni sull&#39;aggiornamento degli elementi di visualizzazione nell&#39;elenco delle richieste, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


<!--
 Removed all these sections because this is common to ALL the Glists/ enhanced lists. So, we will update that article with all the specific steps: 
1. Select the field that you want to filter by. Available options are:

   * Workspace
   * Object type
   * Entry date
   * Request form
   * Status
   * Entered by
   * Custom fields from the request or from the created object   

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.
The filter is saved automatically.
-->

>[!TIP]
>
>Se l&#39;organizzazione ha acquistato Workfront Planning oltre ad Adobe Workfront, il widget Richieste personali includerà le richieste Workfront e Workfront Planning.
> 
>* Per filtrare solo le richieste Workfront, impostare il filtro su **Tipo di oggetto** > **Ha uno di** > **Problemi**.
>* Per filtrare solo le richieste di Workfront Planning, impostare il filtro su **Tipo di oggetto** > **Non contiene** > **Problemi**.

<!--

Use enhanced lists and other requests articles describe all of these:

## Adjust or add columns

You can choose which of the available columns appear on the My Requests widget, and set their order.

Available columns include:

* Subject
* Created object
* Object type
* Status
* Request form
* Entry date
* Entered by

To adjust the columns on the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. In the **My Requests** widget, click **Columns**.
1. (Optional) To reorder columns, click the drag handle ![drag handle](assets/drag-handle.png) of the column you want to move and drag it to the desired locations. The column at the top of the list appears in the My Requests widget as the first column.
1. (Optional) Use the toggle to hide or show the column in the requests list.
1. To add a custom field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list, and click the plus icon next to the custom field that you want to add as a column to the widget.

   Custom fields on forms attached to the object in the list are available to add as columns.

Column preferences are saved automatically.

-->

<!--

## Create a view

You can create views in the My Requests widget to change the way the information displays in the request list. 

Consider the following when working with views in the My Requests widget:

* A view in the My Requests widget contains the columns and filters applied to the view.
* You can create views and share them with others. The filters and columns you select for the view before you share it are included in the views you share. 
* The following is a system view which you cannot edit, share, or delete: 

   * Widget Unified Requests Default View
* Creating and editing a view in the My Requests widget is similar to enhanced lists. For information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). 

-->

## Richieste di ricerca

Per cercare richieste specifiche nel widget Richieste personali:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Per aggiungere il widget **Richieste personali** alla schermata iniziale. Fai clic su **Personalizza** e trova **Le mie richieste**, quindi fai clic su di esso per aggiungerlo alla **Home**.
1. Nella barra di ricerca in alto a destra del widget Richieste personali, immettere il termine che si desidera cercare.

   Le richieste che contengono il termine vengono evidenziate in arancione.

1. (Facoltativo) Per passare alle richieste evidenziate, fai clic sulle frecce su o giù nella barra di ricerca.

## Passare a un oggetto creato da una richiesta

È possibile trovare gli oggetti creati da una richiesta nel widget Richieste personali.

>[!NOTE]
>
>Quando abilitate la nuova esperienza richieste nell&#39;area Richieste, nel widget Richieste personali sono presenti i collegamenti dell&#39;elenco Richieste del widget Richieste personali degli oggetti seguenti:
>
>* Richieste Planning e Workfront nel campo Oggetto.
>* Record di Planning creati dalle richieste di Planning nel campo Oggetto creato.
>* Le attività e i problemi di Workfront convertiti dalle richieste di Workfront nel campo Oggetto creato.

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Per aggiungere il widget **Richieste personali** alla schermata iniziale. Fai clic su **Personalizza** e trova **Le mie richieste**, quindi fai clic su di esso per aggiungerlo alla **Home**.
1. Individuare la richiesta che ha creato l&#39;oggetto.
1. Fare clic sul nome dell&#39;oggetto nella colonna **Oggetto creato** per la richiesta.

   Viene visualizzata la pagina dell&#39;oggetto.

   >[!TIP]
   >
   >Le attività e i progetti Workfront convertiti da problemi e i record Planning creati da richieste Planning hanno un collegamento nel campo **Oggetto creato**.



