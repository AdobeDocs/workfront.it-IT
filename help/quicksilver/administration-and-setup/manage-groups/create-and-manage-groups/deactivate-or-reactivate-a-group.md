---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Disattivare o riattivare un gruppo
description: Puoi disattivare un gruppo gestito che non utilizzi più.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# Disattivare o riattivare un gruppo

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

Puoi disattivare un gruppo gestito che non utilizzi più.

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

## Disattivare o riattivare un gruppo

>[!IMPORTANT]
>
>Quando disattivi un gruppo, vengono disattivati anche tutti i sottogruppi sottostanti.
>
>Se è necessario riattivarne uno, è possibile farlo dopo aver eseguito una delle seguenti operazioni:
>
>* Rimuovi dal gruppo padre. Per ulteriori informazioni, consulta la sezione . [Rimuovere un sottogruppo dal gruppo padre e renderlo un gruppo di livello principale](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) nell&#39;articolo [Gestire un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Spostarlo sotto un gruppo attivo. Per ulteriori informazioni, consulta la sezione . [Creare, spostare, visualizzare, modificare, copiare, rinominare, esportare o eliminare un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) nell&#39;articolo [Gestire un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>


1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, seleziona **Gruppi**.

   Nell’elenco visualizzato, puoi vedere i gruppi gestiti e tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fai clic sul nome del gruppo per aprire la relativa pagina.

1. Fai clic sul menu Altro ![](assets/more-icon.png) accanto al nome del gruppo, quindi fai clic su **Disattiva** o **Riattiva**.

   >[!NOTE]
   >
   >L’opzione È attiva (opzione Riattiva in Anteprima) non è disponibile se il gruppo è un sottogruppo di un gruppo disattivato. Prima di poterla riattivare, è necessario rimuoverlo dal gruppo principale o spostarlo sotto un gruppo attivo, come descritto nella nota importante precedente.

1. (Condizionale) Se stai disattivando il gruppo, fai clic su **Disattiva** in **Disattiva gruppo** che viene visualizzata.

## Considerazioni per i gruppi inattivi

Considera quanto segue su un gruppo disattivato disattivando l&#39;opzione È attivo descritta nella sezione [Disattivare o riattivare un gruppo](#View) in questo articolo.

* La disattivazione di un gruppo disattiva anche tutti i sottogruppi sottostanti. Sono inclusi i sottogruppi aggiunti dopo la disattivazione.

   Per informazioni sulla riattivazione di un sottogruppo in questa situazione, vedi [Informazioni sulla riattivazione di un sottogruppo sotto un gruppo principale inattivo](#about-reactivating-a-subgroup-below-an-inactive-parent-group) in questo articolo.

* Quando si passa all&#39;area Gruppi in Configurazione, è possibile visualizzare solo i gruppi attivi nell&#39;elenco, perché Attivo è il filtro predefinito ![](assets/filter-nwepng.png) per questo. Se desideri visualizzare tutti i gruppi gestiti, inclusi quelli inattivi, puoi utilizzare il filtro Tutto . Oppure utilizza il filtro Inattivo per elencare solo quelli inattivi.

   Per ulteriori informazioni sui filtri negli elenchi, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* La disattivazione di un gruppo non comporta le seguenti modifiche:

   * Le associazioni del gruppo agli oggetti. Gli oggetti associati continuano a funzionare come in precedenza, senza modifiche.

      Ad esempio, se un progetto è associato a un gruppo disattivato, il progetto continua a utilizzare le preferenze e gli stati del gruppo senza apportare alcuna modifica.

   * Possibilità di creare un nuovo oggetto, ad esempio un&#39;approvazione, un team o un&#39;azienda, dalla pagina del gruppo in configurazione. Per impostazione predefinita, il nuovo oggetto è associato al gruppo inattivo.
   * In qualità di amministratore, puoi trovare il gruppo nei filtri e nei rapporti.

      È inoltre possibile trovarlo nei campi tipo avanti del gruppo in cui è possibile gestire le impostazioni del gruppo nell&#39;area Configurazione. Sono incluse le aree Preferenze, Notifiche eventi e Licenze di sistema.

      Ad esempio, se accedi a Configurazione > Preferenze progetto > Progetti e cancelli il campo tipo-avanti sopra le opzioni disponibili, puoi comunque trovare un gruppo inattivo e configurarne le preferenze di progetto.

## Informazioni sulla riattivazione di un sottogruppo sotto un gruppo principale inattivo {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

La disattivazione di un gruppo disattiva anche tutti i sottogruppi sottostanti. Se devi riattivare uno dei sottogruppi sotto un gruppo inattivo, puoi eseguire una delle due operazioni seguenti:

* Spostare il sottogruppo sotto un gruppo attivo. Quindi attiva l’opzione Is Active per il gruppo spostato, come spiegato nella sezione . [Disattivare o riattivare un gruppo](#View) in questo articolo.

   Per istruzioni sullo spostamento di un gruppo, consulta [Spostare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Rimuovere il sottogruppo dal gruppo principale, che lo rende un gruppo di primo livello. Quindi attiva l’opzione Is Active per il gruppo spostato, come spiegato nella sezione . [Disattivare o riattivare un gruppo](#View) in questo articolo.

   Per istruzioni sulla rimozione di un sottogruppo dal gruppo padre, consulta la sezione . [Rimuovere un sottogruppo dal gruppo padre e renderlo un gruppo di livello principale](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) nell&#39;articolo [Gestire un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
