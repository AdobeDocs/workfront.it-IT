---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Consenti assegnazioni utente indipendentemente dal ruolo e dall'appartenenza al gruppo nelle aree di programmazione
description: Nella pianificazione delle risorse, le assegnazioni possono essere effettuate solo agli utenti che hanno un ruolo definito nel proprio profilo utente che corrisponde all'assegnazione del ruolo dell'attività o del problema a cui sono assegnate.
author: Alina
feature: Resource Management
exl-id: 0f90ffde-6f07-4c3c-b963-de28b1b55dc1
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---

# Consenti assegnazioni utente indipendentemente dal ruolo e dall&#39;appartenenza al gruppo nelle aree di programmazione

>[!IMPORTANT]
>  
><span class="preview">La funzionalità di pianificazione descritta in questo articolo è stata rimossa e rimossa da Adobe Workfront a partire dalla versione 23.1 di gennaio 2023.   </span>
>  
> <span class="preview"> Questo articolo verrà rimosso anche poco dopo la versione 23.1, all’inizio del 2023. Al momento, è consigliabile aggiornare di conseguenza tutti i segnalibri. </span>
> 
><span class="preview"> Ora puoi utilizzare il servizio di bilanciamento del carico di lavoro per pianificare il lavoro per le risorse. </span>
>  
> <span class="preview">Per informazioni sulla pianificazione delle risorse tramite il servizio di bilanciamento del carico di lavoro, consulta la sezione . [Il servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer.</span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;***LINKED TO THE UI FROM Resource Scheduling (People> Teams>Working On>Settings>Limit Assignments to the Group Associated with the Project) - ALSO FROM THE WORKING ON TAB OF TEAMS and AT THE PROJECT STAFFING TAB TOO)</p>
<p>NOTE: Alina; broken off the original article; retitle, reformat, relink sections) </p>
</div>
-->

Per impostazione predefinita, le assegnazioni possono essere effettuate solo agli utenti che hanno un ruolo definito nel proprio profilo utente che corrisponde all&#39;assegnazione del ruolo dell&#39;attività o del problema che viene loro assegnato quando si utilizzano gli strumenti di programmazione delle risorse.

È possibile configurare Adobe Workfront per consentire l’assegnazione di attività e problemi a qualsiasi utente, indipendentemente dal fatto che tale utente abbia un ruolo definito sul suo profilo utente che corrisponda all’assegnazione del ruolo dell’attività o del problema a cui è assegnato. Quando si assegna un utente a un&#39;attività o a un problema e tale utente non dispone di un ruolo corrispondente all&#39;assegnazione del ruolo nell&#39;attività o nel problema, l&#39;assegnazione del ruolo originale viene rimossa e l&#39;assegnazione del ruolo viene modificata in base al ruolo dell&#39;utente che si sta assegnando.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Accesso a progetti, attività e problemi</p> <p><strong>NOTA</strong>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute o superiori ai progetti, alle attività e ai problemi per i quali vengono aggiornate le assegnazioni</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Consenti assegnazioni agli utenti indipendentemente dal ruolo

1. Passa alla timeline della programmazione per più progetti, per un singolo progetto o per un team:

   * **Per progetti multipli**:  Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, fai clic su **Origine > Bilanciamento carico di lavoro**, quindi seleziona **Pianificazione** nel menu a discesa in alto a sinistra.
   * **Per un singolo progetto**: Passa a un progetto e fai clic sul pulsante **Bilanciamento del carico di lavoro** nel pannello a sinistra, quindi seleziona **Pianificazione** dal menu a discesa in alto a sinistra.
   * **Per un team**: Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Team**, seleziona un team e fai clic su **Bilanciamento del carico di lavoro** nel pannello a sinistra, seleziona **Pianificazione** dal menu a discesa in alto a sinistra.

1. Fai clic sul pulsante **Impostazioni** sulla timeline della pianificazione.
1. Disattiva l&#39;opzione **Limitare le assegnazioni agli utenti con ruolo corrispondente**.
1. Fai clic su **Torna alla pianificazione**.

## Consenti assegnazioni agli utenti indipendentemente dall&#39;appartenenza al gruppo

<!--
<p>(NOTE: Alina: **^ This section is linked to the UI in a tooltip inside the Settings of the scheduler. do not rename/ remove/ edit the tag!!) </p>
-->

Per impostazione predefinita, le assegnazioni possono essere effettuate solo agli utenti membri del gruppo associato al progetto (gruppo definito durante la modifica del progetto).

>[!IMPORTANT]
>
>Questa impostazione prende in considerazione solo i membri del gruppo associato al progetto e non i membri di alcun sottogruppo del gruppo.

È possibile configurare Workfront per consentire l’assegnazione di attività e problemi a qualsiasi utente, indipendentemente dal fatto che l’utente sia membro del gruppo associato al progetto in cui si trova l’attività o il problema.

1. Passa alla timeline della programmazione per più progetti, per un singolo progetto o per un team:

   * **Per progetti multipli**:  Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, fai clic su **Origine > Bilanciamento carico di lavoro**, quindi seleziona **Pianificazione** nel menu a discesa in alto a sinistra.
   * **Per un singolo progetto**: Passa a un progetto e fai clic sul pulsante **Bilanciamento del carico di lavoro** nel pannello a sinistra, quindi seleziona **Pianificazione** dal menu a discesa in alto a sinistra.
   * **Per un team**: Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Team**, seleziona un team e fai clic su **Bilanciamento del carico di lavoro** nel pannello a sinistra, seleziona **Pianificazione** dal menu a discesa in alto a sinistra.

1. Fai clic sul pulsante **Impostazioni** sulla timeline della pianificazione.
1. Disattiva l&#39;opzione **Limita assegnazioni al gruppo associato al progetto**.
1. Fai clic su **Torna alla pianificazione**.

 
