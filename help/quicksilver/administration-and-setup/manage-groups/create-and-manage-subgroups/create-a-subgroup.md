---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Creare un sottogruppo
description: Puoi creare un sottogruppo sotto un gruppo gestito per organizzare utenti e progetti e assegnare diritti di accesso in Adobe Workfront. In genere, gli amministratori dei gruppi gestiscono gruppi e sottogruppi. Possono utilizzare la pagina Gruppi per gestire i gruppi e i sottogruppi in un’unica posizione.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 3%

---

# Creare un sottogruppo

Puoi creare un sottogruppo sotto un gruppo gestito per organizzare utenti e progetti e assegnare diritti di accesso in Adobe Workfront.

Se ci sono gruppi al di sopra del gruppo che gestisci, i loro amministratori possono farlo anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

In genere, tuttavia, gli amministratori dei gruppi gestiscono gruppi e sottogruppi. Possono utilizzare la pagina Gruppi per gestire i gruppi e i sottogruppi in un’unica posizione. Per informazioni sul funzionamento di gruppi e sottogruppi in Workfront, consulta [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md) e [Panoramica sui sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## Aggiungi un sottogruppo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Gruppi**.

   Nell’elenco visualizzato, puoi vedere i gruppi gestiti e tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Selezionare il gruppo o sottogruppo esistente in cui si desidera aggiungere un nuovo sottogruppo.
1. Fai clic su **Nuovo sottogruppo**.
1. In **Nuovo sottogruppo** casella visualizzata, digitare un **Nome gruppo** per il sottogruppo.
1. (Facoltativo) specificare una delle seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome gruppo</td> 
      <td>Modificare il nome del gruppo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Digitare una descrizione per il sottogruppo. È possibile digitare fino a 512 caratteri.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">È attivo</td> 
      <td> <p>(Abilitato per impostazione predefinita) Rende il gruppo attivo nell’istanza di Workfront.</p> <p>Nei campi di tipo avanti come quello mostrato di seguito, quando gli utenti normali cercano un gruppo per allegarlo a un oggetto o per condividerlo con esso, nell’elenco vengono visualizzati solo i gruppi attivi.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Per semplificare questo processo per gli utenti, puoi disattivare l’opzione È attivo per i gruppi attualmente non in uso.</p> <p>Questo campo consente di visualizzare, filtrare e raggruppare facilmente l’elenco Gruppi in base allo stato attivo o inattivo. Per informazioni sull’utilizzo di viste, filtri e raggruppamenti negli elenchi, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Elementi di reporting: filtri, visualizzazioni e raggruppamenti</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendi pubblici questo gruppo e i relativi sottogruppi</td> 
      <td> <p>(Disponibile solo se visualizzi i Dettagli per un gruppo di livello principale, non per un sottogruppo.) Abilita questa opzione per consentire agli utenti del sottogruppo con accesso per l’utente con autorizzazioni di modifica (che non sono amministratori del gruppo) di aggiungere questo gruppo e i relativi sottogruppi al profilo utente di altri utenti.</p> <p>Per un gruppo pubblico, qualsiasi utente (all'interno o all'esterno del gruppo) con accesso per l'utente con modifica può aggiungere il gruppo al profilo di altri utenti. Non possono farlo per un gruppo privato.</p> <p>È possibile modificare questa opzione solo nel gruppo principale superiore in una gerarchia di gruppi con più di un livello. Tutti i sottogruppi del gruppo padre ereditano le relative impostazioni.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Non è possibile rendere pubblico un sottogruppo di per sé, ma è possibile renderlo pubblico come gruppo principale di primo livello, il che rende pubblici anche tutti i sottogruppi dei genitori.</li> 
         <li>Per impostazione predefinita, un sottogruppo appartenente a un gruppo pubblico è pubblico, pertanto qualsiasi utente con accesso utente per la modifica può aggiungere il sottogruppo anche ad altri utenti.</li> 
        </ul> </p> <p>Se hai bisogno di informazioni sull'accesso necessario per modificare gli utenti, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Concedere l’accesso agli utenti</a>. Per informazioni sulla modifica degli utenti, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Modificare il profilo di un utente</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>È possibile assegnare un utente come Business Leader per un sottogruppo gestito. Un Business Leader è uno che prende decisioni commerciali per il sottogruppo. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Panoramica di Business Leader</a><span>.</span></p> <p>Se la persona non è già membro del sottogruppo, l’aggiunta del suo nome a questo campo li aggiunge anche al gruppo.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Prima di rimuovere il Business Leader da un sottogruppo, è necessario rimuovere il nome dal campo Business Leader.</li> 
         <li>Se si rimuove il nome dal campo Business Leader, l'utente rimane membro del sottogruppo a meno che non lo si rimuova. Per istruzioni su come rimuovere un utente da un gruppo, consulta la sezione . <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Gestire le appartenenze a un gruppo</a> nell'articolo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Gestire un gruppo</a>.</li> 
        </ul> </p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Panoramica di Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membri di gruppi e amministratori di gruppi</td> 
      <td> 
       <ul> 
        <li> <p>Membri del gruppo: Per aggiungere utenti e gruppi al sottogruppo, inizia a digitare il nome di un utente o gruppo esistente che desideri aggiungere, quindi seleziona il nome quando viene visualizzato.</p> <p>Gli utenti e i gruppi aggiunti hanno accesso a tutti gli oggetti condivisi con il gruppo.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.subgroups">Amministratori di gruppo: Un sottogruppo eredita gli amministratori del gruppo sopra di esso, pertanto specificare un utente come amministratore del gruppo per un sottogruppo è facoltativo. È possibile assegnare un membro del gruppo come amministratore al gruppo utilizzando il menu a discesa a destra del nome dell'utente.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ricerca persone e gruppi nell'elenco</td> 
      <td> Se devi trovare un utente o un gruppo già assegnato a questo sottogruppo, puoi digitare il nome qui e selezionarlo quando viene visualizzato.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva.**
