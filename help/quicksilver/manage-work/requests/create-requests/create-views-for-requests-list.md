---
product-area: requests
navigation-topic: create-requests
title: Creare e gestire le viste nell’area Richieste
description: Se utilizzi la nuova esperienza di richiesta, puoi creare e salvare viste per l’area Richieste.
author: Becky
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: 8db8382d63d06c23f93a74a326ddb0e1227f44c8
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 9%

---


# Creare e gestire le viste nell’area Richieste

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span>

-->

Se utilizzi la nuova esperienza di richiesta, puoi creare e salvare viste per l’area Richieste. Queste visualizzazioni includono filtri e disposizioni per le colonne. <!--<span class="preview"> and groupings.</span> -->

Le visualizzazioni possono essere create e gestite nell’area Richieste di Workfront.

>[!IMPORTANT]
>
>* Questa funzionalità è disponibile solo nella nuova esperienza di richiesta.
>* Le impostazioni di visualizzazione non sono disponibili nel widget Richieste personali nella Home.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Collaboratore o successiva</p>
   <p>Richiedente o successiva</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p>  <p>Per aggiungere visualizzazioni ai modelli di layout è necessario essere un amministratore Workfront</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Prodotto</td> 
   <td> <ul><li>Adobe Workfront</li><li>È necessario disporre di Adobe Workfront Planning per visualizzare le richieste o i moduli di richiesta di Planning</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una visualizzazione per le richieste

Puoi creare una vista nell’area Richieste di Workfront,.

1. Per accedere all’elenco Richieste:

   {{step1-to-requests}}

1. Nell&#39;elenco Richieste fare clic sul menu a discesa **Visualizzazioni** ![Visualizzazioni](assets/view-icon-requests.png) e selezionare **Nuova visualizzazione**.

   ![Nuova visualizzazione](assets/create-new-view.png)

1. Immettere un nome per la nuova visualizzazione e fare clic su **Crea**.
1. Continuare a [Modificare una visualizzazione nell&#39;area Richieste](#edit-a-view-in-the-requests-area).

## Modificare una visualizzazione per le richieste

È possibile modificare le viste esistenti, incluse quelle appena create.

1. Per accedere all’elenco Richieste:

   {{step1-to-requests}}
1. Nell&#39;elenco Richieste individuare la visualizzazione da modificare.

1. (Facoltativo) Per rinominare una visualizzazione, fai clic sul menu a discesa **Visualizzazioni** ![Visualizzazioni](assets/view-icon-requests.png) e fai clic sul menu a tre punti accanto alla visualizzazione, seleziona **Rinomina**, quindi digita il nuovo nome per la visualizzazione.
1. Fai clic sul menu a discesa **Viste** ![Viste](assets/view-icon-requests.png) e seleziona la vista da modificare.
1. Per aggiungere un campo personalizzato come colonna, fai clic sull&#39;icona **Aggiungi colonna** ![Aggiungi colonna](assets/add-column.png) a destra dello schermo e fai clic sull&#39;icona più (+) accanto al campo del modulo personalizzato che desideri aggiungere come colonna alla visualizzazione.

   >I campi personalizzati nei moduli allegati all’oggetto nell’elenco sono disponibili per l’aggiunta come colonne.

   >[!TIP]
   >
   >Al momento non è possibile aggiungere colonne nell’ambiente di produzione.
1. (Facoltativo) Fai clic su **Colonne** e nascondi, mostra o ridisponi le colonne nell&#39;elenco richieste.

1. (Facoltativo) Fai clic su **Filtri** e inizia ad aggiungere le condizioni per le richieste che desideri visualizzare.

   Puoi filtrare in base ai seguenti campi:

   * **Workspace**: area di lavoro a cui è associato il modulo di richiesta.
   * **Tipo di record**: il tipo di record a cui è associato il modulo di richiesta.
   * **Data di ingresso**: la data in cui la richiesta è stata inviata.
   * **Modulo di richiesta**: nome del modulo di richiesta utilizzato per inviare la richiesta.
   * **Stato**: lo stato della richiesta.
   * **Inserito da**: nome dell&#39;utente che ha aggiunto la richiesta. Se la richiesta è stata aggiunta da un utente esterno a Workfront, il campo **Immesso da** visualizza `N/A`.

   È inoltre possibile filtrare in base a qualsiasi campo personalizzato aggiunto alla visualizzazione.

   È possibile unire più filtri con **And** o **Or**.
L’elenco delle richieste viene filtrato automaticamente, man mano che aggiungi le condizioni del filtro.


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Le modifiche alle viste vengono salvate automaticamente.
> * Le modifiche apportate alle viste sono visibili a tutti gli utenti della vista.
> * Per fare in modo che la visualizzazione venga applicata alla persona che la utilizza, indipendentemente da chi l&#39;ha creata, è possibile utilizzare il carattere jolly del filtro &quot;Utente connesso&quot; in qualsiasi campo il cui valore sia impostato su Utenti.

## Aggiungere la visualizzazione a un modello di layout.

Un amministratore di Workfront può aggiungere la nuova visualizzazione ai modelli di layout.

Per istruzioni, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Condividere una visualizzazione

Puoi condividere le viste create con altri utenti, team o gruppi.

1. Per accedere all’elenco Richieste:

   {{step1-to-requests}}

1. Nell&#39;elenco Richieste individuare la visualizzazione da condividere.
1. Passa il puntatore del mouse sulla vista da condividere, quindi fai clic sul menu a tre punti quando viene visualizzato.
1. Seleziona **Condividi**.
1. Nella finestra di dialogo visualizzata, immetti i nomi degli utenti, dei team o dei gruppi con cui desideri condividere la visualizzazione, quindi selezionali dall’elenco quando vengono visualizzati.
1. Fai clic su **Salva**.
