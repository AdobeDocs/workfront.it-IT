---
title: Concedere l’accesso a filtri, visualizzazioni e raggruppamenti
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai controlli di filtro, visualizzazione e raggruppamento per elenchi e report.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4fb6eefd-74dd-4941-91d4-0e5f637febf3
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 8%

---

# Concedere l’accesso a filtri, viste e raggruppamenti

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l&#39;accesso di un utente ai controlli di filtro, visualizzazione e raggruppamento per elenchi e report, come descritto in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Per informazioni sui controlli di filtro, visualizzazione e raggruppamento, vedere [Elementi di reporting: filtri, visualizzazioni e raggruppamenti](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare l’accesso degli utenti a filtri, viste e raggruppamenti utilizzando un livello di accesso personalizzato

1. Iniziare a creare o modificare il livello di accesso, come descritto in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull&#39;icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante **Visualizza** o **Modifica** a destra di Filtri, quindi seleziona le funzionalità che desideri concedere in **Ottimizza le impostazioni**.

   ![](assets/gear-icon-filters-dashboards-groupings.png)

   Per impostazione predefinita, gli utenti con una licenza Pianificazione, Lavoro, Revisore o Richiesta dispongono di capacità di visualizzazione e modifica complete. Gli utenti con una licenza per utenti esterni non hanno accesso a filtri, viste e raggruppamenti.

   <!--If this changes, undraft section with table below
   -->

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configura l&#39;accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), ad esempio [Concedi l&#39;accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedi l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fare clic su **Salva**.

   Dopo aver creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--## Access to filters, views, and groupings by license type

Drafting out this section for now because the table is redundant since all four license types can do everything.</span>-->

In questa tabella sono elencati gli elementi che un amministratore di Workfront può consentire agli utenti con ogni tipo di licenza di utilizzare filtri, visualizzazioni e raggruppamenti. Per informazioni sui tipi di licenza di Workfront, vedere [Panoramica sulle licenze di Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<thead>
<tr>
<th> Azione </th>
<th> Pianificatore </th>
<th> Collaboratore </th>
<th> Revisore </th>
<th> Richiedente </th>
</tr>
</thead>
<tbody>
<tr>
<td>Modificare filtri, viste e raggruppamenti</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Creare filtri, viste e raggruppamenti</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Visualizzare filtri, visualizzazioni e raggruppamenti</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Eliminare filtri, viste e raggruppamenti</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Condividere filtri, visualizzazioni e raggruppamenti</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Condividere filtri, visualizzazioni e raggruppamenti a livello di sistema</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
</tbody>
</table>
