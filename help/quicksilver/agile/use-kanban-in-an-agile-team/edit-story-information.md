---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Modifica delle informazioni del racconto
description: Quando visualizzi un riquadro della storia sulla bacheca Kanban, alcune informazioni sono disponibili per la modifica in linea, direttamente dal riquadro della storia.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Modifica delle informazioni del racconto

## Comprendere quali informazioni possono essere visualizzate e modificate {#understand-what-information-can-be-viewed-and-edited}

Quando si visualizza una porzione di storia su [!UICONTROL Kanban] bacheca, sono disponibili le informazioni riportate nella seguente tabella. Puoi modificare la maggior parte delle informazioni in linea, direttamente dalla sezione della storia.

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
   <td> <p>Nome del progetto con un collegamento diretto al progetto</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Il numero di punti o ore di completamento della storia e il numero di punti o ore assegnati alla storia<br>Questi numeri vengono utilizzati per calcolare e visualizzare la percentuale di completamento per ogni storia.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Percentuale di completamento [!UICONTROL] per ogni storia e problema.<br>La percentuale di completamento viene calcolata in base alla percentuale di completamento per ogni storia.<br></p> <p>Quando si aggiorna la percentuale di completamento per una storia o un problema, è possibile scegliere un numero compreso tra 0 e 100.</p> </td> 
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
   <td> <p>Eventuali campi aggiuntivi (compresi i campi personalizzati) che potrebbero essere stati aggiunti alla visualizzazione agile modificando la visualizzazione agile, come descritto in "Creazione e personalizzazione di una visualizzazione Agile" in <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Panoramica delle visualizzazioni in [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>[!UICONTROL Worker] o superiore</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Visualizzare e modificare le informazioni su un riquadro della storia

1. Fai clic sul pulsante *[!UICONTROL *Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Kanban dal menu a discesa o cerca un team nella barra di ricerca.

1. Vai a [!UICONTROL Kanban] consiglio di amministrazione.
1. Espandi la sezione del brano per visualizzare tutti i campi associati al brano.

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Facoltativo) Per modificare un campo, fai clic sul campo, quindi apporta eventuali modifiche.\
   Devi avere [!UICONTROL Modifica] diritti all&#39;attività o al problema per modificare il riquadro della storia.\
   Per ulteriori informazioni su ciascun campo e sulla possibilità di modificarlo, consulta [Comprendere quali informazioni possono essere visualizzate e modificate](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Per modificare la variabile [!UICONTROL Percentuale completata], è necessario digitare un numero compreso tra 0 e 100. Il campo non è un cursore che puoi spostare.
