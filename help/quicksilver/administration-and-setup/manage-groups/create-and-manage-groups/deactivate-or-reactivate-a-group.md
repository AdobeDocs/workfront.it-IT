---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Disattivare o riattivare un gruppo
description: È possibile disattivare un gruppo gestito che non si utilizza più.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Disattivare o riattivare un gruppo

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

È possibile disattivare un gruppo gestito che non si utilizza più.

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
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza disponibile, contattare l&#39;amministratore di Workfront.

## Disattivare o riattivare un gruppo

>[!IMPORTANT]
>
>Quando disattivi un gruppo, vengono disattivati anche tutti i suoi sottogruppi.
>
>Se devi riattivarne uno, puoi farlo dopo aver eseguito una delle seguenti operazioni:
>
>* Rimuoverlo dal gruppo padre. Per ulteriori informazioni, consulta la sezione [Rimuovere un sottogruppo dal relativo gruppo padre e impostarlo come gruppo di livello principale](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) nell’articolo [Gestire un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Spostatela in un gruppo attivo. Per ulteriori informazioni, consulta la sezione [Creare, spostare, visualizzare, modificare, copiare, rinominare, esportare o eliminare un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) nell’articolo [Gestire un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, seleziona **Gruppi**.

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo per aprirne la pagina.

1. Fare clic sul menu Altro ![](assets/more-icon.png) accanto al nome del gruppo, quindi fare clic su **Disattiva** o **Riattiva**.

   >[!NOTE]
   >
   >L&#39;opzione È attivo (opzione Riattiva in Anteprima) non è disponibile se il gruppo è un sottogruppo di un gruppo disattivato. Prima di riattivarla, è necessario rimuoverla dal gruppo padre o spostarla in un gruppo attivo, come descritto nella nota importante precedente.

1. (Condizionale) Se stai disattivando il gruppo, fai clic su **Disattiva** nel **Disattiva gruppo** che viene visualizzata.

## Considerazioni per i gruppi inattivi

Considera quanto segue in merito a un gruppo che disattivi disabilitando l’opzione È attivo descritta nella sezione [Disattivare o riattivare un gruppo](#View) in questo articolo.

* La disattivazione di un gruppo disattiva anche tutti i sottogruppi. Sono inclusi i sottogruppi aggiunti dopo la disattivazione.

  Per informazioni sulla riattivazione di un sottogruppo in questa situazione, consulta [Informazioni sulla riattivazione di un sottogruppo al di sotto di un gruppo padre inattivo](#about-reactivating-a-subgroup-below-an-inactive-parent-group) in questo articolo.

* Quando si passa all&#39;area Gruppi in Configurazione, è possibile visualizzare solo i gruppi attivi nell&#39;elenco, poiché il filtro predefinito è Attivo ![](assets/filter-nwepng.png) per quello. Se desideri visualizzare tutti i gruppi gestiti, inclusi quelli inattivi, puoi utilizzare il filtro Tutto. In alternativa, utilizza il filtro Inattivo per elencare solo quelli inattivi.

  Per ulteriori informazioni sui filtri negli elenchi, consulta [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* La disattivazione di un gruppo non modifica quanto segue:

   * Le associazioni del gruppo agli oggetti. Gli oggetti associati continuano a funzionare come prima, senza alcuna modifica.

     Ad esempio, se un progetto è associato a un gruppo disattivato, il progetto continua a utilizzare le preferenze e gli stati del gruppo senza alcuna modifica.

   * Possibilità di creare un nuovo oggetto, ad esempio un&#39;approvazione, un team o un&#39;azienda, dalla pagina del gruppo in configurazione. Per impostazione predefinita, il nuovo oggetto è associato al gruppo inattivo.
   * La possibilità, in qualità di amministratore, di trovare il gruppo nei filtri e nei rapporti.

     È inoltre possibile trovarlo nei campi di completamento automatico del gruppo, in cui è possibile gestire le impostazioni del gruppo nell&#39;area Configura. Sono incluse le aree Preferenze, Notifiche eventi e Licenze di sistema.

     Ad esempio, se scegli Configurazione > Preferenza progetto > Progetti e cancelli il campo di completamento sopra le opzioni, puoi ancora trovare un gruppo inattivo e configurarne le preferenze di progetto.

## Informazioni sulla riattivazione di un sottogruppo al di sotto di un gruppo padre inattivo {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

La disattivazione di un gruppo disattiva anche tutti i sottogruppi. Se devi riattivare uno dei sottogruppi sotto un gruppo inattivo, puoi effettuare una delle due operazioni seguenti:

* Sposta il sottogruppo sotto un gruppo attivo. Quindi abilita l’opzione È attivo per il gruppo spostato, come spiegato nella sezione [Disattivare o riattivare un gruppo](#View) in questo articolo.

  Per istruzioni sullo spostamento di un gruppo, vedere [Spostare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Rimuove il sottogruppo dal relativo gruppo padre (rendendo il sottogruppo un gruppo di livello superiore). Quindi abilita l’opzione È attivo per il gruppo spostato, come spiegato nella sezione [Disattivare o riattivare un gruppo](#View) in questo articolo.

  Per istruzioni sulla rimozione di un sottogruppo dal relativo gruppo padre, vedere la sezione [Rimuovere un sottogruppo dal relativo gruppo padre e impostarlo come gruppo di livello principale](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) nell’articolo [Gestire un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
