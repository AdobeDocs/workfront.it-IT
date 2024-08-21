---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Creare un sottogruppo
description: Puoi creare un sottogruppo all’interno di un gruppo che gestisci per organizzare utenti e progetti e assegnare diritti di accesso in Adobe Workfront. In genere, gli amministratori di gruppi gestiscono gruppi e sottogruppi. È possibile utilizzare la pagina Gruppi per gestire i gruppi e i sottogruppi in un'unica posizione.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 3%

---

# Creare un sottogruppo

Puoi creare un sottogruppo all’interno di un gruppo che gestisci per organizzare utenti e progetti e assegnare diritti di accesso in Adobe Workfront.

Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

In genere, tuttavia, gli amministratori di gruppi gestiscono gruppi e sottogruppi. È possibile utilizzare la pagina Gruppi per gestire i gruppi e i sottogruppi in un&#39;unica posizione. Per informazioni sul funzionamento dei gruppi e dei sottogruppi in Workfront, vedere [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md) e [Panoramica sui sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Aggiungi un sottogruppo

{{step-1-to-setup}}

1. Fai clic su **Gruppi**.

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Selezionare il gruppo o il sottogruppo esistente in cui si desidera aggiungere un nuovo sottogruppo.
1. Fare clic su **Nuovo sottogruppo**.
1. Nella casella **Nuovo sottogruppo** visualizzata, digitare un **Nome gruppo** per il sottogruppo.
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
      <td> <p>(Abilitato per impostazione predefinita) Attiva il gruppo nell’istanza di Workfront.</p> <p>Nei campi di completamento automatico come quello mostrato di seguito, quando gli utenti normali cercano un gruppo per allegarlo a un oggetto o per condividerlo con esso, nell’elenco vengono visualizzati solo i gruppi attivi.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Per semplificare questa operazione per gli utenti, è possibile disattivare l'opzione È attivo per i gruppi attualmente non in uso.</p> <p>Questo campo consente di visualizzare, filtrare e raggruppare facilmente l’elenco Gruppi in base allo stato attivo o inattivo. Per informazioni sull'utilizzo di viste, filtri e raggruppamenti negli elenchi, vedere <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Elementi di reporting: filtri, viste e raggruppamenti</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendi pubblici questo gruppo e i relativi sottogruppi</td> 
      <td> <p>(Disponibile solo se si visualizzano i dettagli di un gruppo principale e non di un sottogruppo). Abilita questa opzione per consentire agli utenti del sottogruppo con accesso di modifica utente (che non sono amministratori del gruppo) di aggiungere questo gruppo e i relativi sottogruppi al profilo utente di altri utenti.</p> <p>Per un gruppo pubblico, qualsiasi utente (interno o esterno al gruppo) con accesso di modifica utente può aggiungere il gruppo al profilo di altri utenti. Non possono farlo per un gruppo privato.</p> <p>È possibile modificare questa opzione solo sul gruppo padre superiore in una gerarchia di gruppi con più livelli. Tutti i sottogruppi del gruppo padre ereditano l'impostazione.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Non è possibile rendere pubblico un sottogruppo di per sé, ma è possibile rendere pubblico il relativo gruppo principale principale, rendendo pubblici anche tutti i sottogruppi del gruppo principale.</li> 
         <li>Un sottogruppo che appartiene a un gruppo pubblico è pubblico per impostazione predefinita, pertanto qualsiasi utente con accesso di modifica utente può aggiungere il sottogruppo anche ad altri utenti.</li> 
        </ul> </p> <p>Se hai bisogno di informazioni sull'accesso necessario per modificare gli utenti, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Concedere l'accesso agli utenti</a>. Per informazioni sulla modifica degli utenti, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Modificare il profilo di un utente</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Leader aziendale </td> 
      <td> <p>È possibile assegnare un utente come Business Leader per un sottogruppo gestito dall'utente. Un Business Leader è una persona che prende decisioni commerciali per il sottogruppo. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Panoramica di Business Leader</a><span>.</span></p> <p>Se la persona non è già membro del sottogruppo, l’aggiunta del nome a questo campo le aggiunge anche al gruppo.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Prima di rimuovere Business Leader da un sottogruppo, è necessario rimuoverne il nome dal campo Business Leader.</li> 
         <li>Se si rimuove il nome dal campo Business Leader, l'utente rimane membro del sottogruppo a meno che non venga rimosso. Per istruzioni sulla rimozione di un utente da un gruppo, vedere la sezione <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Gestire le appartenenze di un gruppo</a> nell'articolo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Gestire un gruppo</a>.</li> 
        </ul> </p> <p>Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Panoramica di Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membri di gruppi e amministratori di gruppi</td> 
      <td> 
       <ul> 
        <li> <p>Membri del gruppo: per aggiungere utenti e gruppi al sottogruppo, inizia a digitare il nome di un utente o gruppo esistente che desideri aggiungere, quindi seleziona il nome quando viene visualizzato.</p> <p>Gli utenti e i gruppi aggiunti possono accedere a tutti gli oggetti condivisi con il gruppo.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.subgroups">Amministratori di gruppo: un sottogruppo eredita gli amministratori di gruppo del gruppo che lo precede, pertanto la specifica di un utente come amministratore di gruppo per un sottogruppo è facoltativa. È possibile assegnare un membro del gruppo come amministratore del gruppo utilizzando il menu a discesa a destra del nome dell'utente.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ricerca persone e gruppi nell'elenco</td> 
      <td> Se devi trovare un utente o un gruppo già assegnato a questo sottogruppo, puoi digitarne il nome qui e selezionarlo quando viene visualizzato.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva.**
