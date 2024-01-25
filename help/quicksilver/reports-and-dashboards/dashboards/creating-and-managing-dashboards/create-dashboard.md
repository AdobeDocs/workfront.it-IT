---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Creare un dashboard
description: Puoi creare dashboard per accedere rapidamente alle informazioni in Adobe Workfront. Rapporti, calendari e pagine esterne possono essere aggiunti alle dashboard che puoi condividere con altri per una collaborazione ottimale.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: c264c0c96b818934a7c25ed54c7666d2d6c95e54
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Creare un dashboard

<!--Audited: 01/2024-->

Puoi creare dashboard per accedere rapidamente alle informazioni in Adobe Workfront. Rapporti, calendari e pagine esterne possono essere aggiunti alle dashboard che puoi condividere con altri per una collaborazione ottimale.

Per ulteriori informazioni sulle dashboard, consulta [Introduzione alle dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>piano Adobe Workfront</strong></p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Licenza Adobe Workfront*</strong></p> </td> 
   <td> <p>Corrente: Piano </p>
   Oppure
   <p>Nuovo: Standard </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurazioni del livello di accesso</strong> </td> 
   <td> <p>Modificare l’accesso a rapporti, dashboard e calendari</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Otterrai le autorizzazioni di gestione per le dashboard create</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront. Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

Prima di poter aggiungere gli oggetti seguenti a un dashboard, è necessario crearli:

* **Rapporti**: per informazioni sulla creazione di rapporti, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Calendari**: per informazioni sulla creazione di calendari, vedere [Panoramica dei rapporti sul calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

È possibile aggiungere pagine esterne esistenti a un dashboard oppure crearne una dal nuovo dashboard. Per informazioni sulla creazione di pagine esterne, consulta [Incorporare una pagina web esterna in una dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Creare un dashboard

{{step1-to-dashboards}}

1. Clic **Nuovo dashboard**.\
   Viene visualizzata la finestra di dialogo Nuovo dashboard.

1. Specifica quanto segue:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nome</strong></td>
      <td><p>Questo è il nome del dashboard.</p><p>Se non si specifica un nome, per impostazione predefinita il nome del primo report sul dashboard diventa il nome del dashboard.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descrizione (facoltativa)</strong></td>
      <td>Questa è una descrizione del dashboard.</td>
     </tr>
    </tbody>
   </table>

1. Selezionare un layout facendo clic sul pulsante di opzione corrispondente nella parte superiore della **Seleziona layout/ Aggiungi report/ Aggiungi calendari** sezione. Layout in cui verranno visualizzati i report, i calendari o le pagine esterne nel dashboard.

   Il layout a colonna singola è quello predefinito.

   Per informazioni sul layout dei rapporti nei dashboard, consulta [Comprendere come vengono visualizzati i rapporti in un dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. Cercare rapporti, calendari o pagine esterne in **Cerca per nome o tipo ...** e trascinarli nel riquadro di layout, quando vengono visualizzati nell&#39;elenco.

   >[!NOTE]
   >
   >Durante la ricerca di un elemento, la ricerca restituisce uno dei 2.000 rapporti creati più di recente. I nomi dei rapporti che includono caratteri Unicode non vengono restituiti nei risultati della ricerca. Come best practice, evita di includere caratteri unicode durante la denominazione di oggetti in Workfront digitando i nomi anziché copiarli e incollarli da un’altra origine.

   ![Cercare i rapporti](assets/qs-new-dashboard-ui-0722.png)

1. (Facoltativo) Fai clic su **Aggiungi pagina esterna** per aggiungere una nuova pagina esterna al dashboard.

   Per ulteriori informazioni sulla creazione di pagine esterne e sulla loro incorporazione nelle dashboard, consulta [Incorporare una pagina web esterna in una dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Clic **Salva e chiudi**.

   Un timestamp viene visualizzato nell’angolo superiore destro del dashboard. La marca temporale include la data, l’ora e il fuso orario dell’ultimo aggiornamento del dashboard.
