---
product-area: projects
navigation-topic: manage-tasks
title: Associa milestone alle attività
description: È possibile associare le fasi cardine alle attività per indicare quando si raggiungono passaggi importanti nel corso della durata del progetto.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Associa milestone alle attività

È possibile associare le fasi cardine alle attività per indicare quando si raggiungono passaggi importanti nel corso della durata del progetto.

## Requisiti di accesso

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
  <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso alle attività</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per l’attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di associare un&#39;attività cardine a un&#39;attività, è necessario che siano presenti le seguenti informazioni:

* L’amministratore di Workfront deve creare un percorso cardine, come descritto in [Creare un percorso cardine](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Per associare un percorso cardine a un progetto, è necessario che il progetto sia in stato Planning o Current.

>[!TIP]
>
>Per ottenere la migliore panoramica dell’avanzamento delle tappe dei progetti utilizzando la vista Milestone, è necessario creare attività principali e associarle a ogni fase principale del progetto. Quindi, associare queste attività principali a ciascuna delle tappe del percorso cardine.

## Associare un&#39;attività cardine a un&#39;attività

1. Passa a un progetto, quindi fai clic sul pulsante **Altro** icona ![](assets/more-icon.png), quindi **Modifica**.
1. Utilizzo della **Impostazioni** imposta il percorso cardine da utilizzare nel progetto.
1. Fai clic su **Salva**.

   Dopo aver associato un percorso cardine a un progetto, è possibile assegnare alle attività un&#39;attività cardine.

1. Passa a un’attività, quindi fai clic sul pulsante **Altro** icona ![](assets/more-icon.png), quindi **Modifica**.

   Le attività e le attività cardine hanno una relazione 1:1. Non è possibile associare la stessa attività cardine a più attività. Ogni attività può essere collegata a un&#39;unica attività cardine oppure ogni attività cardine può essere mappata a un&#39;unica attività.

1. Fai clic su **Impostazioni**, quindi seleziona una fase cardine nel **Milestone** campo per l’attività.
1. Fai clic su **Salva**.
1. (Facoltativo) In un elenco di attività, aggiungi la **Icone di stato** per identificare le attività con tappe principali.

   ![](assets/amwt3.png)

1. (Facoltativo) In un elenco di progetti, seleziona la **Milestone** per identificare l&#39;avanzamento delle attività cardine.

   ![Screen_Shot_2018-06-13_at_3.57.56_PM.png](assets/screen-shot-2018-06-13-at-3.57.56-pm-350x57.png)
