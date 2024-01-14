---
title: Panoramica sui gruppi
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Un amministratore Workfront può creare gruppi di utenti che coincidono con la struttura del reparto. I gruppi sono simili ma distinti dai team e dalle aziende.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: 9c4aa8d1f812299ba6cdcb664b990c1119e3cb31
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Panoramica sui gruppi

Un amministratore Workfront può creare gruppi di utenti che coincidono con la struttura del reparto. I gruppi sono simili ma distinti dai team e dalle aziende.

L’amministratore di Workfront concede ai gruppi l’accesso alle aree Workfront in cui devono lavorare e comunicare. Ciascun gruppo può quindi mantenere le informazioni relative a Workfront, quali utenti, modelli, moduli personalizzati e progetti, separate da quelle di altri reparti.

È necessario almeno un amministratore di gruppo per ogni gruppo. Gli amministratori di gruppi possono utilizzare la pagina Gruppi per gestire i propri gruppi in un&#39;unica posizione. Per ulteriori informazioni, consulta [Amministratori di gruppi](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

È possibile creare fino a 14 livelli di sottogruppi in un unico gruppo. Per ulteriori informazioni, consulta [Panoramica sui sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) e [Creare un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Utilizzo dei gruppi per organizzare gli utenti

In qualità di amministratore di Workfront o di amministratore di gruppo, puoi associare gli utenti a gruppi e sottogruppi. Se rendi pubblico un gruppo, gli utenti con una licenza Planner possono associarvi gli utenti. Per ulteriori informazioni sugli amministratori di gruppi e sui gruppi pubblici, consulta [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Quando crei un utente, ti consigliamo di aggiungerlo al gruppo predefinito appropriato e ad altri gruppi in cui dovrebbe lavorare l’utente. Un utente può avere un solo Gruppo Predefinito, ma può appartenere a più altri gruppi.

L’appartenenza a un gruppo consente all’utente di accedere agli oggetti condivisi con il gruppo e i sottogruppi. Ad esempio, se condividi un progetto con un gruppo, gli utenti del gruppo e i suoi sottogruppi vi hanno accesso.

>[!TIP]
>
>Se i reparti dell&#39;organizzazione collaborano spesso per gestire i progetti e le risorse relative, potrebbe non essere necessario suddividere i reparti in gruppi più piccoli. Alcuni gruppi di alto livello potrebbero funzionare meglio.

Un gruppo può avere un numero illimitato di utenti.

Per ulteriori informazioni sulla creazione di nuovi utenti, consulta [Aggiungi utenti](../../../administration-and-setup/add-users/add-users.md).

## Concessione a un gruppo dell&#39;accesso agli oggetti

Quando si condivide un oggetto con un gruppo, tutti i membri di tale gruppo, inclusi i membri di eventuali sottogruppi, hanno accesso all&#39;oggetto. Per ulteriori informazioni sulla condivisione in Workfront, consulta [Panoramica delle autorizzazioni di condivisione sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Associazione di un gruppo a un oggetto

Quando si crea o si modifica uno dei seguenti oggetti di Workfront, è possibile associarlo a un gruppo:

* **Progetto**: puoi associare un singolo gruppo a un progetto per indicarne la proprietà.

  Questo non concede implicitamente a ciascun membro del gruppo i diritti sul progetto. Per avere i diritti per il progetto, gli utenti devono avere il progetto condiviso con loro.

  Anche se gli utenti possono essere membri di più gruppi, a un progetto può essere associato un singolo gruppo. Gli utenti di altri gruppi possono comunque lavorare sullo stesso progetto, se il progetto è stato condiviso con loro o con i loro gruppi. Il gruppo associato al progetto è in genere il gruppo responsabile del completamento del progetto oppure il gruppo a cui il progetto è consegnato.

  Per istruzioni sull’associazione di un progetto a un gruppo, consulta [Gestire le informazioni nell’area Panoramica progetto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, programma o azienda**: quando crei o modifichi un portfolio, un programma o una società, puoi assegnarvi un singolo gruppo per indicare che il gruppo ne è proprietario o ne è responsabile. Grazie a questa associazione, gli amministratori e gli utenti possono identificare facilmente i portfolio, i programmi e le aziende su cui lavorano i loro gruppi.

  Ad esempio, un amministratore gruppo può elencare tutti i portfolio dell’organizzazione utilizzando un elenco o un rapporto e annotare nella colonna Gruppo quali portfolio vengono assegnati al proprio gruppo.

  >[!NOTE]
  >
  >L&#39;assegnazione di un gruppo a un portfolio, programma o società con un gruppo non implica automaticamente che le informazioni del gruppo abbiano accesso ai propri dati. È necessario condividere manualmente l’accesso ai dati con il gruppo prima che possa visualizzarli.

  Per istruzioni, consulta [Creare un portfolio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Creare un programma](../../../manage-work/portfolios/create-and-manage-programs/create-program.md), e [Creare e modificare le società](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Processo di approvazione**: puoi rendere disponibile un processo di approvazione per progetti, attività e problemi appartenenti a un determinato gruppo. Per ulteriori informazioni, consulta [Creare un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Percorso milestone**: puoi consentire agli utenti di alcuni gruppi di utilizzare un percorso milestone con i loro progetti. Per ulteriori informazioni, consulta [Creare un percorso milestone](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Modello di layout**: puoi concedere agli amministratori di un gruppo l’autorizzazione per modificare un modello di layout. Per istruzioni, consulta [Concedere l’accesso amministrativo per un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Timesheet Ricorrente**: puoi concedere agli amministratori di un gruppo l’autorizzazione per modificare un profilo di scheda orario. Per ulteriori informazioni, consulta [Creare, modificare e assegnare profili di schede orario](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Schedules**: puoi concedere agli amministratori di un gruppo l’autorizzazione per modificare una pianificazione. Per ulteriori informazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Team**: è possibile associare un gruppo a un team in modo che gli amministratori dei gruppi e dei relativi sottogruppi possano visualizzare e lavorare con tali team dall’area Gruppi. Per ulteriori informazioni, consulta [Creare un team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) o [Modifica impostazioni team](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Modello**: puoi assegnare un gruppo a un modello di progetto. Questo consente di semplificare il processo di creazione del progetto e di identificare più facilmente i gruppi proprietari e i modelli di progetto, per creare rapporti più dettagliati. Per ulteriori informazioni, consulta la sezione [Panoramica](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) nell’articolo [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Elementi eliminati e ripristinati di recente**: puoi visualizzare e gestire i gruppi di elementi eliminati di recente. Per ulteriori informazioni, consulta [Visualizzare e gestire gli elementi eliminati di recente da un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) e [Visualizzare e gestire gli elementi ripristinati di recente di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
