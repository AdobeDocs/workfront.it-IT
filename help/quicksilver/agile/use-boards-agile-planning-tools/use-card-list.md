---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Utilizzare l’elenco delle schede
description: È possibile creare un elenco di schede in un flusso di lavoro e aggiungere le schede alle iterazioni.
author: Jenny
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Utilizza l’elenco delle schede

>[!IMPORTANT]
>
>I flussi di lavoro non sono disponibili per tutti i clienti.

È possibile creare un elenco di schede in un flusso di lavoro e aggiungere le schede alle iterazioni.

L’elenco delle schede può fungere da backlog di lavoro per il flusso di lavoro.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o versione successiva</p> 
   <p>Richiedi o superiore</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungi schede all’elenco delle schede

{{step1-to-boards}}

1. Per aprire un flusso di lavoro, fare clic su [!UICONTROL **Visualizza flusso di lavoro**].
1. Fare clic sulla scheda [!UICONTROL **Elenco schede**].
1. Fai clic su [!UICONTROL **Aggiungi scheda**].
1. Nella finestra di dialogo [!UICONTROL **Crea/Modifica scheda**], aggiungi le seguenti informazioni:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Name]</strong></td> 
      <td>Il nome della carta.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Descrizione]</strong></td> 
      <td>Una descrizione del Card.</td> 
     </tr>
     <tr> 
      <td><strong>Stima [!UICONTROL]</strong></td> 
      <td>Numero stimato di ore per il completamento della carta. Questa è solo una immissione manuale.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Stato]</strong></td> 
      <td>Selezionare uno stato per la scheda.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterazioni]</strong></td> 
      <td>Seleziona un'iterazione a cui assegnare la scheda.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Assegnatari]</strong></td> 
      <td><p>Per assegnare la scheda, inizia a digitare un nome nel campo di ricerca, quindi selezionalo quando viene visualizzato nell’elenco. Puoi aggiungere sia singoli utenti che team e assegnare più persone o team a una scheda.</p><p>Gli assegnatari devono essere membri nel flusso di lavoro oppure non verranno visualizzati nell'elenco di selezione.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Fai clic su [!UICONTROL **Salva**].
1. Continua ad aggiungere schede fino a quando non avrai creato l’elenco delle schede.

## Visualizza schede

Per visualizzare tutte le schede del flusso di lavoro in un unico elenco, fare clic su [!UICONTROL **Vista elenco**] nella scheda Elenco schede.

Per visualizzare tutte le schede del flusso di lavoro raggruppate per iterazione, fare clic su [!UICONTROL **Visualizzazione iterazione**]. Le schede non pianificate vengono visualizzate nel proprio gruppo.

Per modificare una scheda esistente, selezionarla nell&#39;elenco e fare clic su [!UICONTROL **Modifica**].

Per eliminare una scheda, selezionarla nell&#39;elenco e fare clic su [!UICONTROL **Elimina**].

### Filtra schede

Le schede possono essere archiviate solo dalla bacheca di iterazione. Quando una scheda viene archiviata, non viene visualizzata nell’elenco a meno che non si filtra per mostrare le schede archiviate. Per informazioni sull&#39;archiviazione di una scheda, vedere [Eliminare o archiviare una scheda da una scheda](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Accedere all&#39;elenco delle schede per il flusso di lavoro.
1. Fai clic su [!UICONTROL **Filtro**] e seleziona [!UICONTROL **Tutte**], [!UICONTROL **Schede attive**] o [!UICONTROL **Schede archiviate**].

   Quando nell&#39;elenco delle schede viene applicato un filtro diverso da quello predefinito, viene visualizzato un indicatore sull&#39;icona del filtro ![Filtro applicato](assets/boards-filterapplied-30x30.png).

### Cerca nell’elenco delle schede

1. Accedere all&#39;elenco delle schede per il flusso di lavoro.
1. Fai clic su [!UICONTROL **Cerca**] e digita un termine di ricerca. Quindi premere Invio.

   Vengono visualizzate tutte le schede che contengono il termine di ricerca.
Fare clic sulla X per annullare la ricerca.

   ![Cerca le schede in una bacheca](assets/boards-searchbox.png)

## Aggiungere schede a un’iterazione

>[!NOTE]
>
>È necessario creare un&#39;iterazione prima di aggiungervi schede. Per informazioni, vedere [Creare un&#39;iterazione in un flusso di lavoro](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Accedere all&#39;elenco delle schede per il flusso di lavoro.
1. Selezionare la [!UICONTROL **Visualizzazione iterazione**] per vedere quali schede sono assegnate a un&#39;iterazione e quali non sono pianificate.
1. Selezionare una scheda non pianificata nell&#39;elenco e fare clic su [!UICONTROL **Modifica**].
1. Selezionare un&#39;iterazione nel campo [!UICONTROL **Iterazioni**].
1. Se utilizzi i punti storia, immetti un valore nel campo [!UICONTROL **Stima**].
1. Fai clic su [!UICONTROL **Salva**].

   La scheda viene spostata nell&#39;iterazione e le metriche di iterazione riflettono il numero di schede e punti.

   Puoi anche trascinare una scheda dal gruppo di schede non pianificate nell&#39;iterazione, oppure fai clic su [!UICONTROL **Aggiungi scheda**] per aggiungere una nuova scheda all&#39;iterazione.

>[!TIP]
>
>Se è stata creata una bacheca per il processo di iterazione, tutte le schede non pianificate nell&#39;elenco delle schede vengono visualizzate nella colonna [!UICONTROL Backlog]. Quando una scheda viene spostata in un’altra colonna, diventa parte dell’iterazione attiva. Le schede aggiunte all’iterazione nell’elenco delle schede vengono aggiunte a una colonna in base al loro stato.
