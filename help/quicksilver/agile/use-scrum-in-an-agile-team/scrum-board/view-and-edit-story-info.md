---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Visualizzare e modificare le informazioni della storia sulla bacheca Scrum
description: Quando visualizzi una sezione del brano sulla bacheca Kanban, alcune informazioni sono disponibili per la modifica in linea direttamente dalla sezione del brano.
author: Jenny
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 5%

---

# Visualizza e modifica le informazioni sulla storia sulla bacheca [!UICONTROL Scrum]

## Comprendere quali informazioni possono essere visualizzate e modificate

Quando si visualizza una sezione del brano sullo storyboard, sono disponibili le informazioni riportate nella tabella seguente. Puoi modificare la maggior parte delle informazioni in linea, direttamente dal riquadro del brano.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Informazioni</strong> </th> 
   <th><strong>Visibile</strong> </th> 
   <th><strong>In linea modificabile</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Il nome del brano con un collegamento diretto all’attività o al problema</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Il nome del progetto con un collegamento diretto al progetto<br>Questo collegamento viene visualizzato solo nei brani (attività padre e non sottoattività) quando si utilizza la visualizzazione Agile in un'iterazione e non quando si utilizza una visualizzazione Agile in un progetto.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Il numero di punti o ore completate sul brano e il numero di punti o ore assegnate al brano<br>Questi numeri vengono utilizzati per calcolare e visualizzare il [!UICONTROL Percent Complete] per ogni brano.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Il [!UICONTROL Percent Complete] per ogni storia e problema.<br>Il [!UICONTROL Percent Complete] per l'iterazione viene calcolato in base al [!UICONTROL Percent Complete] per ogni brano.</p> <p>Quando aggiorni [!UICONTROL Percent Complete] per una storia o un problema, puoi scegliere un numero qualsiasi tra 0 e 100.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>A chi è assegnata la storia</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Colore o categoria della sezione</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Eventuali campi aggiuntivi (inclusi i campi personalizzati) che potrebbero essere stati aggiunti alla visualizzazione Agile modificando la visualizzazione Agile, come descritto in "Creazione e personalizzazione di una visualizzazione [!UICONTROL Agile]" in <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Panoramica delle visualizzazioni in [!UICONTROL Adobe Workfront]</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>Nuovo: [!UICONTROL Standard]</p> 
   oppure
   <p>Corrente: [!UICONTROL Work] o versione successiva</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Accesso [!UICONTROL Contribute] o [!UICONTROL Manage] all'attività o al problema</td> 
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare e modificare le informazioni su un riquadro del brano

{{step1-to-team}}

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

1. Nel pannello a sinistra, seleziona **[!UICONTROL Iterazioni]** per scegliere un&#39;iterazione specifica oppure seleziona **[!UICONTROL Iterazione corrente]**.

1. Vai alla bacheca delle storie di [!UICONTROL Scrum] Agile.
1. Espandi il riquadro [!UICONTROL storia] per visualizzare tutti i campi associati alla storia.

   ![scheda storia](assets/agile-storycard-scrum-2021-350x333.png)

1. (Facoltativo) Per modificare un campo, fai clic sul campo e apporta le modifiche necessarie.

   Per modificare il riquadro della storia, è necessario disporre dei diritti [!UICONTROL Modifica] per l&#39;attività o il problema.

>[!NOTE]
>
>Per modificare la [!UICONTROL Percentuale completata], è necessario digitare un numero compreso tra 0 e 100. Il campo non è un dispositivo di scorrimento da spostare.
