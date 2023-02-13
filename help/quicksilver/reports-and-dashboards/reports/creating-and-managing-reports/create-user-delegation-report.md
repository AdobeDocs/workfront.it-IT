---
product-area: reporting
keywords: utente, delega, rapporto, delegato, approvazione
navigation-topic: create-and-manage-reports
title: Creare un rapporto Delega utenti
description: Creare un rapporto Delega utenti
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 4%

---

# Creare un rapporto Delega utenti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

In Adobe Workfront, gli utenti possono delegare progetti, attività e approvazioni ad altri utenti per assicurarsi che le loro approvazioni siano gestite quando non sono in ufficio. Gli utenti con una licenza Piano possono creare un rapporto Delega utenti per visualizzare:

* Chi ha delegato attività, problemi e approvazioni dei progetti a un altro utente
* A quali utenti sono stati assegnati task, problemi e approvazioni di progetto delegati?

* Le date di inizio e di fine delle delegazioni

Per ulteriori informazioni sulla delega delle approvazioni, consulta [Delega richiesta di approvazione](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

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
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza le autorizzazioni per gli elementi di cui sono delegate le approvazioni e per gli utenti coinvolti nella delega</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare un rapporto di delega degli utenti

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Rapporti**.

1. Fai clic su **Nuovo rapporto**, quindi seleziona **Delega utenti**.\
   ![](assets/classic-new-report-user-delegation-350x644.png)

   Per impostazione predefinita, in questo rapporto vengono visualizzati i campi seguenti:

   | Campo | Descrizione |
   |---|---|
   | **Da Utente** | Questo è l’utente che delega le proprie attività, i propri problemi e le approvazioni dei progetti a un altro utente. |
   | **A Utente** | Utente a cui sono state delegate attività, problemi e approvazioni di progetti. |
   | **Inizio** | Questo è l&#39;inizio del tempo fuori servizio per l&#39;utente che ha fatto le delegazioni. |
   | **Fine** | Questa è la fine del tempo fuori servizio per l&#39;utente che ha fatto le delegazioni. |

   {style=&quot;table-layout:auto&quot;}

1. (Facoltativo) Nel generatore di report, modifica quanto segue:

   * Colonne
   * Raggruppamenti
   * Filtri
   * Diagramma

   Per ulteriori informazioni su queste funzioni, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Dopo aver completato la creazione del rapporto, fai clic su **Salva e chiudi**.

1. Immetti un nuovo nome nella **Nome del rapporto** campo , quindi fai clic su **Salva rapporto**.

   Viene visualizzato il rapporto .
