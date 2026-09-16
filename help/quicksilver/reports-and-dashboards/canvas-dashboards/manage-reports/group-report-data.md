---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Raggruppare i dati dei rapporti in un dashboard Area di lavoro
description: Organizzare i risultati del rapporto in gruppi. Il raggruppamento funziona in modo diverso a seconda del tipo di rapporto.
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 375d62fc12af075c2224f979d3ef87cdffdf03ea
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 13%
---
# Raggruppare i dati dei rapporti in un dashboard Area di lavoro

>[!IMPORTANT]
>
>La funzione Dashboard di Canvas è attualmente disponibile solo per gli utenti che partecipano alla fase beta. Alcune parti della caratteristica potrebbero non essere complete o non funzionare come previsto in questa fase. Invia un feedback relativo alla tua esperienza seguendo le istruzioni riportate nella sezione [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) dell&#39;articolo di panoramica di Canvas Dashboards beta.<br>
>In caso di feedback su un possibile bug o problema tecnico, invia un ticket al supporto Workfront. Per ulteriori informazioni, consulta [Contattare l’Assistenza clienti](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tieni presente che questa versione beta non è disponibile sui seguenti provider cloud:
>
>* Porta la tua chiave per Amazon Web Services
>* Azure
>* Piattaforma Google Cloud

Il raggruppamento organizza i risultati del rapporto in modo che i record correlati vengano visualizzati insieme. Il funzionamento del raggruppamento dipende dal tipo di rapporto, pertanto questo articolo ha una sezione separata per ciascuno di essi.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td> 
<p>Standard</p> 
<p>Piano</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td> 
   <td><p>Modificare l’accesso a rapporti, dashboard e calendari</p>
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td><p>Gestire le autorizzazioni per il dashboard</p>
  </td> 
  </tr>
</tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Prerequisiti

Prima di poter raggruppare i dati di un dashboard, è necessario disporre di un report su un dashboard o crearne uno. Per ulteriori informazioni, vedere [Creare un dashboard Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Raggruppare le righe in un rapporto di tabella

In un rapporto di tabella, il raggruppamento organizza le righe del rapporto stesso.

1. Nella finestra di dialogo **Configura**, fai clic sull&#39;icona **Impostazioni gruppo** nel pannello a sinistra.

1. Fai clic su **Aggiungi raggruppamento**, quindi seleziona il campo in base al quale desideri eseguire il raggruppamento. Il raggruppamento viene visualizzato nell’anteprima a destra.

1. (Facoltativo) Ripeti per aggiungere altri raggruppamenti.

## Configurare i raggruppamenti di espansione nei rapporti grafico e KPI

Nei rapporti con grafici e KPI non puoi raggruppare la visualizzazione principale. Puoi invece configurare il modo in cui la tabella di espansione viene raggruppata quando un visualizzatore esegue il drill-down in un valore.

1. Nella finestra di dialogo **Configura**, fai clic sull&#39;icona **Impostazioni gruppo di espansione** nel pannello a sinistra.

1. Fai clic su **Aggiungi raggruppamento**, quindi seleziona il campo in base al quale raggruppare la tabella di espansione.

## Configurare i segmenti in un rapporto di tabella pivot

I rapporti di tabella pivot non utilizzano i raggruppamenti. Invece, puoi definire fino a due segmenti, che sono le categorie in base alle quali vengono raggruppate e totalizzate le metriche del pivot.

1. Nella finestra di dialogo **Configura**, fai clic sull&#39;icona **Segmenti** nel pannello a sinistra.

1. Fai clic su **Aggiungi segmento**, quindi seleziona il campo desiderato. Il segmento viene visualizzato come colonna nell’anteprima.

1. Ripeti per aggiungere un secondo segmento (facoltativo). Puoi aggiungere un massimo di due segmenti.

## Visualizzare dati raggruppati su un dashboard

I visualizzatori di report possono espandere, comprimere e ordinare dati raggruppati. Per ulteriori informazioni, vedere [Visualizzare report con dati raggruppati](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md#view-reports-with-grouped-data) in [Utilizzare dashboard di Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).
