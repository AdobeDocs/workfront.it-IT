---
user-type: administrator
product-area: system-administration;user-management
keywords: crea,gruppo,sottogruppo,nuovo
navigation-topic: create-and-manage-groups
title: Creare un gruppo
description: In qualità di amministratore di Adobe Workfront, puoi creare gruppi per organizzare utenti e progetti e assegnare diritti di accesso in Workfront.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: 0afd578ebaa55d911c04a1d08fbcadddc1d05bbc
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 3%

---

# Creare un gruppo

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

In qualità di amministratore di Adobe Workfront, puoi creare gruppi per organizzare utenti e progetti e assegnare diritti di accesso in Workfront. Per ulteriori informazioni, vedere [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Ogni sottogruppo ha bisogno di almeno un amministratore di gruppo. Gli amministratori di gruppi possono utilizzare la pagina Gruppi per gestire i propri gruppi in un&#39;unica posizione.

Gli amministratori di gruppi e gli amministratori di Workfront possono anche creare sottogruppi in un gruppo. Per istruzioni, vedere [Creare un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Requisiti di accesso

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

## Creare un gruppo di primo livello da zero

Questi passaggi spiegano come creare un nuovo gruppo da zero. Per informazioni sulla creazione di un gruppo o di un sottogruppo copiandone uno esistente, vedere [Creare un gruppo di primo livello copiando un gruppo o un sottogruppo esistente](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) in questo articolo.

Per creare un gruppo di primo livello è necessario essere un amministratore di Workfront.

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Sopra l&#39;elenco dei gruppi, fare clic su **Nuovo gruppo**.

   >[!TIP]
   >
   >In fondo all&#39;elenco dei gruppi, puoi anche fare clic su **Aggiungi altri gruppi** per aggiungere un gruppo in linea, quindi fare clic su **Invio** una volta aggiunte le informazioni sul gruppo.

1. Nella casella **Nuovo gruppo** visualizzata digitare un nome per il gruppo.
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
      <td>Digitare una descrizione per il gruppo. È possibile digitare fino a 512 caratteri.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">È attivo</td> 
      <td> <p>(Abilitato per impostazione predefinita) Attiva il gruppo nell’istanza di Workfront.</p> <p>Nei campi di completamento automatico come quello mostrato di seguito, quando gli utenti normali cercano un gruppo per allegarlo a un oggetto o per condividerlo con esso, nell’elenco vengono visualizzati solo i gruppi attivi.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Per semplificare questa operazione per gli utenti, è possibile disattivare l'opzione È attivo per i gruppi attualmente non in uso.</p> <p>Questo campo consente di visualizzare, filtrare e raggruppare facilmente l’elenco Gruppi in base allo stato attivo o inattivo. Per informazioni sull'utilizzo di viste, filtri e raggruppamenti negli elenchi, vedere <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementi di reporting: filtri, viste e raggruppamenti</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendi pubblici questo gruppo e i relativi sottogruppi</td> 
      <td> <p>(Disponibile solo se si visualizzano i dettagli di un gruppo principale e non di un sottogruppo). Abilita questa opzione per consentire agli utenti del gruppo con accesso di modifica utente (che non sono amministratori del gruppo) di aggiungere questo gruppo e i relativi sottogruppi al profilo utente di altri utenti.</p> <p>Per un gruppo pubblico, qualsiasi utente (interno o esterno al gruppo) con accesso di modifica utente può aggiungere il gruppo al profilo di altri utenti. Non possono farlo per un gruppo privato.</p> <p>È possibile modificare questa opzione solo sul gruppo padre superiore in una gerarchia di gruppi con più livelli. Tutti i sottogruppi del gruppo padre ereditano l'impostazione.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Non è possibile rendere pubblico un sottogruppo da solo, ma è possibile rendere pubblico il relativo gruppo padre di livello superiore, rendendo pubblici anche tutti i sottogruppi del padre.</li> 
         <li>Un sottogruppo che appartiene a un gruppo pubblico è pubblico per impostazione predefinita, pertanto qualsiasi utente con accesso di modifica utente può aggiungere il sottogruppo anche ad altri utenti.</li> 
        </ul> </p> <p>Se hai bisogno di informazioni sull'accesso necessario per modificare gli utenti, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>. Per informazioni sulla modifica degli utenti, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>È possibile assegnare un utente come Business Leader per un gruppo gestito dall'utente. Un Business Leader è una persona che prende decisioni commerciali per il gruppo. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Panoramica di Business Leader</a><span>.</span></p> <p>Se la persona non è già membro del gruppo, l’aggiunta del proprio nome a questo campo le aggiunge anche al gruppo.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Prima di rimuovere Business Leader da un gruppo, è necessario rimuoverne il nome dal campo Business Leader.</li> 
         <li>Se si rimuove il nome dal campo Business Leader, l'utente rimane membro del gruppo a meno che non venga rimosso. Per istruzioni sulla rimozione di un utente da un gruppo, vedere la sezione <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Gestire le appartenenze di un gruppo</a> nell'articolo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Gestire un gruppo</a>.</li> 
        </ul> </p> <p>Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Panoramica di Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membri di gruppi e amministratori di gruppi</td> 
      <td>
        <p>Per aggiungere membri del gruppo, iniziare a digitare il nome di un utente o gruppo esistente che si desidera aggiungere, quindi selezionare il nome quando viene visualizzato.</p> 
        <p>Gli utenti e i gruppi aggiunti possono accedere a tutti gli oggetti condivisi con il gruppo.</p>
        <p>Un gruppo di primo livello deve avere almeno un amministratore di gruppo. </p>
     </tr> 
     <tr> 
      <td role="rowheader">Ricerca persone e gruppi nell'elenco</td> 
      <td> Se devi trovare un utente o un gruppo già assegnato a questo gruppo, puoi digitarne il nome qui e selezionarlo quando viene visualizzato.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Crea gruppo**.

## Creare un gruppo di primo livello copiando un gruppo o un sottogruppo esistente {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

In qualità di amministratore di Workfront, puoi creare un nuovo gruppo di primo livello copiando un gruppo o un sottogruppo esistente.

Quando desideri eseguire questa operazione, tieni presente quanto segue:

* Tutti i membri ed eventuali sottogruppi appartenenti al gruppo esistente vengono copiati nel nuovo gruppo principale.
* I membri del gruppo copiato mantengono le assegnazioni che avevano nel gruppo originale. Pertanto, anche gli amministratori di gruppo del gruppo originale vengono designati come amministratori di gruppo nel gruppo copiato.

Per creare un nuovo gruppo di primo livello copiando un gruppo o un sottogruppo:

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Selezionare il gruppo da copiare, quindi fare clic sull&#39;icona Copia ![](assets/copy-icon.png).
1. Nella casella **Copia gruppo** visualizzata, digitare un **Nome gruppo** per il gruppo copiato.

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
      <td>Digitare una descrizione per il gruppo. È possibile digitare fino a 512 caratteri.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">È attivo</td> 
      <td> <p>(Abilitato per impostazione predefinita) Attiva il gruppo nell’istanza di Workfront.</p> <p>Nei campi di completamento automatico come quello mostrato di seguito, quando gli utenti normali cercano un gruppo per allegarlo a un oggetto o per condividerlo con esso, nell’elenco vengono visualizzati solo i gruppi attivi.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Per semplificare questa operazione per gli utenti, è possibile disattivare l'opzione È attivo per i gruppi attualmente non in uso.</p> <p>Questo campo consente di visualizzare, filtrare e raggruppare facilmente l’elenco Gruppi in base allo stato attivo o inattivo. Per informazioni sull'utilizzo di viste, filtri e raggruppamenti negli elenchi, vedere <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Elementi di reporting: filtri, viste e raggruppamenti</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendi pubblici questo gruppo e i relativi sottogruppi</td> 
      <td> <p>(Disponibile solo se si visualizzano i dettagli di un gruppo principale e non di un sottogruppo). Abilita questa opzione per consentire agli utenti del gruppo con accesso di modifica utente (che non sono amministratori del gruppo) di aggiungere questo gruppo e i relativi sottogruppi al profilo utente di altri utenti.</p> <p>Per un gruppo pubblico, qualsiasi utente (interno o esterno al gruppo) con accesso di modifica utente può aggiungere il gruppo al profilo di altri utenti. Non possono farlo per un gruppo privato.</p> <p>È possibile modificare questa opzione solo sul gruppo padre superiore in una gerarchia di gruppi con più livelli. Tutti i sottogruppi del gruppo padre ereditano l'impostazione.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Non è possibile rendere pubblico un sottogruppo di per sé, ma è possibile rendere pubblico il relativo gruppo principale principale, rendendo pubblici anche tutti i sottogruppi del gruppo principale.</li> 
         <li>Un sottogruppo che appartiene a un gruppo pubblico è pubblico per impostazione predefinita, pertanto qualsiasi utente con accesso di modifica utente può aggiungere il sottogruppo anche ad altri utenti.</li> 
        </ul> </p> <p>Se hai bisogno di informazioni sull'accesso necessario per modificare gli utenti, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Concedere l'accesso agli utenti</a>. Per informazioni sulla modifica degli utenti, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Modificare il profilo di un utente</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>È possibile assegnare un utente come Business Leader per un gruppo gestito dall'utente. Un Business Leader è una persona che prende decisioni commerciali per il gruppo. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Panoramica di Business Leader</a><span>.</span></p> <p>Se la persona non è già membro del gruppo, l’aggiunta del proprio nome a questo campo le aggiunge anche al gruppo.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Prima di rimuovere Business Leader da un gruppo, è necessario rimuoverne il nome dal campo Business Leader.</li> 
         <li>Se si rimuove il nome dal campo Business Leader, l'utente rimane membro del gruppo a meno che non venga rimosso. Per istruzioni sulla rimozione di un utente da un gruppo, vedere la sezione <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Gestire le appartenenze di un gruppo</a> nell'articolo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Gestire un gruppo</a>.</li> 
        </ul> </p> <p>Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Panoramica di Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membri di gruppi e amministratori di gruppi</td> 
      <td> 
       <ul> 
        <li> <p>Membri del gruppo: per aggiungere utenti e gruppi al gruppo, inizia a digitare il nome di un utente o gruppo esistente che desideri aggiungere, quindi seleziona il nome quando viene visualizzato.</p> <p>Gli utenti e i gruppi aggiunti possono accedere a tutti gli oggetti condivisi con il gruppo.</p> </li> 
        <li> <p>Amministratori di gruppo: tutti gli amministratori di gruppo del gruppo originale vengono anche designati come amministratori di gruppo nel gruppo copiato. È possibile assegnare un membro del gruppo come amministratore del gruppo utilizzando il menu a discesa a destra del nome dell'utente.</p> <p>Un gruppo di primo livello deve avere almeno un amministratore di gruppo.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ricerca persone e gruppi nell'elenco</td> 
      <td> Se devi trovare un utente o un gruppo già assegnato a questo gruppo, puoi digitarne il nome qui e selezionarlo quando viene visualizzato.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* Se il gruppo originale include sottogruppi, questi ultimi vengono aggiunti al nuovo gruppo e, per impostazione predefinita, il nome del sottogruppo originale (Copia) è &quot;Nome del sottogruppo originale&quot;.
   >* È possibile eliminare qualsiasi utente o sottogruppo dal gruppo originale facendo clic sulla X a destra del nome dell&#39;utente o del sottogruppo.

1. Fai clic su **Crea gruppo**.
