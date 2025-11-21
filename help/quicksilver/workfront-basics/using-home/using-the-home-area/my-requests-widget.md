---
product-area: projects
navigation-topic: use-the-home-area
title: Utilizzare il widget Richieste personali
description: È possibile inviare richieste nel widget Richieste personali. Puoi anche personalizzare il widget con filtri e colonne.
author: Becky
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 59a53f7355032810a05fce2d3f0dfe30d64bbd40
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 5%

---

# Utilizzare il widget Richieste personali

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambiente Sandbox di anteprima.</span>

>[!IMPORTANT]
>
>Questo articolo descrive il nuovo widget Richieste personali. Per visualizzare il nuovo widget, è necessario che sia abilitata la nuova esperienza di richiesta.
>Puoi abilitare la nuova esperienza di richiesta nell’area Richieste.

Il widget Richieste personali visualizza le richieste inviate all&#39;organizzazione. Puoi filtrare le richieste, cercare richieste specifiche o regolare l’ordine e la visibilità delle colonne. Puoi anche creare una nuova richiesta dal widget Richieste personali.

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
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza</strong></td> 
   <td> <p>Collaboratore o versione successiva</p>
   <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
    <tr> 
   <td role="rowheader"><strong>Prodotti aggiuntivi</strong></td> 
   <td> È necessario disporre di Adobe Workfront Planning per visualizzare le richieste o i moduli di richiesta di Planning</td> 
  </tr> 
   <td role="rowheader"><strong>Configurazione del livello di accesso</strong></td> 
   <td> <p>Accesso di visualizzazione o superiore a qualsiasi oggetto per il quale si è taggati in una conversazione o per il quale è necessario risolvere un'approvazione (progetti, attività, problemi, documenti)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Autorizzazioni di [!UICONTROL View] o superiori per progetti, attività, problemi e documenti a cui vengono assegnati tag in una conversazione o in cui è necessario risolvere un'approvazione</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crea una nuova richiesta

È possibile creare una richiesta direttamente dal widget Richieste personali.

Per istruzioni, vedere [Creare una richiesta](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request) nell&#39;articolo Creare elementi di lavoro e progetti dall&#39;area Home.

<div class="preview">

## Copiare una richiesta

È possibile copiare una richiesta nel widget Richieste personali, modificarla e inviarla come nuova richiesta.

Per istruzioni, consulta [Copiare e inviare richieste nella nuova esperienza di richiesta](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md#copy-and-submit-requests-in-the-new-requesting-experience) nell&#39;articolo Copiare e inviare richieste.

</div>

## Filtrare richieste

Il widget Richieste personali dispone di un filtro personalizzabile che consente di controllare quali richieste vengono visualizzate nel widget. Puoi configurare questo filtro per campi e valori diversi e sovrapporre le condizioni utilizzando gli operatori AND e OR.

Per configurare il filtro nel widget Richieste personali:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Per aggiungere il widget **Richieste personali** alla schermata iniziale. Fai clic su **Personalizza** e trova **Le mie richieste**.
1. Nel widget Richieste personali, fare clic su **Filtro**.
1. Nel campo più a sinistra, seleziona in base a cosa desideri filtrare. Le opzioni disponibili sono:

   * Area di lavoro
   * Tipo di oggetto
   * Data inserimento
   * Modulo di richiesta
   * Stato
   * Immesso da

1. Nel campo successivo, seleziona l’operatore da utilizzare per questa condizione di filtro. Gli operatori disponibili dipendono dal campo scelto.
1. (Condizionale) Se a destra dell’operatore viene visualizzato un campo, seleziona il valore in base al quale desideri filtrare.
1. (Facoltativo) Per aggiungere un&#39;altra condizione di filtro, fare clic su **Aggiungi condizione** e ripetere i passaggi 4-6.
1. (Facoltativo e condizionale) Se sono presenti più condizioni, cambiare il valore And o Or facendo clic su **And** o **Or** a sinistra della condizione.

Il filtro viene salvato automaticamente.

>[!TIP]
>
>Se l&#39;organizzazione ha acquistato Workfront Planning, il widget Richieste personali includerà le richieste Workfront e Workfront Planning.
> 
>* Per filtrare solo le richieste Workfront, impostare il filtro su **Tipo di oggetto** > **Ha uno di** > **Problemi**.
>* Per filtrare solo le richieste di Workfront Planning, impostare il filtro su **Tipo di oggetto** > **Non contiene** > **Problemi**.

## Regola colonne

È possibile scegliere quale delle colonne disponibili visualizzare nel widget Richieste personali e impostarne l&#39;ordine.

Le colonne disponibili includono:

* Oggetto
* Oggetto creato
* Tipo di oggetto
* Stato
* Modulo di richiesta
* Data inserimento
* Immesso da

Per regolare le colonne del widget Richieste personali:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Per aggiungere il widget **Richieste personali** alla schermata iniziale. Fai clic su **Personalizza** e trova **Le mie richieste**.
1. Nel widget Richieste personali, fare clic su **Colonne**.
1. (Facoltativo)Per riordinare le colonne, fare clic sul quadratino di trascinamento ![trascinamento](assets/drag-handle.png) della colonna che si desidera spostare e trascinarlo nelle posizioni desiderate. La colonna nella parte superiore dell&#39;elenco viene visualizzata nel widget Richieste personali come colonna all&#39;estrema sinistra.
1. (Facoltativo) Utilizza l&#39;interruttore per controllare se una colonna viene visualizzata nel widget Richieste personali.

Le preferenze di colonna vengono salvate automaticamente.

## Richieste di ricerca

Per cercare richieste specifiche nel widget Richieste personali:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Per aggiungere il widget **Richieste personali** alla schermata iniziale. Fai clic su **Personalizza** e trova **Le mie richieste**.
1. Nella barra di ricerca in alto a destra del widget Richieste personali, immettere il termine che si desidera cercare.

   Le richieste che contengono il termine vengono evidenziate in arancione.

1. (Facoltativo) Per passare alle richieste evidenziate, fai clic sulle frecce su o giù nella barra di ricerca.
