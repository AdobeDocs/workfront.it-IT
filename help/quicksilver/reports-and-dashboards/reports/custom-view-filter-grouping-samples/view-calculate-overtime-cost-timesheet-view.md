---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: calcolare il costo del lavoro straordinario in una visualizzazione scheda attività"'
description: Per impostazione predefinita, in Adobe Workfront non vengono calcolati gli straordinari, ma è possibile creare un rapporto Scheda attività che calcoli gli straordinari.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Visualizza: calcolare il costo del lavoro straordinario in una visualizzazione scheda attività

Per impostazione predefinita, in Adobe Workfront non vengono calcolati gli straordinari, ma è possibile creare un rapporto Scheda attività che calcoli gli straordinari.

Se l’utente è associato a un tasso di costo per ora nel suo profilo, puoi anche calcolare l’importo del costo per il lavoro straordinario di quell’utente.\
Per informazioni sull&#39;associazione degli utenti ai tassi di costo per ora, consulta l&#39;articolo [Configurare le impostazioni personali](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>Il campo Lavoro straordinario che è possibile aggiungere a una visualizzazione Scheda attività in un elenco o in un rapporto visualizza le informazioni presenti nel campo Lavoro straordinario della scheda attività. Queste informazioni vengono aggiornate manualmente da un utente con accesso per modificare la scheda attività. Per ulteriori informazioni sul campo Lavoro straordinario in una scheda attività, vedere l&#39;articolo [Comprendere il layout del foglio presenze](../../../timesheets/timesheets/timesheet-layout.md).

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

## Calcolare il costo del lavoro straordinario in una visualizzazione Scheda attività

Per aggiungere una colonna Calcolata per il lavoro straordinario a una visualizzazione scheda attività:

1. Passare a un elenco di fogli presenze o creare un rapporto Scheda attività.

   Per informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Fai clic su **Personalizza visualizzazione** in un elenco di fogli presenze.

   Oppure

   Seleziona la **Colonne (visualizzazione)** scheda in un report Scheda attività.

1. Fai clic su **Aggiungi colonna**.
1. Fai clic su **Passa alla modalità testo**.
1. In **Mostra in questa colonna** area, fai clic su **Fare clic per modificare il testo**.
1. Copia e incolla il seguente codice della modalità testo nel **Modalità testo** finestra di dialogo.
   <pre>displayname=Costo straordinario calcolato<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >Questo calcolo presuppone che l’utente di solito lavori per una settimana di 40 ore.

1. Fai clic su **Salva**, quindi assegna un nome alla nuova visualizzazione e fai clic su **Salva visualizzazione** in un elenco di fogli presenze.

   Oppure

   Fai clic su **Salva e chiudi** in un rapporto Scheda attività.

1. (Facoltativo e condizionale) se si sta creando un rapporto Scheda attività, specificare un nome per il rapporto, quindi fare clic su **Salva rapporto**.

   Il costo dello straordinario di ogni utente viene visualizzato nella **Costo straordinario calcolato** colonna.

   ![calculate_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
