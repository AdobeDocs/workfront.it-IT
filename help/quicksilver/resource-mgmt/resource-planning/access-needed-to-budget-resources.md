---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Accesso necessario alle risorse di budget in Adobe Workfront
description: È possibile visualizzare e gestire le informazioni sulla pianificazione delle risorse per i progetti a cui si ha accesso quando si dispone di determinate impostazioni del livello di accesso e delle autorizzazioni per gli elementi di lavoro, gli utenti, i ruoli di lavoro e i team.
author: Alina
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Accesso necessario alle risorse di budget in Adobe Workfront

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

Quando la società ha acquistato una licenza Adobe Workfront che include la pianificazione delle risorse, è possibile visualizzare le informazioni di budget delle risorse per i progetti che si dispone delle autorizzazioni per visualizzare. È possibile visualizzare le informazioni sul budget nel Planner risorse.

Per ulteriori informazioni sui prerequisiti per l&#39;utilizzo degli strumenti di budget in Workfront, consulta [Guida introduttiva alla pianificazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Per assegnare un budget alle risorse, gestire i pool di risorse e visualizzare le informazioni sui costi negli strumenti di pianificazione delle risorse, nella tua azienda e devi disporre dei seguenti accessi: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> 
    <ul> 
     <li> <p>Modifica l'accesso a Gestione risorse nel livello di accesso che include:</p> 
      <ul> 
       <li> <p>Accesso alla modifica delle priorità del progetto e delle ore di budget. </p> </li> 
       <li> <p>Accesso alla gestione dei pool di risorse, se è necessario gestire il pool di risorse.</p> </li> 
      </ul> <p>Per informazioni sul livello di accesso a Gestione risorse, vedere l'articolo <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Concedere l’accesso a Gestione risorse</a>.</p> </li> 
     <li> <p>Modifica l’accesso a Progetti e utenti. </p> </li> 
     <li> <p> Modificare l'accesso ai dati finanziari nel livello di accesso, se è necessario visualizzare o gestire le informazioni in base al costo.</p> <p>Per ulteriori informazioni sul livello di accesso ai dati finanziari, consulta l’articolo <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concedere l’accesso ai dati finanziari</a>.</p> </li> 
    </ul>

<p><b>NOTA</b> </p>

<p> Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per il progetto che includono le autorizzazioni di Manage Finance.</p> <p>Per informazioni sulle autorizzazioni del progetto, consulta l’articolo <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Condivisione di un progetto in Adobe Workfront</a>.</p> <p>Per informazioni sulle autorizzazioni finanziarie per un progetto, consulta l’articolo <a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Condividere le autorizzazioni finanziarie su un oggetto</a></a>.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md">Richiedere l’accesso agli oggetti </a>.</p>

<p><b>NOTA</b>

Quando si inserisce nel budget una risorsa nella vista Ruolo, se si dispone di autorizzazioni di gestione inferiori a quelle per almeno un progetto elencato nel ruolo, non è possibile impostare il budget per ore, FTE o Costo per il ruolo. Puoi eseguire il budget solo dei progetti per i quali disponi delle autorizzazioni di gestione .</p> </td>
</tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.
