---
navigation-topic: use-the-gantt-chart
title: Esportare il diagramma di Gantt in PDF
description: Puoi esportare il grafico Gantt in una PDF. In seguito, puoi stamparlo o allegarlo a un messaggio e-mail per condividerlo con altri utenti.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '979'
ht-degree: 2%

---

# Esporta il [!UICONTROL Diagramma di Gantt] in PDF

<!--Audited: 08/2025-->

Puoi esportare il [!UICONTROL Grafico di Gantt] in un PDF. In seguito, puoi stamparlo o allegarlo a un messaggio e-mail per condividerlo con altri utenti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto [!UICONTROL Adobe Workfront]</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">licenza di [!UICONTROL Adobe Workfront]</td> 
   <td> <p>[!UICONTROL Light] o versione successiva</p>
   <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva a progetti e attività</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva al progetto e alle attività</p> </td> 
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
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] license</td> 
   <td> <p>New:[!UICONTROL Light] or higher</p>
   <p>Current:[!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] or higher access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] or higher access to the project</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Esporta il [!UICONTROL diagramma di Gantt]

1. Accedere al [!UICONTROL Grafico di Gantt] che si desidera esportare in PDF, come descritto in [Introduzione al [!UICONTROL Grafico di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Configurare il [!UICONTROL Diagramma di Gantt] per visualizzare le informazioni appropriate da esportare.

   >[!NOTE]
   >
   >Se si esporta il [!UICONTROL Diagramma di Gantt] da un elenco di progetti, il file PDF contiene solo i progetti dell&#39;elenco, non le attività di ciascun progetto. Se si desidera esportare un elenco di attività, è possibile farlo dal progetto a cui sono associate oppure creando un report di attività e visualizzando i risultati del report nella [!UICONTROL Visualizzazione Gantt].

   Configura una delle seguenti informazioni:

   * Fai clic sulle icone **Filtri**, **Visualizza** e **Raggruppamento** sopra il [!UICONTROL Grafico di Gantt] e aggiungi o modifica il filtro, la visualizzazione o il raggruppamento esistenti applicati all&#39;elenco degli elementi nel [!UICONTROL Grafico di Gantt].

     Tutti i filtri e i raggruppamenti selezionati nella vista a elenco vengono mantenuti durante la visualizzazione del [!UICONTROL Grafico di Gantt]. Le visualizzazioni si riflettono sul [!UICONTROL Grafico di Gantt] esportato solo all&#39;interno dell&#39;elenco visualizzato accanto al [!UICONTROL Grafico di Gantt] nella prima pagina. Le visualizzazioni non vengono visualizzate nel [!UICONTROL Diagramma di Gantt] stesso.

     >[!TIP]
     >
     >Per consentire più spazio per il [!UICONTROL Grafico di Gantt], applicare una visualizzazione che contenga il minor numero di colonne possibile.

   * Selezionare l&#39;opzione **Passa a date previste** per visualizzare le date previste anziché quelle pianificate. Per impostazione predefinita, vengono visualizzate le Date pianificate.

   * Fai clic sull&#39;icona **Impostazioni** ![Icona Impostazioni](assets/settings-icon.png) nell&#39;angolo superiore destro del diagramma di Gantt e seleziona le informazioni da visualizzare. Una volta selezionate, queste informazioni vengono incluse nel file PDF di Gantt esportato.

     Selezionare una delle opzioni seguenti:

      * Date effettive
      * Assegnazioni
      * Linea di base
      * Conferma data
      * % completamento
      * Percorso critico
      * Diamanti milestone
      * Linee milestone
      * Predecessori
      * Stato di avanzamento
      * (Condizionale) Date Pianificate
      * (Condizionale) Date Previste

     Per ulteriori informazioni, consulta   [Configura la visualizzazione delle informazioni nel [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Le assegnazioni non vengono visualizzate nel [!UICONTROL Grafico di Gantt] quando il [!UICONTROL Grafico di Gantt] viene esportato in PDF. Dopo l&#39;esportazione, le assegnazioni vengono visualizzate solo nella vista a elenco.

   * Il periodo di tempo visualizzato nel [!UICONTROL diagramma di Gantt]. La modalità di visualizzazione nel file di esportazione dipende dalla selezione di **[!UICONTROL Quello che vedo]** o **[!UICONTROL Più pagine]** in un passaggio successivo.

     Per ulteriori informazioni, vedere [Visualizzazione delle informazioni nel [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).



1. (Facoltativo) Per includere solo alcune attività nel PDF esportato, selezionare le attività che si desidera includere. Se non si seleziona alcuna attività, tutte le attività vengono incluse nel PDF esportato.

   Ad esempio, se visualizzi il [!UICONTROL Grafico di Gantt] per un progetto che contiene 50 attività, ma desideri visualizzare solo 10 attività nel [!UICONTROL Grafico di Gantt] esportato, seleziona le 10 attività che desideri visualizzare.

1. Fare clic sull&#39;icona della stampante ![Icona della stampante](assets/printer-icon.png) nell&#39;angolo superiore destro del diagramma di Gantt.
Viene visualizzata la finestra di dialogo Esporta in PDF&#x200B;**[!UICONTROL .]**

   ![Finestra di dialogo Esporta in PDF](assets/exported-gantt-ui-350x225.png)

1. Nella sezione **Esporta**, seleziona una delle seguenti opzioni per indicare se desideri esportare solo ciò che vedi oppure l&#39;intero [!UICONTROL Grafico di Gantt]:

   * **[!UICONTROL Elementi visualizzati]:** Esporta tutte le attività (incluse le sottoattività) visualizzate sullo schermo prima dell&#39;esportazione di un massimo di 500 elementi. (Questo non è ciò che viene visualizzato nella sezione **[!UICONTROL Anteprima]**; la sezione **Anteprima** contiene solo dati di esempio.)

     Le sottoattività sono incluse nel PDF esportato anche se l&#39;attività padre è compressa e le sottoattività non sono visibili. Per includere solo le attività padre, selezionare le attività padre da includere e lasciare deselezionate le eventuali attività secondarie.

     >[!TIP]
     >
     >È possibile utilizzare lo strumento zoom o cursore per visualizzare solo una parte del [!UICONTROL diagramma di Gantt], come descritto in [Visualizzazione delle informazioni nel [!UICONTROL diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md). Seleziona un’opzione più granulare per visualizzare più pagine da esportare oppure un’opzione meno granulare per visualizzare meno pagine da esportare.


   * **[!UICONTROL Più pagine]:** Esporta l&#39;intero [!UICONTROL Grafico di Gantt] (fino a 500 elementi), inclusi gli elementi non visibili nella schermata corrente.

     >[!NOTE]
     >
     >* Se devi esportare un [!UICONTROL Grafico di Gantt] contenente più di 500 elementi, applica un filtro all&#39;elenco prima di visualizzare il [!UICONTROL Grafico di Gantt] in modo da visualizzare meno di 500 elementi o 250 pagine. Per informazioni su come applicare un filtro, vedere [Panoramica dei filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >* Non è possibile esportare l&#39;intero diagramma di Gantt nelle seguenti circostanze:
     >   
     >   * Quando occupa più di 250 pagine.
     >   * Se contiene più di 500 elementi.


1. Se il PDF verrà stampato dopo l&#39;esportazione in PDF, selezionare le dimensioni della carta da stampare nel menu a discesa **[!UICONTROL Dimensioni pagina]**.
Puoi scegliere una delle opzioni seguenti:

   * **[!UICONTROL Lettera]**
   * **[!UICONTROL Note legali]**
   * **[!UICONTROL Libro contabile]**
   * **[!UICONTROL A1]**
   * **[!UICONTROL A2]**
   * **[!UICONTROL A3]** (disponibile solo per alcune lingue)
   * **[!UICONTROL A4]**
1. Nella sezione **[!UICONTROL Orientamento pagina]**, seleziona se desideri esportare il PDF con orientamento orizzontale o verticale.
1. Selezionare **[!UICONTROL Mostra legenda]** se si desidera includere la legenda nel PDF esportato.
1. Fai clic su **[!UICONTROL Esporta]**. Il PDF viene creato e scaricato nel computer.

   La legenda nella parte inferiore del file esportato spiega solo le opzioni abilitate nel [!UICONTROL Diagramma di Gantt] e disponibili nell&#39;elenco delle attività. Ad esempio, le attività cardine vengono visualizzate nella legenda solo se a esse è associata almeno un&#39;attività.

   ![grafico_gantt_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
