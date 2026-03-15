---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Filtra e cerca in una bacheca
description: Puoi filtrare una bacheca per visualizzare solo determinate schede.
author: Courtney
feature: Agile
exl-id: 26abce82-dcd9-4865-96f4-c710f7f0a0d8
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 6%

---

# Filtrare ed eseguire ricerche in una bacheca

Puoi filtrare una bacheca per visualizzarla:

* Schede assegnate a determinate persone
* Schede con determinati tag
* Schede con uno stato specifico
* Carte scadute in un determinato periodo di tempo
* Schede archiviate
* Schede collegate a un progetto specifico

L’ordinamento della bacheca ordina tutte le schede nelle colonne. Non è possibile ordinare una singola colonna e la colonna di backlog o di input non è ordinata.

La ricerca consente inoltre di individuare una scheda specifica sulla bacheca.

Quando vengono applicati filtri, nella bacheca ![Filtro applicato alla bacheca](assets/boards-filterapplied-30x30.png) viene visualizzato un indicatore. Fai clic su **[!UICONTROL Cancella tutto]** per rimuovere tutti i filtri dalla bacheca, quindi fai clic sull&#39;icona di compressione per chiudere il pannello dei filtri.

![Pannello filtri](assets/boards-all-filters-collapsed-0823.png)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o successiva</p> 
   <p>Richiedente o successiva</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrare una bacheca per assegnatari

{{step1-to-boards}}

1. Accedi a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Fare clic su [!UICONTROL **Filtro**], espandere la sezione [!UICONTROL Membri] e selezionare la persona o le persone di cui si desidera visualizzare le schede. È inoltre possibile visualizzare schede non assegnate.

   ![Filtra per membro](assets/boards-filter-by-assignees-0822.png)

## Filtrare una bacheca per tag

1. Accedi alla bacheca.
1. Fai clic su [!UICONTROL **Filtro**], espandi la sezione [!UICONTROL Tag] e seleziona i tag che desideri visualizzare.

   ![Filtra per tag](assets/boards-filter-by-tags-0822.png)

## Filtrare una bacheca per stato

1. Accedi alla bacheca.
1. Fai clic su [!UICONTROL **Filtro**], espandi la sezione [!UICONTROL Stati] e seleziona i tipi di stato che desideri visualizzare.

   Puoi anche nascondere le schede completate.

   ![Filtra per stato](assets/boards-filter-by-status-0822.png)

## Filtrare una bacheca per data di scadenza

1. Accedi alla bacheca.
1. Fai clic su [!UICONTROL **Filtro**], espandi la sezione [!UICONTROL Scadenza] e seleziona le opzioni di data che desideri visualizzare.

   Vengono visualizzate solo le schede negli intervalli di date selezionati.

   ![Filtra per data di scadenza](assets/boards-filter-by-due-date-0822.png)

## Filtra una bacheca per visualizzare le schede archiviate

Per impostazione predefinita, su una bacheca vengono visualizzate solo le schede attive. È possibile filtrare la scheda per visualizzare anche tutte le schede archiviate.

1. Accedi alla bacheca.
1. Fai clic su [!UICONTROL **Configura**] a destra della bacheca per aprire il pannello Configura.
1. Espandere [!UICONTROL **Schede**].
1. Attiva [!UICONTROL **Visualizza schede archiviate sulla scheda**].
1. Fai clic su [!UICONTROL **Filtro**], espandi la sezione [!UICONTROL Schede archiviate] e seleziona **[!UICONTROL Schede archiviate]** per visualizzare tutte le schede archiviate.

   Il filtro mostra il numero di schede archiviate.

   ![Filtra schede archiviate](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >La sezione [!UICONTROL Schede archiviate] non è disponibile nel filtro se non è stata attivata l&#39;impostazione di configurazione per la visualizzazione delle schede archiviate. Per ulteriori informazioni, vedere [Personalizzare i campi visualizzati in una scheda](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Seleziona di nuovo **[!UICONTROL Schede archiviate]** per cancellare l&#39;opzione e visualizzare solo le schede attive.

## Filtrare una bacheca per connessione

1. Accedi alla bacheca.
1. Fai clic su [!UICONTROL **Filtro**], espandi la sezione [!UICONTROL Connessione] e seleziona i [!DNL Workfront] progetti per le schede connesse che desideri visualizzare.

   È inoltre possibile visualizzare schede non collegate a un progetto.

   ![Filtra per connessione](assets/boards-filter-by-connection.png)

## Ordinare su una bacheca

Quando si seleziona un&#39;opzione in base alla quale eseguire l&#39;ordinamento, vengono ordinate tutte le colonne. Non è possibile ordinare una singola colonna e la colonna di backlog o di input non è ordinata.

1. Accedi alla bacheca.
1. Fai clic su [!UICONTROL **Ordina per**] e seleziona [!UICONTROL **Nome**], [!UICONTROL **Data di scadenza**], [!UICONTROL **Stima**], [!UICONTROL **Stato**] o [!UICONTROL **Connessione**].

   La connessione (nome progetto) si applica solo alle schede connesse e le altre opzioni consentono di ordinare sia le schede connesse che quelle ad hoc nelle colonne.

   L’opzione &quot;ordine utente&quot; ripristina l’ordine in cui le schede sono state impostate manualmente, prima che venissero applicate altre opzioni di ordinamento. Questo è l&#39;ordinamento predefinito per le colonne.

1. Selezionare [!UICONTROL **Ordine inverso**] per ordinare le colonne in ordine inverso rispetto all&#39;opzione di ordinamento.

   La freccia sull&#39;icona di ordinamento indica se le colonne sono ordinate in ordine crescente o decrescente.

   Quando viene applicato un ordinamento diverso da quello predefinito, viene visualizzato un indicatore sull&#39;icona di ordinamento ![Ordinamento applicato](assets/sort-applied-boards.png).

   ![Ordina per colonne in una bacheca](assets/sort-by-columns-in-board.png)

## Cerca in una bacheca

1. Accedi alla bacheca.
1. Fai clic su [!UICONTROL **Cerca**] e digita un termine di ricerca. Quindi premere Invio.

   Vengono visualizzate tutte le schede che contengono il termine di ricerca.

   Fare clic sulla X per annullare la ricerca.

   ![Cerca le schede in una bacheca](assets/boards-searchbox.png)
