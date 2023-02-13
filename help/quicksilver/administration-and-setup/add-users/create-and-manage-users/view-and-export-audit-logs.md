---
title: Visualizzare ed esportare i registri di controllo
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Puoi visualizzare tutti i registri di controllo nel sistema o quelli che soddisfano determinati criteri di filtro. Puoi anche esportare i registri di controllo. I registri di controllo elencano le modifiche utente attivate nel sistema durante gli ultimi 90 giorni.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Visualizzare ed esportare i registri di controllo

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Puoi visualizzare tutti i registri di controllo nel sistema o quelli che soddisfano determinati criteri di filtro. Puoi anche esportare i registri di controllo.

I registri di controllo elencano le modifiche utente attivate nel sistema durante gli ultimi 90 giorni.

Per informazioni su tutti i tipi di log di controllo e su cosa li genera, vedi [Registri di controllo](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

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
   <td> <p>Piano </p> <p>Devi essere un amministratore Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visualizza registri di controllo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Sistema > Registri di controllo**.
1. In **Tipo di registro** dal menu a discesa, selezionare il tipo di registro di controllo che si desidera visualizzare.

   **Tutti i tipi di log** è selezionato per impostazione predefinita.

   Per un elenco di tutti i tipi di log di controllo che è possibile visualizzare e delle informazioni che includono, vedi [Registri di controllo](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Facoltativo) Imposta uno qualsiasi dei filtri disponibili.

   >[!NOTE]
   >
   >Le opzioni nel menu a discesa Tipo azione variano a seconda del registro di controllo selezionato.

   ![](assets/audit-logs.jpg)

1. Fai clic su **Applica**.
1. (Facoltativo) Fai clic su **Cancella filtri** per ripristinare le modifiche apportate ai filtri.

## Esportare i registri di controllo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Sistema > Registri di controllo**.

1. In **Tipo di registro** menu a discesa, selezionare un registro di controllo.

   **Tutti i tipi di log** è selezionato per impostazione predefinita.

1. Imposta uno dei filtri disponibili, quindi fai clic su **Applica**.

   >[!IMPORTANT]
   >
   >Non puoi esportare più di 50.000 log alla volta. Workfront esporta i registri in base ai filtri impostati, non al numero di registri visualizzati nella pagina. Puoi visualizzare il numero totale di registri filtrati nell’angolo in basso a destra della pagina.

1. Fai clic su **Esporta**.
