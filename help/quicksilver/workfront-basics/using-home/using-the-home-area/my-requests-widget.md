---
product-area: projects
navigation-topic: use-the-home-area
title: Utilizzare il widget Richieste personali
description: È possibile inviare richieste nel widget Richieste personali. Puoi anche personalizzare il widget con filtri e colonne.
author: Becky
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 2fe55f61bd24ebb3ecfe09fff29c4aad2ca33608
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 3%

---

# Utilizzare il widget Richieste personali

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

>[!IMPORTANT]
>
>Questo articolo descrive il nuovo widget Richieste personali. Per visualizzare il nuovo widget, è necessario che sia abilitata la nuova esperienza di richiesta.
>>Puoi abilitare la nuova esperienza di richiesta nell’area Richieste.

Il widget Richieste personali visualizza le richieste inviate all&#39;organizzazione. Puoi filtrare le richieste, cercare richieste specifiche o regolare l’ordine e la visibilità delle colonne. Puoi anche creare una nuova richiesta dal widget Richieste personali.

>[!NOTE]
>
>* Quando viene caricato, il widget Richieste personali visualizza fino a 50 richieste. Per visualizzare altre richieste, scorri l’elenco verso il basso.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Product]</strong></td> 
   <td> <ul><li>Adobe Workfront</li><li>È necessario disporre di Adobe Workfront Planning per visualizzare le richieste o i moduli di richiesta di Planning</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>Nuovo: Collaboratore o versione successiva</p>
   Oppure   
   <p>Corrente: [!UICONTROL Request] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazione del livello di accesso</strong></td> 
   <td> <p>Accesso di visualizzazione o superiore a qualsiasi oggetto per il quale si è taggati in una conversazione o per il quale è necessario risolvere un'approvazione (progetti, attività, problemi, documenti)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Autorizzazioni di [!UICONTROL View] o superiori per progetti, attività, problemi e documenti a cui vengono assegnati tag in una conversazione o in cui è necessario risolvere un'approvazione</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront]. Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una richiesta

È possibile creare una richiesta direttamente dal widget Richieste personali.

Per istruzioni, vedere [Creare una richiesta](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request) nell&#39;articolo Creare elementi di lavoro e progetti dall&#39;area Home.

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
