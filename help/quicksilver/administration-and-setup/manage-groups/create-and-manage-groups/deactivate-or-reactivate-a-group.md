---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Disattivare o riattivare un gruppo
description: È possibile disattivare un gruppo gestito che non si utilizza più.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 0%

---

# Disattivare o riattivare un gruppo

È possibile disattivare un gruppo gestito che non si utilizza più.

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

## Disattivare o riattivare un gruppo

>[!IMPORTANT]
>
>Quando disattivi un gruppo, vengono disattivati anche tutti i suoi sottogruppi.
>
>Se devi riattivarne uno, puoi farlo dopo aver eseguito una delle seguenti operazioni:
>
>* Rimuoverlo dal gruppo padre. Per ulteriori informazioni, vedere la sezione [Rimuovere un sottogruppo dal relativo gruppo padre e impostarlo come gruppo di primo livello](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) nell&#39;articolo [Gestire un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Spostatela in un gruppo attivo. Per ulteriori informazioni, vedere la sezione [Creare, spostare, visualizzare, modificare, copiare, rinominare, esportare o eliminare un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) nell&#39;articolo [Gestire un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).

{{step-1-to-setup}}

1. Nel pannello a sinistra, seleziona **Gruppi**.

   Nell’elenco visualizzato puoi visualizzare i gruppi che gestisci, insieme a tutti i relativi sottogruppi. Gli amministratori di Adobe Workfront possono visualizzare tutti i gruppi.

1. Fare clic sul nome del gruppo per aprirne la pagina.

1. Fai clic sull&#39;icona Altro ![Altro](assets/more-icon.png) accanto al nome del gruppo, quindi fai clic su **Disattiva** o **Riattiva**.

   >[!NOTE]
   >
   >L&#39;opzione È attivo (opzione Riattiva in Anteprima) non è disponibile se il gruppo è un sottogruppo di un gruppo disattivato. Prima di riattivarla, è necessario rimuoverla dal gruppo padre o spostarla in un gruppo attivo, come descritto nella nota importante precedente.

1. (Condizionale) Se stai disattivando il gruppo, fai clic su **Disattiva** nella casella **Disattiva gruppo** visualizzata.

## Considerazioni per i gruppi inattivi

Considera quanto segue in merito a un gruppo che hai disattivato disabilitando l&#39;opzione È attivo descritta nella sezione [Disattivare o riattivare un gruppo](#View) in questo articolo.

* La disattivazione di un gruppo disattiva anche tutti i sottogruppi. Sono inclusi i sottogruppi aggiunti dopo la disattivazione.

  Per informazioni sulla riattivazione di un sottogruppo in questa situazione, vedere [Informazioni sulla riattivazione di un sottogruppo al di sotto di un gruppo padre inattivo](#about-reactivating-a-subgroup-below-an-inactive-parent-group) in questo articolo.

* Quando si accede all&#39;area Gruppi in Configurazione, è possibile visualizzare solo i gruppi attivi nell&#39;elenco perché Attivo è l&#39;icona filtro ![Filtro](assets/filter-nwepng.png) predefinita per l&#39;elenco. Se desideri visualizzare tutti i gruppi gestiti, inclusi quelli inattivi, puoi utilizzare il filtro Tutto. In alternativa, utilizza il filtro Inattivo per elencare solo quelli inattivi.

  Per ulteriori informazioni sui filtri negli elenchi, vedere [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* La disattivazione di un gruppo non modifica quanto segue:

   * Le associazioni del gruppo agli oggetti. Gli oggetti associati continuano a funzionare come prima, senza alcuna modifica.

     Ad esempio, se un progetto è associato a un gruppo disattivato, il progetto continua a utilizzare le preferenze e gli stati del gruppo senza alcuna modifica.

   * Possibilità di creare un nuovo oggetto, ad esempio un&#39;approvazione, un team o un&#39;azienda, dalla pagina del gruppo in configurazione. Per impostazione predefinita, il nuovo oggetto è associato al gruppo inattivo.
   * La possibilità, in qualità di amministratore, di trovare il gruppo nei filtri e nei rapporti.

     È inoltre possibile trovarlo nei campi di completamento automatico del gruppo, in cui è possibile gestire le impostazioni del gruppo nell&#39;area Configura. Sono incluse le aree Preferenze, Notifiche eventi e Licenze di sistema.

     Ad esempio, se scegli Configurazione > Preferenza progetto > Progetti e cancelli il campo di completamento sopra le opzioni, puoi ancora trovare un gruppo inattivo e configurarne le preferenze di progetto.

## Informazioni sulla riattivazione di un sottogruppo al di sotto di un gruppo padre inattivo {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

La disattivazione di un gruppo disattiva anche tutti i sottogruppi. Se devi riattivare uno dei sottogruppi sotto un gruppo inattivo, puoi effettuare una delle due operazioni seguenti:

* Sposta il sottogruppo sotto un gruppo attivo. Quindi abilitare l&#39;opzione È attivo per il gruppo spostato, come descritto nella sezione [Disattivare o riattivare un gruppo](#View) in questo articolo.

  Per istruzioni sullo spostamento di un gruppo, vedere [Spostare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Rimuove il sottogruppo dal relativo gruppo padre (rendendo il sottogruppo un gruppo di livello superiore). Quindi abilitare l&#39;opzione È attivo per il gruppo spostato, come descritto nella sezione [Disattivare o riattivare un gruppo](#View) in questo articolo.

  Per istruzioni sulla rimozione di un sottogruppo dal gruppo padre, vedere la sezione [Rimuovere un sottogruppo dal gruppo padre e impostarlo come gruppo di livello principale](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) nell&#39;articolo [Gestire un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
