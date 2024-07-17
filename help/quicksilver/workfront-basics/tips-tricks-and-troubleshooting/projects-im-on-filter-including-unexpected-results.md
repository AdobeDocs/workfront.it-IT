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
   <td role="rowheader"><strong>Licenza Adobe [!DNL Workfront]</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso</strong></td> 
   <td> <p>[!UICONTROL Amministratore di sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

Il filtro [!UICONTROL **Progetti in corso**] include risultati non previsti, in quanto non sono assegnato o associato a tali progetti.

## Soluzione

Il filtro [!UICONTROL **Progetti in corso**] include progetti che contengono l&#39;utente in uno dei campi [!UICONTROL **Dettagli progetto**], inclusi campi facilmente mancanti o compilati automaticamente come [!UICONTROL **Inserito da**] o [!UICONTROL **ID sponsor**]. Per rimuovere i risultati indesiderati, esistono due soluzioni possibili:

1. Controlla [!UICONTROL **Dettagli progetto**] per ogni progetto imprevisto incluso dal filtro e rimuovi il tuo nome da tutti i campi.

   OPPURE

1. Prova a utilizzare un filtro simile, ad esempio [!UICONTROL **Progetti di cui sono Proprietario**], che include solo i progetti specificamente assegnati a te.

Per ulteriori informazioni sull&#39;utilizzo dei filtri in [!DNL Workfront], vedere [Panoramica dei filtri](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
