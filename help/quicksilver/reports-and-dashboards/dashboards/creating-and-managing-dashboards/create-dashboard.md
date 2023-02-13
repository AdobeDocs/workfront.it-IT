---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Creare un dashboard
description: È possibile creare dashboard per accedere rapidamente alle informazioni contenute in rapporti, calendari e pagine esterne.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Creare un dashboard

È possibile creare dashboard per accedere rapidamente alle informazioni contenute in rapporti, calendari e pagine esterne.

Per ulteriori informazioni sulle dashboard, consulta [Guida introduttiva alle dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>piano Adobe Workfront*</strong></p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Licenza Adobe Workfront*</strong></p> </td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Accesso a Reports, Dashboard e Calendari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Ottieni le autorizzazioni di gestione per il nuovo dashboard</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.<br>Per ulteriori informazioni sulle autorizzazioni per le dashboard, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Condividere rapporti, dashboard e calendari </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario creare uno dei seguenti oggetti prima di aggiungerli a un dashboard:

* **Rapporti**: Per informazioni sulla creazione di rapporti, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Calendari**: Per informazioni sulla creazione di calendari, consulta [Panoramica dei rapporti sul calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

* **Pagine esterne**: Per informazioni sulla creazione di pagine esterne, consulta [Incorporare una pagina web esterna in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Creare un dashboard

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon.png), quindi fai clic su **Dashboard.**
1. Fai clic su **Nuovo dashboard**.\
   Viene visualizzata la finestra di dialogo Nuovo dashboard.

1. Specifica quanto segue:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nome</strong></td>
      <td><p>Questo è il nome del dashboard.</p><p>Se non si specifica un nome, per impostazione predefinita il nome del primo rapporto sul dashboard diventa il nome del dashboard.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descrizione (facoltativo)</strong></td>
      <td>Descrizione del dashboard.</td>
     </tr>
    </tbody>
   </table>

1. Seleziona un layout facendo clic sul pulsante di scelta corrispondente.

   Il layout a colonna singola è quello predefinito.

   Per informazioni sul layout dei rapporti sulle dashboard, consulta [Comprendere la modalità di visualizzazione dei rapporti su un dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Consider adding the information from this article here, at some point, instead of linking to it.)
   </MadCap:conditionalText>
   -->

1. Aggiungi rapporti, calendari o pagine esterne esistenti ricercandoli nel **Cerca per nome o tipo ...** quindi trascinarli nel riquadro layout quando vengono visualizzati nell&#39;elenco.

   >[!NOTE]
   >
   >Quando si cerca un elemento, la ricerca restituisce uno qualsiasi dei 2.000 report creati più di recente. I nomi dei rapporti che includono caratteri unicode non vengono restituiti nei risultati della ricerca. Come best practice, evita di includere caratteri unicode durante la denominazione degli oggetti in Workfront digitando dei nomi anziché copiarli e incollarli da un’altra origine.

   ![Cercare rapporti](assets/qs-new-dashboard-ui-0722.png)

1. (Facoltativo) Fai clic su **Aggiungi pagina esterna** per aggiungere una pagina esterna al dashboard.\
   Per ulteriori informazioni sulla creazione di pagine esterne e sulla loro incorporazione nelle dashboard, consulta [Incorporare una pagina web esterna in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Fai clic su **Salva e chiudi**.\
   Nell’angolo superiore destro del dashboard viene visualizzata una marca temporale. La marca temporale include la data, l’ora e il fuso orario dell’ultimo aggiornamento del dashboard.
