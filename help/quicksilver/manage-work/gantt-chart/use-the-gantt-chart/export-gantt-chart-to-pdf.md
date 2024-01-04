---
navigation-topic: use-the-gantt-chart
title: Esportare il diagramma di Gantt in PDF
description: Puoi esportare il grafico Gantt in un PDF.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# Esporta il [!UICONTROL Diagramma di Gantt] a PDF

Puoi esportare la [!UICONTROL Diagramma di Gantt] a un PDF.

Dopo aver esportato [!UICONTROL Diagramma di Gantt] in PDF, puoi stamparlo o allegarlo a un messaggio e-mail, per condividerlo con altri utenti.

## Requisiti di accesso

Per seguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva a progetti e attività</p> <p>Nota: se non disponi ancora dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva al progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Esporta il [!UICONTROL Diagramma di Gantt]

1. Accedere a [!UICONTROL Diagramma di Gantt] che desideri esportare in PDF, come descritto in [Introduzione a [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Verifica di aver configurato [!UICONTROL Diagramma di Gantt] per visualizzare le informazioni appropriate prima dell&#39;esportazione.

   >[!NOTE]
   >
   >Se si esporta [!UICONTROL Diagramma di Gantt] da un elenco di progetti, il file PDF contiene solo i progetti dell’elenco, non le attività di ciascun progetto. Se si desidera esportare un elenco di attività, è possibile farlo dal progetto a cui sono associate oppure creando un report delle attività e visualizzando i risultati del report in [!UICONTROL Vista Gantt].

   Puoi configurare le seguenti informazioni:

   * Filtri, visualizzazioni e raggruppamenti come desiderato nell’elenco delle attività. Tutti i filtri e i raggruppamenti selezionati nella vista a elenco vengono mantenuti durante la visualizzazione del [!UICONTROL Diagramma di Gantt]. Le visualizzazioni si riflettono sul file esportato [!UICONTROL Diagramma di Gantt] solo all&#39;interno dell&#39;elenco visualizzato accanto al [!UICONTROL Diagramma di Gantt] sulla prima pagina. Le visualizzazioni non vengono visualizzate nel [!UICONTROL Diagramma di Gantt] stesso.

     >[!TIP]
     >
     >Per dare più spazio al [!UICONTROL Diagramma di Gantt] applicare una visualizzazione che contenga il minor numero di colonne possibile.

   * Opzioni di configurazione su [!UICONTROL Diagramma di Gantt]. Ad esempio, puoi abilitare le milestone, le date, [!UICONTROL linee di base], o [!UICONTROL percentuale di completamento] da visualizzare sul [!UICONTROL Diagramma di Gantt].

     Per ulteriori informazioni, consulta   [Configurare la modalità di visualizzazione delle informazioni sul [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Le assegnazioni non vengono visualizzate nel [!UICONTROL Diagramma di Gantt] quando [!UICONTROL Diagramma di Gantt] viene esportato in PDF. Quando [!UICONTROL Diagramma di Gantt] viene esportato in PDF, le assegnazioni vengono visualizzate solo nella vista a elenco.

   * Il periodo di tempo visualizzato sul [!UICONTROL Diagramma di Gantt].\

     Per ulteriori informazioni, consulta [Visualizzazione delle informazioni in [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     La modalità di visualizzazione del periodo di tempo nel file di esportazione dipende dalla selezione o meno **[!UICONTROL Quello che vedo]** o **[!UICONTROL Più pagine]** in un passaggio successivo.

1. (Facoltativo) Per includere solo alcune attività nel PDF esportato, selezionare le attività che si desidera includere.

   Se non si seleziona alcuna attività, tutte le attività vengono incluse nel PDF esportato.

   Ad esempio, se visualizzi il [!UICONTROL Diagramma di Gantt] per un progetto che contiene 50 attività, ma si desidera visualizzare solo 10 attività sul file esportato [!UICONTROL Diagramma di Gantt], selezionare le 10 attività che si desidera visualizzare.

1. Fare clic sull&#39;icona della stampante.\
   Il **[!UICONTROL Esporta in PDF]** viene visualizzata.\
   ![export_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Seleziona se desideri esportare solo ciò che vedi o l’intero [!UICONTROL Diagramma di Gantt]:

   * **[!UICONTROL Quello che vedo]:** Esporta tutte le attività (incluse le sottoattività) visualizzate sullo schermo prima dell&#39;esportazione di un massimo di 500 elementi. (Questo non è ciò che viene visualizzato nel **[!UICONTROL Anteprima]** sezione; la sezione [!UICONTROL Anteprima] contiene solo dati di esempio.)

     Le sottoattività sono incluse nel PDF esportato anche se l&#39;attività padre è compressa e le sottoattività non sono visibili. Per includere solo le attività padre, selezionare le attività padre da includere e lasciare deselezionate le eventuali attività secondarie.

     È possibile utilizzare **[!UICONTROL Zoom a]** menu a discesa o dello strumento di scorrimento per visualizzare solo una parte [!UICONTROL Diagramma di Gantt], come descritto in [Visualizzazione delle informazioni in [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL Più pagine]:** Esporta l&#39;intero [!UICONTROL Diagramma di Gantt], anche quello che non è visibile nella schermata corrente fino a 500 elementi.\

     È possibile utilizzare **[!UICONTROL Zoom a]** menu a discesa o lo strumento di scorrimento per determinare la quantità di informazioni visualizzate in ogni pagina, come descritto in [Configurare la modalità di visualizzazione delle informazioni sul [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Seleziona un’opzione più granulare per visualizzare più pagine da esportare oppure un’opzione meno granulare per visualizzare meno pagine da esportare.

     >[!NOTE]
     >
     >Se è necessario esportare un [!UICONTROL Diagramma di Gantt] che contiene più di 500 elementi, applica un filtro all’elenco prima di visualizzare [!UICONTROL Diagramma di Gantt] in modo da visualizzare meno di 500 elementi o 250 pagine. Per informazioni su come applicare un filtro, consulta  [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >Non è possibile esportare l&#39;intero diagramma di Gantt nelle seguenti circostanze:
     >
     >   
     >   
     >   * Quando occupa più di 250 pagine
     >   * Se contiene più di 500 elementi




1. Se il PDF verrà stampato dopo l&#39;esportazione in PDF, nella **[!UICONTROL Dimensioni pagina]** selezionare le dimensioni della carta in cui si desidera stampare.\
   Puoi selezionare **[!UICONTROL Lettera]**, **[!UICONTROL Note legali]**, **[!UICONTROL Ledger]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (disponibile solo per alcune lingue), oppure **[!UICONTROL A4]**.
1. In **[!UICONTROL Orientamento pagina]** , selezionare se si desidera che il PDF venga esportato con orientamento orizzontale o verticale.
1. Seleziona **[!UICONTROL Mostra legenda]** se si desidera includere la legenda nel PDF esportato.
1. Clic **[!UICONTROL Esporta]**.

   Il pdf della sezione [!UICONTROL Diagramma di Gantt] viene creato e scaricato nel computer.

   Osserva la legenda nella parte inferiore del file esportato. Illustra solo le opzioni abilitate nel [!UICONTROL Diagramma di Gantt] e disponibili nell&#39;elenco delle attività.

   Ad esempio, le attività cardine vengono visualizzate nella legenda solo se a esse è associata almeno un&#39;attività.

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
