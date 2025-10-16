---
product-area: projects
navigation-topic: manage-tasks
title: Panoramica sul salvataggio di modifiche simultanee in un elenco di task
description: Quando si modificano le attività in un elenco, è possibile utilizzare impostazioni di salvataggio separate per indicare se si desidera salvare le modifiche automaticamente durante la modifica delle attività in un elenco.
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Panoramica sul salvataggio delle modifiche simultanee in un elenco di attività

Quando si modificano le attività in un elenco, è possibile utilizzare impostazioni di salvataggio separate per indicare se si desidera salvare le modifiche automaticamente durante la modifica delle attività in un elenco.

Per informazioni sulla modifica delle attività in un elenco attività, vedere l&#39;articolo [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

A volte possono verificarsi conflitti se due utenti apportano modifiche alle stesse attività.

Quando si modificano attività in un elenco di attività, tenere presente quanto segue:

* Adobe Workfront salva immediatamente le modifiche apportate alle attività quando si seleziona di salvare automaticamente le modifiche se il tipo di aggiornamento del progetto è Automatico o Automatico o In caso di modifica. Per informazioni sul tipo di aggiornamento del progetto, vedere [Selezionare il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
* Workfront aggiorna le informazioni contenute nell&#39;elenco su cui stai lavorando ogni minuto con le modifiche che altri utenti potrebbero apportare in qualsiasi altro punto del sistema. In questo modo è possibile ottenere sempre le informazioni più recenti sulle attività.

Quando più utenti modificano le stesse attività, si verificano gli scenari seguenti:

* **Un utente salva le modifiche in un elenco di attività automaticamente e un altro manualmente**: se un utente (utente A) salva le modifiche manualmente mentre l&#39;utente B modifica le stesse attività, ma le modifiche vengono salvate automaticamente, le modifiche live apportate dall&#39;utente B vengono aggiornate nell&#39;elenco per l&#39;utente A ogni minuto. In caso di conflitti tra le modifiche apportate dai due utenti, l’utente che esegue il salvataggio manuale (Utente A) visualizza un messaggio di avviso prima di poter salvare le modifiche. Il messaggio di avviso mostra gli elementi con le modifiche in conflitto. In questo momento, l’utente A può scegliere se mantenere le proprie modifiche (che sovrascrive le modifiche apportate dall’utente B) o eliminarle (che mantiene le modifiche apportate dall’utente B).

>[!NOTE]
>
>Quando si sceglie di ignorare le modifiche apportate, questo vale per tutte le modifiche e non solo per quelle in conflitto con le modifiche apportate da un altro utente.

* **Diversi utenti stanno salvando manualmente le modifiche in un elenco di attività**: se più utenti che stanno apportando modifiche alle attività in un elenco vengono salvati manualmente contemporaneamente, Workfront salva le modifiche apportate dall&#39;utente che esegue prima il salvataggio. Il salvataggio di queste modifiche non dovrebbe causare alcun conflitto. Workfront confronta quindi le modifiche apportate da tutti gli altri utenti con le informazioni già salvate e visualizza un avviso relativo alle modifiche in conflitto per gli altri utenti prima che possano salvare le informazioni.

>[!IMPORTANT]
>
>Quando si sceglie di mantenere le modifiche su tutte le altre modifiche, tutte le modifiche vengono salvate, a meno che le attività modificate non siano state eliminate da un altro utente. In questo caso, il messaggio di avviso informa che le modifiche apportate alle attività eliminate andranno perse.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - when replaced with the above live section; does it need an edit??) </p>
<div>
<p>When editing tasks in a list, you can select whether you want each change to be saved automatically or if you want to manually save multiple changes at one time by clicking the Save button. This depends on whether you enable the Autosave setting in the task list or not. </p>
<p>For information about editing tasks in a task list, see the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref" xrefformat="{para}">Edit tasks</a>. </p>
<p>Sometimes, conflicts might appear if two users are making changes on the same tasks. </p>
<p>Consider the following when editing tasks in a task list: </p>
<ul>
<li>Workfront saves the changes you make to tasks immediately when you have enabled the Autosave setting. </li>
<li>Workfront updates the information on the list you are working on every minute with changes that other users might make anywhere else in the system. This ensures that you always get the latest information on the tasks. </li>
</ul>
<p>The following scenarios exist when multiple users are editing the same tasks:</p>
<ul>
<li>One user has Autosave disabled and another has it enabled: If a user (User A) has disabled the Autosave setting and is editing the task list while User B is editing the same tasks but they have enabled the Autosave setting, the live changes made by User B are updated on the list for User A every minute. If there are conflicts between the changes made by the two users, the user with the Autosave setting disabled (User A) sees a warning message before they can save their changes, that shows the items that have those conflicting changes. At this time, User A can choose whether they should keep their changes (which overwrites the changes made by User B), or discard them (which keeps the changes made by User B.) </li>
</ul> <note type="note">
When you select to discard the changes you made, this applies to all the changes and not just to those that have conflicts with the edits made by another user.
</note>
<ul>
<li>Several users have disabled the Autosave setting: If several users that have disabled the Autosave setting are making changes at the same time, Workfront saves the changes made by the user who saves first. Saving these changes should not encounter any conflicts. Workfrontthen compares the changes made by all the other users with the information that it already saved and displays a warning about the conflicting changes to the other users before they can save their information. </li>
</ul> <note type="important">
When you select to keep your changes over all other changes, your changes are saved, unless the tasks you made changes to were deleted by another user. In this case, the warning message informs you that the changes you made to the deleted tasks are lost.
</note>
</div>
</div>
-->
