---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Creare una dashboard
description: Potete creare dashboard per accedere rapidamente alle informazioni in Adobe Workfront. Report, calendari e pagine esterne possono essere aggiunti ai dashboard che è possibile condividere con altri utenti per una collaborazione ottimale.
author: Courtney
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 11%

---

# Creare una dashboard

<!--Audited: 01/2025-->

Potete creare dashboard per accedere rapidamente alle informazioni in Adobe Workfront. È possibile aggiungere fino a 25 report, calendari e pagine esterne ai dashboard che è possibile condividere con altri utenti per una collaborazione ottimale.

Per ulteriori informazioni sui dashboard, consulta [Introduzione ai dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
      <p>Standard</p>
      <p>Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard e calendari</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Otterrai le autorizzazioni Gestisci per i dashboard creati</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Per poter aggiungere gli oggetti a un dashboard, è necessario crearli come segue:

* **Report**: per informazioni sulla creazione di report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Calendari**: per informazioni sulla creazione di calendari, vedere [Panoramica dei report del calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

È possibile aggiungere pagine esterne esistenti a un dashboard oppure crearne una dal nuovo dashboard. Per informazioni sulla creazione di pagine esterne, vedere [Incorporare una pagina Web esterna in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Creare una dashboard

{{step1-to-dashboards}}

1. Fai clic su **Nuovo dashboard**.\
   Viene visualizzata la finestra di dialogo Nuovo dashboard.

1. Specificate quanto segue:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nome</strong></td>
      <td><p>Questo è il nome del dashboard. Si consiglia di utilizzare solo caratteri UTF-8 per evitare problemi di compatibilità.</p><p>Se non si specifica un nome, per impostazione predefinita il nome del primo report nel dashboard diventa il nome del dashboard.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descrizione (facoltativa)</strong></td>
      <td>Questa è una descrizione del dashboard.</td>
     </tr>
    </tbody>
   </table>

1. Seleziona un layout facendo clic sul pulsante di scelta corrispondente nella parte superiore della sezione **Seleziona layout/Aggiungi report/Aggiungi calendari**. Layout in cui verranno visualizzati i report, i calendari o le pagine esterne nel dashboard.

   Il layout a colonna singola è quello predefinito.

   Per informazioni sul layout dei report nei dashboard, vedere [Informazioni sulla visualizzazione dei report in un dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. Nella sezione **Report e calendari disponibili**, inizia a digitare il nome di un report, di un calendario o di una pagina esterna nella barra di ricerca, quindi trascina il report, il calendario o la pagina esterna nel riquadro del layout a destra.

   >[!NOTE]
   >
   >Quando si cerca un elemento, la ricerca restituisce uno dei 2.000 report creati più di recente. I nomi dei report che includono caratteri Unicode non vengono restituiti nei risultati di ricerca. Come procedura consigliata, evitate di includere caratteri Unicode durante la denominazione degli oggetti in Workfront digitando i nomi invece di copiare e incollare i nomi da un&#39;altra origine.

   ![Cerca report](assets/unshimmed-dashboard-ui.png)

1. (Facoltativo) Fare clic su **Aggiungi pagina esterna** per aggiungere una nuova pagina esterna al dashboard.

   Per ulteriori informazioni sulla creazione di pagine esterne e sull&#39;incorporamento di tali pagine nei dashboard, vedere [Incorporare una pagina Web esterna in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Fai clic su **Salva e Chiudi**.

   Nell&#39;angolo superiore destro del dashboard viene visualizzato un timestamp. La marca temporale include la data, l&#39;ora e il fuso orario dell&#39;ultimo aggiornamento del dashboard.
