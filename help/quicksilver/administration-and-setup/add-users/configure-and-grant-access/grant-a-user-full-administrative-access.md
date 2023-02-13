---
title: Concedere a un utente pieno accesso amministrativo
description: Puoi concedere agli utenti l’accesso amministrativo completo a Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 1%

---

# Concedere a un utente pieno accesso amministrativo

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate nell’Admin Console. Se l’organizzazione è stata configurata per Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Per istruzioni su come concedere l’accesso completo all’amministratore in Adobe Admin Console:
>
>* Vedi [Creare amministratori di sistema in Workfront con Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create2)
>* Vedi la sezione &quot;Modifica dettagli utente&quot; nell&#39;articolo [Gestire gli utenti individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) nella documentazione di Adobe Admin Console.
>* Contattare l&#39;amministratore Adobe Admin Console.
>
>Per un elenco delle procedure che variano a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

In qualità di amministratore di Adobe Workfront, puoi creare un altro amministratore di Workfront assegnandogli il livello di accesso Amministratore di sistema. Un utente con questo livello di accesso dispone di accesso amministrativo completo a tutto ciò che si trova in Workfront, inclusi gli elementi che non ha creato da solo.

>[!NOTE]
>
>Ciò è diverso dall&#39;utilizzo di un livello di accesso per concedere agli utenti l&#39;accesso amministrativo a determinate aree del sistema. Per ulteriori informazioni, consulta quanto segue:
>
>* [Consentire agli utenti l&#39;accesso amministrativo a determinate aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Accesso di un amministratore Workfront e accesso di un utente del piano con diritti amministrativi](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) nel presente articolo
>


## Requisiti di accesso

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront. Per ulteriori informazioni, consulta <a href="#" class="MCXref xref selected">Concedere a un utente pieno accesso amministrativo</a>.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Concedere l’accesso completo dell’amministratore di sistema a un singolo utente

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).

1. Fare clic sul nome dell&#39;utente a cui si desidera concedere i diritti di amministratore.
1. Fai clic sul menu Altro ![](assets/more-icon.png), quindi fai clic su **Modifica**.

1. Sulla **Modifica persona** casella visualizzata, fai clic su **Accesso**.

1. In **livello di accesso** elenco a discesa, seleziona la **Amministratore di sistema** livello di accesso.

   A seconda delle modifiche apportate al sistema, il nome di questo livello di accesso potrebbe essere stato modificato.

1. Fai clic su **Salva le modifiche.**

   L&#39;utente dispone ora dei diritti completi di amministratore di sistema nel sistema.

## Accesso di un amministratore Workfront e accesso di un utente del piano con diritti amministrativi  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

Le due tabelle seguenti mostrano la differenza tra i diritti di accesso di un utente con un livello di accesso amministratore Workfront e quelli di un utente con una licenza Plan con alcuni diritti amministrativi.

Gli amministratori di Workfront possono visualizzare tutti gli oggetti del sistema (indipendentemente da chi li ha creati), crearne di nuovi e modificare o eliminare quelli esistenti. Hanno accesso completo a tutti gli oggetti del sistema.

Gli utenti con una licenza di piano che possono modificare funzionalità in un’area hanno accesso completo alle funzionalità in quell’area.

>[!NOTE]
>
>Gli utenti con una licenza di piano designati come amministratori di gruppo possono eseguire alcune delle azioni consentite per gli amministratori di Workfront. È consentito eseguire queste azioni solo per i gruppi che amministrano, i loro sottogruppi e gli utenti di tali gruppi e sottogruppi. Per ulteriori informazioni, consulta [Amministratori di gruppo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Accesso all&#39;area di configurazione](#access-to-the-setup-area)
* [Accesso agli oggetti](#access-to-objects)

### Accesso all&#39;area di configurazione {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/oggetto</th> 
   <th>Amministratore Workfront </th> 
   <th>Utente con licenza Plan e alcuni diritti amministrativi</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Preferenze progetto: Progetti</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Preferenze progetto: Attività e problemi</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Preferenze progetto: Stati</td> 
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
   <td>Preferenze progetto: Tassi di cambio</td> 
   <td>Accesso completo</td> 
   <td>Accesso completo</td> 
  </tr> 
  <tr> 
   <td>Processi: Approvazioni</td> 
   <td> <p>Accesso completo</p> </td> 
   <td>Accesso completo</td> 
  </tr> 
  <tr> 
   <td>Processi: Percorsi Milestone</td> 
   <td>Accesso completo</td> 
   <td>Accesso completo</td> 
  </tr> 
  <tr> 
   <td>Moduli personalizzati</td> 
   <td>Accesso completo</td> 
   <td> <p>Gestisci moduli personalizzati creati o moduli personalizzati condivisi con loro.</p> <p>Allegare moduli personalizzati creati o moduli personalizzati condivisi con loro agli oggetti a cui hanno autorizzazioni di gestione o di contributo.</p> </td> 
  </tr> 
  <tr> 
   <td>Cestino: Eliminato di recente</td> 
   <td>Accesso completo</td> 
   <td> <p>Gli utenti amministratori di gruppo possono ripristinare i progetti assegnati ai gruppi da essi gestiti e le attività, i problemi o i documenti associati a tali progetti.</p> </td> 
  </tr> 
  <tr> 
   <td>Cestino: Ripristinato di recente</td> 
   <td>Accesso completo</td> 
   <td>Gli utenti amministratori di gruppo possono vedere gli elementi ripristinati di recente.</td> 
  </tr> 
  <tr> 
   <td>Ruoli</td> 
   <td>Accesso completo</td> 
   <td> <p>Modifica ma non elimina i ruoli di lavoro esistenti.</p> <p>Aggiungi nuovi ruoli di lavoro.</p> </td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per creare team.</p> <p>Aggiungi i team esistenti agli utenti durante la creazione o la modifica degli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td>Gruppi</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per creare gruppi.</p> <p>Solo gli amministratori di gruppo possono gestire l’appartenenza al gruppo, i sottogruppi e gli stati a livello di gruppo per i gruppi gestiti. </p> </td> 
  </tr> 
  <tr> 
   <td>Aziende</td> 
   <td>Accesso completo</td> 
   <td>Accesso completo</td> 
  </tr> 
  <tr> 
   <td>Accedi come</td> 
   <td>Accesso completo </td> 
   <td> <p>Se il loro accesso amministrativo al gruppo è abilitato al livello di accesso e sono designati come amministratore del gruppo, possono accedere come utenti del gruppo che amministrano e dei relativi sottogruppi. Non possono accedere come amministratore di sistema.<br>Per ulteriori informazioni sull'abilitazione dell'accesso amministrativo ai gruppi per gli utenti, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Schedule</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso alla modifica delle pianificazioni.</p> <p>Accesso per aggiungere pianificazioni esistenti ad altri utenti, a livello di utente. </p> </td> 
  </tr> 
  <tr> 
   <td>Scheda attività e ore: Profili scheda attività</td> 
   <td>Accesso completo</td> 
   <td> <p>Accesso per assegnare agli utenti i profili esistenti della scheda attività, a livello di utente.</p> <p>Gli utenti amministratori di gruppo possono creare profili della scheda attività per i gruppi che amministrano e i relativi sottogruppi. </p> </td> 
  </tr> 
  <tr> 
   <td>Scheda attività e ore: Tipi di ore</td> 
   <td>Accesso completo</td> 
   <td> <p>Accesso per assegnare tipi di ora agli utenti, a livello di utente.</p> </td> 
  </tr> 
  <tr> 
   <td>Scheda attività e ore: Preferenze</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>E-mail: Notifiche: Notifiche degli eventi</td> 
   <td>Attiva/Disattiva tutto</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>E-mail: Notifiche: Notifiche di promemoria</td> 
   <td>Accesso completo</td> 
   <td>Accesso completo</td> 
  </tr> 
  <tr> 
   <td>E-mail: Notifiche: Modelli e-mail</td> 
   <td>Accesso completo</td> 
   <td> <p>Non è possibile modificare i modelli e-mail.</p> <p>Accesso per aggiungere modelli e-mail esistenti alle notifiche dei promemoria.</p> </td> 
  </tr> 
  <tr> 
   <td>E-mail: Promemoria automatica</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>E-mail: Inviti</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per modificare gli inviti e-mail.</p> <p>Accesso per inviare nuovamente gli inviti e-mail agli utenti non registrati solo dalla scheda Persone.</p> </td> 
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
   <td> <p>Accesso completo per modificare tutti i livelli di accesso.</p> <p>Per impostazione predefinita non è possibile modificare i livelli di accesso amministratore di sistema e utente esterno.</p> </td> 
   <td> <p>Nessun accesso alla modifica dei livelli di accesso.</p> <p>Assegna un livello di accesso ad altri utenti inferiore o uguale al proprio a livello di utente.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia: Modelli di layout</td> 
   <td>Accesso completo</td> 
   <td> <p>Accesso per assegnare modelli di layout esistenti ad altri utenti, a livello di utente. </p> <p>Gli utenti designati come amministratori di gruppo possono creare modelli di layout per i gruppi e i sottogruppi che gestiscono.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia: Aggiorna feed</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per modificare Aggiorna feed.</p> <p>Accesso per aggiungere campi da tracciare nei feed di aggiornamento durante la modifica di Custom Forms.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia: Filtri</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per creare filtri nell’area Configurazione.</p> <p>Accesso per creare nuovi filtri in un elenco di oggetti.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia: Viste</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per creare visualizzazioni nell'area Configurazione.</p> <p>Accesso per creare nuove viste in un elenco di oggetti.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia: Raggruppamenti</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per creare i gruppi nell'area Configurazione.</p> <p>Consente di creare nuovi raggruppamenti in un elenco di oggetti.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia: Controlli elenco</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso</p> </td> 
  </tr> 
  <tr> 
   <td>Documenti: Provider cloud</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per configurare i provider cloud.</p> <p>Accedere a e da Cloud Provider dalla scheda Documenti dopo l’integrazione di Cloud Provider con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documenti: Mappatura metadati</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Documenti: Integrazione SharePoint</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per configurare un’integrazione SharePoint.</p> <p>Accesso a documenti da e verso SharePoint dalla scheda Documenti, dopo la configurazione dell’integrazione SharePoint con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documenti: Integrazione personalizzata</td> 
   <td>Accesso completo</td> 
   <td> <p>Nessun accesso per configurare un'integrazione personalizzata.</p> <p>Accesso ai documenti da e verso provider di terze parti dalla scheda Documenti dopo l’integrazione di fornitori di terze parti con Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Sistema: Branding</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Informazioni cliente</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Single Sign-On (SSO)</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Aggiorna utenti per SSO</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Avvio</td> 
   <td>Accesso completo</td> 
   <td>Nessun accesso</td> 
  </tr> 
  <tr> 
   <td>Sistema: Diagnostica</td> 
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
   <th>Utente con licenza Plan e alcuni diritti amministrativi</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendari</td> 
   <td>Accesso completo</td> 
   <td>Gestire i calendari creati e i calendari condivisi con gli utenti.</td> 
  </tr> 
  <tr> 
   <td>Dashboard</td> 
   <td>Accesso completo</td> 
   <td>Gestisci le dashboard che creano e le dashboard condivise con loro.</td> 
  </tr> 
  <tr> 
   <td>Documenti</td> 
   <td>Accesso completo</td> 
   <td>Gestisci i documenti caricati o i documenti condivisi con loro.</td> 
  </tr> 
  <tr> 
   <td>Problemi</td> 
   <td>Accesso completo</td> 
   <td>Gestisci i problemi che creano o i problemi condivisi con loro.</td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Accesso completo</td> 
   <td>Gestisci i portfolio che creano o i portfolio condivisi con loro. </td> 
  </tr> 
  <tr> 
   <td>Programmi</td> 
   <td>Accesso completo</td> 
   <td>Gestisci i programmi creati o i programmi condivisi con loro.</td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>Accesso completo</td> 
   <td>Gestisci i progetti creati o i progetti condivisi con loro.</td> 
  </tr> 
  <tr> 
   <td>Report</td> 
   <td>Accesso completo</td> 
   <td>Gestisci i rapporti che creano o i rapporti condivisi con loro. Visualizzare, copiare e modificare i rapporti sul sistema.</td> 
  </tr> 
  <tr> 
   <td>Attività</td> 
   <td>Accesso completo</td> 
   <td>Gestione delle attività create o delle attività condivise con</td> 
  </tr> 
  <tr> 
   <td>Modelli</td> 
   <td>Accesso completo</td> 
   <td>Gestire i modelli che creano o i modelli condivisi con loro</td> 
  </tr> 
  <tr> 
   <td>Schede orario</td> 
   <td>Accesso completo</td> 
   <td>Accesso completo</td> 
  </tr> 
  <tr> 
   <td>Utenti</td> 
   <td>Accesso completo</td> 
   <td> <p>Accesso limitato</p> <p>Non possono assegnare gruppi a utenti per i quali non sono un amministratore di gruppo o a gruppi che non sono pubblici.</p> <p>Non possono assegnare un livello di accesso agli utenti più alto del proprio livello di accesso.</p> <p>Se il loro accesso amministrativo al gruppo è abilitato al livello di accesso e viene designato come amministratore di gruppo in un gruppo, possono reimpostare la password di e accedere come utenti del gruppo che amministrano e dei relativi sottogruppi. Non possono reimpostare la password o accedere come amministratore di sistema.<br>Per ulteriori informazioni sull'abilitazione dell'accesso amministrativo ai gruppi per gli utenti, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
