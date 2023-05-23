---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizzazione: calcolo del costo del lavoro straordinario in una visualizzazione Scheda orario"
description: Il lavoro straordinario non viene calcolato per impostazione predefinita in Adobe Workfront, ma puoi creare un rapporto Scheda orario che calcola il lavoro straordinario.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Visualizzazione: consente di calcolare il costo del lavoro straordinario in una visualizzazione Scheda orario

Il lavoro straordinario non viene calcolato per impostazione predefinita in Adobe Workfront, ma puoi creare un rapporto Scheda orario che calcola il lavoro straordinario.

Se l&#39;utente è associato a una tariffa Costo orario nel suo profilo, puoi anche calcolare l&#39;importo del costo per il lavoro straordinario dell&#39;utente.\
Per informazioni sull’associazione degli utenti alle tariffe orarie, consulta l’articolo [Configura le mie impostazioni](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>Nel campo Straordinari che è possibile aggiungere a una visualizzazione Scheda orario in un elenco o in un report vengono visualizzate le informazioni presenti nel campo Straordinari della scheda orario. Queste informazioni vengono aggiornate manualmente da un utente con accesso in modifica alla scheda orario. Per ulteriori informazioni sul campo Straordinari in una scheda orario, consulta l’articolo [Comprendere il layout della scheda orario](../../../timesheets/timesheets/timesheet-layout.md).

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
   <td> <p>Richiesta di modifica di una vista </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Calcolare il costo del lavoro straordinario in una visualizzazione Scheda orario

Per aggiungere una colonna Tempo eccessivo calcolato a una visualizzazione Scheda orario:

1. Vai a un elenco di schede orario o crea un Rapporto Scheda orario.

   Per informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Clic **Personalizza visualizzazione** in un elenco di schede orario.

   Oppure

   Seleziona la **Colonne (visualizzazione)** in un report Scheda orario.

1. Clic **Aggiungi colonna**.
1. Clic **Passa alla modalità testo**.
1. In **Mostra in questa colonna** , fare clic su **Fare clic per modificare il testo**.
1. Copia e incolla il seguente codice in modalità testo nel **Modalità testo** .
   <pre>displayname=Costo lavoro straordinario calcolato<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >Questo calcolo presuppone che l’utente lavori di solito una settimana di 40 ore.

1. Clic **Salva**, quindi assegna un nome alla nuova visualizzazione e fai clic su **Salva visualizzazione** in un elenco di schede orario.

   Oppure

   Clic **Salva e chiudi** in un rapporto Scheda orario.

1. (Facoltativo e condizionale) se stai creando un rapporto Scheda orario, specifica un nome per il rapporto, quindi fai clic su **Salva report**.

   Il costo del lavoro straordinario di ciascun utente viene visualizzato nel **Costo lavoro straordinario calcolato** colonna.

   ![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
