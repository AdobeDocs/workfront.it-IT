---
product-area: requests
navigation-topic: create-requests
title: Creare viste nell’area Richieste
description: Se utilizzi la nuova esperienza di richiesta, puoi creare e salvare viste per l’area Richieste.
author: Becky
feature: Work Management
source-git-commit: 1c7e2fb7de500083f0f7e42f1016323305054d88
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Creare o modificare le viste nell’area Richieste

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambiente Sandbox di anteprima.</span>

Se utilizzi la nuova esperienza di richiesta, puoi creare e salvare viste per l’area Richieste. Queste visualizzazioni includono filtri e disposizioni per le colonne.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.


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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Collaboratore o versione successiva</p>
   <p>Richiedi o superiore</p>
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

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una vista nell’area Richieste

{{step1-to-requests}}

1. (Facoltativo e condizionale) Seleziona l&#39;impostazione **Passa alla nuova esperienza** in alto a destra dello schermo, se all&#39;organizzazione e all&#39;istanza di Workfront si applicano le seguenti condizioni:

   * La tua organizzazione ha acquistato un pacchetto Workfront
   * La tua organizzazione è stata integrata in Adobe Unified Experience.
   * L&#39;amministratore ti ha concesso l&#39;accesso a Workfront Planning
   * Si dispone almeno delle autorizzazioni di visualizzazione per un&#39;area di lavoro di Workfront Planning

   Per ulteriori informazioni, vedere [Inviare le richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md)

1. Fai clic sul menu a discesa **Viste** ![Viste](assets/view-icon-requests.png) e seleziona **Nuova vista**.

   ![Nuova visualizzazione](assets/create-new-view.png)

1. Immettere un nome per la nuova visualizzazione e fare clic su **Crea**.
1. Continuare a [Modificare una visualizzazione nell&#39;area Richieste](#edit-a-view-in-the-requests-area).

## Modificare una vista nell’area Richieste

È possibile modificare le viste esistenti, incluse quelle appena create.

{{step1-to-requests}}

1. (Facoltativo e condizionale) Seleziona l&#39;impostazione **Passa alla nuova esperienza** in alto a destra dello schermo, se all&#39;organizzazione e all&#39;istanza di Workfront si applicano le seguenti condizioni:

   * La tua organizzazione ha acquistato un pacchetto Workfront
   * La tua organizzazione è stata integrata in Adobe Unified Experience.
   * L&#39;amministratore ti ha concesso l&#39;accesso a Workfront Planning
   * Si dispone almeno delle autorizzazioni di visualizzazione per un&#39;area di lavoro di Workfront Planning

   Per ulteriori informazioni, vedere [Inviare le richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md)1.

1. (Facoltativo) Per rinominare una visualizzazione, fai clic sul menu a discesa **Visualizzazioni** ![Visualizzazioni](assets/view-icon-requests.png) e fai clic sul menu a tre punti accanto alla visualizzazione, seleziona **Rinomina**, quindi digita il nuovo nome per la visualizzazione.
1. Fai clic sul menu a discesa **Viste** ![Viste](assets/view-icon-requests.png) e seleziona la vista da modificare.
1. (Facoltativo) Fai clic su **Filtri** e inizia ad aggiungere le condizioni per le richieste che desideri visualizzare nella scheda Planning.

   ![Modifica dei filtri nella scheda Richieste di Planning](assets/filters-editing-box-in-requests-planning-tab.png)

   Puoi filtrare in base ai seguenti campi:

   * **Workspace**: area di lavoro a cui è associato il modulo di richiesta.
   * **Tipo di record**: il tipo di record a cui è associato il modulo di richiesta.
   * **Data di ingresso**: la data in cui la richiesta è stata inviata.
   * **Modulo di richiesta**: nome del modulo di richiesta utilizzato per inviare la richiesta.
   * **Stato**: lo stato della richiesta.
   * **Inserito da**: nome dell&#39;utente che ha aggiunto la richiesta. Se la richiesta è stata aggiunta da un utente esterno a Workfront, il campo **Immesso da** visualizza `N/A`.

   È possibile unire più filtri con **And** o **Or**.
L’elenco delle richieste viene filtrato automaticamente, man mano che aggiungi le condizioni del filtro.

1. (Facoltativo) Fai clic su **Colonne** e nascondi, mostra o ridisponi le colonne nell&#39;elenco richieste.

   ![Casella Colonne](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >Impossibile aggiungere altre colonne.

>[!IMPORTANT]
>
> * Le modifiche alle viste vengono salvate automaticamente.
> * Le modifiche apportate alle viste sono visibili a tutti gli utenti della vista.

## Aggiungere la visualizzazione a un modello di layout.

Un amministratore Workfront può aggiungere la nuova visualizzazione ai modelli di layout.

Per istruzioni, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).
