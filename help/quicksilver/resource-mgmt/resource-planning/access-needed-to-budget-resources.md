---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Accesso necessario alle risorse del budget in Workfront
description: È possibile visualizzare e gestire le informazioni sulla pianificazione delle risorse per i progetti a cui si ha accesso quando si dispone di determinate impostazioni del livello di accesso e delle autorizzazioni per gli elementi di lavoro, gli utenti, le mansioni e i team.
author: Lisa
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Accesso necessario alle risorse del budget in Workfront

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

Quando la società ha acquistato una licenza Adobe Workfront che include la pianificazione delle risorse, è possibile visualizzare le informazioni sul budget delle risorse per i progetti per i quali si dispone delle autorizzazioni di visualizzazione. È possibile visualizzare le informazioni di budget nella Programmazione risorse.

Per ulteriori informazioni sui prerequisiti per l&#39;utilizzo degli strumenti di definizione del budget in Workfront, vedere [Introduzione alla pianificazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Per preventivare le risorse, gestire i gruppi di risorse e visualizzare le informazioni sui costi negli strumenti di pianificazione delle risorse, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> 
    <ul> 
     <li> <p>Modifica l'accesso a Gestione risorse nel tuo livello di accesso, che include:</p> 
      <ul> 
       <li> <p>Accesso per modificare le priorità del progetto e le ore preventivate. </p> </li> 
       <li> <p>Accesso per gestire i gruppi di risorse, se è necessario gestire i gruppi di risorse.</p> </li> 
      </ul> <p>Per informazioni sul livello di accesso Gestione risorse, vedere l'articolo <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Concedere l'accesso a Gestione risorse</a>.</p> </li> 
     <li> <p>Modifica l'accesso a Progetti e Utenti. </p> </li> 
     <li> <p> Modificare l'accesso ai dati finanziari nel proprio livello di accesso, se è necessario visualizzare o gestire le informazioni in base al costo.</p> <p>Per ulteriori informazioni sul livello di accesso ai dati finanziari, vedere l'articolo <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concedere l'accesso ai dati finanziari</a>.</p> </li> 
    </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Consente di gestire le autorizzazioni per il progetto che includono le autorizzazioni Gestisci dati finanziari.</p> <p>Per informazioni sulle autorizzazioni del progetto, vedere l'articolo <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Condividere un progetto in Adobe Workfront</a>.</p> <p>Per informazioni sulle autorizzazioni finanziarie per un progetto, vedere l'articolo <a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Condividere le autorizzazioni finanziarie su un oggetto</a></a>.</p>

<p><b>NOTA:</b> quando si impostano le risorse nel budget nella visualizzazione Ruolo, se si dispone di autorizzazioni di gestione inferiori per almeno un progetto elencato sotto il ruolo, non è possibile preventivare ore, FTE o Costo per il ruolo. Puoi preventivare solo i progetti per i quali disponi delle autorizzazioni di gestione.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
