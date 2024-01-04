---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Il filtro Progetti in corso include risultati imprevisti
description: Leggi questo articolo per risolvere i problemi relativi al filtro Progetti in corso, inclusi i risultati imprevisti.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 1%

---

# Il filtro Progetti in corso include risultati imprevisti

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licenza</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso</strong></td> 
   <td> <p>[!UICONTROL Amministratore di sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

Il [!UICONTROL **Progetti a cui collaboro**] Il filtro include risultati che non mi aspetterei, in quanto non sono assegnato o associato a tali progetti.

## Soluzione

Il [!UICONTROL **Progetti a cui collaboro**] Il filtro include i progetti che contengono l’utente in uno qualsiasi dei suoi [!UICONTROL **Dettagli progetto**] campi, compresi i campi facilmente mancanti o compilati automaticamente come [!UICONTROL **Immesso da**] o [!UICONTROL **ID Sponsor**]. Per rimuovere i risultati indesiderati, esistono due soluzioni possibili:

1. Controlla la [!UICONTROL **Dettagli progetto**] per ogni progetto imprevisto incluso dal filtro e rimuovi il tuo nome da tutti i campi.

   OPPURE

1. Prova a utilizzare un filtro simile, ad esempio [!UICONTROL **Progetti di mia proprietà**], che include solo i progetti specificamente assegnati a te.

Per ulteriori informazioni sull’utilizzo dei filtri in [!DNL Workfront], vedi [Panoramica dei filtri](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
