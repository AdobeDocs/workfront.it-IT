---
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: Come organizzare i rapporti su un dashboard
description: Puoi vedere se un rapporto viene aggiunto a una dashboard in Adobe Workfront. Ciò può essere utile quando si decide quali rapporti è possibile mantenere e quali possono essere eliminati dal sistema. Se i rapporti si trovano su dashboard, gli utenti potrebbero ancora fare affidamento su di essi. È consigliabile non eliminare i rapporti elencati nelle dashboard utilizzate dagli utenti. Per ulteriori informazioni sull’aggiunta di rapporti alle dashboard, consulta l’articolo Aggiungere un rapporto a una dashboard.
author: Nolan
feature: Reports and Dashboards
exl-id: ce00c307-9e64-49f5-997b-f7fc461c960c
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 1%

---

# Come organizzare i rapporti su un dashboard

## Accedere alle informazioni del dashboard in un elenco di report

Puoi vedere se un rapporto viene aggiunto a una dashboard in Adobe Workfront. Ciò può essere utile quando si decide quali rapporti è possibile mantenere e quali possono essere eliminati dal sistema. Se i rapporti si trovano su dashboard, gli utenti potrebbero ancora fare affidamento su di essi. È consigliabile non eliminare i rapporti elencati nelle dashboard utilizzate dagli utenti.\
Per ulteriori informazioni sull&#39;aggiunta di report alle dashboard, vedere l&#39;articolo [Aggiungere un report a una dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

Per verificare se un rapporto viene aggiunto a un dashboard, eseguire una delle operazioni seguenti:

* Creazione di una visualizzazione per un elenco di rapporti e inclusione delle informazioni del dashboard nelle colonne
* Filtrare un elenco di rapporti in base a uno o più dashboard specifici che sai di essere utilizzati attivamente
* Creazione di un report per l&#39;oggetto report e utilizzo di una visualizzazione o di un filtro che includa le informazioni del dashboard

Chiunque può creare una vista o un filtro, ma per creare un rapporto è necessario disporre dell&#39;accesso in modifica ai rapporti nel proprio livello di accesso.\
Per ulteriori informazioni sull&#39;accesso ai report, vedere l&#39;articolo [Concedere l&#39;accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).\
Per ulteriori informazioni sulla creazione di un report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Visualizzare le informazioni del dashboard nella visualizzazione di un elenco di report

>[!WARNING]
>
>L’inclusione della colonna Dashboard in un elenco di rapporti può aumentare notevolmente i tempi di caricamento, in particolare per gli elenchi di rapporti lunghi.

Per creare una vista con le informazioni del dashboard per un elenco di report:

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Workfront, quindi fai clic su **Reports**.
1. Nell&#39;elenco dei report fare clic sul menu a discesa **Visualizza**.
1. Fare clic su **Nuova visualizzazione**.
1. Fai clic su **Aggiungi colonna**.
1. Inizia a digitare &quot;Dashboard&quot; nel campo **Inizia a digitare il nome del campo**.
1. Nell&#39;oggetto **Report**, selezionare **Dashboard**.

1. Fai clic su **Salva vista**.\
   Le dashboard in cui viene visualizzato un report vengono visualizzate nella colonna Dashboard dell’elenco dei report.\
   ![Dashboard nel report](assets/qs-dashboards-in-report-view.png)

## Filtrare un elenco di rapporti in base alle informazioni del dashboard

Per filtrare un elenco di rapporti in base alle informazioni del dashboard:

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Workfront, quindi fai clic su **Reports**.

1. Nell&#39;elenco dei report fare clic sul menu a discesa **Filtro**.
1. Fai clic su **Nuovo filtro**, quindi fai clic su **Aggiungi una regola filtro**.

1. Inizia a digitare &quot;Dashboard&quot; nel campo **Inizia a digitare il nome del campo**.

1. Nell&#39;oggetto **Dashboards**, selezionare **Name**.

1. Seleziona **Uguale** nel menu a discesa del modificatore, quindi inizia a digitare il nome del dashboard in base al quale desideri filtrare. Puoi selezionare più dashboard per il filtro.\
   ![Dashboard nei filtri dei report](assets/qs-dashboards-in-report-filters-350x143.png)

1. Fai clic su **Salva e Chiudi**.\
   Viene visualizzato un elenco di rapporti elencati solo nei dashboard specificati.\
   È inoltre possibile creare un report per l&#39;oggetto report e utilizzare questo filtro nel report.
