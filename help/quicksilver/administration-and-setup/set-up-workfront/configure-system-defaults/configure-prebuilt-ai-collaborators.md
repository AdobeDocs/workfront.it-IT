---
user-type: administrator
product-area: system-administration;setup
title: Configurare i collaboratori IA predefiniti
description: In qualità di amministratore di Adobe Workfront, puoi configurare i collaboratori basati su IA predefiniti di Adobe, come ad esempio il coordinatore dell’acquisizione, come agenti di lavoro che gli utenti possono assegnare ad attività e problemi.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: c95c5a71a2706d4ddbf3e53a579b348bd072a04e
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 7%
---
# Configurare i collaboratori IA predefiniti

## Panoramica

I collaboratori basati su IA predefiniti sono agenti di lavoro pronti di Adobe configurati per eseguire un processo specifico, ad esempio controllare le richieste di informazioni mancanti. Sono disponibili come agenti di lavoro nativi di Adobe, quindi non è necessario configurare un agente in una piattaforma esterna o fornire credenziali di piattaforma esterna.

Quando si configura un agente di lavoro, si seleziona un collaboratore predefinito come origine dell&#39;agente. È quindi possibile assegnare un nome all&#39;agente di lavoro, impostarne il livello di accesso e scegliere le azioni da eseguire. Gli utenti assegnano l’agente di lavoro configurato alle attività o ai problemi nello stesso modo in cui assegnano qualsiasi altro agente di lavoro. Gli utenti non devono sapere che l&#39;agente è un collaboratore predefinito.

Per ulteriori informazioni sugli agenti di lavoro e sugli altri tipi di collaboratori IA, vedere [Configurare i collaboratori IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Seleziona, Prime o Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>[!UICONTROL Standard]</p></td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL System Administrator] o Group Administrator</td> 
  </tr> 
  </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

La tua organizzazione deve avere Adobe CX Coworker abilitato. Per ulteriori informazioni, vedere [Panoramica di CX Enterprise Coworker in Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

## Configurare un Collaboratore IA predefinito

Quando si configura un agente di lavoro, viene configurato un collaboratore AI predefinito. Nell&#39;area **Scegli l&#39;origine dell&#39;agente**, selezionare **Adobe Native**, quindi selezionare il collaboratore predefinito che si desidera utilizzare dall&#39;elenco seguente.

Per i passaggi completi, vedere [Configurare un agente di lavoro in Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent-in-workfront).

Dopo aver configurato Collaborator, gli utenti possono assegnarlo ad attività o problemi. Per ulteriori informazioni, vedere [Utilizzare agenti di lavoro](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

## Collaboratori IA predefiniti disponibili

### CX Enterprise Coworker {#cx-enterprise-coworker}

Agente CX Enterprise Coworker basato su Adobe Agent Orchestrator.

Per ulteriori informazioni, vedere [Panoramica di CX Enterprise Coworker in Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

### Coordinatore acquisizione {#intake-coordinator}

Il coordinatore dell’acquisizione controlla i dettagli, i moduli personalizzati e gli allegati delle richieste di informazioni mancanti, non chiare o incoerenti. Pubblica feedback o apporta modifiche con l’approvazione dell’utente.

>[!NOTE]
>
>È possibile assegnare il coordinatore di assunzione a una regola di instradamento quando la regola viene creata, ma non è possibile assegnarlo in un secondo momento.

<!--
### Context Carrier {#context-carrier}

The Context Carrier keeps brief information flowing downstream so that context doesn't get scattered. It helps campaign managers and project managers keep the project team current without writing reports.

Requirements: A Workfront project and a Workfront Planning project must be connected to a Planning record. The Context Carrier must be triggered to run.

Steps to be added.

### Production Specialist {#production-specialist}

The Production Specialist produces images in every size you need, so designers don't have to resize them manually.

Requirement: Users must assign the Production Specialist to a task or issue.

Steps to be added.

### Version Comparer {#version-comparer}

The Version Comparer compares versions of a document so project teams can move content faster instead of spotting differences by hand.

Requirement: The document must have more than one version.

Steps to be added.

### Metadata Manager {#metadata-manager}

The Metadata Manager helps marketing teams find, tag, and label documents while work is in progress instead of later in the process.

Requirement: The Metadata Manager is available when you upload a document. Users must trigger it from the toolbar.

Steps to be added.

### Resource PTO Detector {#resource-pto-detector}

The Resource PTO Detector helps project teams make sure delivery isn't affected by time off, by identifying tasks assigned to people who are out of office.

Requirements: Tasks must be assigned, and PTO must be logged in Workfront.

Steps to be added.

### Campaign Summarizer {#campaign-summarizer}

Description and steps to be added.
-->
