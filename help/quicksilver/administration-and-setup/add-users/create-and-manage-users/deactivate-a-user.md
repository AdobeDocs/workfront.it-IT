---
title: Disattivare o riattivare un utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: In qualità di amministratore di Workfront, puoi disattivare o riattivare un utente.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: 198129edd8690393e3214f5041b183b5516617a7
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 0%

---

# Disattivare o riattivare un utente

<!--Audited 2/2024-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Se un utente abbandona l’organizzazione, potrebbe essere necessario rimuoverlo da Adobe Workfront. Non devono rimanere attivi nel sistema, perché questo creerebbe confusione per altri utenti quando li si aggiunge agli aggiornamenti o si assegna loro un lavoro. Quando disattivi un utente, gli altri utenti non visualizzano più il proprio nome durante la ricerca di persone nel sistema.

Gli amministratori possono visualizzare gli utenti inattivi nell’area Configurazione.

Puoi riattivare un utente in qualsiasi momento.

>[!IMPORTANT]
>
>È consigliabile disattivare gli utenti che hanno abbandonato l’organizzazione, anziché eliminarli. Se un utente viene eliminato, tutta la cronologia in Workfront associata a tale utente viene persa. Ciò include le assegnazioni di lavoro, l&#39;associazione con note, ore, documenti e tutti gli altri oggetti creati.
>
>La disattivazione di un utente in Workfront rimuove le licenze dell’utente sia per Workfront che per la verifica digitale. Inoltre, all’utente non può più essere assegnato un lavoro. Quando un utente viene disattivato, la licenza Workfront e la licenza di verifica dell’utente diventano disponibili per essere utilizzate da un altro utente. Tutte le altre informazioni nel profilo dell’utente disattivato rimangono invariate.
>
>Per ulteriori informazioni sull’impatto dell’eliminazione e della disattivazione degli utenti, consulta [Elimina utenti](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

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
   <td>  <p>Nuovo: Standard </p> <p>Oppure </p><p>Corrente: Piano </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Livello di accesso Amministratore di sistema. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
     <li> <p><b>Utenti</b> impostazione nel livello di accesso configurato su <b>Modifica</b> accesso, con <b>Crea</b> e almeno uno dei due <b>Amministratore utenti</b> opzioni abilitate in <b>Metti a punto le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se Utente <b>Amministratore (utenti gruppo)</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> <p>Per ulteriori informazioni su <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti

Prima di disattivare un utente con licenza Amministratore Workfront o Standard o Piano, è necessario associare i relativi oggetti e attività a un altro utente.

Per ulteriori informazioni, consulta [Informazioni sulla disattivazione degli amministratori di Workfront e degli utenti con licenza Pianificazione](#about-deactivating-workfront-administrators-and-plan-license-users) in questo articolo.

## Disattivare un utente

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).

1. Seleziona un utente, fai clic su **Altro** icona ![](assets/more-icon.png), quindi fai clic su **Disattiva**.

1. Clic **Disattiva** nella casella visualizzata.

## Pianifica la disattivazione degli utenti

In qualità di manager, potresti voler contrassegnare gli utenti per la disattivazione prima che lascino effettivamente l’organizzazione. Ad esempio, se lavori con un utente vincolato contrattualmente, tale utente rimane nel tuo sistema per un periodo di tempo limitato e conosci la data di cessazione. Puoi pianificarne la disattivazione in tale data.

Gli amministratori di Workfront e gli utenti con licenza Pianificazione possono visualizzare la data di disattivazione nel proprio profilo utente.

Per pianificare la disattivazione di un utente:

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).

1. Selezionare il nome dell&#39;utente.

   Oppure

   (Facoltativo) Seleziona più utenti per pianificarne la disattivazione in blocco.

1. Fai clic sull’icona Modifica ![](assets/edit-icon.png).
1. Nella casella Modifica utente visualizzata fare clic su **Pianificazione delle risorse** per andare in quella zona.
1. Abilita **Pianifica disattivazione** opzione.

1. Nel calendario visualizzato, specifica la data e l’ora per il **Data disattivazione pianificata**.

   >[!NOTE]
   >
   >* Nella casella ora è possibile selezionare solo incrementi di un&#39;ora intera, non di minuti.
   >* Se selezioni un orario per il giorno corrente che è passato, Workfront pianificherà la disattivazione per il giorno successivo alle 00:00. L&#39;ora selezionata corrisponde al fuso orario del computer dell&#39;utente che sta pianificando la disattivazione.

1. Fai clic su **Salva modifiche**.

   L’utente viene disattivato nel giorno selezionato qualche volta dopo l’ora selezionata. Se hai selezionato più utenti da disattivare in blocco, tutti gli utenti selezionati vengono disattivati nel giorno selezionato qualche volta dopo l’ora selezionata.

È consigliabile creare un rapporto per gli utenti per i quali è stata pianificata la disattivazione, in modo da tenere informati i prossimi utenti da disattivare. Non c’è conferma che la disattivazione sia avvenuta dopo la disattivazione degli utenti.

## Riattivare un utente

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).

1. Seleziona un utente e fai clic sull’icona Altro ![](assets/more-icon.png), quindi fai clic su **Attiva**.

1. Assegna un nuovo **Livello di accesso** nel menu a discesa, quindi fai clic su **Riattiva**.

### Impatto della bozza durante la riattivazione di un utente

Gli utenti disattivati perdono il ruolo di bozza predefinito loro assegnato e la loro licenza di bozza (se sei in un piano legacy di Workfront Premium). Se scegli di riattivare l’utente, devi:

* Riassegnare la licenza (se si utilizza un piano legacy Workfront Premium). Per ulteriori informazioni sui piani di verifica di Workfront, vedere [Accesso alla funzionalità di verifica in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Verifica che abbiano il ruolo di bozza corretto. Agli utenti delle bozze riattivate viene assegnato qualsiasi ruolo di bozza specificato come predefinito per i nuovi utenti. Consulta [Configurare i ruoli di verifica predefiniti](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) per ulteriori informazioni.

## Informazioni sulla disattivazione degli amministratori di Workfront e degli utenti con licenze Standard o Plan

Prima di disattivare un amministratore Workfront o un utente con una licenza Pianificazione, è importante verificare la presenza di oggetti e attività Workfront che coinvolgono tale persona, quindi associarli a un altro amministratore Workfront o a un utente con licenza Pianificazione, a seconda delle necessità.

Tali oggetti e attività possono includere quanto segue:

* Attività o problemi assegnati all&#39;utente
* Progetti di proprietà dell’utente
* Rapporti impostati per l’esecuzione con i diritti di accesso dell’utente
* Modelli di proprietà dell’utente
* Progetti e modelli in cui l’utente è stato impostato come responsabile risorse
* Regole di instradamento della coda richieste per le quali l&#39;amministratore di Workfront o l&#39;utente con licenza Pianificazione è l&#39;assegnatario predefinito
* Processi di approvazione con una fase che include l’utente (in particolare se erano l’unico approvatore della fase)
* Schede orario in cui l&#39;utente è elencato come approvatore
* Profili delle schede orario che elencano l’utente come approvatore
* Verifica dei flussi di lavoro automatizzati che includono l’utente

## Impatto sulla pianificazione delle risorse quando si pianifica la disattivazione di un utente

Quando si pianifica la disattivazione di un utente, questi non vengono più visualizzati nella Programmazione risorse come disponibili per le ore di impostazione del budget. Se rimangono parte dei Pool di Risorse, vengono visualizzati nella Pianificazione risorse, ma la loro disponibilità verrà impostata su zero ore a partire dalla data della loro disattivazione pianificata.

La Programmazione delle risorse tiene conto di tutte le mansioni degli utenti e delle Date di completamento pianificate delle attività e calcola le risorse di conseguenza.

Per ulteriori informazioni sulla Programmazione delle risorse, consulta [Panoramica di Programmazione delle risorse](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
