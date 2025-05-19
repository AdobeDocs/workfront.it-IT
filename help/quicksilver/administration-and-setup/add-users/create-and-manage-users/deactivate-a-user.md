---
title: Disattivare o riattivare un utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Gli amministratori di Workfront possono disattivare o riattivare un utente.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: b235945deb3254feaf671083fc992786851a3286
workflow-type: tm+mt
source-wordcount: '1104'
ht-degree: 2%

---

# Disattivare o riattivare un utente {#deactivate-or-reactivate-a-user}

>[!CONTEXTUALHELP]
>id="wf_users_deactivate_user"
>title="Disattivare un utente"
>abstract="La disattivazione di un utente fa sì che venga rimosso da Workfront e Frame.io. Gli utenti disattivati possono essere riattivati in un secondo momento."

<!--Audited 5/2025-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/it/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Se un utente abbandona l’organizzazione, si consiglia di disattivarlo nel sistema per evitare di creare confusione per altri utenti quando li aggiunge agli aggiornamenti o li assegna al lavoro. Quando disattivi un utente, gli altri utenti non visualizzano più il proprio nome durante la ricerca di persone nel sistema.

Gli amministratori possono visualizzare gli utenti inattivi nell’area Configurazione.

Puoi riattivare un utente in qualsiasi momento.

>[!IMPORTANT]
>
>* È consigliabile disattivare gli utenti che hanno abbandonato l’organizzazione, anziché eliminarli. Se un utente viene eliminato, tutta la cronologia in Workfront associata a tale utente viene persa. Ciò include le assegnazioni di lavoro, l&#39;associazione con note, ore, documenti e tutti gli altri oggetti creati.
>
>* La disattivazione di un utente in Workfront rimuove le licenze dell’utente sia per Workfront che per la verifica digitale. Inoltre, all’utente non può più essere assegnato un lavoro. Quando un utente viene disattivato, la licenza Workfront e la licenza di verifica dell’utente diventano disponibili per essere utilizzate da un altro utente. Tutte le altre informazioni nel profilo dell’utente disattivato rimangono invariate.
>
>* La disattivazione di un utente in Workfront non ne comporta la rimozione dal profilo di prodotto Workfront in Adobe Admin Console. Per ulteriori informazioni, vedere [Elimina utenti](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).


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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p><p>Oppure</p><p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Livello di accesso Amministratore di sistema. </li> 
     <li> <p>Utenti che impostano nel proprio livello di accesso l'accesso Modifica, con Crea e almeno una delle due opzioni Amministratore utenti abilitate in Ottimizza le impostazioni <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se l'opzione Amministratore utenti (Utenti gruppi) è abilitata, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di disattivare un utente con licenza Amministratore Workfront o Standard o Piano, è necessario associare i relativi oggetti e attività a un altro utente.

Per ulteriori informazioni, vedere [Informazioni sulla disattivazione degli amministratori di Workfront e sugli utenti con licenza Pianificazione](#about-deactivating-workfront-administrators-and-plan-license-users) in questo articolo.

## Disattivare un utente

Quando disattivi un utente tieni presente quanto segue:

* L&#39;utente non potrà accedere al sistema.
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* Tutti i dati associati all’utente verranno conservati.
* È possibile assegnare la licenza di un utente disattivato a un altro utente.

Per disattivare un utente:

{{step-1-to-users}}

1. Selezionare un utente nell&#39;elenco degli utenti.
1. Fai clic sull&#39;icona **Altro** ![Altro icona](assets/more-icon.png), quindi fai clic su **Disattiva**.

1. Nella finestra di dialogo **Disattiva utente** fare clic su **Disattiva**.

## Pianifica la disattivazione degli utenti

In qualità di manager, potresti voler contrassegnare gli utenti per la disattivazione prima che lascino effettivamente l’organizzazione. Ad esempio, se lavori con un utente vincolato contrattualmente, tale utente rimane nel tuo sistema per un periodo di tempo limitato e conosci la data di cessazione. Puoi pianificarne la disattivazione in tale data.

Gli amministratori di Workfront e gli utenti con licenza Pianificazione possono visualizzare la data di disattivazione nel proprio profilo utente.

Per pianificare la disattivazione di un utente:

{{step-1-to-users}}

1. Selezionare l&#39;utente nell&#39;elenco Utenti.

   Oppure

   (Facoltativo) Seleziona più utenti per pianificarne la disattivazione in blocco.

1. Fai clic sull&#39;icona **Modifica** ![Modifica](assets/edit-icon.png).
1. Nel pannello a sinistra della casella **Modifica utente**, fare clic su **Pianificazione risorse**.
1. Selezionare la casella di controllo **Pianifica disattivazione**.

1. Selezionare la data e l&#39;ora per la **Data disattivazione pianificata**.

   >[!NOTE]
   >
   >* Nella casella ora è possibile selezionare solo incrementi di un&#39;ora intera, non di minuti.
   >* Se selezioni un orario per il giorno corrente che è passato, Workfront pianificherà la disattivazione per il giorno successivo alle 00:00.
   >* L&#39;ora selezionata corrisponde al fuso orario del computer dell&#39;utente che sta pianificando la disattivazione.

1. Fai clic su **Salva modifiche**.

L’utente viene disattivato nel giorno selezionato qualche volta dopo l’ora selezionata. Se hai selezionato più utenti da disattivare in blocco, tutti gli utenti selezionati vengono disattivati nel giorno selezionato qualche volta dopo l’ora selezionata.

È consigliabile creare un rapporto per gli utenti per i quali è stata pianificata la disattivazione, in modo da tenere informati i prossimi utenti da disattivare. Non c’è conferma che la disattivazione sia avvenuta dopo la disattivazione degli utenti.

## Riattivare un utente

{{step-1-to-users}}

1. Seleziona un utente, fai clic sull&#39;icona **Altro** ![Altro](assets/more-icon.png), quindi su **Attiva**.

1. Nella finestra di dialogo **Riattiva utente**, seleziona un nuovo **Livello di accesso** nel menu a discesa, quindi fai clic su **Riattiva**.
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### Impatto della bozza durante la riattivazione di un utente

Gli utenti disattivati perdono il ruolo di bozza predefinito loro assegnato e la loro licenza di bozza (se sei in un piano legacy di Workfront Premium). Se scegli di riattivare l’utente, devi:

* Riassegnare la licenza (se si utilizza un piano legacy Workfront Premium). Per ulteriori informazioni sui piani di verifica di Workfront, vedere [Accesso alla funzionalità di verifica in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Verifica che abbiano il ruolo di bozza corretto. Agli utenti delle bozze riattivate viene assegnato qualsiasi ruolo di bozza specificato come predefinito per i nuovi utenti. Per ulteriori informazioni, vedere [Configurare i ruoli di verifica predefiniti](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md).

## Informazioni sulla disattivazione degli amministratori di Workfront e degli utenti con licenze Standard o Plan

Prima di disattivare un amministratore Workfront o un utente con una licenza Pianificazione, è importante verificare la presenza di oggetti e attività Workfront che coinvolgono tale persona, quindi associarli a un altro amministratore Workfront o a un utente con licenza Pianificazione, a seconda delle necessità.

Tali oggetti e attività possono includere quanto segue:

* Attività o problemi assegnati all&#39;utente.
* Progetti di proprietà dell’utente.
* Report impostati per l&#39;esecuzione con i diritti di accesso dell&#39;utente.
* Modelli di proprietà dell’utente.
* Progetti e modelli in cui l’utente è stato impostato come responsabile risorse.
* Regole di instradamento della coda richieste l&#39;amministratore di Workfront o l&#39;utente con licenza Pianificazione è l&#39;assegnatario predefinito.
* Processi di approvazione con una fase che include l’utente (in particolare se è stato l’unico approvatore della fase).
* Schede orario che elencano l’utente come approvatore.
* Profili delle schede orario che elencano l’utente come approvatore.
* Verifica dei flussi di lavoro automatizzati che includono l’utente.

## Impatto sulla pianificazione delle risorse quando si pianifica la disattivazione di un utente

Quando si pianifica la disattivazione di un utente, questi non vengono più visualizzati nella Programmazione risorse come disponibili per le ore di impostazione del budget. Se rimangono parte dei Pool di Risorse, vengono visualizzati nella Pianificazione risorse, ma la loro disponibilità verrà impostata su zero ore a partire dalla data della loro disattivazione pianificata.

La Programmazione delle risorse tiene conto di tutte le mansioni degli utenti e delle Date di completamento pianificate delle attività e calcola le risorse di conseguenza.

Per ulteriori informazioni sulla Programmazione delle risorse, vedere [Panoramica sulla programmazione delle risorse](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

