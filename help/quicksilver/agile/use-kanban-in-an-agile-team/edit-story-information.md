---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Modifica informazioni storia
description: Quando visualizzi una sezione del brano sulla bacheca Kanban, alcune informazioni sono disponibili per la modifica in linea direttamente dalla sezione del brano.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Modifica informazioni brano

## Comprendere quali informazioni possono essere visualizzate e modificate {#understand-what-information-can-be-viewed-and-edited}

Quando si visualizza un riquadro storia sulla bacheca [!UICONTROL Kanban], sono disponibili le informazioni riportate nella tabella seguente. Puoi modificare la maggior parte delle informazioni in linea, direttamente dal riquadro del brano.

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
   <td> <p>Il nome del progetto con un collegamento diretto al progetto</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Il numero di punti o ore completate sul brano e il numero di punti o ore assegnate al brano<br>Questi numeri vengono utilizzati per calcolare e visualizzare la percentuale di completamento per ogni brano.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Il [!UICONTROL Percent Complete] per ogni storia e problema.<br>[!UICONTROL La percentuale di completamento] per l'iterazione viene calcolata in base alla [!UICONTROL Percent Complete] per ogni brano.<br></p> <p>Quando aggiorni [!UICONTROL Percent Complete] per una storia o un problema, puoi scegliere un numero qualsiasi tra 0 e 100.</p> </td> 
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
   <td> <p>Eventuali campi aggiuntivi (inclusi i campi personalizzati) che potrebbero essere stati aggiunti alla visualizzazione Agile modificando la visualizzazione Agile, come descritto in "Creazione e personalizzazione di una visualizzazione Agile" in <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Panoramica delle visualizzazioni in [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare e modificare le informazioni su un riquadro del brano

{{step1-to-team}}

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Kanban dal menu a discesa o cerca un team nella barra di ricerca.

1. Vai alla bacheca [!UICONTROL Kanban].
1. Espandere il riquadro del brano per visualizzare tutti i campi associati al brano.

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Facoltativo) Per modificare un campo, fai clic sul campo e apporta le modifiche necessarie.
Per modificare il riquadro della storia, è necessario disporre dei diritti [!UICONTROL Modifica] per l&#39;attività o il problema.
Per ulteriori informazioni su ciascun campo e sulla possibilità di modificarlo, vedere [Informazioni sulle informazioni visualizzabili e modificabili](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Per modificare la [!UICONTROL Percentuale completata], è necessario digitare un numero compreso tra 0 e 100. Il campo non è un dispositivo di scorrimento da spostare.
