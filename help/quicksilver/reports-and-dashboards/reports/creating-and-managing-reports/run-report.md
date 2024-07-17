---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Eseguire un rapporto
description: Puoi eseguire qualsiasi rapporto a cui hai accesso.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---


# Eseguire un rapporto

Puoi eseguire qualsiasi rapporto a cui hai accesso.

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
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso a report, dashboard e calendari</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Eseguire un rapporto

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Rapporti**.

1. Selezionare una delle opzioni seguenti:

   * **I miei report:** report creati.
   * **Condiviso con me:** report condivisi da altri utenti con te.
   * **Tutti i report:** Tutti i report nel sistema a cui hai accesso.

1. Fare clic sul nome del report che si desidera eseguire.\
   Oppure\
   Se il report è stato creato utilizzando i prompt, selezionare le informazioni appropriate dai menu a discesa, quindi fare clic su **Esegui report**.\
   Per ulteriori informazioni sui prompt, vedere [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   Il contenuto del report viene visualizzato con una marca temporale nell’angolo superiore destro del report, che include la data, l’ora e il fuso orario in cui il report è stato eseguito dal contesto dell’utente che ha eseguito il report.

1. (Facoltativo) Fai clic sull&#39;icona **Ricarica** ![](assets/qs-report-refresh-icon.png) per aggiornare i risultati in un report se il report è stato visualizzato nel browser per un po&#39;.

1. (Condizionale) Se il report utilizza filtri o prompt, fare clic su **Mostra filtri e prompt** per visualizzare un elenco di filtri e prompt utilizzati nel report visualizzato. Se il report contiene solo filtri o solo prompt, verrà visualizzato **Mostra filtri** o **Mostra prompt**.

   ![Mostra filtri e prompt](assets/qs-reports-showfiltersandprompts-2022-350x136.png)

   Le informazioni vengono visualizzate sotto il nome del rapporto sul lato sinistro della pagina. Per i prompt, si tratta di informazioni sulle selezioni effettuate al momento dell&#39;esecuzione del report, come descritto nel passaggio 4.

1. Se si utilizzano i prompt personalizzati, non vengono visualizzati. Vengono visualizzati solo i prompt di sistema. I filtri personalizzati vengono sempre visualizzati.

## Visualizzare un rapporto memorizzato nella cache

Il report potrebbe essere memorizzato nella cache se è stato visualizzato nel browser per un po’. Puoi forzare il ricaricamento di un rapporto memorizzato nella cache quando esegui una delle seguenti azioni:

* Modifica le impostazioni del rapporto e salva il rapporto.
* Modificare la visualizzazione, il gruppo o il filtro.
* Fai clic sull&#39;icona **Ricarica**
Questa opzione è disponibile nell&#39;angolo superiore destro della pagina all&#39;interno della finestra di messaggio che indica l&#39;ora in cui il report è stato salvato oppure è disponibile nell&#39;angolo superiore destro del dashboard in cui è posizionato il report. Per ulteriori informazioni sul ricaricamento dei dashboard, vedere la sezione &quot;Dashboard di visualizzazione&quot; nell&#39;articolo [Introduzione ai dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* Accedere a qualsiasi pagina del report oltre la prima pagina passando alle schede Riepilogo, Matrice o Grafico.
