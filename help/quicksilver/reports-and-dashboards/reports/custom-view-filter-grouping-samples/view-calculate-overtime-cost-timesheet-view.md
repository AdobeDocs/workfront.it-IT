---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizzazione: calcolo del costo del lavoro straordinario in una visualizzazione Scheda orario'
description: Il lavoro straordinario non viene calcolato per impostazione predefinita in Adobe Workfront, ma puoi creare un rapporto Scheda orario che calcola il lavoro straordinario.
author: Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Visualizzazione: consente di calcolare il costo del lavoro straordinario in una visualizzazione Scheda orario

<!--Audited: 11/2024-->

Il lavoro straordinario non viene calcolato per impostazione predefinita in Adobe Workfront, ma puoi creare un rapporto Scheda orario che calcola il lavoro straordinario.

Se l&#39;utente è associato a una tariffa Costo orario nel suo profilo, puoi anche calcolare l&#39;importo del costo per il lavoro straordinario dell&#39;utente.\
Per informazioni sull&#39;associazione degli utenti alle tariffe orarie, vedere l&#39;articolo [Configurazione delle impostazioni personali](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>Nel campo Straordinari che è possibile aggiungere a una visualizzazione Scheda orario in un elenco o in un report vengono visualizzate le informazioni presenti nel campo Straordinari della scheda orario. Queste informazioni vengono aggiornate manualmente da un utente con accesso in modifica alla scheda orario. Per ulteriori informazioni sul campo Straordinari in una scheda orario, vedere l&#39;articolo [Panoramica del layout della scheda orario](../../../timesheets/timesheets/timesheet-layout.md).

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Calcolare il costo del lavoro straordinario in una visualizzazione Scheda orario

Per aggiungere una colonna Tempo eccessivo calcolato a una visualizzazione Scheda orario:

1. Vai a un elenco di schede orario.

1. Fai clic sul menu a discesa **Visualizza**, quindi fai clic su **Nuova visualizzazione**.

1. Fai clic su **Aggiungi colonna**.
1. Fare clic su **Passa alla modalità testo**, quindi su **Modifica modalità testo**.
1. Nella casella **Modifica modalità testo** rimuovere il testo nella casella, quindi copiare e incollare il codice della modalità testo seguente:

   ```
   displayname=Calculated Overtime Cost
   linkedname=direct
   namekey=totalHours
   querysort=totalHours 
   textmode=true
   valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})
   valueformat=currencyStringCurrencyRounded
   ```

   >[!NOTE]
   >
   >Questo calcolo presuppone che l’utente lavori di solito una settimana di 40 ore.

1. Fai clic su **Fine**, quindi denomina la nuova visualizzazione e fai clic su **Salva visualizzazione** in un elenco di schede orario.

   Il costo del lavoro straordinario di ciascun utente viene visualizzato nella colonna **Costo lavoro straordinario calcolato**.


