---
product-area: resource-management
keywords: lavoro,team,personale,risorse
navigation-topic: the-workload-balancer
title: Individuare il Bilanciatore dei carichi di lavoro
description: È possibile utilizzare il Bilanciatore dei carichi di lavoro per pianificare le risorse per il lavoro o esaminarne la disponibilità e le allocazioni correnti.
author: Lisa
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: 23c6d9335b0adcafc4e2ecdd8ef2d0ab09709fa8
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 1%

---

# Individuare il Bilanciatore dei carichi di lavoro

È possibile utilizzare il Bilanciatore dei carichi di lavoro per pianificare le risorse per il lavoro o esaminarne la disponibilità e le allocazioni correnti.

Puoi accedere al Bilanciatore dei carichi di lavoro nei seguenti modi:

* Da diverse aree predefinite di Adobe Workfront
* Aggiungendolo a una sezione personalizzata

Questo articolo descrive le aree in cui è possibile accedere al Bilanciatore dei carichi di lavoro.

>[!NOTE]
>
>Indipendentemente dal metodo utilizzato per accedere al Bilanciatore dei carichi di lavoro, la navigazione e la gestione delle risorse sono identiche.
>
>Per informazioni sul Bilanciatore dei carichi di lavoro e su come utilizzarlo per gestire e pianificare le risorse per il lavoro, vedi i seguenti articoli:
>
>* [Panoramica del Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [Navigare nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)
>* [Panoramica sull&#39;assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
>* [Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>oppure</p>
       <p>Corrente: piano, quando si utilizza il Bilanciatore dei carichi di lavoro nell'area Risorse;</br>
       Utilizzare il Bilanciatore dei carichi di lavoro di un team o di un progetto</p></td>
  </tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore ai seguenti elementi:</p> 
    <ul> 
     <li>Gestione risorse</li> 
     <li>Progetti</li> 
     <li>Attività</li> 
     <li>Problemi</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Visualizza le autorizzazioni o versioni successive per i progetti, le attività e i problemi</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Accedere al Bilanciatore dei carichi di lavoro in aree predefinite

Le sezioni seguenti illustrano dove è possibile accedere al Bilanciatore dei carichi di lavoro all’interno di Workfront.

### Accesso al Bilanciatore dei carichi di lavoro per più progetti nell’area Risorse

{{step1-to-resourcing}}

1. Fai clic su **Bilanciatore dei carichi di lavoro** nel pannello a sinistra.

   ![Bilanciamento del carico di lavoro](assets/nwe-balancer-global.png)

   Per impostazione predefinita, il Bilanciatore dei carichi di lavoro visualizza quanto segue per informazioni nell’area Risorse:

   * **Lavoro non assegnato**: nessun elemento di lavoro non assegnato.
   * **Lavoro assegnato**: tutti gli utenti attivi nel sistema.

     È consigliabile utilizzare i filtri durante la visualizzazione degli utenti nell’area Lavoro assegnato. Per ulteriori informazioni, vedere [Informazioni sul filtro nel Bilanciatore dei carichi di lavoro](../workload-balancer/filter-information-workload-balancer.md).

### Accedere al Bilanciatore dei carichi di lavoro per un team

{{step1-to-team}}

Viene visualizzata la pagina del team predefinito.

1. Fai clic su **Bilanciatore dei carichi di lavoro** nel pannello a sinistra.

   ![Bilanciatore dei carichi di lavoro per il team](assets/nwe-balancer-team-350x172.png)

   Il Bilanciatore dei carichi di lavoro di un team visualizza le seguenti informazioni, per impostazione predefinita:

   * **Lavoro non assegnato**: elementi assegnati al team e non assegnati agli utenti.
   * **Lavoro assegnato**: tutti i membri del team con tutte le loro assegnazioni.

     >[!TIP]
     >
     >I membri del team possono essere assegnati a un lavoro assegnato anche al team o a un lavoro assegnato ad altri team o ruoli.

### Accedere al Bilanciatore dei carichi di lavoro per un progetto

{{step1-to-projects}}

1. Fai clic sul nome di un progetto per aprire la pagina del progetto.
1. Fai clic su **Bilanciatore dei carichi di lavoro** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**, quindi su **Bilanciatore dei carichi di lavoro**.

   Viene visualizzato il Bilanciatore dei carichi di lavoro per il progetto.

   ![Bilanciatore dei carichi di lavoro per il progetto](assets/nwe-balancer-project-350x152.png)

   Per impostazione predefinita, nel Bilanciatore dei carichi di lavoro di un progetto vengono visualizzate le seguenti informazioni:

   * **Lavoro non assegnato**: elementi del progetto assegnati a mansioni o team e non assegnati agli utenti.
   * **Lavoro assegnato**: utenti assegnati agli elementi del progetto.

     >[!TIP]
     >
     >Per visualizzare tutti gli utenti nel sistema anziché solo quelli del progetto (nell’area Lavoro assegnato), abilita l’opzione Mostra tutti gli utenti. Per informazioni, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../workload-balancer/navigate-the-workload-balancer.md).


## Aggiungere il Bilanciatore dei carichi di lavoro a una sezione personalizzata

Puoi aggiungere il Bilanciatore dei carichi di lavoro a qualsiasi sezione personalizzata.

La maggior parte delle personalizzazioni già applicate al Bilanciatore dei carichi di lavoro viene mantenuta quando viene aggiunta a una sezione personalizzata.

1. Accedi al Bilanciatore dei carichi di lavoro scegliendo una delle seguenti aree:

   * Area risorse
   * Un team
   * Un progetto

1. Ottieni un collegamento condivisibile e copialo negli Appunti come descritto in [Condividi il Bilanciatore dei carichi di lavoro con un collegamento](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
1. Creare un dashboard con una pagina esterna come descritto in [Incorporare una pagina Web esterna in un dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Utilizza il collegamento condivisibile ottenuto nel passaggio 2 per la pagina esterna.

   <!--
      (NOTE: ensure this stays correct)
      -->

1. Creare una sezione personalizzata come descritto in [Creare schede o sezioni personalizzate](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) per inserire il dashboard nella scheda personalizzata.

   Quando si accede al Bilanciatore dei carichi di lavoro dalla sezione personalizzata, è possibile visualizzarlo come se si stesse accedendo direttamente da una delle aree originali elencate nel passaggio 1.

   <!--
      (NOTE: ensure this stays correct)
     -->

1. (Facoltativo) Condividere la scheda personalizzata in un modello di layout come descritto in [Personalizzare il pannello sinistro utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md) .


<!--
For a team:

* From the Workload Balancer section of a team.

  You can adjust allocations and review or assign work from multiple projects to individual team members.

For a project:

  You can do the following when you use the Workload Balancer within a project:

   * Assign work on the project to users already assigned other work on the project.
   * Assign work to any user that might not be on the project.

   * View additional work that users are assigned to on other projects.
   * Adjust user allocations to work items.-->