---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Utilizza l'elenco delle schede
description: È possibile creare un elenco di schede in un flusso di lavoro e aggiungere le schede alle iterazioni.
author: Lisa
feature: Agile
source-git-commit: e5f65106226d82b24c7fa359e53136226f3d1239
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Utilizza l&#39;elenco delle schede

{{highlighted-preview-article-level}}

È possibile creare un elenco di schede in un flusso di lavoro e aggiungere le schede alle iterazioni.

L&#39;elenco delle schede può fungere da backlog del lavoro per il flusso di lavoro.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Request] o superiore</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aggiungi schede all&#39;elenco delle schede

{{step1-to-boards}}

1. Per aprire un flusso di lavoro, fai clic su [!UICONTROL **Visualizza flusso di lavoro**].
1. Fai clic sul pulsante [!UICONTROL **Elenco a schede**] scheda .
1. Fai clic su [!UICONTROL **Aggiungi scheda**].
1. In [!UICONTROL **Crea/Modifica scheda**] aggiungi le seguenti informazioni:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Name]</strong></td> 
      <td>Nome della scheda.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Descrizione]</strong></td> 
      <td>Una descrizione del Card.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimation]</strong></td> 
      <td>Numero stimato di ore per il completamento della scheda. Questa è solo una voce manuale.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Status]</strong></td> 
      <td>Seleziona uno stato per la scheda.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterazioni]</strong></td> 
      <td>Selezionate un'iterazione a cui assegnare la scheda.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Assignees]</strong></td> 
      <td><p>Per assegnare la scheda, inizia a digitare un nome nel campo di ricerca, quindi selezionalo quando viene visualizzato nell’elenco. Puoi aggiungere sia singoli che team e assegnare più di una persona o un team a una scheda.</p><p>Gli assegnatari devono essere membri del flusso di lavoro o non verranno visualizzati nell'elenco di selezione.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Fai clic su [!UICONTROL **Salva**].
1. Continua ad aggiungere schede fino a quando non avrai creato l’elenco delle schede.

## Visualizza schede

Per visualizzare tutte le schede per il flusso di lavoro in un unico elenco, fare clic su [!UICONTROL **Vista a elenco**] nella scheda Elenco schede.

Per visualizzare tutte le schede per il flusso di lavoro raggruppate per iterazione, fare clic su [!UICONTROL **Visualizzazione iterazione**]. Le schede non pianificate vengono visualizzate nel proprio gruppo.

Per modificare una scheda esistente, selezionala nell’elenco e fai clic su [!UICONTROL **Modifica**].

Per eliminare una scheda, selezionala nell’elenco e fai clic su [!UICONTROL **Elimina**].

### Carte filtro

Le schede possono essere archiviate solo dal pannello di iterazione. Quando una scheda viene archiviata, non viene visualizzata nell&#39;elenco delle schede a meno che non si utilizzi un filtro per mostrare le schede archiviate. Per informazioni sull&#39;archiviazione di una scheda, vedi [Eliminare o archiviare una scheda da una bacheca](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Accedi all&#39;elenco delle schede per il flusso di lavoro.
1. Fai clic su [!UICONTROL **Filtro**] e seleziona [!UICONTROL **Tutto**], [!UICONTROL **Carte attive**] oppure [!UICONTROL **Carte archiviate**].

   Quando nell&#39;elenco delle schede viene applicato un filtro diverso da quello predefinito, sull&#39;icona del filtro viene visualizzato un indicatore ![Filtro applicato](assets/boards-filterapplied-30x30.png).

### Cerca nell&#39;elenco delle schede

1. Accedi all&#39;elenco delle schede per il flusso di lavoro.
1. Fai clic su [!UICONTROL **Ricerca**] e digitare un termine di ricerca. Quindi, premere Invio.

   Vengono visualizzate tutte le schede contenenti il termine di ricerca.
Fai clic sulla X per cancellare la ricerca.

   ![Cercare schede in una bacheca](assets/boards-searchbox.png)

## Aggiunta di schede a un&#39;iterazione

>[!NOTE]
>
>È necessario creare un&#39;iterazione prima di poter aggiungere schede. Per informazioni, consulta [Creare un’iterazione](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md).

1. Accedi all&#39;elenco delle schede per il flusso di lavoro.
1. Seleziona la [!UICONTROL **Visualizzazione iterazione**] per vedere quali schede sono assegnate a un&#39;iterazione e quali non sono pianificate.
1. Seleziona una scheda non pianificata nell’elenco e fai clic su [!UICONTROL **Modifica**].
1. Seleziona un’iterazione nella [!UICONTROL **Iterazioni**] campo .
1. Se utilizzi i punti della storia, inserisci un valore nella [!UICONTROL **Stima**] campo .
1. Fai clic su [!UICONTROL **Salva**].

   La scheda viene spostata nell’iterazione e le metriche di iterazione riflettono il numero di schede e punti.

   Puoi anche trascinare una scheda dal gruppo di schede non pianificate nell’iterazione, oppure fare clic su [!UICONTROL **Aggiungi scheda**] per aggiungere una nuova scheda all’iterazione.

>[!TIP]
>
>Se è stata creata una bacheca del processo di iterazione, tutte le schede non pianificate nell&#39;elenco delle schede vengono visualizzate nella scheda [!UICONTROL Backlog] colonna. Quando una scheda viene spostata in un’altra colonna, diventa parte dell’iterazione attiva. Le schede aggiunte all&#39;iterazione nell&#39;elenco delle schede vengono aggiunte a una colonna in base al loro stato.

