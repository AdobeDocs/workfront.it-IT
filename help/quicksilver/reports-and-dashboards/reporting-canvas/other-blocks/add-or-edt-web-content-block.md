---
product-area: reporting
navigation-topic: other-blocks
title: Aggiungere o modificare un blocco di contenuto web in Reporting Canvas
description: I blocchi di contenuto web ti consentono di visualizzare informazioni da siti web esterni direttamente all’interno del rapporto.
author: Nolan
feature: Reports and Dashboards
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 2%

---


# Aggiungere o modificare un blocco di contenuto web in Reporting Canvas

I blocchi di contenuto web ti consentono di visualizzare informazioni da siti web esterni direttamente all’interno del rapporto.

## Prerequisiti

Prima di iniziare, è necessario iscriversi alla versione beta di Reporting Canvas. Per ulteriori informazioni, consulta [Reporting Canvas beta: panoramica](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Aggiungere o modificare un blocco di contenuto web

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Reporting**.
1. Fai clic su **Nuovo rapporto**.

   Oppure

   Passa a un rapporto esistente e fai clic sul pulsante **Altro** icona ![](assets/more-icon-27x15.png) nell’intestazione del rapporto, quindi fai clic su **Modifica**.

1. Sul lato destro dello schermo, sotto **Aggiungi un blocco** oppure

   Trascina **Contenuto web** sull’area di lavoro direttamente nella posizione desiderata.

   Oppure

   Fai doppio clic sul pulsante **Contenuto web** per aggiungere un blocco all’inizio dell’area di lavoro.

   >[!TIP]
   >
   >È possibile modificare le dimensioni del blocco dopo averlo posizionato trascinandone le maniglie d’angolo.

1. Fai clic su **Contenuto web senza titolo** nell’intestazione del blocco , digita un titolo per il blocco .
1. Fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png) nell’intestazione del blocco .

   ![](assets/web-content-block-header-350x76.png)

1. In **Impostazioni** nel pannello che si apre, immetti l’URL completo per la pagina da visualizzare (incluso &quot;https://&quot;) nel **URL** campo .

   >[!NOTE]
   >
   >Al momento, è possibile visualizzare solo i siti da domini selezionati. I domini attualmente utilizzabili sono:
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com


   Un avviso viene visualizzato sotto l’URL immesso se non è possibile incorporarlo. Questi avvisi includono:

   | Nome avviso | Motivo |
   |---|---|
   | URL non valido | L&#39;URL immesso non restituisce un sito valido. |
   | Restrizioni al sito del fornitore | Il sito che si sta tentando di incorporare non è consentito. |

   {style=&quot;table-layout:auto&quot;}

1. (Facoltativo) Fai clic sul pulsante **Passa parametri** per aprire un elenco dei parametri di passaggio disponibili.

   >[!WARNING]
   >
   >I parametri di passaggio sono attualmente disabilitati.

1. Fai clic su **URL di incorporamento** per salvare le selezioni e tornare al rapporto.
