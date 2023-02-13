---
user-type: administrator
product-area: system-administration;user-management
keywords: gestire, raggruppare, modificare,
navigation-topic: create-and-manage-groups
title: Gestire un gruppo
description: In qualità di amministratore del gruppo, è possibile gestire un gruppo amministrato dall'area Gruppi in Configurazione. Se ci sono gruppi al di sopra del gruppo che gestisci, i loro amministratori possono farlo anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 0%

---

# Gestire un gruppo

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

In qualità di amministratore del gruppo, è possibile gestire un gruppo amministrato dall&#39;area Gruppi in Configurazione. Se ci sono gruppi al di sopra del gruppo che gestisci, i loro amministratori possono farlo anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

>[!NOTE]
>
>Quando si è assegnati come amministratore di un gruppo, si eredita il ruolo di amministratore del gruppo per tutti i sottogruppi che si trovano sotto di esso. Gli unici utenti che possono gestire un sottogruppo sono gli amministratori del gruppo per il gruppo principale sopra di esso e gli amministratori del gruppo che sono assegnati al sottogruppo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>È necessario essere un amministratore del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Gestire le appartenenze a un gruppo

Puoi aggiungere e rimuovere utenti e altri gruppi da un gruppo che amministri. È inoltre possibile assegnare i membri del gruppo come amministratori per il gruppo e gestire le informazioni sul profilo utente dei membri del gruppo.

Per istruzioni, consulta [Visualizzare e gestire le appartenenze a un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## Gestire i dettagli di un gruppo

È possibile visualizzare e modificare la pagina Dettagli gruppo per un gruppo o sottogruppo gestito. Questa pagina include una descrizione del gruppo, i nomi del Business Leader e degli amministratori del gruppo e un’opzione che consente di rendere pubblico o privato il gruppo e tutti i relativi sottogruppi. Inoltre, se il livello di accesso consente di gestire moduli personalizzati, è possibile allegare un modulo personalizzato a un gruppo.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

Per istruzioni, consulta [Visualizzare e gestire i dettagli di un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Modificare, copiare o eliminare un gruppo

Senza uscire dalla pagina principale di un gruppo che stai visualizzando, puoi modificare, copiare o eliminare rapidamente

<!--
DRAFTED IN FLARE:
or deactivate

-->

il gruppo.

<!--
DRAFTED IN FLARE:
Make this change when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Gruppi**.

   Nell’elenco visualizzato, puoi vedere i gruppi gestiti e tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Seleziona il gruppo, quindi fai clic su Modifica ![](assets/edit-icon.png), Copia ![](assets/copy-icon.png)o Elimina ![](assets/delete.png) icona.

   Per informazioni sull’utilizzo della casella visualizzata, consulta una delle seguenti opzioni:

   * **Modifica**: [Visualizzare e gestire i dettagli di un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **Copia**: [Creare un gruppo di primo livello copiando un gruppo o un sottogruppo esistente](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) nell&#39;articolo [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **Elimina**: [Eliminare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## Configurare le preferenze di progetto, attività ed emissione per un gruppo

Se sei un amministratore di gruppo e il gruppo ha bisogno di progetti, attività e impostazioni delle preferenze diverse da quelle impostate a livello di sistema, puoi chiedere all’amministratore di Workfront di sbloccare una preferenza per tutti i gruppi dell’organizzazione. Una volta sbloccato, puoi configurarlo (e gli amministratori di gruppo per tutti gli altri gruppi) per i gruppi gestiti.

Per istruzioni, consulta [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e  [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Elencare, aggiungere e configurare sottogruppi

Puoi creare, visualizzare, modificare, copiare, rinominare, esportare ed eliminare i sottogruppi sotto un gruppo amministrato.

## Configurare le notifiche evento per un gruppo

Se un amministratore di Workfront sblocca la possibilità di configurare le notifiche degli eventi per i gruppi dell’organizzazione, puoi configurarle per un gruppo da amministrare. Per istruzioni, consulta [Visualizzare e configurare le notifiche evento per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Creare e personalizzare gli stati di un gruppo

In qualità di amministratore del gruppo, puoi creare stati personalizzati per un gruppo di livello principale gestito. Questo offre al tuo gruppo autonomia e aiuta a eliminare la necessità di dozzine di stati personalizzati a livello aziendale. Questo può essere fatto anche da un amministratore Workfront, per qualsiasi gruppo.

Puoi anche personalizzare gli stati del sistema per un gruppo di livello principale se un amministratore Workfront li ha configurati per consentire la personalizzazione.

Per istruzioni, consulta [Creare o modificare uno stato di gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Lavorare con i progetti di un gruppo

Nell’area Gruppi in Configurazione, quando si visualizza la pagina principale di un gruppo amministrato, è possibile effettuare le seguenti operazioni con i progetti:

* Elenca ed esporta (modifica, copia, elimina ed esporta) i progetti associati al gruppo e ai relativi sottogruppi e che sono stati condivisi con te
* Crea un nuovo progetto per il gruppo

Per istruzioni, consulta [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## Visualizzare e gestire i processi di approvazione di un gruppo

Quando si visualizza un gruppo gestito nell&#39;area Gruppi, è possibile visualizzare e lavorare con i processi di approvazione per i quali gli amministratori del gruppo, o uno dei relativi sottogruppi, hanno accesso amministrativo.

Per istruzioni, consulta [Processi di approvazione a livello di gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Visualizzare e gestire i modelli di layout di un gruppo

Quando si visualizza un gruppo gestito nell’area Gruppi, è possibile visualizzare e utilizzare il modello di layout a cui hanno accesso gli amministratori del gruppo o di uno dei relativi sottogruppi.

Per istruzioni, consulta [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Visualizza e gestisci le pianificazioni dei membri del gruppo

Un amministratore del gruppo che crea una pianificazione per un gruppo deve specificare il gruppo di cui saranno gestiti gli amministratori. In genere si tratta del gruppo per il quale viene creata la pianificazione, ma potrebbe essere un gruppo diverso se l’amministratore del gruppo gestisce più gruppi e specifica invece uno degli altri.

Quando visualizzi la pagina principale di un gruppo gestito, se il gruppo è designato come quello i cui amministratori possono modificare una pianificazione, puoi visualizzare e gestire la pianificazione dalla pagina del gruppo.

Per istruzioni, consulta [Creare e modificare le pianificazioni di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## Visualizzare e gestire i profili della scheda attività dei membri del gruppo

Quando si visualizza la pagina principale di un gruppo amministrato, è possibile gestire i profili della scheda attività che l&#39;utente e gli altri amministratori del gruppo, o uno dei relativi sottogruppi, dispongono dell&#39;autorizzazione per la modifica. Per istruzioni, consulta [Creare e gestire i profili della scheda attività di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## Visualizzare e gestire i membri del sottogruppo di un gruppo

Quando visualizzi la pagina principale di un gruppo che gestisci, puoi visualizzare e gestire tutti gli utenti dei sottogruppi del gruppo. Per istruzioni, consulta [Visualizzare e gestire i membri dei sottogruppi](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Visualizzare e gestire i team di un gruppo

Quando visualizzi un gruppo gestito nell’area Gruppi, puoi visualizzare e lavorare con i team associati al gruppo o a uno dei relativi sottogruppi.

Per istruzioni, consulta [Creare e modificare i team di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## Visualizzare e gestire le aziende di un gruppo

Quando visualizzi un gruppo gestito nell’area Gruppi, puoi visualizzare e lavorare con le aziende associate al gruppo o a uno dei suoi sottogruppi. Per istruzioni, consulta [Creare e modificare le aziende di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## Visualizzare e gestire i portfolio e i programmi di un gruppo

Quando visualizzi un gruppo gestito nell’area Gruppi, puoi visualizzare e lavorare con portfolio e programmi quando sono soddisfatte entrambe le seguenti condizioni:

* Sono associati al gruppo che stai visualizzando o a uno dei suoi sottogruppi
* Autorizzazioni disponibili per visualizzarli perché li hai creati o sono stati condivisi con te

Per istruzioni, consulta [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) e [Creare, modificare e visualizzare i programmi di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Disattivare o riattivare un gruppo

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

È possibile mantenere attivo un gruppo o disattivarlo.

La disattivazione di un gruppo può essere utile quando non è in uso, in quanto gli utenti non lo visualizzano più nei campi tipo-avanti quando cercano un gruppo che desiderano associare a un altro oggetto.

Per istruzioni su come rendere un gruppo inattivo o attivo, consulta [Disattivare o riattivare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
