---
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: Informazioni su come organizzare i rapporti in un dashboard
description: Puoi verificare se un rapporto viene aggiunto a un dashboard in Adobe Workfront. Questo può essere utile quando si decide quali rapporti è possibile mantenere e quali possono essere eliminati dal sistema. Se i rapporti si trovano sulle dashboard, gli utenti potrebbero comunque fare affidamento su di essi. È consigliabile non eliminare i rapporti elencati nelle dashboard utilizzate dagli utenti. Per ulteriori informazioni sull’aggiunta di rapporti alle dashboard, consulta l’articolo Aggiungere un rapporto a una dashboard.
author: Nolan
feature: Reports and Dashboards
exl-id: ce00c307-9e64-49f5-997b-f7fc461c960c
source-git-commit: d738ef3f6642d5b1a646f58896575a2971bbc06a
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Informazioni su come organizzare i rapporti in un dashboard

## Accedere alle informazioni del dashboard in un elenco di rapporti

Puoi verificare se un rapporto viene aggiunto a un dashboard in Adobe Workfront. Questo può essere utile quando si decide quali rapporti è possibile mantenere e quali possono essere eliminati dal sistema. Se i rapporti si trovano sulle dashboard, gli utenti potrebbero comunque fare affidamento su di essi. È consigliabile non eliminare i rapporti elencati nelle dashboard utilizzate dagli utenti.\
Per ulteriori informazioni sull’aggiunta di rapporti alle dashboard, consulta l’articolo [Aggiungere un rapporto a un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

Per verificare se un rapporto viene aggiunto a un dashboard, effettua una delle seguenti operazioni:

* Creazione di una visualizzazione per un elenco di rapporti e inclusione delle informazioni del dashboard nelle colonne
* Filtrare un elenco di rapporti per una o più dashboard specifiche che sai essere utilizzate attivamente
* Creazione di un report per l&#39;oggetto report e utilizzo di una visualizzazione o di un filtro che include informazioni sul dashboard

Per creare un rapporto è possibile creare una visualizzazione o un filtro, ma è necessario disporre dell’accesso Modifica ai rapporti nel livello di accesso.\
Per ulteriori informazioni sull’accesso ai rapporti, consulta l’articolo [Consentire l’accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).\
Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizzazione delle informazioni del dashboard nella visualizzazione di un elenco di rapporti

>[!WARNING]
>
>L’inclusione della colonna Dashboard in un elenco di rapporti può aumentare notevolmente i tempi di caricamento, in particolare per gli elenchi di rapporti lunghi.

Per creare una visualizzazione con le informazioni del dashboard per un elenco di rapporti:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Rapporti**.
1. Nell’elenco dei rapporti, fai clic sul pulsante **Visualizza** menu a discesa.
1. Fai clic su **Nuova vista**.
1. Fai clic su **Aggiungi colonna**.
1. Inizia a digitare &quot;Dashboard&quot; nella sezione **Inizia a digitare il nome del campo** campo .
1. Sotto la **Rapporto** oggetto, selezionare **Dashboard**.

1. Fai clic su **Salva visualizzazione**.\
   Le dashboard visualizzate in un report vengono visualizzate nella colonna Dashboard dell&#39;elenco dei report.\
   ![](assets/qs-dashboards-in-report-view.png)

## Filtrare un elenco di rapporti in base alle informazioni del dashboard

Per filtrare un elenco di rapporti in base alle informazioni del dashboard:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Rapporti**.

1. Nell’elenco dei rapporti, fai clic sul pulsante **Filtro** menu a discesa.
1. Fai clic su **Nuovo filtro**, quindi fai clic su **Aggiungere una regola filtro**.

1. Inizia a digitare &quot;Dashboard&quot; nella sezione **Inizia a digitare il nome del campo** campo .

1. Sotto la **Dashboard** oggetto, selezionare **Nome**.

1. Seleziona **Uguale** nel menu a discesa del modificatore , inizia a digitare il nome del dashboard per il quale desideri filtrare. Puoi selezionare più dashboard per il filtro.\
   ![](assets/qs-dashboards-in-report-filters-350x143.png)

1. Fai clic su **Salva e chiudi**.\
   Viene visualizzato un elenco di rapporti elencati solo nelle dashboard specificate.\
   È inoltre possibile creare un rapporto per l&#39;oggetto report e utilizzare questo filtro nel report.
