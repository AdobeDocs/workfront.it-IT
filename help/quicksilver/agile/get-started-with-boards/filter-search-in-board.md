---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Filtrare ed eseguire ricerche in una bacheca
description: Puoi filtrare una bacheca per visualizzare solo determinate schede.
author: Lisa
feature: Agile
exl-id: 26abce82-dcd9-4865-96f4-c710f7f0a0d8
source-git-commit: a4ccd48956fedbafc04ce19198592efdad49e5a3
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Filtrare ed eseguire ricerche in una bacheca

Puoi filtrare una bacheca per visualizzarla:

* Schede assegnate a determinate persone
* Schede con determinati tag
* Schede con uno stato specifico
* Schede in scadenza in un determinato intervallo di tempo
* Schede archiviate
* Schede connesse a un progetto specifico

L’ordinamento della bacheca ordina tutte le schede nelle colonne. Non è possibile ordinare una singola colonna e la colonna backlog o acquisizione non è ordinata.

La ricerca consente inoltre di individuare una scheda specifica sulla bacheca.

Quando vengono applicati filtri, sulla scheda viene visualizzato un indicatore ![Filtro applicato alla bacheca](assets/boards-filterapplied-30x30.png). Clic **[!UICONTROL Cancella tutto]** per rimuovere tutti i filtri dalla bacheca, quindi fai clic su **[!UICONTROL Nascondi filtri]** per chiudere il pannello dei filtri.

![Pannello Filtro](assets/boards-all-filters-collapsed-1022.png)

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
   <td> <p>[!UICONTROL Request] o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Filtrare una bacheca per assegnatari

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Schede]**.
1. Accedi a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Clic [!UICONTROL **Filtro**], espandi [!UICONTROL Membri] e selezionare la persona o le persone di cui si desidera visualizzare le schede. Puoi anche visualizzare le schede non assegnate.

   ![Filtra per membro](assets/boards-filter-by-assignees-0822.png)

## Filtrare una bacheca per tag

1. Accedi alla bacheca.
1. Clic [!UICONTROL **Filtro**], espandi [!UICONTROL Tag] e selezionare i tag che si desidera visualizzare.

   ![Filtra per tag](assets/boards-filter-by-tags-0822.png)

## Filtrare una bacheca per stato

1. Accedi alla bacheca.
1. Clic [!UICONTROL **Filtro**], espandi [!UICONTROL Stati] e selezionare i tipi di stato da visualizzare.

   Puoi anche nascondere le schede completate.

   ![Filtra per stato](assets/boards-filter-by-status-0822.png)

## Filtrare una bacheca per data di scadenza

1. Accedi alla bacheca.
1. Clic [!UICONTROL **Filtro**], espandi [!UICONTROL Data di scadenza] e selezionare le opzioni di data desiderate.

   Vengono visualizzate solo le schede negli intervalli di date selezionati.

   ![Filtra per scadenza](assets/boards-filter-by-due-date-0822.png)

## Filtrare una bacheca per mostrare le schede archiviate

Per impostazione predefinita, su una bacheca vengono visualizzate solo le schede attive. Puoi filtrare la bacheca per visualizzare anche eventuali schede archiviate.

1. Accedi alla bacheca.
1. Clic [!UICONTROL **Filtro**], espandi [!UICONTROL Schede archiviate] e seleziona **[!UICONTROL Schede archiviate]** per visualizzare le schede archiviate.

   Il filtro mostra il numero di schede archiviate.

   ![Filtra schede archiviate](assets/boards-filter-by-archived-cards_0822.png)

1. Seleziona **[!UICONTROL Schede archiviate]** per cancellare l&#39;opzione e visualizzare solo le schede attive.

## Filtrare una bacheca per connessione

1. Accedi alla bacheca.
1. Clic [!UICONTROL **Filtro**], espandi [!UICONTROL Connessione] e seleziona la sezione [!DNL Workfront] progetti per le schede collegate che si desidera visualizzare.

   È inoltre possibile visualizzare schede non collegate a un progetto.

   ![Filtra per connessione](assets/boards-filter-by-connection.png)

## Ordinare su una bacheca

Quando si seleziona un&#39;opzione in base alla quale eseguire l&#39;ordinamento, vengono ordinate tutte le colonne. Non è possibile ordinare una singola colonna e la colonna backlog o acquisizione non è ordinata.

1. Accedi alla bacheca.
1. Clic [!UICONTROL **Ordina per**] e seleziona [!UICONTROL **Nome**], [!UICONTROL **Data di scadenza**], [!UICONTROL **Stima**], [!UICONTROL **Stato**], o [!UICONTROL **Connessione**].

   La connessione (nome progetto) si applica solo alle schede collegate e le altre opzioni ordinano le schede connesse e quelle ad hoc nelle colonne.

   L’opzione &quot;user order&quot; (Ordine utente) riporta le schede nell’ordine in cui sono state impostate manualmente, prima che venissero applicate altre opzioni di ordinamento. Questo è l’ordinamento predefinito per le colonne.

1. Seleziona [!UICONTROL **Ordine inverso**] per ordinare le colonne in ordine inverso rispetto all&#39;opzione di ordinamento.

   La freccia sull&#39;icona di ordinamento indica se le colonne sono in ordine crescente o decrescente.

   Quando viene applicato un ordinamento diverso da quello predefinito, sull’icona di ordinamento viene visualizzato un indicatore ![Ordinamento applicato](assets/sort-applied-boards.png).

   ![Ordinare per colonne su una bacheca](assets/sort-by-columns-in-board.png)

## Cerca in una bacheca

1. Accedi alla bacheca.
1. Clic [!UICONTROL **Ricerca**] e digita un termine di ricerca. Quindi premere Invio.

   Vengono visualizzate tutte le schede che contengono il termine di ricerca.

   Fare clic sulla X per annullare la ricerca.

   ![Cercare le schede in una bacheca](assets/boards-searchbox.png)
