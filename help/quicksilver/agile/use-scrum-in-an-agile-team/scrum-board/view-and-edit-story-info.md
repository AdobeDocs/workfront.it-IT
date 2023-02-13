---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Visualizza e modifica le informazioni sulla storia sulla bacheca di Scrum
description: Quando visualizzi un riquadro della storia sulla bacheca Kanban, alcune informazioni sono disponibili per la modifica in linea, direttamente dal riquadro della storia.
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Visualizza e modifica le informazioni sul brano [!UICONTROL Scratto] bacheca

## Comprendere quali informazioni possono essere visualizzate e modificate

Quando si visualizza una porzione di storia sulla bacheca, sono disponibili le informazioni riportate nella tabella seguente. Puoi modificare la maggior parte delle informazioni in linea, direttamente dalla sezione della storia.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Informazione</strong> </th> 
   <th><strong>Visibile</strong> </th> 
   <th><strong>Modificabile in linea</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nome del brano con un collegamento diretto all’attività o al problema</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Nome del progetto con un collegamento diretto al progetto<br>Questo collegamento viene visualizzato solo sui brani (attività principali, non sottoattività) quando si utilizza la visualizzazione agile su un'iterazione; non viene visualizzato quando si utilizza una visualizzazione agile su un progetto.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Il numero di punti o ore di completamento della storia e il numero di punti o ore assegnati alla storia<br>Questi numeri vengono utilizzati per calcolare e visualizzare la [!UICONTROL Percent Complete] per ogni storia.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Percentuale di completamento [!UICONTROL] per ogni storia e problema.<br>Il [!UICONTROL Percent Complete] per l’iterazione viene calcolato in base alla [!UICONTROL Percent Complete] per ogni storia.</p> <p>Quando si aggiorna la percentuale di completamento per una storia o un problema, è possibile scegliere un numero compreso tra 0 e 100.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>A chi è assegnata la storia</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Colore o categoria della tessera</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Eventuali campi aggiuntivi (compresi i campi personalizzati) che potrebbero essere stati aggiunti alla visualizzazione agile modificando la visualizzazione agile, come descritto in "Creazione e personalizzazione di una visualizzazione di Agile" in <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Panoramica delle visualizzazioni in Adobe Workfront</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Work] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superiore</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Modificare l’accesso all’attività o al problema</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Visualizzare e modificare le informazioni su un riquadro della storia

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

1. Nel pannello a sinistra, seleziona **[!UICONTROL Iterazioni]** per scegliere un&#39;iterazione specifica o selezionare **[!UICONTROL Iterazione corrente]**.

1. Vai a [!UICONTROL Scratto] tabellone di storia agile.
1. Espandi la [!UICONTROL storia] per visualizzare tutti i campi associati al brano.

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. (Facoltativo) Per modificare un campo, fai clic sul campo, quindi apporta eventuali modifiche.

   Devi avere [!UICONTROL Modifica] diritti all&#39;attività o al problema per modificare il riquadro della storia.

>[!NOTE]
>
>Per modificare la variabile [!UICONTROL Percentuale completata], è necessario digitare un numero compreso tra 0 e 100. Il campo non è un cursore che puoi spostare.
