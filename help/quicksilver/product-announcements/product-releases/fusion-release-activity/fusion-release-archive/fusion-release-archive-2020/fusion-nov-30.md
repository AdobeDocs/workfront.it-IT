---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
keywords: fusione
navigation-topic: fusion-release-activity
title: "Attività di rilascio di Workfront Fusion: settimana del 30 novembre 2020"
description: Questa pagina descrive tutti i miglioramenti apportati ad Adobe Workfront Fusion la settimana del 30 novembre 2020.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 9621683b-735d-40a6-8d7c-b5bd167cbdd2
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Attività di rilascio di Workfront Fusion: settimana del 30 novembre 2020

Questa pagina descrive tutti i miglioramenti apportati ad Adobe Workfront Fusion la settimana del 30 novembre 2020.

Per un elenco di tutte le modifiche recenti, vedere [Attività di Adobe Workfront Fusion release](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Per un elenco delle correzioni di bug recenti in Workfront Fusion, vedere la pagina [Aggiornamenti di manutenzione di Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) e verificare la presenza di eventuali aggiornamenti etichettati Aggiornamento di manutenzione di Workfront Fusion.

## Limite di frequenza per i webhook di Workfront Fusion 2.0.

È stato introdotto un nuovo guardrail delle prestazioni per Workfront Fusion 2.0. Adesso, i webhook hanno un limite di velocità di 100 richieste al secondo. Al raggiungimento di questo limite, Workfront Fusion 2.0 invia lo stato 429 (Troppe richieste).

In precedenza, le richieste di webhook non erano limitate.

Per ulteriori informazioni, vedere [Guardrail delle prestazioni di Adobe Workfront Fusion](../../../../../workfront-fusion/get-started/fusion-performance-guardrails.md).

## Aggiungere un modulo personalizzato a un oggetto Workfront in Workfront Fusion 2.0

Per consentire l’aggiunta di moduli personalizzati agli oggetti è Workfront Fusion 2.0, è stata aggiunta l’azione AssegnaCategorie a Workfront > Varie. Modulo azione.

In precedenza, non era possibile utilizzare un modulo di Workfront Fusion 2.0 per aggiungere un modulo personalizzato a un oggetto in Workfront.

Per ulteriori informazioni su Workfront > Varie. Modulo azione, vedi [Moduli Adobe Workfront](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Jira Server connector and modules now available</h2>
<p>We've added a Jira Server connector to Workfront Fusion. The Jira Server connector offers the same functionality as the current Jira Cloud connector. </p>
<p>With Jira Server modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, modified, or deleted</p> </li>
<li> <p>Create, read, update, or delete a record</p> </li>
<li> <p>List or search records</p> </li>
<li> <p>Download an attachment</p> </li>
<li> <p>Add an issue to a sprint</p> </li>
<li> <p>Make a custom API call</p> </li>
</ul>
<p>Previously, Jira modules were available only for Jira Cloud.</p>
<p>For more information on available Jira modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref" xrefformat="{para}">Jira Software modules</a>.</p>
<h2>Azure DevOps connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Azure DevOps applications. With the Azure DevOps modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, updated, or deleted.</p> </li>
<li> <p>Create or update records.</p> </li>
<li> <p>Get data from existing records.</p> </li>
<li> <p>Download or upload attachments.</p> </li>
<li> <p>Link work items together.</p> </li>
<li> <p>Retrieve a list of work items.</p> </li>
<li> <p>Perform a custom API call.</p> </li>
</ul>
<p>For more information see <a href="../../../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref" xrefformat="{para}">Azure DevOps modules</a>.</p>
<h2>Microsoft Dynamics 365 connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Microsoft Dynamics 365 account. With the Microsoft Dynamics 365 modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when records are added or updated in Microsoft Dynamics 365</p> </li>
<li> <p>Create, read, update, or delete a Microsoft Dynamics 365record</p> </li>
<li> <p>Perform a custom API call</p> </li>
</ul>
<p>For information about available Microsoft Dynamics 365 modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref" xrefformat="{para}">Microsoft Dynamics 365 modules</a>.</p>
</div>
-->
