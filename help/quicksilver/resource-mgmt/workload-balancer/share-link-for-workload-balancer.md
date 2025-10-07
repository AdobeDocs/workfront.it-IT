---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Condividere il Bilanciatore dei carichi di lavoro con un collegamento
description: È possibile condividere il Bilanciatore dei carichi di lavoro con altri utenti che potrebbero non disporre dell’area Risorse. Per informazioni sull’utilizzo del Bilanciatore dei carichi di lavoro, consulta Navigare nel Bilanciatore dei carichi di lavoro.
author: Lisa
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 58567104d88e7e1363d4196aec8a36ee0566b95a
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 1%

---

# Condividere il Bilanciatore dei carichi di lavoro con un collegamento

Puoi condividere il Bilanciatore dei carichi di lavoro con altri utenti che potrebbero non avere l’area Risorse disponibile nel menu principale. Per informazioni sull&#39;utilizzo del Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

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
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore ai seguenti elementi:</p> 
    <ul> 
     <li>Gestione risorse</li> 
     <li>Progetti</li> 
     <li>Attività</li> 
     <li>Problemi</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Visualizza o autorizzazioni superiori per i progetti, le attività e i problemi</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informazioni incluse nel Bilanciatore dei carichi di lavoro quando viene visualizzato da un collegamento condiviso

Quando condividi un collegamento al Bilanciatore dei carichi di lavoro con altri utenti, le seguenti informazioni sono incluse nel collegamento condiviso:

* L’area Assigned Work (Lavoro assegnato) del Bilanciatore dei carichi di lavoro.
* Progetto, attività, informazioni utente. Ciò include le informazioni sull’allocazione degli utenti.
* Le informazioni vengono visualizzate in base al filtro selezionato.

  >[!IMPORTANT]
  >
  >Se elimini i filtri dopo aver condiviso il collegamento, gli utenti che visualizzano il Bilanciatore dei carichi di lavoro dal collegamento ricevono un avviso che informa che i filtri sono stati eliminati. Visualizza tutti gli utenti nell’area Lavoro assegnato. Questa è la vista predefinita per il Bilanciatore dei carichi di lavoro.

* Il numero di settimane precedentemente selezionate.

Per consentire agli utenti che visualizzano il Bilanciatore dei carichi di lavoro da un collegamento condiviso di aggiornarsi, sono disponibili le seguenti opzioni:

* Le seguenti selezioni della timeline:

   * Oggi
   * Icone avanti e indietro
   * Selezione calendario

* Icone Giorno, Settimana e Mese
* Icona Impostazioni
* Icona Mostra allocazioni

  Per informazioni sull&#39;utilizzo di queste opzioni, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* Icona Mostra allocazioni ruolo

  Questa opzione è disponibile solo per il Bilanciatore dei carichi di lavoro di un progetto.

L’utente che riceve il collegamento condiviso non può effettuare le seguenti operazioni nel Bilanciatore dei carichi di lavoro da questo collegamento:

* Assegna elementi di lavoro agli utenti
* Gestire le allocazioni utente
* Creare nuovi filtri o aggiornare quelli applicati in origine

## Accesso necessario per visualizzare le informazioni nel Bilanciatore dei carichi di lavoro da un collegamento condiviso

Per visualizzare le informazioni nel Bilanciatore dei carichi di lavoro da un collegamento condiviso, è necessario disporre dei seguenti diritti di accesso:

* Una licenza Adobe Workfront valida e devi aver effettuato l’accesso a Workfront.
* Almeno visualizzare l&#39;accesso alla gestione delle risorse nel proprio livello di accesso. Per informazioni sulla concessione dell&#39;accesso a Gestione risorse, vedere [Concedere l&#39;accesso a Gestione risorse](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* Visualizzare le autorizzazioni per i progetti, le attività, i problemi e gli utenti visualizzati nel Bilanciatore dei carichi di lavoro.

## Condividere il Bilanciatore dei carichi di lavoro con altri utenti da un collegamento

1. Vai al Bilanciatore dei carichi di lavoro

   Per informazioni sull&#39;accesso al Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. (Facoltativo) Effettuate una o più delle seguenti operazioni:

   * Aggiorna la selezione del periodo di tempo.
   * Fai clic su **Giorno, Settimana** o **Mese** per visualizzare informazioni giornaliere, settimanali o mensili.

     ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * Applicare i filtri alle aree Lavoro non assegnato e Lavoro assegnato.

     Per informazioni sul filtro delle informazioni nel Bilanciatore dei carichi di lavoro, vedere [Informazioni sul filtro nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. Fai clic sull&#39;icona **collegamento** ![collegamento](assets/wb-shearable-link-icon-small.png).

   Questo aggiunge il collegamento agli Appunti.

1. Effettua una delle seguenti operazioni per condividere il collegamento con altri utenti:

   * Incollalo in un messaggio di posta elettronica, in un messaggio di chat o in qualsiasi altra applicazione e condividilo con altri utenti.
   * Aggiungilo a una dashboard come pagina esterna, aggiungi la dashboard al profilo di un utente o a un modello di layout, quindi condividi il modello di layout con utenti, team, mansioni o gruppi.

     Per informazioni sulla creazione di una pagina esterna, vedere [Incorporare una pagina Web esterna in un dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Per informazioni sull&#39;aggiunta di dashboard a un modello layout, vedere [Personalizzare il pannello sinistro utilizzando un modello layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

     >[!IMPORTANT]
     >
     >Quando aggiungi il Bilanciatore dei carichi di lavoro come dashboard al pannello sinistro di un oggetto, le informazioni nel Bilanciatore dei carichi di lavoro non vengono filtrate dall’oggetto. Il Bilanciatore dei carichi di lavoro visualizza le informazioni filtrate dai filtri applicati originariamente.
