---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Aggiungi storie a un'iterazione esistente
description: È possibile aggiungere storie a un'iterazione in molti modi.
author: Jenny
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 3%

---

# Aggiungere brani a un&#39;iterazione esistente

È possibile aggiungere brani a un&#39;iterazione in uno dei seguenti modi:

* Dal backlog dopo la creazione dell&#39;iterazione, come descritto nella sezione [Spostare i brani dal backlog a un&#39;iterazione o [!UICONTROL Kanban] board](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) in [Gestire il backlog Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Dalla pagina [!UICONTROL Dettagli] della singola attività o problema
* Da un elenco di attività o problemi
* Da un rapporto
* Da un dashboard

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Work o successiva</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Gestire l'accesso al progetto a cui appartiene il brano </td> 
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Comprendere come l’aggiunta di storie influisce sulle date delle attività

Per impostazione predefinita, quando si aggiunge un&#39;attività esistente a un&#39;iterazione, la [!UICONTROL Data inizio pianificata] e la [!UICONTROL Data completamento pianificata] dell&#39;attività vengono impostate come segue:

### Attività [!UICONTROL Data inizio pianificata]

* L&#39;attività utilizza la data di inizio dell&#39;iterazione quando:

   * Il progetto non ha una [!UICONTROL Data inizio pianificata] impostata.
   * La [!UICONTROL data di inizio pianificata] del progetto è *precedente* o *uguale* alla data di inizio dell&#39;iterazione.

* L&#39;attività utilizza la [!UICONTROL Data inizio pianificata] del progetto quando:

   * La [!UICONTROL data di inizio pianificata] del progetto è *successiva* alla data di inizio dell&#39;iterazione.

### Attività [!UICONTROL Data di completamento Pianificata]

* L&#39;attività utilizza la data di fine dell&#39;iterazione quando:

   * Il progetto non ha una [!UICONTROL Data di completamento Pianificata] impostata.
   * La [!UICONTROL data inizio pianificata] del progetto è *precedente o uguale a* la data inizio dell&#39;iterazione o la [!UICONTROL data completamento pianificata] del progetto è *precedente o uguale a* la data fine dell&#39;iterazione.

* L&#39;attività utilizza la [!UICONTROL data di completamento pianificata] del progetto quando:

   * La [!UICONTROL data inizio pianificata] del progetto è *successiva* alla data inizio dell&#39;iterazione e la [!UICONTROL data completamento pianificata] del progetto è *successiva* alla data fine dell&#39;iterazione.

È possibile configurare singoli team Scrum in modo che utilizzino le date del progetto per impostazione predefinita, anziché le date di iterazione. Per informazioni, vedere la sezione [Configurare le modalità di applicazione delle date durante l&#39;aggiunta di elementi di lavoro a un&#39;iterazione](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) nell&#39;articolo [Configurare Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Aggiungere una storia a un&#39;iterazione esistente

Puoi aggiungere qualsiasi attività o problema a qualsiasi iterazione se disponi dell’accesso Manage al progetto. Quando si sposta un’attività o un problema in un’iterazione, tieni presente quanto segue:

* Se aggiungi più team, l’attività o il problema può essere visualizzato solo nell’iterazione di un team. Questa è l&#39;iterazione scelta al passaggio 3.
* Se l’attività o il problema viene assegnato a un team agile e spostato nell’iterazione di un altro team, l’assegnazione del team non cambia.
* Se l’attività o il problema non è assegnato a un team, l’attività o il problema viene assegnato al team a cui appartiene l’iterazione.
* Impossibile aggiungere attività padre all&#39;iterazione. Se aggiungete delle attività figlio, l&#39;attività padre viene visualizzata sulla bacheca Scrum come corsia di scorrimento.

>[!IMPORTANT]
>
>Dopo che l&#39;attività è stata spostata nell&#39;iterazione, non è possibile aggiornare [!UICONTROL Tipo di durata] o [!UICONTROL Vincolo attività]. [!UICONTROL Tipo di durata] è impostato su [!UICONTROL Semplice] e [!UICONTROL Vincolo attività] è impostato su [!UICONTROL Date fisse] per mantenere la sequenza temporale dell&#39;attività coerente con quella dell&#39;iterazione.

1. Apri l’attività o il problema che desideri aggiungere a un’iterazione.
Oppure
Passare al progetto, report o dashboard contenente l&#39;attività o il problema che si desidera aggiungere a un&#39;iterazione. Quindi, seleziona una o più attività o problemi.

1. Fai clic sull&#39;icona **[!UICONTROL Altro]** ![Altro](assets/more-icon.png) > **[!UICONTROL Aggiungi all&#39;iterazione]**.
Non puoi assegnare attività o problemi ai team non agili.

1. Nella casella **[!UICONTROL Aggiungi a]** digitare il nome dell&#39;iterazione e selezionarlo quando viene visualizzato nell&#39;elenco.

   >[!NOTE]
   >
   >Potete spostare una storia da un&#39;iterazione esistente a una nuova iterazione.

1. Fai clic su **[!UICONTROL Aggiungi]**.
