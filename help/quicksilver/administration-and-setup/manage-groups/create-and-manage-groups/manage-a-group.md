---
user-type: administrator
product-area: system-administration;user-management
keywords: gestisci,raggruppa,modifica,
navigation-topic: create-and-manage-groups
title: Gestire un gruppo
description: In qualità di amministratore di gruppo, puoi gestire un gruppo che amministri dall’area Gruppi in Configurazione. Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 0%

---

# Gestire un gruppo

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

In qualità di amministratore di gruppo, puoi gestire un gruppo che amministri dall’area Gruppi in Configurazione. Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

>[!NOTE]
>
>Quando si è assegnati come amministratore di un gruppo, si eredita il ruolo di amministratore del gruppo per tutti i sottogruppi al di sotto di esso. Gli unici utenti che possono gestire un sottogruppo sono gli amministratori di gruppo per il gruppo superiore e gli amministratori di gruppo assegnati al sottogruppo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>Oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gestire le appartenenze di un gruppo

È possibile aggiungere e rimuovere utenti e altri gruppi da un gruppo amministrato. È inoltre possibile assegnare membri del gruppo come amministratori e gestire le informazioni sul profilo utente dei membri del gruppo.

Per istruzioni, vedere [Visualizzare e gestire le appartenenze di un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## Gestire i dettagli di un gruppo

È possibile visualizzare e modificare la pagina Dettagli gruppo per un gruppo o un sottogruppo gestito dall&#39;utente. Questa pagina include una descrizione del gruppo, i nomi del Business Leader e degli amministratori di gruppi e un&#39;opzione che consente di rendere il gruppo e tutti i relativi sottogruppi pubblici o privati. Inoltre, se il proprio livello di accesso consente di gestire i moduli personalizzati, è possibile allegare un modulo personalizzato a un gruppo.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

Per istruzioni, vedere [Visualizzare e gestire i dettagli di un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Modificare, copiare o eliminare un gruppo

Senza uscire dalla pagina principale di un gruppo che si sta visualizzando, è possibile modificare, copiare o eliminare rapidamente il gruppo.

{{step-1-to-setup}}

1. Fai clic su **Gruppi**.

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Selezionare il gruppo, quindi fare clic sull&#39;icona Modifica ![](assets/edit-icon.png), Copia ![](assets/copy-icon.png) o Elimina ![](assets/delete.png).

   Per informazioni sull&#39;utilizzo della casella visualizzata, vedere una delle seguenti sezioni:

   * **Modifica**: [Visualizza e gestisci i dettagli di un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **Copia**: [Crea un gruppo di primo livello copiando un gruppo o un sottogruppo esistente](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) nell&#39;articolo [Crea un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **Elimina**: [Elimina un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## Configurare le preferenze di progetto, attività e problema per un gruppo

Se l&#39;amministratore di un gruppo necessita di impostazioni di preferenza di progetto, attività e problema diverse da quelle impostate a livello di sistema, è possibile chiedere all&#39;amministratore di Workfront di sbloccare una preferenza per tutti i gruppi dell&#39;organizzazione. Una volta sbloccato, l’utente (e gli amministratori di gruppi per tutti gli altri gruppi) possono configurarlo per i gruppi gestiti.

Per istruzioni, consulta [Configurare le preferenze del progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Elencare, aggiungere e configurare sottogruppi

Potete creare, visualizzare, modificare, copiare, rinominare, esportare ed eliminare sottogruppi sotto un gruppo amministrato.

## Configurare le notifiche degli eventi per un gruppo

Se un amministratore di Workfront sblocca la possibilità di configurare le notifiche degli eventi per i gruppi dell’organizzazione, puoi configurarle per un gruppo amministrato. Per istruzioni, vedere [Visualizzare e configurare le notifiche degli eventi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Creare e personalizzare gli stati di un gruppo

In qualità di amministratore di gruppo, puoi creare stati personalizzati per un gruppo di livello principale da gestire. In questo modo il gruppo è autonomo ed è possibile eliminare la necessità di decine di stati personalizzati a livello aziendale. Un amministratore Workfront può eseguire questa operazione per qualsiasi gruppo.

È inoltre possibile personalizzare gli stati di sistema per un gruppo di livello superiore se un amministratore di Workfront li ha configurati per consentire la personalizzazione.

Per istruzioni, vedere [Creare o modificare lo stato di un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Utilizzare i progetti di un gruppo

Nell’area Gruppi di Configura, quando visualizzi la pagina principale di un gruppo amministrato, puoi effettuare le seguenti operazioni con i progetti:

* Elencare e utilizzare (modificare, copiare, eliminare ed esportare) i progetti associati al gruppo e ai relativi sottogruppi e che sono stati condivisi con l’utente
* Crea un nuovo progetto per il gruppo

Per istruzioni, vedere [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## Visualizzare e gestire i processi di approvazione di un gruppo

Quando si visualizza un gruppo gestito nell&#39;area Gruppi, è possibile visualizzare e utilizzare i processi di approvazione per i quali gli amministratori del gruppo o di uno dei suoi sottogruppi dispongono dell&#39;accesso amministrativo.

Per istruzioni, vedere [Processi di approvazione a livello di gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Visualizzare e gestire i modelli di layout di un gruppo

Quando si visualizza un gruppo gestito nell&#39;area Gruppi, è possibile visualizzare e utilizzare il modello di layout per il quale gli amministratori del gruppo o di uno dei suoi sottogruppi dispongono dell&#39;accesso amministrativo.

Per istruzioni, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Visualizzare e gestire le pianificazioni dei membri del gruppo

L’amministratore di un gruppo che crea una pianificazione per un gruppo deve specificare il gruppo i cui amministratori gestiranno la pianificazione. In genere si tratta del gruppo per il quale viene creata la pianificazione, ma potrebbe trattarsi di un gruppo diverso se l’amministratore del gruppo gestisce più gruppi e specifica uno degli altri.

Quando si visualizza la pagina principale di un gruppo gestito, se il gruppo è designato come quello di cui gli amministratori possono modificare una pianificazione, è possibile visualizzare e gestire la pianificazione dalla pagina del gruppo.

Per istruzioni, vedere [Creare e modificare le pianificazioni di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## Visualizza e gestisci i profili delle schede orario dei membri del gruppo

Quando visualizzi la pagina principale di un gruppo che amministri, puoi gestire i profili della scheda orario che tu e gli altri amministratori del gruppo, o uno dei suoi sottogruppi, disponete dell’autorizzazione per modificare. Per istruzioni, consulta [Creare e gestire i profili delle schede orario di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## Visualizzare e gestire i membri del sottogruppo di un gruppo

Quando visualizzi la pagina principale di un gruppo che amministri, puoi visualizzare e gestire tutti gli utenti dei sottogruppi del gruppo. Per istruzioni, vedere [Visualizzare e gestire i membri del sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Visualizzare e gestire i team di un gruppo

Quando visualizzi un gruppo che gestisci nell’area Gruppi, puoi visualizzare e lavorare con i team associati al gruppo o a uno qualsiasi dei suoi sottogruppi.

Per istruzioni, consulta [Creare e modificare i team di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## Visualizzare e gestire le società di un gruppo

Quando visualizzi un gruppo che gestisci nell’area Gruppi, puoi visualizzare e lavorare con le aziende associate al gruppo o a uno qualsiasi dei suoi sottogruppi. Per istruzioni, vedere [Creare e modificare le società di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## Visualizzare e gestire i portfolio e i programmi di un gruppo

Quando si visualizza un gruppo che si gestisce nell&#39;area Gruppi, è possibile visualizzare e utilizzare i portafogli e i programmi quando si verificano entrambe le condizioni seguenti:

* Sono associati al gruppo che stai visualizzando o a uno qualsiasi dei suoi sottogruppi
* Si dispone delle autorizzazioni per visualizzarle perché sono state create o sono state condivise con te

Per istruzioni, vedere [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) e [Creare, modificare e visualizzare i programmi di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Disattivare o riattivare un gruppo

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

È possibile mantenere un gruppo attivo o disattivarlo.

La disattivazione di un gruppo può essere utile quando non è attualmente in uso perché gli utenti non lo visualizzano più nei campi di completamento automatico quando cercano un gruppo che desiderano associare a un altro oggetto.

Per istruzioni su come rendere un gruppo inattivo o attivo, vedere [Disattivare o riattivare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
