---
title: Visualizzare ed esportare i registri di controllo
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Puoi visualizzare tutti i registri di audit nel sistema o quelli che soddisfano determinati criteri di filtro. Puoi anche esportare i registri di audit. I registri di controllo elencano le modifiche utente attivate nel sistema negli ultimi 90 giorni.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 1%

---

# Visualizzare ed esportare i registri di audit

<!--Audited: 08/2025-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Puoi visualizzare tutti i registri di audit nel sistema o quelli che soddisfano determinati criteri di filtro. Puoi anche esportare i registri di controllo in un file CSV.

I registri di controllo elencano le modifiche utente attivate nel sistema negli ultimi 90 giorni.

Per informazioni su tutti i tipi di log di controllo e su cosa li genera, vedere [Panoramica dei log di controllo](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td><p>Amministratore di Sistema</p></td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>System Administrator</p></td>
  </tr> 
 </tbody> 
</table>-->

## Visualizzare i registri di audit

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Sistema > Registri di controllo**.
1. Nel menu a discesa **Tipo azione**, seleziona il tipo di controllo che desideri visualizzare.

   >[!NOTE]
   >
   >Le opzioni nel menu a discesa Tipo di azione variano a seconda del registro di controllo selezionato.

1. Nel menu a discesa **Tipo di registro**, selezionare il tipo di registro di controllo che si desidera visualizzare.

   **Tutti i tipi di registro** sono selezionati per impostazione predefinita.

   Per un elenco di tutti i tipi di log di controllo visualizzabili e delle informazioni che includono, vedere [Panoramica dei log di controllo](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Facoltativo) Imposta uno dei filtri disponibili per i campi seguenti:

   * **Utenti**: digitare il nome dell&#39;utente che ha apportato una modifica.
   * **Da**: data di inizio dell&#39;intervallo di tempo in cui è stata apportata la modifica.
   * **A**: data di fine dell&#39;intervallo di tempo in cui è stata apportata la modifica.

   ![Registri di controllo](assets/audit-logs.png)

1. Fare clic su **Applica**.
1. (Facoltativo) Fai clic su **Cancella** per ripristinare le modifiche apportate ai filtri.

## Esportare i registri di audit

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Sistema** > **Registri di controllo**.

1. Nel menu a discesa **Log Type**, selezionare un log di controllo.

   **Tutti i tipi di registro** sono selezionati per impostazione predefinita.

1. Imposta uno dei filtri disponibili, quindi fai clic su **Applica**.

   >[!IMPORTANT]
   >
   >Non puoi esportare più di 50.000 registri contemporaneamente. Workfront esporta i registri in base ai filtri impostati, non al numero di registri visualizzati nella pagina. Puoi visualizzare il numero totale di registri filtrati nell’angolo in basso a destra della pagina.

1. Fai clic su **Esporta**.

   Viene visualizzata la casella Salva file (Save file), che consente di salvare il file esportato sul computer.

   Puoi salvare i registri di controllo solo in formato CSV.

   Completate il salvataggio del file esportato. Ora è possibile trovarlo nel computer e condividerlo con altri utenti.
