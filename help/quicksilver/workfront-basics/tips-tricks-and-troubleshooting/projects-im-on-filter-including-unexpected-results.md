---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Progetti su filtro, inclusi risultati imprevisti
description: Leggi questo articolo per risolvere i problemi relativi al filtro Progetti su , inclusi i risultati imprevisti.
feature: Get Started with Workfront
author: Nolan
source-git-commit: ba261e5121b4a28f71c58f883c784f4e8d2ada81
workflow-type: tm+mt
source-wordcount: '170'
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
   <td role="rowheader"><strong>Configurazioni a livello di accesso</strong></td> 
   <td> <p>[!UICONTROL System Administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

La [!UICONTROL **Progetti in corso**] Il filtro include risultati che non mi aspetto, in quanto non sono assegnato o associato a tali progetti.

## Soluzione

La [!UICONTROL **Progetti in corso**] Il filtro include i progetti che contengono l’utente in uno dei suoi [!UICONTROL **Dettagli progetto**] campi, inclusi campi compilati facilmente o automaticamente, ad esempio [!UICONTROL **Inserito da**] o [!UICONTROL **ID sponsor**]. Per rimuovere i risultati indesiderati, esistono due possibili soluzioni:

1. Controlla la [!UICONTROL **Dettagli progetto**] per ogni progetto imprevisto incluso dal filtro e rimuovi il tuo nome da tutti i campi.

   OPPURE

1. Prova a utilizzare un filtro simile, ad esempio [!UICONTROL **Progetti di proprietà**], che include solo i progetti specificamente assegnati all’utente.

Per ulteriori informazioni sull’utilizzo dei filtri in [!DNL Workfront], vedi [Panoramica dei filtri in [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)