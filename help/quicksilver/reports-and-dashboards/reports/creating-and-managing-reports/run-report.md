---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Eseguire un rapporto
description: Puoi eseguire qualsiasi rapporto a cui hai accesso in Visualizza.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---


# Eseguire un rapporto

Puoi eseguire qualsiasi rapporto a cui hai accesso in Visualizza.

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>Accesso a Report, Dashboard, Calendari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per un report</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Eseguire un rapporto

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Rapporti**.

1. Seleziona tra le seguenti opzioni:

   * **Rapporti personali:** Report creati dall&#39;utente.
   * **Condiviso con me:** Report condivisi da altri utenti con te.
   * **Tutti i rapporti:** Tutti i report nel sistema a cui hai accesso.

1. Fare clic sul nome del rapporto che si desidera eseguire.\
   Oppure\
   Se il rapporto è stato creato utilizzando i prompt, seleziona le informazioni appropriate dai menu a discesa, quindi fai clic su **Esegui rapporto**.\
   Per ulteriori informazioni sui prompt, vedi [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   Il contenuto del rapporto viene visualizzato con una marca temporale nell’angolo in alto a destra del rapporto che include la data, l’ora e il fuso orario in cui il rapporto è stato eseguito dal contesto dell’utente che ha eseguito il rapporto.

1. (Facoltativo) Fai clic sul pulsante **Icona Ricarica** ![](assets/qs-report-refresh-icon.png) per aggiornare i risultati in un report se il report è stato visualizzato nel browser per un po&#39;.

1. (Condizionale) Se il rapporto utilizza filtri o prompt, fai clic su **Mostra filtri e prompt** per visualizzare un elenco di filtri e prompt utilizzati nel rapporto che stai visualizzando. Se il rapporto contiene solo filtri o solo prompt, **Mostra filtri** o **Mostra prompt** viene invece visualizzato.

   ![Mostra filtri e prompt](assets/qs-reports-showfiltersandprompts-2022-350x136.png)

   Le informazioni vengono visualizzate sotto il nome del rapporto sul lato sinistro della pagina. Per i prompt, si tratta di informazioni sulle selezioni dei prompt effettuate al momento dell&#39;esecuzione del report, come descritto nel passaggio 4.

1. Se utilizzi i prompt personalizzati, questi non vengono visualizzati. Vengono visualizzati solo i prompt del sistema. I filtri personalizzati vengono sempre visualizzati.

## Visualizzare un rapporto nella cache

Il rapporto potrebbe essere memorizzato nella cache se viene visualizzato nel browser da un po&#39; di tempo. È possibile forzare il ricaricamento di un rapporto memorizzato nella cache quando si esegue una delle seguenti operazioni:

* Modificare le impostazioni del rapporto e salvarlo.
* Modificare la visualizzazione, il gruppo o il filtro.
* Fai clic sul pulsante **Icona Ricarica**
Questa opzione è disponibile nell’angolo in alto a destra della pagina all’interno della finestra di messaggio che indica il momento in cui il rapporto è stato salvato o nell’angolo in alto a destra del dashboard in cui è posizionato il rapporto. Per ulteriori informazioni sul ricaricamento delle dashboard, consulta la sezione &quot;Display Dashboards&quot; nell’articolo [Guida introduttiva alle dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* Accedi a qualsiasi pagina del report oltre la prima pagina passando alle schede Riepilogo, Matrice o Grafico.
