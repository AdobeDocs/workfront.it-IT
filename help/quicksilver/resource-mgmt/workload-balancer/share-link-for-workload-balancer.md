---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Condivisione del bilanciamento del carico di lavoro con un collegamento
description: È possibile condividere il servizio di bilanciamento del carico di lavoro con altri utenti che potrebbero non disporre dell'area di determinazione origine. Per informazioni sull'utilizzo del servizio di bilanciamento del carico di lavoro, vedere Navigare nel servizio di bilanciamento del carico di lavoro.
author: Alina
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---

# Condivisione del bilanciamento del carico di lavoro con un collegamento

È possibile condividere il servizio di bilanciamento del carico di lavoro con altri utenti che potrebbero non disporre dell&#39;area di determinazione origine. Per informazioni sull&#39;utilizzo del servizio di bilanciamento del carico di lavoro, vedi [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Pianificare quando si utilizza il servizio di bilanciamento del carico di lavoro nell'area Origine</p>
   <p>Lavoro, quando si utilizza il bilanciamento del carico di lavoro di un team o di un progetto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizza o accedi di più a quanto segue:</p> 
    <ul> 
     <li> <p>Gestione risorse</p> </li> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Attività</p> </li> 
     <li> <p>Problemi</p> </li> 
    </ul> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per progetti, attività e problemi </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Informazioni incluse nel servizio di bilanciamento del carico di lavoro quando vengono visualizzate da un collegamento condiviso

Quando condividi un collegamento al servizio di bilanciamento del carico di lavoro con altri utenti, con il collegamento condiviso sono incluse le seguenti informazioni:

* Area di lavoro assegnata del servizio di bilanciamento del carico di lavoro.
* Progetto, attività, informazioni utente. Ciò include le informazioni di allocazione utente.
* Le informazioni vengono visualizzate in base al filtro selezionato.

   >[!IMPORTANT]
   >
   >Se elimini i filtri dopo aver condiviso il collegamento, gli utenti che visualizzano il servizio di bilanciamento del carico di lavoro dal collegamento ricevono un avviso relativo all’eliminazione dei filtri. Visualizza tutti gli utenti nell’area Lavoro assegnato. Questa è la vista predefinita per il servizio di bilanciamento del carico di lavoro.

* Numero di settimane selezionate in precedenza.

Le seguenti opzioni sono disponibili per l&#39;utente che visualizza il servizio di bilanciamento del carico di lavoro da un collegamento condiviso per aggiornarsi:

* Le seguenti selezioni della timeline:

   * Oggi
   * Icone avanti e indietro
   * Selezione del calendario

* Icone Giorno, Settimana e Mese
* Icona Impostazioni
* Icona Mostra allocazioni

   Per informazioni sull’utilizzo di queste opzioni, consulta [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* Icona Mostra allocazioni ruolo

   Questa funzione è disponibile solo per il servizio di bilanciamento del carico di lavoro di un progetto.

L&#39;utente che riceve il collegamento condiviso non può effettuare le seguenti operazioni nel servizio di bilanciamento del carico di lavoro da questo collegamento:

* Assegnare gli elementi di lavoro agli utenti
* Gestione delle allocazioni utente
* Creare filtri nuovi o aggiornati originariamente applicati

## Accesso necessario per visualizzare le informazioni nel servizio di bilanciamento del carico di lavoro da un collegamento condiviso

Per visualizzare le informazioni nel servizio di bilanciamento del carico di lavoro da un collegamento condiviso è necessario disporre del seguente accesso:

* Una licenza Adobe Workfront valida e devi aver effettuato l&#39;accesso a Workfront.
* Almeno visualizzare l&#39;accesso a Gestione risorse nel livello di accesso. Per informazioni sulla concessione dell&#39;accesso a Gestione risorse, vedere [Concedere l’accesso a Gestione risorse](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* Visualizza le autorizzazioni per i progetti, le attività, i problemi e gli utenti visualizzati nel servizio di bilanciamento del carico di lavoro.

## Condivisione del servizio di bilanciamento del carico di lavoro con altri utenti da un collegamento

1. Passa al load balancer

   Per informazioni sull&#39;accesso al load balancer, vedi [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. (Facoltativo) Effettua una o più delle seguenti operazioni:

   * Aggiorna la selezione del periodo di tempo.
   * Fai clic su **Giorno, settimana** oppure **Mese** per visualizzare informazioni giornaliere, settimanali o mensili.

      ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * Applicare filtri alle aree di lavoro non assegnate e assegnate.

      Per informazioni sul filtro delle informazioni nel servizio di bilanciamento del carico di lavoro, consulta [Filtrare le informazioni nel servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. Fai clic sul pulsante **icona collegamento** ![](assets/wb-shearable-link-icon-small.png).

   Questo aggiunge il collegamento agli Appunti.

1. Per condividere il collegamento con altri, effettua una delle seguenti operazioni:

   * Incollalo in un messaggio di posta elettronica, chat o in qualsiasi altra applicazione e condividetelo con altri utenti.
   * Aggiungilo a una sezione personalizzata come pagina esterna, aggiungi la sezione personalizzata al profilo di un utente o a un modello di layout, quindi condividi il modello di layout con utenti, team, ruoli di lavoro o gruppi.

      Per informazioni sulla creazione di una pagina esterna, consulta [Incorporare una pagina web esterna in un dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Per informazioni sull’aggiunta di sezioni personalizzate a un modello di layout, consultare [Personalizzare il pannello a sinistra utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

      >[!IMPORTANT]
      >
      >Quando si aggiunge il servizio di bilanciamento del carico di lavoro alla sezione personalizzata di un oggetto, le informazioni nel servizio di bilanciamento del carico di lavoro non vengono filtrate dall’oggetto. Il servizio di bilanciamento del carico di lavoro visualizza le informazioni filtrate dai filtri applicati originariamente.
