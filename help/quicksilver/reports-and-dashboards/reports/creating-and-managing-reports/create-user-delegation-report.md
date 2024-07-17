---
product-area: reporting
keywords: utente,delega,report,delegato,approvazione
navigation-topic: create-and-manage-reports
title: Creare un rapporto di delega utente
description: Creare un rapporto di delega utente
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 1%

---

# Creare un rapporto di delega utente

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per gli elementi le cui approvazioni sono delegate e per gli utenti coinvolti nella delega</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Creare un rapporto di delega utente

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Rapporti**.

1. Fai clic su **Nuovo report**, quindi seleziona **Delega utente**.\
   ![](assets/classic-new-report-user-delegation-350x644.png)

   I campi seguenti vengono visualizzati in questo rapporto per impostazione predefinita:

   | Campo | Descrizione |
   |---|---|
   | **Dall&#39;utente** | Questo è l’utente che delega le proprie approvazioni di attività, problemi e progetti a un altro utente. |
   | **All&#39;Utente** | Questo è l’utente al quale sono delegate le approvazioni di attività, problemi e progetti. |
   | **Inizio** | Questo è l&#39;inizio del periodo di fuori sede per l&#39;utente che ha effettuato le deleghe. |
   | **Fine** | Questo è il termine del tempo fuori sede per l&#39;utente che ha effettuato le deleghe. |

   {style="table-layout:auto"}

1. (Facoltativo) Nel generatore di report, modifica quanto segue:

   * Colonne
   * Raggruppamenti
   * Filtri
   * Diagramma

   Per ulteriori informazioni su queste caratteristiche, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Dopo aver completato la creazione del report, fai clic su **Salva + Chiudi**.

1. Immetti un nuovo nome nel campo **Nome report**, quindi fai clic su **Salva report**.

   Viene visualizzato il rapporto.
