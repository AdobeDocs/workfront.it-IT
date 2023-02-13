---
navigation-topic: use-the-gantt-chart
title: Esportare il Diagramma di Gantt in PDF
description: È possibile esportare il diagramma di Gantt in un PDF.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# Esporta il [!UICONTROL Diagramma di Gantt] a PDF

Puoi esportare i [!UICONTROL Diagramma di Gantt] a un PDF.

Dopo l’esportazione del [!UICONTROL Diagramma di Gantt] in PDF è possibile stamparlo o allegarlo a un’e-mail per condividerlo con altri utenti.

## Requisiti di accesso

Devi disporre dei seguenti elementi per seguire i passaggi descritti in questo articolo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizzazione progetti e attività o accesso successivo</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>[!UICONTROL View] o accesso successivo al progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Esporta il [!UICONTROL Diagramma di Gantt]

1. Accedere al [!UICONTROL Diagramma di Gantt] da esportare in PDF, come descritto in [Introduzione al [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Verifica di aver configurato il [!UICONTROL Diagramma di Gantt] per visualizzare le informazioni appropriate prima di esportarle.

   >[!NOTE]
   >
   >Se si esporta il [!UICONTROL Diagramma di Gantt] in un elenco di progetti, il file PDF contiene solo i progetti elencati, non le attività di ciascun progetto. Se si desidera esportare un elenco di attività, è possibile farlo dal progetto a cui sono associate oppure creando un rapporto di attività e visualizzando i risultati del rapporto nel [!UICONTROL Visualizzazione Gantt].

   Puoi configurare le seguenti informazioni:

   * Filtri, visualizzazioni e raggruppamenti come desiderato nell’elenco delle attività. Eventuali filtri e raggruppamenti selezionati nella vista a elenco vengono mantenuti quando si visualizza il [!UICONTROL Diagramma di Gantt]. Le visualizzazioni si riflettono sull&#39;esportazione [!UICONTROL Diagramma di Gantt] solo all’interno dell’elenco visualizzato accanto al [!UICONTROL Diagramma di Gantt] nella prima pagina. Le visualizzazioni non vengono visualizzate sul [!UICONTROL Diagramma di Gantt] stesso.

      >[!TIP]
      >
      >Per dare più spazio al [!UICONTROL Diagramma di Gantt] applica a se stesso una visualizzazione contenente il minor numero possibile di colonne.

   * Opzioni di configurazione [!UICONTROL Diagramma di Gantt]. Ad esempio, puoi abilitare tappe, date, [!UICONTROL linee di base]oppure [!UICONTROL percentuale di completamento] da visualizzare sul [!UICONTROL Diagramma di Gantt].

      Per ulteriori informazioni, consulta   [Configurare la modalità di visualizzazione delle informazioni nel [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

      >[!NOTE]
      >
      > Le assegnazioni non vengono visualizzate sul [!UICONTROL Diagramma di Gantt] quando [!UICONTROL Diagramma di Gantt] viene esportato in PDF. Quando il [!UICONTROL Diagramma di Gantt] le assegnazioni vengono esportate in PDF e visualizzate solo nella vista a elenco.

   * Il periodo di tempo visualizzato nel [!UICONTROL Diagramma di Gantt].\

      Per ulteriori informazioni, consulta [Visualizzazione delle informazioni nel [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

      La modalità di visualizzazione del periodo di tempo nel file di esportazione dipende dalla selezione o meno dell’opzione **[!UICONTROL Cosa vedo]** o **[!UICONTROL Pagine multiple]** in un passaggio successivo.

1. (Facoltativo) Per includere solo alcune attività in PDF esportato, selezionare le attività da includere.

   Se non si selezionano attività, tutte le attività vengono incluse nel PDF esportato.

   Ad esempio, se visualizzi il [!UICONTROL Diagramma di Gantt] per un progetto che contiene 50 attività, ma si desidera visualizzare solo 10 attività sulla [!UICONTROL Diagramma di Gantt], seleziona le 10 attività da visualizzare.

1. Fare clic sull&#39;icona della stampante.\
   La **[!UICONTROL Esportare in PDF]** viene visualizzata la finestra di dialogo.\
   ![export_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Seleziona se esportare solo ciò che vedi o l&#39;intero [!UICONTROL Diagramma di Gantt]:

   * **[!UICONTROL Cosa vedo]:** Esporta tutte le attività (comprese eventuali sottoattività) visualizzate sullo schermo prima di esportare fino a 500 elementi. (Questo non è ciò che viene visualizzato nel **[!UICONTROL Anteprima]** sezione; la [!UICONTROL Anteprima] contiene solo dati di esempio).

      Le sottoattività vengono incluse nel PDF esportato anche se l’attività principale è compressa e le sottoattività non sono visibili. Per includere solo le attività principali, selezionare le attività principali che si desidera includere e lasciare deselezionate le sottoattività.

      È possibile utilizzare **[!UICONTROL Zoom a]** menu a discesa o strumento di scorrimento per visualizzare solo una parte del [!UICONTROL Diagramma di Gantt], come descritto in [Visualizzazione delle informazioni nel [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL Pagine multiple]:** Esporta l&#39;intero [!UICONTROL Diagramma di Gantt], anche se non è visibile sullo schermo corrente fino a 500 elementi.\

      È possibile utilizzare **[!UICONTROL Zoom a]** menu a discesa o strumento di scorrimento per determinare la quantità di informazioni visualizzate su ogni pagina, come descritto in [Configurare la modalità di visualizzazione delle informazioni nel [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Seleziona un’opzione più granulare per visualizzare più pagine da esportare oppure un’opzione meno granulare per visualizzare meno pagine da esportare.

      >[!NOTE]
      >
      >Se devi esportare un [!UICONTROL Diagramma di Gantt] che contiene più di 500 elementi, applica un filtro all’elenco prima di visualizzare il [!UICONTROL Diagramma di Gantt] in modo da visualizzare meno di 500 elementi o 250 pagine. Per informazioni su come applicare un filtro, consulta  [Panoramica dei filtri in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
      >
      >
      >Non è possibile esportare l&#39;intero diagramma di Gantt nelle seguenti circostanze:
      >
      >   
      >   
      >   * Quando si estende su più di 250 pagine
      >   * Quando contiene più di 500 elementi





1. Se il PDF viene stampato dopo l’esportazione in PDF, nella **[!UICONTROL Dimensioni pagina]** selezionare le dimensioni della carta in cui si desidera stampare.\
   È possibile selezionare **[!UICONTROL Lettera]**, **[!UICONTROL Note legali]**, **[!UICONTROL Libro contabile]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (disponibile solo per alcune lingue), oppure **[!UICONTROL A4]**.
1. In **[!UICONTROL Orientamento pagina]** seleziona se desideri esportare il PDF in orientamento orizzontale o verticale.
1. Seleziona **[!UICONTROL Mostra legenda]** per includere la legenda nel PDF esportato.
1. Fai clic su **[!UICONTROL Esporta]**.

   Il pdf del [!UICONTROL Diagramma di Gantt] viene creato e scaricato nel computer.

   Osserva la legenda nella parte inferiore del file esportato. Vengono illustrate solo le opzioni abilitate nel [!UICONTROL Diagramma di Gantt] disponibili nell&#39;elenco delle attività.

   Ad esempio, le tappe principali vengono visualizzate nella legenda solo se alla milestone è associata almeno un&#39;attività.

   ![gantt_Chart_with_update_limited_legenda_limitata.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
