---
title: Consentire l’accesso a filtri, visualizzazioni e raggruppamenti
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso dell’utente al filtro, alla visualizzazione e al raggruppamento dei controlli per elenchi e rapporti.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4fb6eefd-74dd-4941-91d4-0e5f637febf3
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 1%

---

# Consentire l’accesso a filtri, visualizzazioni e raggruppamenti

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso dell’utente al filtro, alla visualizzazione e al raggruppamento dei controlli per elenchi e rapporti, come spiegato in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Per informazioni sui controlli filtro, visualizzazione e raggruppamento, consulta [Elementi di reporting: filtri, visualizzazioni e raggruppamenti](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare l’accesso utente a filtri, viste e raggruppamenti utilizzando un livello di accesso personalizzato

1. Inizia a creare o modificare il livello di accesso, come spiegato in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sulla **Visualizza** o **Modifica** a destra di Filtri, quindi seleziona le capacità che desideri concedere in **Ottimizzare le impostazioni**.

   ![](assets/gear-icon-filters-dashboards-groupings.jpg)

   Per impostazione predefinita, gli utenti con una licenza Piano, Lavoro, Revisore o Richiesta dispongono di funzionalità di visualizzazione e modifica complete. Gli utenti con una licenza Utente esterno non possono accedere a filtri, viste e raggruppamenti.

   <!--If this changes, undraft section with table below
   -->

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l’accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), quali [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fai clic su **Salva**.

   Una volta creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--## Access to filters, views, and groupings by license type

Drafting out this section for now because the table is redundant since all four license types can do everything.</span>-->

In questa tabella sono elencate le operazioni che un amministratore di Workfront può eseguire sugli utenti con ogni tipo di licenza per filtrare, visualizzare e raggruppare. Per informazioni sui tipi di licenza Workfront, consulta [Panoramica sulle licenze di Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

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
<td>Modificare filtri, visualizzazioni e raggruppamenti</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Creare filtri, visualizzazioni e raggruppamenti</td>
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
<td>Eliminare filtri, visualizzazioni e raggruppamenti</td>
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
<td>Condivisione di filtri, visualizzazioni e raggruppamenti a livello di sistema</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
</tbody>
</table>
