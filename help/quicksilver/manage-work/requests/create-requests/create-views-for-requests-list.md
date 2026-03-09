---
product-area: requests
navigation-topic: create-requests
title: Creare e gestire le viste nell’area Richieste
description: Se utilizzi la nuova esperienza di richiesta, puoi creare e salvare viste per l’area Richieste.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: e4d57d0b5042dc4889d5b676396b56c05ab1515d
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 7%

---


# Creare e gestire le viste nell’area Richieste

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>





Se utilizzi la nuova esperienza di richiesta in Adobe Workfront, puoi creare e salvare viste per l’area Richieste. Queste visualizzazioni includono filtri e disposizioni per le colonne.

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* Questa funzionalità è disponibile solo nella nuova esperienza di richiesta nell’area Richieste.
>* Le impostazioni di visualizzazione sono disponibili anche nel widget Richieste personali nella Home. Tuttavia, le viste dall’area Richieste sono separate da quelle del widget Richieste personali.
>* L’elenco delle richieste nell’area Richieste utilizza l’elenco avanzato in Workfront. Per ulteriori informazioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

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

Puoi creare una visualizzazione nell’area Richieste di Workfront quando utilizzi la nuova esperienza Richieste.

1. Per accedere all’elenco Richieste:

   {{step1-to-requests}}

1. Verificare che l&#39;impostazione **Usa nuova esperienza** sia attivata.

1. Nell&#39;elenco **Richieste**, fare clic sul menu a discesa **Visualizzazioni** ![Visualizzazioni](assets/view-icon-requests.png) e fare clic su **Nuova visualizzazione**.

   ![Nuova visualizzazione](assets/create-new-view.png)

1. Immettere un nome per la nuova visualizzazione e fare clic su **Crea**.
1. Continuare a [Modificare una visualizzazione nell&#39;area Richieste](#edit-a-view-in-the-requests-area).

## Modificare una visualizzazione per le richieste

Puoi modificare le viste esistenti, comprese quelle appena create, nell’area Richieste di Workfront.

Modificando una vista nell&#39;area Richieste, è possibile modificare i seguenti elementi della vista:

* Nome
* Filtri
* Colonne

Le modifiche apportate a una visualizzazione sono visibili a tutti gli utenti con cui la si condivide.

1. Per accedere a un elenco di richieste nelle Richieste:

   {{step1-to-requests}}

1. Verificare che l&#39;impostazione **Usa nuova esperienza** sia attivata.
1. Nell&#39;elenco **Richieste** individuare la visualizzazione che si desidera modificare dal menu a discesa **Visualizzazioni** ![Visualizzazioni](assets/view-icon-requests.png).

1. Fai clic sul menu a discesa **Visualizzazioni** ![Visualizzazioni](assets/view-icon-requests.png) e fai clic sul menu a tre punti accanto alla visualizzazione, seleziona **Rinomina**, quindi digita il nuovo nome per la visualizzazione.
1. Premi Invio per salvare il nuovo nome.
1. Fai clic sul menu a discesa **Viste** ![Viste](assets/view-icon-requests.png) e seleziona la vista da modificare.
1. Per aggiungere un campo come colonna, fare clic sull&#39;icona **Aggiungi colonna** ![Aggiungi colonna](assets/add-column.png) nell&#39;angolo superiore destro dell&#39;elenco.

   Verrà aperto **Gestione colonne**.
1. Fai clic sull&#39;icona più accanto al campo che desideri aggiungere come colonna alla visualizzazione, quindi fai clic su **Salva**.

   I campi associati agli oggetti nell&#39;elenco sono disponibili per l&#39;aggiunta come colonne. <!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >I campi aggiunti alle colonne devono esistere prima che siano disponibili nel **Gestione colonne**.


1. (Facoltativo) Fai clic su **Colonne** per aprire la casella F **ields visibility and order**.
1. Attivare l&#39;impostazione di ogni campo che si desidera visualizzare nell&#39;elenco, disattivarla per nasconderla oppure trascinare i campi in un ordine diverso.

1. (Facoltativo) Fai clic su **Filtri** e inizia ad aggiungere le condizioni per le richieste che desideri visualizzare.

   Puoi filtrare in base ai seguenti campi di richiesta:

   * **Workspace**: area di lavoro a cui è associato il modulo di richiesta.
   * **Tipo di oggetto**: tipo di record a cui è associato il modulo di richiesta.
   * **Data di ingresso**: la data in cui la richiesta è stata inviata.
   * **Modulo di richiesta**: nome del modulo di richiesta utilizzato per inviare la richiesta.
   * **Stato**: lo stato della richiesta.
   * **Inserito da**: nome dell&#39;utente che ha aggiunto la richiesta. Se la richiesta è stata aggiunta da un utente esterno a Workfront, il campo **Immesso da** visualizza `N/A`.

   È inoltre possibile filtrare in base a qualsiasi campo aggiunto alla visualizzazione per qualsiasi oggetto visibile nella visualizzazione.

   È possibile unire più filtri con **And** o **Or**.
L’elenco delle richieste viene filtrato automaticamente, man mano che aggiungi le condizioni del filtro.


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Le modifiche alle viste vengono salvate automaticamente.
> * Le modifiche apportate alle viste sono visibili a tutti gli utenti della vista.
> * Utilizza il carattere jolly del filtro **Me (utente connesso)** in qualsiasi campo il cui valore è utenti.

## Aggiungi la vista richieste a un modello di layout.

Un amministratore di Workfront può aggiungere la nuova visualizzazione ai modelli di layout.

Per istruzioni, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Condividere una visualizzazione

Puoi condividere le viste create con altri utenti, team o gruppi.

1. Per accedere a un elenco di richieste nelle Richieste:

   {{step1-to-requests}}

1. Verificare che l&#39;impostazione **Usa nuova esperienza** sia attivata.
1. Nell&#39;elenco **Richieste** individuare la visualizzazione che si desidera condividere.
1. Passa il puntatore del mouse sulla visualizzazione da condividere, quindi fai clic sul menu a tre punti a destra del nome della visualizzazione, quindi fai clic su **Condividi**.
1. Nella casella **Condividi** immettere le persone, i team, i ruoli, i gruppi o le società con cui si desidera condividere la visualizzazione, quindi selezionarli dall&#39;elenco quando vengono visualizzati.
1. Fai clic su **Salva**.

   La vista viene condivisa con le entità indicate. Possono visualizzare gli elementi della vista aggiornati che hai modificato per la vista prima di condividerla. <span class="preview">Se aggiorna la visualizzazione, le modifiche apportate non saranno visibili agli altri utenti, a meno che non creino una copia della stessa visualizzazione e non mantengano le modifiche prima di condividere la copia. Per ulteriori informazioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
