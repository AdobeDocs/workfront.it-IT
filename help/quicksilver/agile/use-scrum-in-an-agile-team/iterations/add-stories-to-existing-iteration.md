---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Aggiungere storie a un'iterazione esistente
description: È possibile aggiungere storie a un'iterazione in molti modi.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Aggiungere storie a un&#39;iterazione esistente

Puoi aggiungere storie a un&#39;iterazione in uno dei seguenti modi:

* Dal backlog dopo la creazione dell’iterazione, come descritto in [Spostare le storie dal backlog a un&#39;iterazione o [!UICONTROL Kanban] bacheca](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) sezione [Gestire il backlog agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Da [!UICONTROL Dettagli] pagina della singola attività o problema
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
   <td> <p>[!UICONTROL Work] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superiore</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso a [!UICONTROL Gestire] il progetto su cui si trova la storia</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Comprendere in che modo l&#39;aggiunta di storie influisce sulle date delle attività

Per impostazione predefinita, quando si aggiunge un&#39;attività esistente a un&#39;iterazione, l&#39; [!UICONTROL Data di inizio prevista] e [!UICONTROL Data completamento pianificata] sono fissati come segue:

### Attività [!UICONTROL Data di inizio prevista]

* L&#39;attività utilizza la data di inizio dell&#39;iterazione quando:

   * Il progetto non ha un [!UICONTROL Data di inizio prevista] impostato.
   * Il progetto [!UICONTROL Data di inizio prevista] è *prima* o *su* la data di inizio dell&#39;iterazione.

* L’attività utilizza l’ [!UICONTROL Data di inizio prevista] quando:

   * Il progetto [!UICONTROL Data di inizio prevista] è *dopo* la data di inizio dell&#39;iterazione.

### Attività [!UICONTROL Data completamento pianificata]

* L&#39;attività utilizza la Data di fine dell&#39;iterazione quando:

   * Il progetto non ha un [!UICONTROL Data completamento pianificata] impostato.
   * Il progetto [!UICONTROL Data di inizio prevista] è *prima o dopo* la data di inizio dell&#39;iterazione o il progetto [!UICONTROL Data completamento pianificata] è *prima o dopo* la data di fine dell&#39;iterazione.

* L’attività utilizza l’ [!UICONTROL Data completamento pianificata] quando:

   * Il progetto [!UICONTROL Data di inizio prevista] è *dopo* la data di inizio dell&#39;iterazione e il [!UICONTROL Data completamento pianificata] è *dopo* la data di fine dell&#39;iterazione.

È possibile configurare i singoli team Scrum in modo che utilizzino le date del progetto per impostazione predefinita, anziché le date di iterazione. Per informazioni, consulta la sezione . [Configura come vengono applicate le date quando si aggiungono elementi di lavoro a un&#39;iterazione](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) nell&#39;articolo [Configura punteggio](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Aggiungere un brano a un&#39;iterazione esistente

Per aggiungere storie a un&#39;iterazione direttamente dall&#39;attività o dal problema:

>[!IMPORTANT]
>
>Una volta che l’attività si sposta nell’iterazione, non è possibile aggiornare il [!UICONTROL Tipo di durata] o [!UICONTROL Vincolo attività]. [!UICONTROL Tipo di durata] è impostato su [!UICONTROL Semplice] e [!UICONTROL Vincolo attività] è impostato su [!UICONTROL Date fisse] per mantenere la timeline dell’attività coerente con quella dell’iterazione.

### Dalla scheda attività o problemi

Puoi aggiungere qualsiasi attività o problema a qualsiasi iterazione se disponi dell’accesso Gestione al progetto. Quando si sposta un&#39;attività o un problema in un&#39;iterazione, tenere presente quanto segue:

* Se si aggiungono più team, l&#39;attività o il problema possono essere visualizzati solo nell&#39;iterazione di un team. Questa è l&#39;iterazione scelta nel passaggio 3 successivo.
* Se l&#39;attività o il problema viene assegnato a un team agile e spostato nell&#39;iterazione di un altro team, l&#39;assegnazione del team non viene modificata.
* Se l&#39;attività o il problema non viene assegnato a un team, l&#39;attività o il problema viene assegnato al team proprietario dell&#39;iterazione.
* Non è possibile aggiungere attività principali all&#39;iterazione. Se si aggiungono attività secondarie, l&#39;attività principale viene visualizzata sulla scheda Scrum come una corsia da bagno.

1. Passa al progetto, al report o al dashboard contenente l&#39;attività o il problema che desideri aggiungere a un&#39;iterazione.
1. Selezionare una o più attività o problemi.
1. Fai clic su **[!UICONTROL Altro]** ![](assets/more-icon.png) > **[!UICONTROL Aggiungi a iterazione]**.\
   Non è possibile assegnare attività o problemi assegnati a team non mobili.

1. In **[!UICONTROL Aggiungi storie]** digitare il nome dell&#39;iterazione.

   >[!NOTE]
   >
   >È possibile spostare un brano da un&#39;iterazione esistente a una nuova iterazione.

1. Se si aggiungono attività, fare clic su **[!UICONTROL Aggiungi storie]**.\
   Oppure\
   Se stai aggiungendo dei problemi, fai clic su **[!UICONTROL Aggiungi problemi]**.
