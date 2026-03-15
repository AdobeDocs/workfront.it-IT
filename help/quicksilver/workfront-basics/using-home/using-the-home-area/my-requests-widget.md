---
product-area: projects
navigation-topic: use-the-home-area
title: Utilizzare il widget Le mie richieste
description: È possibile inviare richieste nel widget Richieste personali. Puoi anche personalizzare il widget con filtri e colonne.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 3893a57fb7ae31a1649b20beccc1f0b79f2421fb
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 8%

---

# Utilizzare il widget Le mie richieste

>[!IMPORTANT]
>
>Questo articolo descrive il nuovo widget Richieste personali. Per visualizzare il nuovo widget, è necessario che sia abilitata la nuova esperienza di richiesta.
>Puoi abilitare la nuova esperienza di richiesta nell’area Richieste.

Il widget Richieste personali visualizza le richieste inviate. Puoi filtrare le richieste, cercare richieste specifiche o regolare l’ordine e la visibilità delle colonne. Puoi anche creare una nuova richiesta dal widget Richieste personali.

>[!NOTE]
>
>* Quando viene caricato, il widget Richieste personali visualizza fino a 50 richieste. Per visualizzare altre richieste, scorri l’elenco verso il basso.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Qualsiasi pacchetto di Workfront o flusso di lavoro</p>
   <p>Qualsiasi pacchetto Workfront Planning per accedere alle richieste Workfront Planning e ai relativi oggetti creati</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza</strong></td> 
   <td> <p>Collaboratore o successiva</p>
   <p>Richiedente o successiva</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>Configurazione del livello di accesso</strong></td> 
   <td> <p>Visualizzare o accedere a un livello superiore a qualsiasi oggetto a cui si è assegnati tag in una conversazione o per il quale è necessario risolvere un'approvazione (progetti, attività, problemi, documenti)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni sugli oggetti</strong></td> 
   <td> <p>Autorizzazioni di [!UICONTROL View] o superiori per progetti, attività, problemi e documenti a cui sono stati aggiunti tag in una conversazione o per i quali è necessario risolvere un'approvazione</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una richiesta

È possibile creare una richiesta direttamente dal widget Richieste personali.

Per istruzioni, vedere la sezione [Creare una richiesta](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md/#create-a-request) nell&#39;articolo [Creare elementi di lavoro e progetti dall&#39;area Home](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Copiare una richiesta

È possibile copiare una richiesta nel widget Richieste personali, modificarla e inviarla come nuova richiesta.

Per istruzioni, consulta [Copiare e inviare richieste](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Filtrare richieste

Il widget Richieste personali dispone di un filtro personalizzabile che consente di controllare quali richieste vengono visualizzate nel widget. Puoi configurare questo filtro per campi e valori diversi e sovrapporre le condizioni utilizzando gli operatori AND e OR.

Per configurare il filtro nel widget Richieste personali:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Per aggiungere il widget **Richieste personali** alla schermata iniziale. Fai clic su **Personalizza** e trova **Le mie richieste**, quindi fai clic su di esso per aggiungerlo a **Home**.
1. Nel widget **Richieste personali**, fare clic su **Filtro**.
1. Seleziona il campo in base al quale desideri filtrare. Le opzioni disponibili sono:

   * Area di lavoro
   * Tipo di oggetto
   * Data inserimento
   * Modulo di richiesta
   * Stato
   * Immesso da
   * Campi personalizzati dalla richiesta o dall&#39;oggetto creato

1. Nel campo successivo, seleziona l’operatore da utilizzare per questa condizione di filtro. Gli operatori disponibili dipendono dal campo scelto.
1. (Condizionale) Se a destra dell’operatore viene visualizzato un campo, seleziona il valore in base al quale desideri filtrare.
1. (Facoltativo) Per aggiungere un&#39;altra condizione di filtro, fare clic su **Aggiungi condizione** e ripetere i passaggi 4-6.
1. (Facoltativo e condizionale) Se sono presenti più condizioni, cambiare il valore And o Or facendo clic su **And** o **Or** a sinistra della condizione.

Il filtro viene salvato automaticamente.

>[!TIP]
>
>Se l&#39;organizzazione ha acquistato Workfront Planning oltre ad Adobe Workfront, il widget Richieste personali includerà le richieste Workfront e Workfront Planning.
> 
>* Per filtrare solo le richieste Workfront, impostare il filtro su **Tipo di oggetto** > **Con uno dei** > **Problemi**.
>* Per filtrare solo le richieste di Workfront Planning, impostare il filtro su **Tipo di oggetto** > **Non presenta** > **Problemi**.

## Regolare o aggiungere colonne

È possibile scegliere le colonne disponibili da visualizzare nel widget Richieste personali e impostarne l&#39;ordine.

Le colonne disponibili includono:

* Soggetto
* Oggetto creato
* Tipo di oggetto
* Stato
* Modulo di richiesta
* Data inserimento
* Immesso da

Per regolare le colonne del widget Richieste personali:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Per aggiungere il widget **Richieste personali** alla schermata iniziale. Fai clic su **Personalizza** e trova **Le mie richieste**, quindi fai clic su di esso per aggiungerlo alla **Home**.
1. Nel widget **Richieste personali**, fare clic su **Colonne**.
1. (Facoltativo) Per riordinare le colonne, fare clic sull&#39;handle di trascinamento ![handle di trascinamento](assets/drag-handle.png) della colonna che si desidera spostare e trascinarlo nelle posizioni desiderate. La colonna nella parte superiore dell&#39;elenco viene visualizzata nel widget Richieste personali come prima colonna.
1. (Facoltativo) Utilizza l’interruttore per nascondere o mostrare la colonna nell’elenco delle richieste.
1. Per aggiungere un campo personalizzato come colonna, fai clic sull&#39;icona **Aggiungi colonna** ![Aggiungi colonna](assets/add-column.png) nell&#39;angolo superiore destro dell&#39;elenco, quindi fai clic sull&#39;icona più accanto al campo personalizzato che desideri aggiungere come colonna al widget.

   I campi personalizzati nei moduli allegati all’oggetto nell’elenco sono disponibili per l’aggiunta come colonne.

Le preferenze delle colonne vengono salvate automaticamente.

## Creare una vista

È possibile creare visualizzazioni nel widget Richieste personali per modificare il modo in cui vengono visualizzate le informazioni nell&#39;elenco delle richieste.

Quando si utilizzano le visualizzazioni nel widget Richieste personali, tenere presente quanto segue:

* Una vista nel widget Richieste personali contiene le colonne e i filtri applicati alla vista.
* Potete creare viste e condividerle con altri utenti. I filtri e le colonne selezionati per la visualizzazione prima della condivisione vengono inclusi nelle visualizzazioni condivise.
* Di seguito è riportata una vista di sistema che non è possibile modificare, condividere o eliminare:

   * Visualizzazione predefinita richieste unificate widget
* La creazione e la modifica di una visualizzazione nel widget Richieste personali è simile a quella degli elenchi avanzati. Per informazioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Cerca richieste

Per cercare richieste specifiche nel widget Richieste personali:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Per aggiungere il widget **Richieste personali** alla schermata iniziale. Fai clic su **Personalizza** e trova **Le mie richieste**, quindi fai clic su di esso per aggiungerlo alla **Home**.
1. Nella barra di ricerca in alto a destra del widget Richieste personali, immettere il termine che si desidera cercare.

   Le richieste che contengono il termine vengono evidenziate in arancione.

1. (Facoltativo) Per passare alle richieste evidenziate, fai clic sulle frecce su o giù nella barra di ricerca.

## Passare a un oggetto creato da una richiesta

È possibile trovare gli oggetti creati da una richiesta nel widget Richieste personali.

>[!NOTE]
>
>I collegamenti agli oggetti creati sono disponibili nella nuova esperienza di richiesta solo per le richieste di Planning, nei casi in cui la richiesta stessa abbia creato un oggetto. Se una richiesta di Workfront viene convertita in un progetto o in un altro oggetto, il collegamento all’oggetto convertito non è disponibile nell’elenco delle richieste nella nuova esperienza.

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Per aggiungere il widget **Richieste personali** alla schermata iniziale. Fai clic su **Personalizza** e trova **Le mie richieste**, quindi fai clic su di esso per aggiungerlo a **Home**.
1. Individuare la richiesta che ha creato l&#39;oggetto.
1. Fare clic sul nome dell&#39;oggetto nella colonna **Oggetto creato** per la richiesta.

   Viene visualizzata la pagina dell&#39;oggetto.

