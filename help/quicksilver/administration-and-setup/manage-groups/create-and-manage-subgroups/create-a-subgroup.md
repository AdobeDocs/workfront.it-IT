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
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# Creare un sottogruppo

Puoi creare un sottogruppo all’interno di un gruppo che gestisci per organizzare utenti e progetti e assegnare diritti di accesso in Adobe Workfront.

Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

In genere, tuttavia, gli amministratori di gruppi gestiscono gruppi e sottogruppi. È possibile utilizzare la pagina Gruppi per gestire i gruppi e i sottogruppi in un&#39;unica posizione. Per informazioni sul funzionamento dei gruppi e dei sottogruppi in Workfront, vedere [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md) e [Panoramica sui sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr>
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungi un sottogruppo

{{step-1-to-setup}}

1. Fai clic su **Gruppi**.

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Selezionare il gruppo o il sottogruppo esistente in cui si desidera aggiungere un nuovo sottogruppo.
1. Fare clic su **Nuovo sottogruppo**.
1. Nella casella **Nuovo sottogruppo** visualizzata, digitare un **nome gruppo** per il sottogruppo.
1. (Facoltativo) Inserire una delle seguenti informazioni:

   * **Descrizione**: digitare una descrizione per il sottogruppo. È possibile digitare fino a 512 caratteri.
   * **È attivo**: questa opzione è attivata per impostazione predefinita e rende il gruppo attivo nell&#39;istanza di Workfront.

     Nei campi typeahead come quelli riportati di seguito, quando gli utenti normali cercano un gruppo per allegarlo a un oggetto o condividerlo con esso, nell&#39;elenco vengono visualizzati solo i gruppi attivi.

     ![Campo automatico per un gruppo](assets/typeahead-for-group.png)

     Per semplificare questa operazione per gli utenti, è possibile disabilitare l&#39;opzione **È attivo** per i gruppi attualmente non in uso.

     Questo campo consente di visualizzare, filtrare e raggruppare facilmente l’elenco Gruppi in base allo stato attivo o inattivo. Per informazioni sull&#39;utilizzo di viste, filtri e raggruppamenti negli elenchi, vedere [Elementi di reporting: filtri, viste e raggruppamenti](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   * **Business Leader**: è possibile assegnare un utente come Business Leader per un sottogruppo gestito dall&#39;utente. Un Business Leader è una persona che prende decisioni commerciali per il sottogruppo. Per ulteriori informazioni, vedere [Panoramica di Business Leader](/help/quicksilver/administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

     Se la persona non è già membro del sottogruppo, l’aggiunta del nome a questo campo le aggiunge anche al gruppo.

     >[!NOTE]
     >
     >* Prima di rimuovere Business Leader da un sottogruppo, è necessario rimuoverne il nome dal campo Business Leader.
     >* Se si rimuove il nome dal campo Business Leader, l&#39;utente rimane membro del sottogruppo a meno che non venga rimosso. Per istruzioni sulla rimozione di un utente da un gruppo, vedere [Visualizzare e gestire le appartenenze di un gruppo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

   * **Membri del gruppo e amministratori del gruppo**: per aggiungere utenti e gruppi come membri del sottogruppo, iniziare a digitare il nome di un utente o di un gruppo esistente che si desidera aggiungere, quindi selezionare il nome quando viene visualizzato.

     Gli utenti e i gruppi aggiunti possono accedere a tutti gli oggetti condivisi con il gruppo.

     Un sottogruppo eredita gli amministratori del gruppo al di sopra di esso, pertanto la specifica di un utente come amministratore del gruppo per un sottogruppo è facoltativa. È possibile assegnare un membro del gruppo come amministratore del gruppo utilizzando il menu a discesa a destra del nome dell&#39;utente.

   * **Cerca persone e gruppi nell&#39;elenco**: se devi trovare un utente o un gruppo già assegnato a questo sottogruppo, puoi digitarne il nome qui e selezionarlo quando viene visualizzato.

1. Fai clic su **Salva.**
