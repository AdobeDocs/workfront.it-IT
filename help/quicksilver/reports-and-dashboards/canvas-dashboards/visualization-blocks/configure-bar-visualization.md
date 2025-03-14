---
title: Configurare una visualizzazione a barre nell’area di lavoro Reporting
description: Configurare una visualizzazione a barre nell’area di lavoro Reporting
hidefromtoc: true
hide: true
exl-id: 7dc4f156-d262-482f-aa82-c905f0d1b20f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 2%

---

# Configurare una visualizzazione a barre nell’area di lavoro Reporting

Una visualizzazione a barre consente di raccontare rapidamente una storia sui dati evidenziando informazioni importanti mediante barre orizzontali.

## Prerequisiti

Prima di iniziare, devi iscriverti alla versione beta di Reporting Canvas. Per ulteriori informazioni, vedere [Reporting Canvas beta: overview](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configurare una visualizzazione a barre

>[!NOTE]
>
>Tutte le modifiche vengono salvate automaticamente durante la generazione e la modifica dei blocchi nel report.

1. Inizia aggiungendo un blocco di visualizzazione con tipo di visualizzazione **Barra** a un rapporto, come spiegato in [Aggiungi o modifica un blocco di visualizzazione nell&#39;area di lavoro di reporting](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. Fai clic sull&#39;icona Modifica visualizzazione ![Icona Modifica](assets/edit-icon.png) nell&#39;angolo superiore destro della visualizzazione, quindi effettua una delle seguenti operazioni.

   1. Nella scheda **Impostazioni**:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Tipo di visualizzazione</td>
         <td><p>Passa a un tipo diverso di visualizzazione. In questo caso, le opzioni successive del menu potrebbero cambiare.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Asse verticale</td>
         <td><p>Seleziona i dati da rappresentare lungo il bordo verticale sinistro o l’asse Y della visualizzazione a barre. La visualizzazione confronta gli elementi su questo asse in base a ciascun elemento sull’asse orizzontale.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Asse orizzontale</td>
         <td><p>Nel menu a discesa a sinistra, seleziona i dati che desideri rappresentare lungo l’asse orizzontale o X. Gli elementi su questo asse vengono visualizzati come barre di confronto, in base ai relativi valori.</p><p>Nel menu a discesa a destra, seleziona la modalità di calcolo e visualizzazione dei valori lungo l’asse orizzontale:</p>
          <ul>
           <li><p><b>Count</b>: numero di valori</p></li>
           <li><p><b>Somma</b>: il totale di tutti i valori </p></li>
           <li><p><b>Media</b>: la media di tutti i valori</p></li>
           <li><p><b>Minimo</b>: solo il valore più basso</p></li>
           <li><p><b>Massimo</b>: solo il valore più alto</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">+ Aggiungi valore</td>
         <td>Aggiungere un altro campo che si desidera tracciare lungo l'asse orizzontale.</td>
        </tr>
       </tbody>
      </table>

   1. Nella scheda **Dati**:

      | Origine dati (menu a discesa) | Modifica l’origine dati per la visualizzazione in un’altra tabella nell’area di lavoro del rapporto. |
      |---|---|
      | Mostra Source dati | Abilita questa opzione per mostrare la tabella di origine per la visualizzazione nell’area di lavoro del rapporto oppure disabilita l’opzione per nasconderla. |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. Fai clic in un punto qualsiasi al di fuori del menu delle impostazioni di visualizzazione per chiuderlo.
