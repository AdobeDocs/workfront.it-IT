---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Creare un dashboard
description: Puoi creare dashboard per accedere rapidamente alle informazioni in Adobe Workfront. Rapporti, calendari e pagine esterne possono essere aggiunti alle dashboard che puoi condividere con altri per una collaborazione ottimale.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 6e665acd48ce5ee4f870282cbdb59e89c5d21096
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Creare un dashboard

<!--Audited: 01/2025-->

Puoi creare dashboard per accedere rapidamente alle informazioni in Adobe Workfront. È possibile aggiungere ai dashboard fino a 25 rapporti, calendari e pagine esterne da condividere con altri utenti per una collaborazione ottimale.

Per ulteriori informazioni sulle dashboard, vedere [Introduzione alle dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td> <p><strong>Licenza Adobe Workfront</strong></p> </td> 
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

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di poter aggiungere gli oggetti seguenti a un dashboard, è necessario crearli:

* **Report**: per informazioni sulla creazione di report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Calendari**: per informazioni sulla creazione di calendari, vedere [Panoramica sui report calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

È possibile aggiungere pagine esterne esistenti a un dashboard oppure crearne una dal nuovo dashboard. Per informazioni sulla creazione di pagine esterne, vedere [Incorporare una pagina Web esterna in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Creare un dashboard

{{step1-to-dashboards}}

1. Fai clic su **Nuovo dashboard**.\
   Viene visualizzata la finestra di dialogo Nuovo dashboard.

1. Specifica quanto segue:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nome</strong></td>
      <td><p>Questo è il nome del dashboard. Per evitare problemi di compatibilità, si consiglia di utilizzare solo caratteri UTF-8.</p><p>Se non si specifica un nome, per impostazione predefinita il nome del primo report sul dashboard diventa il nome del dashboard.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descrizione (facoltativa)</strong></td>
      <td>Questa è una descrizione del dashboard.</td>
     </tr>
    </tbody>
   </table>

1. Selezionare un layout facendo clic sul pulsante di opzione corrispondente nella parte superiore della sezione **Seleziona layout/ Aggiungi report/ Aggiungi calendari**. Layout in cui verranno visualizzati i report, i calendari o le pagine esterne nel dashboard.

   Il layout a colonna singola è quello predefinito.

   Per informazioni sul layout dei report nei dashboard, vedere [Informazioni sulla visualizzazione dei report in un dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. Nella sezione **Report e calendari disponibili**, inizia a digitare il nome di un report, di un calendario o di una pagina esterna nella barra di ricerca, quindi trascina e rilascia il report, il calendario o la pagina esterna nel riquadro di layout a destra.

   >[!NOTE]
   >
   >Durante la ricerca di un elemento, la ricerca restituisce uno dei 2.000 rapporti creati più di recente. I nomi dei rapporti che includono caratteri Unicode non vengono restituiti nei risultati della ricerca. Come best practice, evita di includere caratteri unicode durante la denominazione di oggetti in Workfront digitando i nomi anziché copiarli e incollarli da un’altra origine.

   ![Cerca i report](assets/unshimmed-dashboard-ui.png)

1. (Facoltativo) Fai clic su **Aggiungi pagina esterna** per aggiungere una nuova pagina esterna al dashboard.

   Per ulteriori informazioni sulla creazione di pagine esterne e sull&#39;incorporamento delle stesse nei dashboard, vedere [Incorporare una pagina Web esterna in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Fai clic su **Salva e Chiudi**.

   Un timestamp viene visualizzato nell’angolo superiore destro del dashboard. La marca temporale include la data, l’ora e il fuso orario dell’ultimo aggiornamento del dashboard.
