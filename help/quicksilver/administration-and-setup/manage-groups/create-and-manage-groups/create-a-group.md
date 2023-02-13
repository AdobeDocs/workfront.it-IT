---
user-type: administrator
product-area: system-administration;user-management
keywords: creare, gruppo, sottogruppo, nuovo
navigation-topic: create-and-manage-groups
title: Creare un gruppo
description: In qualità di amministratore di Adobe Workfront, puoi creare gruppi per organizzare utenti e progetti e assegnare diritti di accesso all’interno di Workfront.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 3%

---

# Creare un gruppo

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

In qualità di amministratore di Adobe Workfront, puoi creare gruppi per organizzare utenti e progetti e assegnare diritti di accesso all’interno di Workfront. Per ulteriori informazioni, consulta [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Per ogni sottogruppo è necessario almeno un amministratore di gruppo. Gli amministratori dei gruppi possono utilizzare la pagina Gruppi per gestire i gruppi in un’unica posizione.

Se sei un amministratore di gruppo o un amministratore di Workfront, puoi anche creare sottogruppi all’interno di un gruppo. Per istruzioni, consulta [Creare un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

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

## Creare un gruppo di primo livello da zero

Questi passaggi spiegano come creare un nuovo gruppo da zero. Per informazioni sulla creazione di un gruppo o sottogruppo copiandone uno esistente, consulta [Creare un gruppo di primo livello copiando un gruppo o un sottogruppo esistente](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) in questo articolo.

Per creare un gruppo di livello principale, devi essere un amministratore di Workfront.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Sopra l&#39;elenco dei gruppi, fai clic su **Nuovo gruppo**.

   >[!TIP]
   >
   >In fondo all’elenco dei gruppi, puoi anche fare clic su **Aggiungi altri gruppi** per aggiungere un gruppo in linea, fai clic su **Invio** al termine, aggiungi le informazioni sul gruppo.

1. In **Nuovo gruppo** digitare un nome per il gruppo.
1. Specifica le seguenti informazioni:

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
      <td>Digita una descrizione per il gruppo. È possibile digitare fino a 512 caratteri.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">È attivo</td> 
      <td> <p>(Abilitato per impostazione predefinita) Rende il gruppo attivo nell’istanza di Workfront.</p> <p>Nei campi di tipo avanti come quello mostrato di seguito, quando gli utenti normali cercano un gruppo per allegarlo a un oggetto o per condividerlo con esso, nell’elenco vengono visualizzati solo i gruppi attivi.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Per semplificare questo processo per gli utenti, puoi disattivare l’opzione È attivo per i gruppi attualmente non in uso.</p> <p>Questo campo consente di visualizzare, filtrare e raggruppare facilmente l’elenco Gruppi in base allo stato attivo o inattivo. Per informazioni sull’utilizzo di viste, filtri e raggruppamenti negli elenchi, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementi di reporting: filtri, visualizzazioni e raggruppamenti</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendi pubblici questo gruppo e i relativi sottogruppi</td> 
      <td> <p>(Disponibile solo se visualizzi i Dettagli per un gruppo di livello principale, non per un sottogruppo.) Abilita questa opzione per consentire agli utenti del gruppo con accesso per l’utente con privilegi di modifica (che non sono amministratori del gruppo) di aggiungere questo gruppo e i relativi sottogruppi al profilo utente di altri utenti.</p> <p>Per un gruppo pubblico, qualsiasi utente (all'interno o all'esterno del gruppo) con accesso per l'utente con modifica può aggiungere il gruppo al profilo di altri utenti. Non possono farlo per un gruppo privato.</p> <p>È possibile modificare questa opzione solo nel gruppo principale superiore in una gerarchia di gruppi con più di un livello. Tutti i sottogruppi del gruppo padre ereditano le relative impostazioni.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Non è possibile rendere pubblico un sottogruppo di per sé, ma è possibile renderlo pubblico come gruppo principale di primo livello, il che rende pubblici anche tutti i sottogruppi dei genitori.</li> 
         <li>Per impostazione predefinita, un sottogruppo appartenente a un gruppo pubblico è pubblico, pertanto qualsiasi utente con accesso utente per la modifica può aggiungere il sottogruppo anche ad altri utenti.</li> 
        </ul> </p> <p>Se hai bisogno di informazioni sull'accesso necessario per modificare gli utenti, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>. Per informazioni sulla modifica degli utenti, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>È possibile assegnare un utente come Business Leader per un gruppo gestito. Un Business Leader è qualcuno che prende decisioni commerciali per il gruppo. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Panoramica di Business Leader</a><span>.</span></p> <p>Se la persona non è già membro del gruppo, l’aggiunta del suo nome a questo campo li aggiunge anche al gruppo.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Prima di rimuovere il Business Leader da un gruppo, è necessario rimuovere il nome dal campo Business Leader.</li> 
         <li>Se si rimuove il nome dal campo Business Leader, l'utente rimane membro del gruppo a meno che non lo si rimuova. Per istruzioni su come rimuovere un utente da un gruppo, consulta la sezione . <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Gestire le appartenenze a un gruppo</a> nell'articolo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Gestire un gruppo</a>.</li> 
        </ul> </p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Panoramica di Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membri di gruppi e amministratori di gruppi</td> 
      <td> 
       <ul> 
        <p>Per aggiungere i membri del gruppo, inizia a digitare il nome di un utente o gruppo esistente da aggiungere, quindi seleziona il nome quando viene visualizzato.</p> 
        <p>Gli utenti e i gruppi aggiunti hanno accesso a tutti gli oggetti condivisi con il gruppo.</p>
        <p>Un gruppo di primo livello deve avere almeno un amministratore di gruppo. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ricerca persone e gruppi nell'elenco</td> 
      <td> Se devi trovare un utente o un gruppo già assegnato a questo gruppo, puoi digitare il loro nome qui e selezionarlo quando viene visualizzato.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Crea gruppo**.

## Creare un gruppo di primo livello copiando un gruppo o un sottogruppo esistente {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

In qualità di amministratore di Workfront, puoi creare un nuovo gruppo di livello principale copiando un gruppo o un sottogruppo esistente.

Tieni presente quanto segue quando desideri eseguire questa operazione:

* Tutti i membri e tutti i sottogruppi appartenenti al gruppo esistente vengono copiati nel nuovo gruppo di livello principale.
* I membri del gruppo copiato conservano le assegnazioni che avevano nel gruppo originale. Pertanto, anche gli amministratori del gruppo originale sono designati come amministratori del gruppo nel gruppo copiato.

Per creare un nuovo gruppo di livello principale copiando un gruppo o un sottogruppo:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

   Nell’elenco visualizzato, puoi vedere i gruppi gestiti e tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Seleziona il gruppo da copiare, quindi fai clic sull’icona Copia ![](assets/copy-icon.png).
1. In **Copia gruppo** casella visualizzata, digitare un **Nome gruppo** per il gruppo copiato.

1. Specifica le seguenti informazioni:

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
      <td>Digita una descrizione per il gruppo. È possibile digitare fino a 512 caratteri.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">È attivo</td> 
      <td> <p>(Abilitato per impostazione predefinita) Rende il gruppo attivo nell’istanza di Workfront.</p> <p>Nei campi di tipo avanti come quello mostrato di seguito, quando gli utenti normali cercano un gruppo per allegarlo a un oggetto o per condividerlo con esso, nell’elenco vengono visualizzati solo i gruppi attivi.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Per semplificare questo processo per gli utenti, puoi disattivare l’opzione È attivo per i gruppi attualmente non in uso.</p> <p>Questo campo consente di visualizzare, filtrare e raggruppare facilmente l’elenco Gruppi in base allo stato attivo o inattivo. Per informazioni sull’utilizzo di viste, filtri e raggruppamenti negli elenchi, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Elementi di reporting: filtri, visualizzazioni e raggruppamenti</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendi pubblici questo gruppo e i relativi sottogruppi</td> 
      <td> <p>(Disponibile solo se visualizzi i Dettagli per un gruppo di livello principale, non per un sottogruppo.) Abilita questa opzione per consentire agli utenti del gruppo con accesso per l’utente con privilegi di modifica (che non sono amministratori del gruppo) di aggiungere questo gruppo e i relativi sottogruppi al profilo utente di altri utenti.</p> <p>Per un gruppo pubblico, qualsiasi utente (all'interno o all'esterno del gruppo) con accesso per l'utente con modifica può aggiungere il gruppo al profilo di altri utenti. Non possono farlo per un gruppo privato.</p> <p>È possibile modificare questa opzione solo nel gruppo principale superiore in una gerarchia di gruppi con più di un livello. Tutti i sottogruppi del gruppo padre ereditano le relative impostazioni.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Non è possibile rendere pubblico un sottogruppo di per sé, ma è possibile renderlo pubblico come gruppo principale di primo livello, il che rende pubblici anche tutti i sottogruppi dei genitori.</li> 
         <li>Per impostazione predefinita, un sottogruppo appartenente a un gruppo pubblico è pubblico, pertanto qualsiasi utente con accesso utente per la modifica può aggiungere il sottogruppo anche ad altri utenti.</li> 
        </ul> </p> <p>Se hai bisogno di informazioni sull'accesso necessario per modificare gli utenti, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Concedere l’accesso agli utenti</a>. Per informazioni sulla modifica degli utenti, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Modificare il profilo di un utente</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>È possibile assegnare un utente come Business Leader per un gruppo gestito. Un Business Leader è qualcuno che prende decisioni commerciali per il gruppo. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Panoramica di Business Leader</a><span>.</span></p> <p>Se la persona non è già membro del gruppo, l’aggiunta del suo nome a questo campo li aggiunge anche al gruppo.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Prima di rimuovere il Business Leader da un gruppo, è necessario rimuovere il nome dal campo Business Leader.</li> 
         <li>Se si rimuove il nome dal campo Business Leader, l'utente rimane membro del gruppo a meno che non lo si rimuova. Per istruzioni su come rimuovere un utente da un gruppo, consulta la sezione . <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Gestire le appartenenze a un gruppo</a> nell'articolo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Gestire un gruppo</a>.</li> 
        </ul> </p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Panoramica di Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membri di gruppi e amministratori di gruppi</td> 
      <td> 
       <ul> 
        <li> <p>Membri del gruppo: Per aggiungere utenti e gruppi al gruppo, inizia a digitare il nome di un utente o gruppo esistente che desideri aggiungere, quindi seleziona il nome quando viene visualizzato.</p> <p>Gli utenti e i gruppi aggiunti hanno accesso a tutti gli oggetti condivisi con il gruppo.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.copied groups">Amministratori di gruppo: Tutti gli amministratori di gruppo del gruppo originale sono anche designati come amministratori di gruppo nel gruppo copiato. È possibile assegnare un membro del gruppo come amministratore al gruppo utilizzando il menu a discesa a destra del nome dell'utente.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Un gruppo di primo livello deve avere almeno 1 amministratore di gruppo.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ricerca persone e gruppi nell'elenco</td> 
      <td> Se devi trovare un utente o un gruppo già assegnato a questo gruppo, puoi digitare il loro nome qui e selezionarlo quando viene visualizzato.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* Se il gruppo originale dispone di sottogruppi, i sottogruppi vengono aggiunti al nuovo gruppo e i loro nomi sono, per impostazione predefinita, &quot;Il nome del sottogruppo originale (Copia)&quot;.
   >* Per eliminare qualsiasi utente o sottogruppo dal gruppo originale, fai clic sulla X a destra del nome dell’utente o del sottogruppo.


1. Fai clic su **Crea gruppo**.
