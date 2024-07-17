---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Condividere il Bilanciatore dei carichi di lavoro con un collegamento
description: È possibile condividere il Bilanciatore dei carichi di lavoro con altri utenti che potrebbero non disporre dell’area Risorse. Per informazioni sull’utilizzo del Bilanciatore dei carichi di lavoro, consulta Navigare nel Bilanciatore dei carichi di lavoro.
author: Lisa
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---

# Condividere il Bilanciatore dei carichi di lavoro con un collegamento

È possibile condividere il Bilanciatore dei carichi di lavoro con altri utenti che potrebbero non disporre dell’area Risorse. Per informazioni sull&#39;utilizzo del Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Pianificare, quando si utilizza il Bilanciatore dei carichi di lavoro nell'area Risorse</p>
   <p>Utilizzare il Bilanciatore dei carichi di lavoro di un team o di un progetto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso di visualizzazione o superiore ai seguenti elementi:</p> 
    <ul> 
     <li> <p>Gestione risorse</p> </li> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Attività</p> </li> 
     <li> <p>Problemi</p> </li> 
    </ul> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per i progetti, le attività e i problemi </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

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

1. Fai clic sull&#39;icona **collegamento** ![](assets/wb-shearable-link-icon-small.png).

   Questo aggiunge il collegamento agli Appunti.

1. Effettua una delle seguenti operazioni per condividere il collegamento con altri utenti:

   * Incollalo in un messaggio di posta elettronica, in un messaggio di chat o in qualsiasi altra applicazione e condividilo con altri utenti.
   * Aggiungilo a una sezione personalizzata come pagina esterna, aggiungi la sezione personalizzata al profilo di un utente o a un modello di layout, quindi condividi il modello di layout con utenti, team, mansioni o gruppi.

     Per informazioni sulla creazione di una pagina esterna, vedere [Incorporare una pagina Web esterna in un dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Per informazioni sull&#39;aggiunta di sezioni personalizzate a un modello di layout, vedere [Personalizzare il pannello sinistro utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

     >[!IMPORTANT]
     >
     >Quando si aggiunge il Bilanciatore dei carichi di lavoro alla sezione personalizzata di un oggetto, le informazioni nel Bilanciatore dei carichi di lavoro non vengono filtrate dall’oggetto. Il Bilanciatore dei carichi di lavoro visualizza le informazioni filtrate dai filtri applicati originariamente.
