---
title: Gruppi
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Un amministratore Workfront può creare gruppi di utenti che coincidono con la struttura del reparto. I gruppi sono simili ma diversi dai team e dalle aziende. L’amministratore di Workfront concede ai gruppi l’accesso alle aree Workfront in cui devono lavorare e comunicare. Ogni gruppo può quindi mantenere le proprie informazioni Workfront, ad esempio utenti, modelli, moduli personalizzati e progetti separati da quelle di altri reparti. Per ogni gruppo è necessario almeno un amministratore di gruppo. Gli amministratori dei gruppi possono utilizzare la pagina Gruppi per gestire i gruppi in un’unica posizione. È possibile creare fino a 14 livelli di sottogruppi in un unico gruppo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 0%

---

# Panoramica sui gruppi

Un amministratore Workfront può creare gruppi di utenti che coincidono con la struttura del reparto. I gruppi sono simili ma diversi dai team e dalle aziende.

L’amministratore di Workfront concede ai gruppi l’accesso alle aree Workfront in cui devono lavorare e comunicare. Ogni gruppo può quindi mantenere le proprie informazioni Workfront, ad esempio utenti, modelli, moduli personalizzati e progetti separati da quelle di altri reparti.

Per ogni gruppo è necessario almeno un amministratore di gruppo. Gli amministratori dei gruppi possono utilizzare la pagina Gruppi per gestire i gruppi in un’unica posizione. Per ulteriori informazioni, consulta [Amministratori di gruppo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

È possibile creare fino a 14 livelli di sottogruppi in un unico gruppo. Per ulteriori informazioni, consulta [Panoramica sui sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) e [Creare un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Utilizzo dei gruppi per organizzare gli utenti

In qualità di amministratore Workfront o amministratore di gruppo, puoi associare gli utenti a gruppi e sottogruppi. Se un gruppo viene reso pubblico, gli utenti con una licenza Planner possono associarvi gli utenti. Per ulteriori informazioni sugli amministratori dei gruppi e sui gruppi pubblici, consulta [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Quando crei un utente, ti consigliamo di aggiungere tale utente al gruppo principale appropriato e ad altri gruppi in cui l’utente dovrebbe lavorare. Un utente può avere un solo gruppo principale, ma può trovarsi in più gruppi.

L’appartenenza a un gruppo consente all’utente di accedere agli oggetti condivisi con il gruppo e i sottogruppi. Ad esempio, se condividi un progetto con un gruppo, gli utenti del gruppo e i sottogruppi del gruppo possono accedervi.

>[!TIP]
>
>Se i dipartimenti dell’organizzazione lavorano spesso insieme per gestire i progetti e le risorse relative a tali progetti, potrebbe non essere necessario suddividere i dipartimenti in molti gruppi più piccoli. Alcuni gruppi di alto livello potrebbero funzionare meglio.

Un gruppo può avere un numero illimitato di utenti.

Per ulteriori informazioni sulla creazione di nuovi utenti, consulta [Aggiungi utenti](../../../administration-and-setup/add-users/add-users.md).

## Concessione di un accesso di gruppo agli oggetti

Quando si condivide un oggetto con un gruppo, tutti i membri del gruppo (inclusi i membri di qualsiasi sottogruppo) hanno accesso all’oggetto. Per ulteriori informazioni sulla condivisione in Workfront, vedi [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Associazione di un gruppo a un oggetto

Quando si crea o si modifica uno dei seguenti oggetti Workfront, è possibile associarlo a un gruppo:

* **Progetto**: È possibile associare un singolo gruppo a un progetto per indicare la proprietà del progetto.

   Ciò non concede implicitamente al progetto i diritti di ciascun membro del gruppo. Per poter disporre dei diritti per il progetto, gli utenti devono ricevere i diritti condividendo il progetto con loro.

   Anche se gli utenti possono essere membri di più gruppi, a un progetto può essere associato un singolo gruppo. Gli utenti di altri gruppi possono comunque lavorare sullo stesso progetto, se i progetti sono stati condivisi con loro o con i loro gruppi. Il gruppo associato al progetto è in genere il gruppo responsabile del completamento del progetto o il gruppo per il quale il progetto viene consegnato.

   Per istruzioni su come associare un progetto a un gruppo, consulta [Gestire le informazioni nell’area Panoramica del progetto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, programma o azienda**: Quando crei o modifichi un portfolio, un programma o un&#39;azienda, puoi assegnargli un singolo gruppo per indicare che il gruppo è proprietario o responsabile di tale portafoglio. Con questa associazione, amministratori e utenti possono identificare facilmente su quali portafogli, programmi e aziende stanno lavorando i loro gruppi.

   Ad esempio, un amministratore di gruppo può elencare tutti i portafogli dell’organizzazione utilizzando un elenco o un rapporto e nella colonna Gruppo può indicare quali portafogli sono assegnati al gruppo.

   >[!NOTE]
   >
   >L&#39;assegnazione di un gruppo a un portfolio, a un programma o a una società con un gruppo non implica automaticamente che le informazioni in quanto il gruppo ha accesso ai suoi dati. È necessario condividere manualmente l’accesso ai dati con il gruppo prima che possa visualizzarli.

   Per istruzioni, consulta [Creare un portfolio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Crea un programma](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)e [Creare e modificare aziende](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Processo di approvazione**: È possibile rendere disponibile un processo di approvazione per progetti, attività e problemi appartenenti a un determinato gruppo. Per ulteriori informazioni, consulta [Creazione di un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Percorso Milestone**: Puoi consentire agli utenti di determinati gruppi di utilizzare un percorso cardine con i loro progetti. Per ulteriori informazioni, consulta [Creare un percorso cardine](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Modello di layout**: È possibile concedere agli amministratori di un gruppo l’autorizzazione per modificare un modello di layout. Per istruzioni, consulta [Consentire l’accesso amministrativo per un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Profilo scheda attività**: È possibile concedere agli amministratori di un gruppo l&#39;autorizzazione per modificare un profilo della scheda attività. Per ulteriori informazioni, consulta [Creare, modificare e assegnare profili della scheda attività](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Pianificazioni**: Puoi concedere agli amministratori di un gruppo l’autorizzazione per modificare una pianificazione. Per ulteriori informazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Team**: È possibile associare un gruppo a un team in modo che gli amministratori dei gruppi e dei relativi sottogruppi possano visualizzare e lavorare con tali team dall’area Gruppi. Per ulteriori informazioni, consulta [Creare un team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) o [Modificare le impostazioni del team](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Modello**: È possibile assegnare un gruppo a un modello di progetto. Questo consente di semplificare il processo di creazione del progetto e di identificare e creare rapporti più semplici sui gruppi di appartenenza che possiedono i modelli di progetto. Per ulteriori informazioni, consulta la sezione . [Panoramica](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) nell&#39;articolo [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Elementi eliminati e ripristinati di recente**: È possibile visualizzare e gestire i gruppi di elementi eliminati di recente. Per ulteriori informazioni, consulta [Visualizzare e gestire gli elementi eliminati di un gruppo di recente](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) e [Visualizzare e gestire gli elementi ripristinati di recente di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
