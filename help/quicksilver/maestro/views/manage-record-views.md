---
title: Gestire le visualizzazioni record
description: È possibile visualizzare i record in una vista tabella o sequenza temporale quando si utilizza Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---


# Gestire le visualizzazioni record

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

Dopo aver selezionato un tipo di record in Adobe Maestro, è possibile visualizzare tutti i record di quel tipo nelle seguenti visualizzazioni:

* Tabella

  Per ulteriori informazioni, consulta [Gestire la vista tabella](../views/manage-the-table-view.md).
* Timeline

  Per ulteriori informazioni, consulta [Gestire la visualizzazione della timeline](../views/manage-the-timeline-view.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> prodotto Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>La tua organizzazione deve essere iscritta al programma beta chiuso Adobe Maestro. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td>
   <td>
   <p>Qualsiasi</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Livello di accesso</td>
   <td> <p>Qualsiasi</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Modello di layout</td>
   <td> <p>L’amministratore di sistema deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/grant-access.md">Concedere l’accesso a Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerazioni durante l’utilizzo delle visualizzazioni Maestro

* Le visualizzazioni in Maestro sono specifiche per il tipo di record. Non è possibile applicare la stessa visualizzazione a due tipi di record diversi.
* Le visualizzazioni create sono visibili a tutti coloro che accedono all’area Maestro. <!-- edit this when we have permissions and the views will be shared only to be visible by others-->
  <!-- this is not yet possible: * You can share views with others if you want them to also apply them to the same record types.-->
* La creazione di viste per i tipi di record operativi è identica alla creazione di viste per i tipi di record della tassonomia.
* Quando modificate o eliminate una vista, questa viene modificata ed eliminata per tutti gli utenti che possono accedere all&#39;area Maestro.
* I seguenti elementi sono specifici per ogni vista in Maestro:

   * Filtro
   * Raggruppamento
   * Ordina

  <!-- some of these are not available in all of the views - edit above-->

  Ad esempio, quando si crea un filtro in una vista tabella, i risultati del filtro sono visibili solo nella vista selezionata e non in tutte le viste elencate nel menu a discesa Vista.

  >[!NOTE]
  >
  > Poiché Maestro è attualmente in stato beta, alcuni elementi di visualizzazione potrebbero non essere disponibili per entrambe le visualizzazioni.


Questo articolo descrive le seguenti informazioni sulle visualizzazioni Maestro:

* [Creare e modificare una vista](#create-or-edit-record-views)
* [Eliminare una visualizzazione](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
  <!--* [Share a view](#share-views) - not possible yet-->

## Somiglianze e differenze tra le viste tabella e timeline

La tabella seguente mostra le somiglianze e le differenze tra le viste tabella e timeline in Maestro:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Funzionalità | Vista tabella | Vista Timeline |
|-----------------------------------------------------------------------|------------|---------------|
| Visualizzare i record in un elenco o in una tabella | ✓ |              |
| Visualizza tutti i campi come colonne nella tabella per impostazione predefinita | ✓ |              |
| Nascondere o mostrare campi o colonne | ✓ |               |
| Modifica i valori dei campi per ogni record | ✓ |               |
| Aggiungere record come nuove righe nella visualizzazione | ✓ |               |
| Aggiungere campi come nuove colonne nella visualizzazione | ✓ |               |
| Copiare le righe da un elenco esterno e incollarle in una tabella | ✓ |               |
| Visualizzare i record in una timeline |            | ✓ |
| Filtra record | ✓ | ✓ |
| Raggruppa record |           | ✓ |
| Ordinare i record | ✓ |              |

<!--| Sort groupings                                                        | ✓          | ✓             |-->

<!--| Display a limited number of fields as columns, by default                      | ✓          |               |-->

<!--| Color-code records                     |           | ✓              |-->
<!--| Color-code groupings                     |           | ✓              |-->

## Creare o modificare le viste {#create-or-edit-views}

1. Fai clic su **Menu principale** icona ![](assets/main-menu-workfront.png) nell’angolo superiore destro <!--or the **Main Menu** icon ![](assets/main-menu-shell.png) in the upper-left corner, if available-->, quindi fai clic su **Maestro** ![](assets/maestro-icon.png).
Per impostazione predefinita, viene aperta l&#39;ultima area di lavoro a cui si è effettuato l&#39;accesso. Per informazioni sulla creazione delle aree di lavoro, consulta [Creare aree di lavoro](../architecture-and-fields/create-workspaces.md).
1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Crea tipi di record](../architecture-and-fields/create-record-types.md).

   Per impostazione predefinita, tutti i record del tipo selezionato vengono visualizzati nella vista tabella.

1. Fai clic su **Visualizza** e selezionare un menu a discesa esistente **Vista tabella** ![](assets/table-view-icon.png) o fai clic su **Crea vista > Tabella** per creare una vista tabella

   Oppure

   Seleziona un elemento esistente **Vista Timeline** ![](assets/timeline-view-icon.png) visualizzare o fare clic su **Crea vista > Timeline** per creare una vista timeline.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    Per creare una visualizzazione timeline, il tipo di record per il quale viene creata la visualizzazione deve avere almeno due campi data. In caso contrario, l&#39;opzione Timeline (Timeline) è disattivata.

1. (Facoltativo) Aggiorna il nome della visualizzazione, quindi fai clic su **Crea** per salvarlo.

   Per impostazione predefinita, Maestro assegna alla vista il nome &quot;Table &lt; number >&quot; o &quot;Timeline &lt; number >&quot;. Il numero è un incremento generato automaticamente.

1. (Facoltativo) Per rinominare una vista dopo la sua creazione, fai clic sul menu a discesa Vista, quindi fai clic su **Altro** menu ![](assets/more-menu.png) > **Rinomina** per aggiornare il nome della vista. <!--ensure there is not another saving step here?!-->
1. (Facoltativo) Per gestire una visualizzazione, vedere i seguenti articoli per ulteriori informazioni:

   * [Gestire la vista tabella](../views/manage-the-table-view.md)
   * [Gestire la visualizzazione della timeline](../views/manage-the-timeline-view.md)


<!--# Add a view as a favorite - this is not possible yet-->

<!-- ## Share views - not possible yet-->

## Eliminare le viste

1. Dalla sezione **Menu principale** ![](assets/main-menu-workfront.png) nell’angolo superiore destro dello schermo, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner of the screen, if available,--> click **Maestro** ![](assets/maestro-icon.png).

   Per impostazione predefinita, viene aperta l&#39;ultima area di lavoro a cui si è effettuato l&#39;accesso. Per informazioni sulla creazione delle aree di lavoro, consulta [Creare aree di lavoro](../architecture-and-fields/create-workspaces.md).
1. Fare clic su una scheda del tipo di record.

   Per informazioni sulla creazione di un tipo di record, vedere [Crea tipi di record](../architecture-and-fields/create-record-types.md).

   Per impostazione predefinita, tutti i record del tipo selezionato vengono visualizzati nella vista tabella.

1. Fai clic sul menu a discesa delle viste, passa il puntatore del mouse su una delle viste nell’elenco, quindi fai clic sul pulsante **Altro** menu ![](assets/more-menu.png) > **Elimina**.
1. Clic **Elimina** per confermare. <!--ensure there is not another saving step here?!-->

   La vista viene eliminata per tutti gli utenti che possono accedere all’area Maestro e non può essere recuperata.

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture-and-fields/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->