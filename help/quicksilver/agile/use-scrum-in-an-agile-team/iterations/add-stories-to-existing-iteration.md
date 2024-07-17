---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Aggiungere brani a un'iterazione esistente
description: È possibile aggiungere storie a un'iterazione in molti modi.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Aggiungere brani a un&#39;iterazione esistente

È possibile aggiungere brani a un&#39;iterazione in uno dei seguenti modi:

* Dal backlog dopo la creazione dell&#39;iterazione, come descritto nella sezione [Spostare i brani dal backlog a un&#39;iterazione o [!UICONTROL Kanban] board](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) in [Gestire il backlog Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Dalla pagina [!UICONTROL Dettagli] della singola attività o problema
* Da un elenco di attività o problemi
* Da un rapporto
* Da un dashboard

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
   <td> <p>[!UICONTROL Work] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o versione successiva</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso [!UICONTROL Gestisci] al progetto in cui si trova il brano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

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

È possibile configurare singoli team Scrum in modo che utilizzino le date del progetto per impostazione predefinita, anziché le date di iterazione. Per informazioni, vedere la sezione [Configurare le modalità di applicazione delle date durante l&#39;aggiunta di elementi di lavoro a un&#39;iterazione](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) nell&#39;articolo [Configurare Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Aggiungere una storia a un&#39;iterazione esistente

Per aggiungere brani a un’iterazione direttamente dall’attività o dal problema:

>[!IMPORTANT]
>
>Dopo che l&#39;attività è stata spostata nell&#39;iterazione, non è possibile aggiornare [!UICONTROL Tipo di durata] o [!UICONTROL Vincolo attività]. [!UICONTROL Tipo di durata] è impostato su [!UICONTROL Semplice] e [!UICONTROL Vincolo attività] è impostato su [!UICONTROL Date fisse] per mantenere la sequenza temporale dell&#39;attività coerente con quella dell&#39;iterazione.

### Dalla scheda attività o problemi

Puoi aggiungere qualsiasi attività o problema a qualsiasi iterazione se disponi dell’accesso Manage al progetto. Quando si sposta un’attività o un problema in un’iterazione, tieni presente quanto segue:

* Se aggiungi più team, l’attività o il problema può essere visualizzato solo nell’iterazione di un team. Questa è l&#39;iterazione scelta al passaggio 3.
* Se l’attività o il problema viene assegnato a un team agile e spostato nell’iterazione di un altro team, l’assegnazione del team non cambia.
* Se l’attività o il problema non è assegnato a un team, l’attività o il problema viene assegnato al team a cui appartiene l’iterazione.
* Impossibile aggiungere attività padre all&#39;iterazione. Se aggiungete delle attività figlio, l&#39;attività padre viene visualizzata sulla bacheca Scrum come corsia di scorrimento.

1. Passare al progetto, report o dashboard contenente l&#39;attività o il problema che si desidera aggiungere a un&#39;iterazione.
1. Seleziona una o più attività o problemi.
1. Fai clic su **[!UICONTROL Altro]** ![](assets/more-icon.png) > **[!UICONTROL Aggiungi a iterazione]**.\
   Non puoi assegnare attività o problemi ai team non agili.

1. Nella casella **[!UICONTROL Aggiungi storie]** digitare il nome dell&#39;iterazione.

   >[!NOTE]
   >
   >Potete spostare una storia da un&#39;iterazione esistente a una nuova iterazione.

1. Se stai aggiungendo attività, fai clic su **[!UICONTROL Aggiungi storie]**.\
   Oppure\
   Se stai aggiungendo dei problemi, fai clic su **[!UICONTROL Aggiungi problemi]**.
