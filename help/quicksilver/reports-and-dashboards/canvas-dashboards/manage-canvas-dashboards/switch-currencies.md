---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Utilizzare i campi di valuta nei dashboard di Canvas
description: È possibile utilizzare i campi della valuta in un dashboard Area di lavoro.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 3e4ab2dfc66efd262c0c2ad30a9c62758084f8ce
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 4%

---


# Utilizzare i campi di valuta nei dashboard di Canvas

>[!IMPORTANT]
>
>La funzione Dashboard di Canvas è attualmente disponibile solo per gli utenti che partecipano alla fase beta. Alcune parti della caratteristica potrebbero non essere complete o non funzionare come previsto in questa fase. Invia un feedback relativo alla tua esperienza seguendo le istruzioni riportate nella sezione [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) dell&#39;articolo di panoramica della versione beta di Canvas Dashboards.<br>
>In caso di feedback su un possibile bug o problema tecnico, invia un ticket al supporto Workfront. Per ulteriori informazioni, vedere [Contattare l&#39;Assistenza clienti](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tieni presente che questa versione beta non è disponibile sui seguenti provider cloud:
>
>* Porta la tua chiave per Amazon Web Services
>* Azure
>* Piattaforma Google Cloud

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
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td> 
<p>Standard</p> 
<p>Piano</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td> 
   <td><p>Modificare l’accesso a rapporti, dashboard e calendari</p>
   <p>Visualizza accesso ai dati finanziari</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td><p>Gestire le autorizzazioni per il dashboard</p>
  </td> 
  </tr> 
</tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Prerequisiti

1. Per utilizzare le funzionalità descritte in questo articolo, nell’istanza di Workfront devono essere impostati più tipi di valuta. Per ulteriori informazioni, vedere [Impostare i tassi di cambio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   >[!IMPORTANT]
   >
   >La funzionalità descritta in questo articolo si applica solo ai campi della valuta nativa. Il supporto per i campi di valuta personalizzati sarà presto disponibile.


## Impostare una valuta predefinita per un dashboard Area di lavoro

Durante la creazione di un dashboard di Canvas, è possibile impostare una valuta predefinita per il dashboard. Questa valuta verrà utilizzata per visualizzare tutti i campi della valuta nativa nei report nel dashboard, a meno che il campo della valuta non sia bloccato a livello di report.

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.

1. Fai clic su **Nuovo dashboard** nell&#39;angolo in alto a destra.

1. Nella casella **Crea dashboard**,

1. Specifica quanto segue:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nome</strong></td>
      <td><p>Immetti un nome per il dashboard. Per evitare problemi di compatibilità, si consiglia di utilizzare solo caratteri UTF-8.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descrizione (facoltativa)</strong></td>
      <td>Immetti una descrizione del dashboard.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>Valuta</strong></td>
      <td>Scegliere il tipo di valuta predefinito per il dashboard. <br>
      <br>Gli utenti possono passare da un tipo di valuta all'altro quando filtrano il dashboard.</td>
     </tr>
    </tbody>
   </table>


## Passare da una valuta all’altra in un dashboard di Canvas

A livello di dashboard è possibile passare da un tipo di valuta all’altro. I rapporti che contengono campi di valuta verranno aggiornati per riflettere il tipo di valuta selezionato.

I campi Valuta possono essere bloccati a livello di report. Se un campo valuta è bloccato, il tipo di valuta per il report non verrà modificato quando si modifica il tipo di valuta per il dashboard.

Per modificare il tipo di valuta per il dashboard:

1. Fai clic sul menu a discesa della valuta nell’angolo superiore destro della pagina dei dettagli della dashboard.
1. Selezionare il tipo di valuta desiderato dall&#39;elenco.

   ![elenco a discesa cambio valuta](assets/filter-by-currency.png)


## Limitazioni

La tabella seguente illustra le limitazioni relative alle valute definite nell&#39;area Tassi di cambio in Configurazione.

<table> 
<tr>
<td></td>
<td>Gli utenti possono</td>
<td>Gli utenti non possono</td>
</tr>
<tr> 
<td>Definizione della moneta unica</td>
<td>
<ul>
<li>Utilizzare i campi della valuta nativa nei report di grafici, indicatori KPI e tabelle dell'area di lavoro</li>
<li>Utilizzare campi di valuta personalizzati nei report grafico, KPI e grafico dell’area di lavoro</li>
</ul>
</td>
<td>
<ul>
<li>Assegna una valuta predefinita al dashboard (al momento della creazione o della modifica del dashboard)</li>
<li>Visualizzare e utilizzare l’interruttore della valuta a livello di dashboard</li>
<li>Blocca una valuta specifica per la visualizzazione in un grafico a quadro, in un indicatore KPI o in un rapporto di tabella</li>
<li>Utilizzare i campi della valuta di Planning in un grafico a quadro, in un indicatore KPI e in rapporti di tabella</li>
</ul>
</td> 
</tr>
</td> 
</tr> 
<tr>
<td>Sono definite più valute</td>
<td>
<ul>
  <li>Utilizzare i campi della valuta nativa nei report di grafici, indicatori KPI e tabelle dell'area di lavoro</li>
  <li>Imposta una valuta predefinita per il dashboard (durante la creazione o la modifica del dashboard)</li>
  <li>Visualizzare e utilizzare l’interruttore della valuta a livello di dashboard</li>
  <li>Blocca una valuta specifica per la visualizzazione in un rapporto di grafico, indicatore KPI o tabella per ignorare la preferenza di attivazione/disattivazione della valuta nel dashboard</li>
</ul>
</td>
<td><ul>
  <li>Utilizzare campi di valuta dei dati personalizzati nei rapporti di grafico, KPI e tabella dell’area di lavoro</li>
  <li>Utilizzare i campi della valuta di Planning in un grafico a quadro, in un indicatore KPI e in rapporti di tabella</li>
</ul>
</td>
</tr></table>





