---
title: Concedere a un utente l'accesso amministrativo completo
description: Puoi concedere agli utenti l’accesso amministrativo completo a Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '1551'
ht-degree: 1%

---

# Concedere a un utente l&#39;accesso amministrativo completo

<!--Audited: 12/2024-->

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non hanno ancora effettuato l’onboarding nell’Admin Console. Se la tua organizzazione è stata integrata in Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Per istruzioni su come concedere l&#39;accesso completo come amministratore in Adobe Admin Console, vedere [Gestire gli amministratori di sistema in Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Per un elenco delle procedure che differiscono a seconda che l&#39;organizzazione sia stata integrata in Adobe Admin Console, consulta [Differenze di amministrazione basate su Platform (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

In qualità di amministratore di Adobe Workfront, puoi creare un altro amministratore Workfront assegnandogli il livello di accesso Amministratore di sistema. Un utente con questo livello di accesso ha accesso amministrativo completo a tutto ciò che si trova in Workfront, inclusi gli elementi che non ha creato personalmente.

>[!NOTE]
>
>Questo è diverso dall&#39;utilizzo di un livello di accesso per concedere agli utenti l&#39;accesso amministrativo a determinate aree del sistema. Per ulteriori informazioni, vedi:
>
>* [Concedi agli utenti l&#39;accesso amministrativo ad alcune aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Accesso di un amministratore di Workfront e accesso di un utente del piano con diritti amministrativi](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) in questo articolo
>

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
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Standard</p>
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront. </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Concedere a un singolo utente l&#39;accesso completo come amministratore di sistema

{{step-1-to-users}}

1. Fare clic sul nome dell&#39;utente a cui si desidera concedere i diritti di amministratore.
1. Fai clic sul menu **Altro** ![](assets/more-icon.png) a destra del nome utente, quindi fai clic su **Modifica**.

   Viene visualizzata la casella **Modifica persona**.
1. Fai clic su **Accesso** nel pannello a sinistra.
1. Nell&#39;elenco a discesa **Livello di accesso**, selezionare il livello di accesso **Amministratore di sistema**.

   A seconda delle modifiche apportate nel sistema, il nome di questo livello di accesso potrebbe essere stato modificato.

1. Fai clic su **Salva modifiche.**

   L’utente ora dispone dei diritti completi di amministratore di sistema nel sistema.

## Accesso di un amministratore di Workfront e accesso di un utente del piano con diritti amministrativi  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

Le due tabelle seguenti mostrano la differenza tra i diritti di accesso di un utente con un livello di accesso Amministratore di sistema di Workfront e quelli di un utente con una licenza Pianificazione con alcuni diritti amministrativi.

Gli amministratori di Workfront possono visualizzare tutti gli oggetti del sistema, indipendentemente da chi li ha creati, crearne di nuovi e modificare o eliminare quelli esistenti. Hanno accesso completo a tutti gli oggetti nel sistema.

Gli utenti con una licenza Pianificazione che possono modificare le funzionalità in un’area hanno accesso completo alle funzionalità in tale area.

>[!NOTE]
>
>Gli utenti con una licenza Pianificazione designati come amministratori di gruppi possono eseguire alcune delle azioni consentite per gli amministratori di Workfront. Possono eseguire queste azioni solo per i gruppi che amministrano, i loro sottogruppi e gli utenti in questi gruppi e sottogruppi. Per ulteriori informazioni, vedere [Amministratori di gruppi](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Accesso all’area Setup (Configurazione)](#access-to-the-setup-area)
* [Accesso agli oggetti](#access-to-objects)

### Accesso all’area Setup (Configurazione) {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/oggetto</th> 
   <th>Amministratore Workfront </th> 
   <th>Utente con una licenza Pianificazione e alcuni diritti amministrativi</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Preferenze progetto: Progetti</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Preferenze progetto: attività e problemi</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Preferenze progetto: stati</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso</p> </td> 
  </tr> 
  <tr> 
   <td>Preferenze progetto: Priorità</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Preferenze progetto: Gravità</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Preferenze progetto: tassi di cambio</td> 
   <td>Accesso completo</td> 
   <td>Accesso completo</td> 
  </tr> 
  <tr> 
   <td>Processi: approvazioni</td> 
   <td> <p>Accesso completo</p> </td> 
   <td>Accesso completo</td> 
  </tr> 
  <tr> 
   <td>Processi: Percorsi milestone</td> 
   <td>Accesso completo</td> 
   <td>Accesso completo</td> 
  </tr> 
  <tr> 
   <td>Moduli personalizzati</td> 
   <td>Accesso completo</td> 
   <td> <p>Gestisci i moduli personalizzati creati o condivisi con loro.</p> <p>Allega i moduli personalizzati creati o i moduli personalizzati condivisi con loro agli oggetti per i quali dispongono delle autorizzazioni di gestione o di contribuzione.</p> </td> 
  </tr> 
  <tr> 
   <td>Cestino: eliminato di recente</td> 
   <td>Accesso completo</td> 
   <td> <p>Gli utenti che sono amministratori di gruppi possono ripristinare i progetti assegnati ai gruppi che gestiscono e le attività, i problemi o i documenti associati a tali progetti.</p> </td> 
  </tr> 
  <tr> 
   <td>Cestino: ripristinato di recente</td> 
   <td>Accesso completo</td> 
   <td>Gli utenti amministratori di gruppi possono visualizzare gli elementi ripristinati di recente.</td> 
  </tr> 
  <tr> 
   <td>Ruoli</td> 
   <td>Accesso completo</td> 
   <td> <p>Modificare ma non eliminare i ruoli esistenti.</p> <p>Aggiungi nuove mansioni.</p> </td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per creare i team.</p> <p>Aggiungere team esistenti agli utenti durante la creazione o la modifica degli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td>Gruppi</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per creare gruppi.</p> <p>Solo gli amministratori dei gruppi possono gestire l'appartenenza ai gruppi, i sottogruppi e gli stati a livello di gruppo per i gruppi che gestiscono. </p> </td> 
  </tr> 
  <tr> 
   <td>Aziende</td> 
   <td>Accesso completo</td> 
   <td>Accesso completo</td> 
  </tr> 
  <tr> 
   <td>Accedi come</td> 
   <td>Accesso completo </td> 
   <td> <p>Se l'accesso amministrativo al gruppo è abilitato nel livello di accesso e il gruppo è designato come amministratore di gruppo, è possibile accedere come utenti del gruppo amministrato e dei relativi sottogruppi. Non possono accedere come amministratore di sistema.<br>Per ulteriori informazioni sull'abilitazione dell'accesso amministrativo di gruppo per gli utenti, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Schedule</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per modificare le pianificazioni.</p> <p>Accesso per aggiungere pianificazioni esistenti ad altri utenti, a livello di utente. </p> </td> 
  </tr> 
  <tr> 
   <td>Schede orario e ore: profili scheda orario</td> 
   <td>Accesso completo</td> 
   <td> <p>Accesso per assegnare agli utenti i profili esistenti delle schede orario, a livello di utente.</p> <p>Gli utenti che sono amministratori di gruppi possono creare Profili Scheda orario per i gruppi che amministrano e i relativi sottogruppi. </p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Tipi di Ora</td> 
   <td>Accesso completo</td> 
   <td> <p>Accesso per assegnare tipi di lavoro agli utenti, a livello di utente.</p> </td> 
  </tr> 
  <tr> 
   <td>Schede orario e ore: preferenze</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>E-mail: Notifiche: Notifiche evento</td> 
   <td>Attiva/Disattiva tutto</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>E-mail: Notifiche: Avvisi di Promemoria</td> 
   <td>Accesso completo</td> 
   <td>Accesso completo</td> 
  </tr> 
  <tr> 
   <td>E-mail: Notifiche: Modelli e-mail</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per la modifica dei modelli e-mail.</p> <p>Accesso per aggiungere modelli e-mail esistenti alle notifiche promemoria.</p> </td> 
  </tr> 
  <tr> 
   <td>E-mail: Promemoria automatici</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>E-mail: Inviti</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per modificare gli inviti e-mail.</p> <p>Puoi accedere nuovamente agli inviti e-mail per gli utenti non registrati solo dalla scheda Persone.</p> </td> 
  </tr> 
  <tr> 
   <td>E-mail: Configurazione</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso</p> </td> 
  </tr> 
  <tr> 
   <td>Scorecard</td> 
   <td>Accesso completo</td> 
   <td> <p>Accesso completo</p> </td> 
  </tr> 
  <tr> 
   <td>Tipi di spesa</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso</p> </td> 
  </tr> 
  <tr> 
   <td>Tipi di rischio</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Livelli di accesso</td> 
   <td> <p>Accesso completo per modificare tutti i livelli di accesso.</p> <p>Per impostazione predefinita, non è possibile modificare i livelli di accesso Amministratore di sistema e Utente esterno.</p> </td> 
   <td> <p>Nessun accesso per la modifica dei livelli di accesso.</p> <p>Assegna ad altri utenti un livello di accesso inferiore o uguale al loro a livello di utente.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia: modelli di layout</td> 
   <td>Accesso completo</td> 
   <td> <p>Accesso per assegnare modelli di layout esistenti ad altri utenti, a livello di utente. </p> <p>Gli utenti designati come amministratori di gruppi possono creare modelli di layout per i gruppi e i sottogruppi che gestiscono.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia: Aggiorna feed</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per modificare i feed di aggiornamento.</p> <p>Accesso per aggiungere campi da tracciare nei feed di aggiornamento durante la modifica di Forms personalizzati.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia: Filtri</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per la creazione di filtri nell’area Configurazione.</p> <p>Accesso per creare nuovi filtri in un elenco di oggetti.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia: Visualizzazioni</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per creare visualizzazioni nell'area Configurazione.</p> <p>Accesso per creare nuove viste in un elenco di oggetti.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia: Raggruppamenti</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per creare raggruppamenti nell’area Configurazione.</p> <p>Accesso per creare nuovi raggruppamenti in un elenco di oggetti.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia: Controlli elenco</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso</p> </td> 
  </tr> 
  <tr> 
   <td>Documenti: provider cloud</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per configurare i provider di cloud.</p> <p>Dalla scheda Documenti, dopo l’integrazione dei Cloud Provider con Workfront, puoi accedere ai documenti collegati a e da Cloud Provider.</p> </td> 
  </tr> 
  <tr> 
   <td>Documenti: mappatura metadati</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Documenti: Integrazione SharePoint</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per configurare un’integrazione SharePoint.</p> <p>È possibile accedere ai documenti da e verso SharePoint dalla scheda Documenti, dopo aver configurato l’integrazione di SharePoint con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documenti: integrazione personalizzata</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per configurare un’integrazione personalizzata.</p> <p>È possibile accedere ai documenti da e verso provider di terze parti tramite la scheda Documenti, dopo l'integrazione dei provider di terze parti con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Sistema: Branding</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Informazioni Cliente</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Single Sign-On (SSO)</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: aggiornamento utenti per SSO</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Kick-Start</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: diagnostica</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Preferenze</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
 </tbody> 
</table>

### Accesso agli oggetti {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/oggetto</th> 
   <th>Amministratore Workfront </th> 
   <th>Utente con una licenza Pianificazione e alcuni diritti amministrativi</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendari</td> 
   <td>Accesso completo</td> 
   <td>Consente di gestire i calendari creati e quelli condivisi con gli altri.</td> 
  </tr> 
  <tr> 
   <td>Dashboard</td> 
   <td>Accesso completo</td> 
   <td>Gestisci le dashboard che creano e le dashboard condivise con loro.</td> 
  </tr> 
  <tr> 
   <td>Documenti</td> 
   <td>Accesso completo</td> 
   <td>Gestisci i documenti che caricano o i documenti condivisi con loro.</td> 
  </tr> 
  <tr> 
   <td>Problemi</td> 
   <td>Accesso completo</td> 
   <td>Gestisci i problemi che creano o i problemi condivisi con loro.</td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Accesso completo</td> 
   <td>Gestisci i portfolio creati o condivisi con loro. </td> 
  </tr> 
  <tr> 
   <td>Programmi</td> 
   <td>Accesso completo</td> 
   <td>Gestisci i programmi creati o condivisi con loro.</td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>Accesso completo</td> 
   <td>Gestisci i progetti che creano o che condividono con loro.</td> 
  </tr> 
  <tr> 
   <td>Report</td> 
   <td>Accesso completo</td> 
   <td>Gestisci i report che creano o quelli condivisi con loro. Visualizzare, copiare e modificare i report di sistema.</td> 
  </tr> 
  <tr> 
   <td>Attività</td> 
   <td>Accesso completo</td> 
   <td>Gestisci le attività che creano o le attività condivise con</td> 
  </tr> 
  <tr> 
   <td>Modelli</td> 
   <td>Accesso completo</td> 
   <td>Gestire i modelli creati o i modelli condivisi</td> 
  </tr> 
  <tr> 
   <td>Schede orario</td> 
   <td>Accesso completo</td> 
   <td>Accesso completo</td> 
  </tr> 
  <tr> 
   <td>Utenti</td> 
   <td>Accesso completo</td> 
   <td> <p>Accesso limitato</p> <p>Non possono assegnare gruppi a utenti per i quali non sono amministratori di gruppi o a gruppi non pubblici.</p> <p>Non possono assegnare agli utenti un livello di accesso superiore al loro livello di accesso.</p> <p>Se l’accesso amministrativo al gruppo è abilitato al livello di accesso e il gruppo è designato come amministratore di gruppo, è possibile reimpostare la password di e accedere come utenti del gruppo che amministrano e dei relativi sottogruppi. Non è possibile reimpostare la password o accedere come amministratore di sistema.<br>Per ulteriori informazioni sull'abilitazione dell'accesso amministrativo di gruppo per gli utenti, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
