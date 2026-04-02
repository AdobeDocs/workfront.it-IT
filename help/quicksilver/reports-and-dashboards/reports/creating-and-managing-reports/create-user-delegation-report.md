---
product-area: reporting
keywords: utente,delega,report,delegato,approvazione
navigation-topic: create-and-manage-reports
title: Creare un rapporto di delega utente
description: Creare un rapporto di delega utente
author: Courtney
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 17%

---

# Creare un rapporto di delega utente

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

In Adobe Workfront, gli utenti possono delegare le approvazioni di progetti, attività e problemi ad altri utenti per assicurarsi che le loro approvazioni siano gestite quando sono fuori sede. Gli utenti con una licenza Pianificazione possono creare un report Delega utenti per visualizzare:

* Chi ha delegato le proprie approvazioni di attività, problemi e progetti a un altro utente
* Quali utenti hanno delegato le approvazioni di attività, problemi e progetti loro assegnate

* Le date di inizio e di fine delle delegazioni

Per ulteriori informazioni sulla delega delle approvazioni, vedere [Delegare la richiesta di approvazione](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
      <p>Standard</p>
      <p>Piano</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
 <td> <p>Visualizzare le autorizzazioni per gli elementi le cui approvazioni sono delegate e per gli utenti coinvolti nella delega</p></td>  
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un rapporto di delega utente

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Reports**.

1. Fai clic su **Nuovo report**, quindi seleziona **Delega utente**.

   ![Nuova delega utente report](assets/classic-new-report-user-delegation-350x644.png)

   I campi seguenti vengono visualizzati in questo rapporto per impostazione predefinita:

   | Campo | Descrizione |
   |---|---|
   | **Dall&#39;utente** | Questo è l’utente che delega le proprie approvazioni di attività, problemi e progetti a un altro utente. |
   | **All&#39;Utente** | Questo è l’utente al quale sono delegate le approvazioni di attività, problemi e progetti. |
   | **Data inizio** | Questo è l&#39;inizio del periodo di fuori sede per l&#39;utente che ha effettuato le deleghe. |
   | **Data di fine** | Questo è il termine del tempo fuori sede per l&#39;utente che ha effettuato le deleghe. |

   {style="table-layout:auto"}

1. (Facoltativo) Nel generatore di report, modifica quanto segue:

   * Colonne (Visualizzazione)
   * Raggruppamenti
   * Filtri
   * Diagramma

   Per ulteriori informazioni su queste caratteristiche, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Dopo aver completato la creazione del report, fai clic su **Salva + Chiudi**.

   Viene visualizzato il rapporto.
