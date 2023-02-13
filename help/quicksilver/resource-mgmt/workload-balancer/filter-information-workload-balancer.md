---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Filtrare le informazioni nel servizio di bilanciamento del carico di lavoro
description: Per trovare in modo efficiente gli elementi di lavoro e concentrarsi sugli utenti o sugli elementi gestiti, si consiglia vivamente di utilizzare i filtri nel servizio di bilanciamento del carico di lavoro.
author: Alina
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: 10b905c8a66f2507cbfac7c15a01f38d40ab3e00
workflow-type: tm+mt
source-wordcount: '2466'
ht-degree: 0%

---

# Filtrare le informazioni nel servizio di bilanciamento del carico di lavoro

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

In qualità di gestore delle risorse, puoi utilizzare il servizio di bilanciamento del carico di lavoro per visualizzare e gestire il carico di lavoro degli utenti. Per informazioni più generali sul servizio di bilanciamento del carico di lavoro, consulta i seguenti articoli:

* [Panoramica del servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Per trovare in modo efficiente gli elementi di lavoro e concentrarsi sugli utenti o sugli elementi gestiti, si consiglia vivamente di utilizzare i filtri nel servizio di bilanciamento del carico di lavoro. In questo modo è possibile visualizzare le informazioni corrette prima di iniziare a gestire le assegnazioni delle risorse.
>
>Quando salvi e applichi un nuovo filtro e poi ti allontani dal servizio di bilanciamento del carico di lavoro, il filtro viene mantenuto anche dopo la disconnessione e l’accesso.


Questo articolo contiene informazioni sui filtri nel servizio di bilanciamento del carico di lavoro. Per informazioni sui filtri in Workfront, vedi [Panoramica sui filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Pianificare, quando si utilizza il servizio di bilanciamento del carico di lavoro per un team o nell'area di determinazione origine </p>
   <p>Operazioni da eseguire quando si utilizza il servizio di bilanciamento del carico di lavoro di un progetto </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Visualizza o accedi di più a quanto segue:</p> 
    <ul> 
     <li> <p>Gestione risorse</p> </li> 
     <li> <p>Progetti</p> </li> 
     <li> <p>Attività</p> </li> 
     <li> <p>Problemi</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Filtri, visualizzazioni e raggruppamenti</p> </li> 
    </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>Modificare l’accesso a Filtri, Visualizzazioni e Gruppi durante la creazione o la modifica di filtri</span> </p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per progetti, attività, problemi</p>
   <p>Gestisci le autorizzazioni per i filtri che desideri modificare o eliminare</p>
     </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Panoramica dei filtri nel load balancer

Quando si lavora con i filtri nel bilanciamento del carico di lavoro, considera quanto segue:

* A seconda di dove accedi al servizio di bilanciamento del carico di lavoro, Workfront potrebbe già filtrare le informazioni per tuo conto. Per informazioni sui filtri preapplicati, consulta la sezione . [Filtri preapplicati nel load balancer](#pre-applied-filters-in-the-workload-balancer) in questo articolo.
* È possibile creare e applicare un filtro senza salvarlo oppure salvare un filtro da riutilizzare in un secondo momento.
* Quando applichi un filtro senza salvarlo, puoi ripristinare gli elenchi originali aggiornando la pagina.
* Puoi visualizzare i filtri creati o quelli che altri utenti hanno creato e condiviso con te.
* Quando elimini o modifichi un filtro condiviso, il filtro viene anche eliminato o modificato per tutti gli utenti con cui è condiviso.
* Quando crei filtri nel servizio di bilanciamento del carico di lavoro in un’area, questi non sono disponibili in altre aree.

   Ad esempio, i filtri creati nell’area Origine non sono disponibili nel servizio di bilanciamento del carico di lavoro di un progetto o di un team.

   Per informazioni su dove individuare il servizio di bilanciamento del carico di lavoro, consulta [Individua il servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* È possibile visualizzare solo gli elementi che corrispondono ai filtri selezionati e che corrispondono anche alle date all’interno della timeline visualizzata sullo schermo del servizio di bilanciamento del carico di lavoro.

## Filtri preapplicati nel load balancer {#pre-applied-filters-in-the-workload-balancer}

Il servizio di bilanciamento del carico di lavoro visualizza le informazioni in due aree distinte:

* **Area di lavoro non assegnata**: elementi di lavoro non ancora assegnati agli utenti.
* **Area di lavoro assegnata**: elementi di lavoro assegnati agli utenti.

   Per informazioni sugli elementi visualizzati in ciascuna area, consulta [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>Ogni area del bilanciamento del carico di lavoro dispone di un proprio set di filtri che funzionano in modo indipendente l’una dall’altra. È necessario configurare entrambi i filtri per indicare le informazioni che si desidera visualizzare in ogni area.

Il servizio di bilanciamento del carico di lavoro visualizza gli utenti e i relativi elementi di lavoro.
Gli elementi di lavoro assegnati agli utenti vengono visualizzati solo quando le date degli elementi corrispondono all&#39;intervallo di tempo visualizzato sullo schermo.

A seconda della posizione di accesso al servizio di bilanciamento del carico di lavoro, le aree non assegnate e assegnate vengono già filtrate in base a determinati criteri, come descritto nella tabella seguente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Area Workfront in cui si accede al servizio di bilanciamento del carico di lavoro</strong></td> 
   <td><b>Elementi visualizzati per impostazione predefinita nell'area di lavoro non assegnata</b> </td> 
   <td><b>Elementi visualizzati per impostazione predefinita nell'area Lavoro assegnato</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">L'area Risorse</td> 
   <td>Per impostazione predefinita non viene visualizzato alcun elemento. È necessario personalizzare i filtri per visualizzare gli elementi di lavoro in questa area.</td> 
   <td>Utenti membri di qualsiasi team e relativi elementi di lavoro. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un team</td> 
   <td>Elementi di lavoro assegnati al team o al team e un ruolo di lavoro. </td> 
   <td> <p>Utenti membri del team selezionato e relativi elementi di lavoro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un progetto</td> 
   <td> <p>In questa area vengono visualizzati gli elementi di lavoro non assegnati o assegnati a team o ruoli di lavoro nel progetto selezionato.</p> </td> 
   <td> <p>Utenti assegnati ad almeno un elemento di lavoro nel progetto selezionato e ai relativi elementi di lavoro nel progetto quando il filtro predefinito del sistema <b>Elementi di lavoro di questo progetto</b> è selezionato. </p>

<p>Quando il filtro predefinito del sistema <b>Elementi di lavoro di questo progetto</b> deselezionata, l’area Lavoro assegnato di un progetto visualizza tutti gli elementi di lavoro degli utenti assegnati ad almeno un elemento del progetto selezionato.  </p> Questo filtro è deselezionato per impostazione predefinita.

<b>NOTA</b>
<p>Puoi abilitare l’opzione Mostra tutti gli utenti nel servizio di bilanciamento del carico di lavoro di un progetto per visualizzare tutti gli utenti nel sistema. Per ulteriori informazioni, consulta <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Naviga nel bilanciamento del carico di lavoro</a></p>

</td> 
  </tr> 
 </tbody> 
</table>

## Creare filtri di bilanciamento del carico di lavoro

Il processo per la creazione di filtri per le aree Lavoro non assegnato e Lavoro assegnato nel servizio di bilanciamento del carico di lavoro è identico, indipendentemente da dove si accede al servizio di bilanciamento del carico di lavoro. Per informazioni su come individuare il servizio di bilanciamento del carico di lavoro, vedi [Individua il servizio di bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

Puoi creare un filtro da zero o modificare uno dei filtri predefiniti. Per informazioni sui filtri esistenti modificabili, consulta la sezione [Modificare un filtro esistente nel servizio di bilanciamento del carico di lavoro](#edit-an-existing-filter-in-the-workload-balancer) in questo articolo.

1. Passa al servizio di bilanciamento del carico di lavoro.

   Per informazioni sull&#39;accesso al load balancer, vedi [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Fai clic sul pulsante **Filtro** icona ![](assets/filter-icon.png) nell&#39;angolo superiore destro di **Lavoro non assegnato** o **Lavoro assegnato** aree.

   La casella del generatore di filtri viene visualizzata a destra. Il nome dell’area per la quale si crea il filtro viene visualizzato nell’intestazione della casella.

   ![](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. (Facoltativo e condizionale) Se si accede al servizio di bilanciamento del carico di lavoro nell&#39;area Determinazione origine, il filtro predefinito potrebbe essere già applicato all&#39;area Lavoro assegnato. Puoi modificare e salvare una copia del filtro Predefinito.

   >[!TIP]
   >
   >Il filtro Predefinito visualizza gli utenti che appartengono a uno qualsiasi dei tuoi team e dei loro elementi di lavoro. Puoi modificare una copia di questo filtro.

   Se si accede al [!UICONTROL Bilanciamento del carico di lavoro] da un progetto, il[!UICONTROL Elementi di lavoro di questo progetto]&quot; filtro già applicato. In questo modo vengono visualizzati solo gli elementi di lavoro assegnati agli utenti di questo progetto. Puoi duplicare e salvare una copia di questo filtro.

   Per impostazione predefinita, la [!UICONTROL Bilanciamento del carico di lavoro] di un progetto visualizza tutti gli elementi di lavoro assegnati a tutti gli utenti del progetto.


1. Fai clic su **Nuovo filtro.**

   ![](assets/new-filters-empty-panel-workload-balancer-350x460.png)

1. Per creare un filtro, procedi come segue:

   1. Seleziona un nome di campo nel primo menu a discesa o fai clic su **Campi di ricerca** per iniziare a digitare il nome di un campo che non viene visualizzato per impostazione predefinita.

      >[!IMPORTANT]
      >
      >Quando si fa riferimento a campi personalizzati, è necessario digitare il nome del campo e non l’etichetta del campo. L’etichetta del campo viene visualizzata in un modulo personalizzato associato a un oggetto. Per informazioni sulla differenza tra l’etichetta e il nome di un campo personalizzato, consulta [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. (Condizionale) Se hai fatto clic su **Campi di ricerca**, digita il nome di un campo nel campo **Ricerca** e selezionalo quando viene visualizzato nell’elenco.

      ![](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >È possibile selezionare un campo dalle sezioni seguenti:
      >
      >* **Selezioni recenti**: i campi per i quali hai filtrato di recente.
      >* **Campi consigliati**: i campi più comunemente utilizzati.



   1. Selezionare un modificatore dal secondo menu a discesa. Per informazioni sui modificatori del filtro Workfront, consulta [Filtri e modificatori di condizioni](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).
   1. Seleziona o digita un valore per il campo a cui stai filtrando.

      >[!NOTE]
      >
      > Per visualizzare gli oggetti di lavoro di un portfolio specifico, puoi applicare il filtro seguente: &quot;Il nome del Portfolio contiene marketing.&quot; Vengono visualizzati gli elementi di lavoro che appartengono a qualsiasi portfolio che contiene il nome &quot;marketing&quot;.
      >
      >![](assets/portfolio-name-filter-statement-wb-350x262.png)

   1. (Facoltativo) Fai clic sul pulsante **Elimina** icona ![](assets/delete.png) per rimuovere un criterio di filtro.

1. (Facoltativo) Fai clic su **Aggiungi filtro** per aggiungere un altro criterio di filtro, ripeti le azioni del passaggio 4.

   <!--(NOTE: ensure this stays correct)-->

1. Fai clic su **Applica** applicare i risultati del filtro all&#39;area di bilanciamento del carico di lavoro selezionata senza salvarli.

   L&#39;elenco degli elementi di lavoro viene aggiornato a sinistra.

   >[!IMPORTANT]
   >
   >I risultati vengono visualizzati nel servizio di bilanciamento del carico di lavoro quando tutte le istruzioni filtro aggiunte sono simultaneamente true.

   Il filtro viene mantenuto finché non aggiorni la pagina.

   La **Applica** viene sostituito da un pulsante **Salva come nuovo** pulsante .

1. Fai clic su **Salva come nuovo** per salvare il filtro per un utilizzo futuro.

   ![](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >Clic **Annulla** in qualsiasi momento, ti riporta all&#39;area di costruzione del filtro.

1. Seleziona **Filtro senza titolo** e immetti il nome del nuovo filtro.
1. Seleziona un’icona per il nuovo filtro dal **Icona** menu a discesa.

   ![](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. (Facoltativo) Aggiungi una descrizione per il filtro per indicare l’elemento univoco. La descrizione viene visualizzata sotto il nome del filtro nell’elenco dei filtri.
1. Fai clic su **Salva**.

   I filtri salvati vengono visualizzati nell’area I filtri della casella del filtro.

   Per informazioni sull’applicazione dei filtri salvati, consulta la sezione . [Eliminare un filtro salvato nel servizio di bilanciamento del carico di lavoro](#delete-a-saved-filter-in-the-workload-balancer) in questo articolo.

1. (Condizionale) Passate il puntatore del mouse sul pulsante **Icona Filtro** ![](assets/filter-icon.png) nell&#39;angolo superiore destro del **Lavoro non assegnato** o **Lavoro assegnato** aree in cui visualizzare una descrizione comandi con il nome o il numero di filtri attualmente applicati.

   ![](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## Duplicare un filtro

Puoi duplicare e modificare un filtro per crearne uno nuovo.

1. Passa al servizio di bilanciamento del carico di lavoro.

   Per informazioni sull&#39;accesso al load balancer, vedi [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Fai clic sul pulsante **Filtro** icona ![](assets/filter-icon.png) nell&#39;angolo superiore destro di **Lavoro non assegnato** o **Lavoro assegnato** aree.

   La casella del generatore di filtri viene visualizzata a destra. Il nome dell’area per la quale si crea il filtro viene visualizzato nell’intestazione della casella.

1. Passa il puntatore del mouse su un filtro esistente e fai clic sul pulsante **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Duplica**.

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Durante la modifica di un filtro, puoi fare clic sul pulsante **Altro** nell&#39;angolo inferiore sinistro della casella Modifica filtro fare clic su **Duplica**.

1. Modifica le seguenti informazioni per il filtro duplicato:

   * Nome

      Per impostazione predefinita, il nuovo nome del filtro è &quot;(Nome filtro originale) Copia&quot;.

   * Icona
   * Descrizione
   * Qualsiasi campo, modificatore o valore.

1. (Facoltativo) Fai clic su **Aggiungi filtro** per aggiungere più istruzioni al filtro duplicato.
1. Fai clic su **Salva** per salvare il filtro duplicato nel **I miei filtri** area.

   Il filtro originale rimane invariato e il filtro duplicato viene salvato come nuovo filtro.

## Modificare un filtro esistente nel servizio di bilanciamento del carico di lavoro {#edit-an-existing-filter-in-the-workload-balancer}

Puoi modificare un filtro salvato nel servizio di bilanciamento del carico di lavoro.

>[!TIP]
>
>Quando modifichi un filtro condiviso con altri utenti, visualizzeranno anche le modifiche apportate.

1. Passa al servizio di bilanciamento del carico di lavoro.

   Per informazioni sull&#39;accesso al load balancer, vedi [Naviga nel bilanciamento del carico di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Fai clic sul pulsante **Icona Filtro** ![](assets/filter-icon.png) nell&#39;angolo superiore destro del **Non assegnato** o **Lavoro assegnato** aree.\
   Il generatore di filtri viene visualizzato a destra.

1. Passa il puntatore del mouse sul filtro da modificare, quindi fai clic sul pulsante **Modifica** ![](assets/wb-edit-filter-icon.png).

   ![](assets/filter-more-menu-options-wb.png)

1. Esegui una delle operazioni seguenti:

   * Modificare una delle istruzioni del filtro
   * Fai clic su **Aggiungi filtro** per aggiungere nuove istruzioni filtro
   * Fai clic sul pulsante **Elimina** icona ![](assets/delete.png) per rimuovere le istruzioni filtro esistenti.

1. (Facoltativo) Fai clic su **Applica**.

   I risultati vengono aggiornati nel servizio di bilanciamento del carico di lavoro a sinistra per illustrare le modifiche apportate al filtro.

1. Fai clic su **Salva.**

   I risultati vengono aggiornati nel load balancer a sinistra e il filtro viene aggiornato con le nuove informazioni selezionate.

## Eliminare un filtro salvato nel servizio di bilanciamento del carico di lavoro {#delete-a-saved-filter-in-the-workload-balancer}

Prima di eliminare un filtro, considera quanto segue:

* Non è possibile recuperare i filtri eliminati.
* Non è possibile eliminare i filtri predefiniti.
* Non è possibile eliminare un filtro non salvato. Vengono rimossi automaticamente dopo la disconnessione e il successivo accesso a Workfront.
* Quando elimini un filtro condiviso, questo viene eliminato anche per tutti gli utenti con cui è condiviso.
* Dopo aver eliminato tutti i filtri salvati, il servizio di bilanciamento del carico di lavoro viene visualizzato in base alle impostazioni predefinite originali.

>[!NOTE]
>
>Quando elimini un filtro condiviso con altri, verrà eliminato anche per loro.

1. Passa al load balancer
1. Fai clic sul pulsante **Icona Filtro** ![](assets/filter-icon.png) nell&#39;angolo superiore destro del **Lavoro non assegnato** o **Lavoro assegnato** aree.\
   La casella del generatore di filtri viene visualizzata a destra.

1. Passa il puntatore del mouse su un filtro, quindi fai clic sul pulsante **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Elimina**.
   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >Durante la modifica di un filtro, puoi fare clic sul pulsante **Altro** nell&#39;angolo inferiore sinistro della casella Modifica filtro fare clic su **Elimina**.

1. (Facoltativo) Fai clic su **Annulla** per evitare l’eliminazione e tornare all’elenco dei filtri.
1. Fai clic su **Elimina** per confermare l’eliminazione.

   Il filtro viene eliminato per te e per tutti gli utenti che disponevano delle autorizzazioni necessarie.

## Condivisione di un filtro nel servizio di bilanciamento del carico di lavoro

Puoi condividere un filtro creato o condiviso con te da altri utenti.

Quando condividi i filtri nel load balancer, considera quanto segue:

* Puoi condividere i filtri con utenti attivi, team, ruoli e aziende oppure puoi renderli visibili a tutti gli utenti della tua istanza Workfront.
* I filtri condivisi nell’area Origine non sono visibili nel servizio di bilanciamento del carico di lavoro di un progetto o di un team.
* I filtri di bilanciamento del carico di lavoro condivisi con altri non sono visibili in altre aree di Workfront.

Per condividere un filtro:

1. Passa al load balancer
1. Fai clic sul pulsante **Icona Filtro** ![](assets/filter-icon.png) nell&#39;angolo superiore destro del **Lavoro non assegnato** o **Lavoro assegnato** aree.\
   La casella del generatore di filtri viene visualizzata a destra.

1. Passa il puntatore del mouse su un filtro, quindi fai clic sul pulsante **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Condividi.**

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Durante la modifica di un filtro, puoi fare clic sul pulsante **Altro** nell&#39;angolo inferiore sinistro della casella Modifica filtro fare clic su **Condividi**.

   Viene visualizzata la casella Condivisione filtro .

1. Abilita la **Visualizza a livello di sistema** impostazione. Questo consente a chiunque in Workfront di visualizzare il filtro.

   Oppure

   Inizia a digitare i nomi degli utenti, team, ruoli, gruppi o aziende con cui desideri condividere il filtro nel **Dare accesso a** campo .

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. (Facoltativo) Fai clic sulla freccia rivolta a destra accanto al nome di un’entità per modificare le proprie autorizzazioni al filtro, quindi attiva la **Visualizza** o **Gestisci** opzione .

   ![](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. (Facoltativo) Abilita o disabilita le autorizzazioni aggiuntive per un&#39;entità eseguendo una delle operazioni seguenti:

   1. Fai clic su **Visualizza** e disattivare **Condividi** opzione . È attivata per impostazione predefinita.

   1. Fai clic su **Gestisci** e disattivare **Condividi** o **Elimina** opzione . Sono attivati per impostazione predefinita.
   >[!TIP]
   >
   >Gli utenti non possono ricevere autorizzazioni più elevate del loro livello di accesso. Se non hanno accesso ai filtri di modifica nel loro livello di accesso, non possono ricevere le autorizzazioni per gestire un filtro. Workfront disabilita l’opzione Gestisci per questi utenti e l’opzione è disattivata.

1. Fai clic su **Condividi**. Il filtro viene condiviso con le entità specificate.

   I filtri condivisi vengono visualizzati nel **Condiviso con me** area della casella del filtro.

   ![](assets/new-filters-shared-with-me-area-wb-350x236.png)

<!--   

## Add a filter to your favorites list

You can mark a filter as a favorite for quicker access to it. 

The filters that you mark as a favorite do not count towards your system Favorites list. There is no limit for how many filters you can favorite. 

1. Go to the Workload Balancer
1. Click the **Filter** icon ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas. The filter builder box displays on the right. 
1. Mouse over a filter, then click the **Favorite** ![](assets/favorites-icon-small.png). 
(NOTE: insert screen shot here with Favorite as part of this menu - same as above ones but with Favorite)
1. The filter is listed in the **Favorited** section inside the filter panel. 
1. (Optional) Click the **Favorite** icon again to remove the filter from the list of favorite filters
(I logged bugs for "Favorited" and "Unfavorite" wordings - make sure these have not updated)
-->
