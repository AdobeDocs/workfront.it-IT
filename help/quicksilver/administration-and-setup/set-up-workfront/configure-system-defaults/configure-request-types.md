---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurare i tipi di richiesta
description: Quando lavori a un progetto, potresti scoprire che si verificano eventi imprevisti. È possibile registrare tali eventi imprevisti come problemi per un progetto o un'attività particolare. Puoi anche inviare richieste, che vengono registrate come problemi in un progetto designato come coda di richieste. I problemi e le richieste sono considerati intercambiabili in Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Configurare i tipi di richiesta

Quando lavori a un progetto, potresti scoprire che si verificano eventi imprevisti. È possibile registrare tali eventi imprevisti come problemi per un progetto o un&#39;attività particolare. Puoi anche inviare richieste, che vengono registrate come problemi in un progetto designato come coda di richieste. I problemi e le richieste sono considerati intercambiabili in Adobe Workfront.

Per informazioni sulla creazione di problemi in [!DNL Workfront], vedi [Crea problemi](../../../manage-work/issues/manage-issues/create-issues.md). Per informazioni sulla creazione di richieste in [!DNL Workfront], vedere [Creare e inviare [!DNL Adobe Workfront] richieste](../../../manage-work/requests/create-requests/create-submit-requests.md). Per informazioni sull&#39;associazione dei tipi di richiesta ai progetti, vedere [Definire i tipi di richiesta per un progetto](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td><p>Nuovo: [!UICONTROL Standard]</p>
   Oppure
   <p>Corrente: [!UICONTROL Plan]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
THIS IS DRAFTED IN FLARE
<h2>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind of unexpected work might occur during the lifetime of a project.</p>
<p>You can specify the type of requests that can be logged on a project when you configure the <strong>Queue Details</strong> area for the project. </p>
<ol>
<li value="1"> <p> Click <strong>Projects</strong> in the Main Menu. <img src="assets/main-menu-icon.png"> </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> In the left panel, click <strong>Queue Details</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## Personalizzare i nomi dei tipi di richiesta

In qualità di amministratore [!DNL Workfront], puoi configurare i nomi dei tipi di richiesta nel sistema. I nuovi nomi sono visibili in qualsiasi area di [!DNL Workfront] in cui vengono visualizzati i campi **[!UICONTROL Tipo di problema]** o **[!UICONTROL Tipo di richiesta]**:

* Nell&#39;area **[!UICONTROL Dettagli coda]** di un progetto che riceverà i problemi o le richieste.
* Se per una coda di richieste sono selezionati più tipi di richiesta, nel modulo **[!UICONTROL Nuovo problema]** nel campo **[!UICONTROL Tipo problema]** quando si crea un nuovo problema o si invia una nuova richiesta.

  Per ulteriori informazioni sulla creazione di problemi in [!DNL Workfront], vedi [Crea problemi](../../../manage-work/issues/manage-issues/create-issues.md)

  Per ulteriori informazioni sulla creazione di richieste in [!DNL Workfront], vedere [Creare e inviare [!DNL Adobe Workfront] richieste](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Nel modulo **[!UICONTROL Dettagli argomento coda]**, quando si configura l&#39;argomento coda.\
   Per ulteriori informazioni sulla creazione degli argomenti della coda, vedere [Creare argomenti della coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Per personalizzare i nomi dei tipi di richiesta:

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Preferenze progetto]** > **[!UICONTROL Stati]**.

1. Fai clic sulla scheda **[!UICONTROL Issues]**.
1. Nella parte superiore della scheda **[!UICONTROL Problemi]**, passa il puntatore del mouse sul nome di un tipo di richiesta, quindi fai clic sull&#39;icona **[!UICONTROL Modifica]** visualizzata.

   ![Modifica nome tipo di richiesta](assets/edit-request-type-name-nwe.png)

1. Nella casella visualizzata digitare un nuovo nome e premere **[!UICONTROL Invio]**.

## Configurare gli stati dei problemi in diversi tipi di richiesta

È possibile associare ogni tipo di richiesta a diversi stati di problema. Puoi anche modificare l’ordine in cui gli stati vengono visualizzati su un problema, a seconda del tipo di problema.

Per ulteriori informazioni sulla modifica dell&#39;ordine predefinito degli stati dei problemi e sulla configurazione degli stati dei problemi, vedere la sezione [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) in [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
