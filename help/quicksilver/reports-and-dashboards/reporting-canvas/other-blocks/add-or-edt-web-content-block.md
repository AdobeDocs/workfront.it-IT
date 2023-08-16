---
product-area: reporting
navigation-topic: other-blocks
title: Aggiungere o modificare un blocco di contenuto web nell’area di lavoro rapporti
description: I blocchi di contenuto web consentono di visualizzare informazioni provenienti da siti web esterni direttamente all’interno del rapporto.
author: Nolan
feature: Reports and Dashboards
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
hidefromtoc: true
hide: true
source-git-commit: a9c36ff874d3272e1d2de70578c420af29b9d44c
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---


# Aggiungere o modificare un blocco di contenuto web nell’area di lavoro rapporti

I blocchi di contenuto web consentono di visualizzare informazioni provenienti da siti web esterni direttamente all’interno del rapporto.

## Prerequisiti

Prima di iniziare, devi iscriverti alla versione beta di Reporting Canvas. Per ulteriori informazioni, consulta [Reporting Canvas beta: panoramica](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Aggiungere o modificare un blocco di contenuto web

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Generazione rapporti**.
1. Clic **Nuovo rapporto**.

   Oppure

   Vai a un rapporto esistente, fai clic su **Altro** icona ![](assets/more-icon-27x15.png) nell’intestazione del rapporto, fai clic su **Modifica**.

1. Sul lato destro dello schermo, sotto **Aggiungi un blocco**, oppure:

   Trascina **Contenuto web** nell’area di lavoro direttamente nella posizione desiderata.

   Oppure

   Fai doppio clic su **Contenuto web** per aggiungere un blocco nella parte superiore dell’area di lavoro.

   >[!TIP]
   >
   >Puoi modificare le dimensioni del blocco dopo averlo posizionato trascinandone le maniglie d’angolo.

1. Clic **Contenuto web senza titolo** nell’intestazione del blocco, digita un titolo per il blocco.
1. Fai clic su **Modifica** icona ![](assets/edit-icon.png) nell’intestazione del blocco.

   ![](assets/web-content-block-header-350x76.png)

1. In **Impostazioni** che si apre, inserisci l’URL completo della pagina che desideri visualizzare (incluso &quot;https://&quot;) nel **URL** campo.

   >[!NOTE]
   >
   >Attualmente, è possibile visualizzare solo i siti di determinati domini. I domini attualmente utilizzabili sono:
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com

   Se non è possibile incorporarlo, viene visualizzato un avviso sotto l’URL immesso. Queste avvertenze includono:

   | Nome avviso | Motivo |
   |---|---|
   | URL non valido | L&#39;URL immesso non restituisce un sito valido. |
   | Limitazioni per il sito del provider | Il sito che stai tentando di incorporare non è consentito. |

   {style="table-layout:auto"}

1. (Facoltativo) Fai clic su **Parametri di passaggio** attiva per aprire un elenco dei parametri di passaggio disponibili.

   >[!WARNING]
   >
   >I parametri di passaggio sono attualmente disabilitati.

1. Clic **URL di incorporamento** per salvare le selezioni e tornare al report.
