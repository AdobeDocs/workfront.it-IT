---
product-area: reporting
navigation-topic: reporting-elements
title: Creare o modificare filtri in Adobe Workfront
description: È possibile limitare la quantità di informazioni visualizzate sullo schermo in un elenco di elementi con un filtro. È possibile definire determinati criteri in base a particolari informazioni su un oggetto e visualizzare solo gli oggetti che soddisfano tali criteri.
author: Nolan
feature: Reports and Dashboards
exl-id: 2e912e32-7924-418d-9d55-ce3c09f67d3e
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '2380'
ht-degree: 1%

---

# Creare o modificare filtri in Adobe Workfront

È possibile limitare la quantità di informazioni visualizzate sullo schermo in un elenco di elementi con un filtro. È possibile definire determinati criteri in base a particolari informazioni su un oggetto e visualizzare solo gli oggetti che soddisfano tali criteri.

In Adobe Workfront puoi applicare i seguenti tipi di filtri:

* Filtra rapidamente un elenco di oggetti per trovare un elemento utilizzando una parola chiave. Si tratta di filtri temporanei che non è possibile salvare per utilizzi futuri.

   Per informazioni sui filtri rapidi, vedi [Applicare il filtro rapido a un elenco](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

* Filtri permanenti che consentono di risparmiare e utilizzare più tempo su più elenchi e rapporti. Questo articolo descrive come creare un filtro permanente o modificarne uno esistente in un elenco o in un rapporto.

* Filtri in altre aree di Workfront, al di fuori degli elenchi e dei rapporti.

   Per un elenco di tutti i filtri in Workfront e delle aree in cui è possibile applicarli, vedi [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni e Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Gestione delle autorizzazioni di un filtro</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Tipi di interfacce per la creazione di filtri

Puoi creare filtri utilizzando i tipi di generatore di filtri descritti nella tabella seguente:

<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Tipo di generatore</strong></td>
<td><strong>Oggetto Filter</strong></td>
<td><strong>Se disponibile</strong></td>
</tr>
<tr>
<td>Generatore standard</td>
<td>
<ul>
<li> <p>Progetti</p> </li>
<li> <p>Attività </p> </li>
<li> <p>Problemi</p> </li>
<li> <p>Portfolio</p> </li>
<li> <p>Programmi</p> </li>
<li> <p>Utenti</p> </li>
<li> <p>Modelli</p> </li>
<li> <p>Gruppi</p> </li>
</ul>
</td>
<td>
<ul>
<li> <p>Elenchi </p> </li>
</ul>
<ul>
<li> <p>Elenco Progetti nel Planner scenario</p> <p>Il planner scenario richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedi <a href="../../../scenario-planner/scenario-planner-overview.md">Panoramica di Scenario Planner</a>. </p> </li>
</ul>
<p>NOTA: I generatori standard per i filtri non sono disponibili nei rapporti.
</td>
</tr>
<tr>
<td>Generatore legacy</td>
<td>Tutti gli oggetti </td>
<td>Elenchi e rapporti</td>
</tr>
</tbody>
</table>

Per informazioni sugli oggetti Workfront, vedere [Comprendere gli oggetti in Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Quando crei filtri utilizzando diverse interfacce, considera quanto segue:

* Puoi trovare il generatore standard nelle stesse posizioni in cui trovi l’interfaccia filtro legacy per le aree elencate nella tabella precedente.
* Il generatore standard è l’esperienza predefinita per tutte le aree in cui è disponibile. Per passare al generatore di filtri legacy, fai clic sul pulsante **Altro** accanto a [!UICONTROL **Filtri**] e seleziona [!UICONTROL **Torna ai filtri legacy**].

   ![Torna ai Filtri legacy](assets/use-legacy-filters.png)

* I filtri salvati sono disponibili in entrambi i generatori, indipendentemente dall’esperienza utilizzata per generarli originariamente. Ad esempio, se hai creato un filtro utilizzando il generatore legacy, puoi trovarlo e modificarlo anche nell’interfaccia standard del generatore.

   >[!TIP]
   >
   >Un filtro &quot;All&quot; non è incluso nel generatore standard perché tutte le voci di elenco vengono visualizzate quando non vengono applicati filtri. Fai clic su [!UICONTROL **Cancella tutto**] in alto a destra nel generatore per cancellare eventuali filtri attivi e visualizzare tutti gli elementi. Se [!UICONTROL **Cancella tutto**] è oscurato, non vengono applicati filtri.

* I generatori standard e legacy hanno una sintassi leggermente diversa durante la creazione di filtri con più istruzioni che combinano gli operatori AND e OR. Di conseguenza, questi filtri possono essere visualizzati in modo diverso quando si passa da un generatore all’altro.

   >[!INFO]
   >
   >Esiste lo scenario seguente:
   >
   >1. Utilizza il generatore standard per creare un filtro con la seguente sintassi:
   >
   >   `(A OR B) AND C`
   >
   >1. Passa al generatore legacy e modifica il filtro utilizzando la sintassi del generatore legacy come descritto in [Creare o modificare un filtro nel generatore legacy](#create-filter-in-legacy-builder) in questo articolo. La sintassi per il generatore legacy visualizza le istruzioni del filtro come segue:
   >
   >   `A AND C`
   >   `OR`
   >   `B AND C`
   >
   >1. Apporta una modifica al filtro nell’interfaccia legacy.
   >1. Torna al generatore standard. L’istruzione filter viene visualizzata in base alla logica supportata nel generatore legacy, come descritto in precedenza.

   >
   >   Il filtro viene visualizzato nell’interfaccia standard del generatore come segue:
   >  
   >   `A AND C`
   >   `OR`
   >   `B AND C`
   > 
   >   Questo accade perché il filtro è stato modificato nell’interfaccia legacy.

## Creare o modificare un filtro nel generatore standard

Puoi creare filtri utilizzando l’interfaccia standard di generazione nei seguenti modi:

* Da zero
* Modificare un filtro esistente
* Duplicare un filtro esistente
* Duplicare un filtro esistente, modificarlo e salvarlo come nuovo filtro

Crea un filtro utilizzando l’interfaccia standard di generazione:

1. Passa a un elenco in cui desideri creare un filtro o che contiene il filtro che desideri personalizzare.
1. Fai clic sul pulsante **Filtro** icona ![Icona Filtro](assets/filter-nwepng.png) per aprire l&#39;interfaccia del generatore.

   ![Generatore di filtri standard](assets/new-filters-all-filter-types.png)

1. Rivedi i seguenti elenchi di filtri:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Preferiti</strong></td>
   <td>Filtri contrassegnati come preferiti. Quando si preferisce un filtro, la sua posizione originale viene visualizzata sotto il nome del filtro e viene nascosta dall'elenco originale a meno che non lo si rimuova come preferito.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Salvato</strong></td>
   <td>Filtri creati e salvati da soli.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Impostazioni predefinite di sistema</strong></td>
   <td>Filtri predefiniti del sistema Workfront e filtri aggiunti dall’amministratore di Workfront all’elenco dei filtri, a livello di sistema o nel modello di layout.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Condivisi con me</strong></td>
   <td>Filtri creati e condivisi da altri utenti o condivisi a livello di sistema.</td>
   </tr>
   </tbody>
   </table>

1. Esegui una delle operazioni seguenti:

   * Fai clic su **Nuovo filtro** per creare un filtro da zero.
   * Passa il puntatore del mouse su un filtro esistente da gestire e fai clic sul pulsante **Modifica** icona ![Icona Modifica](assets/edit-icon.png) per modificarlo.

      Oppure

      Passa il puntatore del mouse su un filtro esistente per il quale disponi delle autorizzazioni di visualizzazione, quindi fai clic sul pulsante **Altro** menu ![Menu Altro](assets/more-icon-spectrum.png)e fai clic su **Duplica** per copiare il filtro esistente e modificare una copia.
   ![Altre opzioni di menu](assets/new-filters-more-menu-options-with-delete.png)

1. (Condizionale) A seconda che si desideri trovare oggetti che corrispondono a tutte o a una delle istruzioni di un gruppo di filtri, seleziona una delle seguenti opzioni:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Includi se tutti sono true</strong></td>
   <td>Gli oggetti trovati dal filtro devono corrispondere a tutti i criteri di filtro di un gruppo di filtri. In questo caso, le istruzioni del filtro sono collegate dall’operatore AND. Questa è la selezione predefinita.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Includi se almeno una è true</strong></td>
   <td>Gli oggetti trovati dal filtro devono corrispondere a qualsiasi criterio di filtro in un gruppo di filtri. In questo caso, le istruzioni del filtro sono collegate dall’operatore OR.</td>
   </tr>
   </tbody>
   </table>

   ![Includi se il menu a discesa è tutto o uno o vero](assets/new-filters-all-or-any-are-true-drop-down-menu-nwe.png)

   Per ulteriori informazioni sugli operatori dei filtri, vedi [Panoramica sui filtri in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Fai clic sul menu a discesa del campo per visualizzare un elenco dei campi utilizzati di recente e dei campi consigliati per filtrare. I campi suggeriti sono attualmente visualizzati nell’elenco a cui si sta filtrando.

   Puoi anche selezionare **Campi di ricerca** per visualizzare un elenco di tutti i campi che è possibile filtrare per. I campi nella ricerca avanzata sono raggruppati per categoria di oggetti.

   ![Individua un campo per filtrare in base a](assets/new-filter-search-for-field.png)

1. Fai clic sul menu a discesa del modificatore per selezionare un modificatore. Il modificatore predefinito è &quot;Uguale a&quot;.

   Per ulteriori informazioni, consulta [Modificatori di filtri e condizioni](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!TIP]
   >
   >Durante la creazione del filtro, i risultati vengono visualizzati immediatamente nell’elenco. Se il pannello dei filtri copre l’elenco, puoi chiuderlo per visualizzarne la visualizzazione. Le informazioni immesse rimangono nel generatore quando riapri il pannello.

1. Inizia a digitare il valore di un campo per il quale desideri eseguire il filtro. Ad esempio, inizia a digitare il nome di un problema, se desideri filtrare per `Issue:Name`. Seleziona il valore quando viene visualizzato nell’elenco.

   >[!TIP]
   >
   >A seconda del modificatore selezionato, è possibile selezionare più valori.

1. Fai clic su **Aggiungi filtro** per selezionare un altro campo e aggiungere un nuovo criterio di filtro all’istruzione del filtro.
1. (Facoltativo) Fai clic sul pulsante **Elimina** icona ![Icona Elimina](assets/delete.png) per rimuovere le istruzioni filtro esistenti.

   Oppure

   Fai clic su **Cancella tutto** per cancellare tutti i criteri di filtro.

1. (Facoltativo) Fai clic su **Aggiungi gruppo di filtri** per aggiungere un altro set di criteri di filtro. L&#39;operatore predefinito tra i set è AND. Fai clic sull’operatore per modificarlo in OR.

   >[!TIP]
   >
   >È possibile utilizzare un altro gruppo di filtri quando si desidera che i gruppi siano collegati da un operatore diverso rispetto all&#39;operatore in un&#39;istruzione di filtro.

   >[!INFO]
   >
   >Quando filtri i progetti che contengono &quot;marketing&quot; nel nome che non sono completi e che non sono bloccati, puoi utilizzare i seguenti gruppi di filtri multipli:
   >`(Project: Name Contains Marketing AND Project: Percent Complete Does not equal 100)`
   >`OR`
   >`(Project: Name Contains Marketing AND Project: Status Does not equal On Hold)`
   >In questo caso, ogni istruzione filtro è connessa da un AND e i gruppi di filtri sono collegati da un operatore OR.

1. (Facoltativo) Fai clic su **Modalità testo** per continuare a creare il filtro utilizzando la modalità testo.

   ![Seleziona modalità testo](assets/new-filter-select-text-mode.png)

   Viene visualizzata l’interfaccia della modalità testo.

   ![Interfaccia della modalità testo](assets/text-mode-interface-for-beta-filters-nwe.png)

   >[!TIP]
   >
   >È consigliabile creare il maggior numero possibile di filtri utilizzando l’interfaccia standard di generazione e utilizzando la modalità testo solo quando è necessario apportare modifiche al filtro supportate solo in modalità testo.

   Per ulteriori informazioni sulla creazione di un filtro tramite l’interfaccia della modalità testo, consulta [Modificare un filtro utilizzando la modalità testo](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

1. Fai clic su **Esci da modalità testo** per tornare all’interfaccia standard del generatore.

   >[!WARNING]
   >
   >Alcune istruzioni di modalità testo non sono supportate nel generatore standard o nell’interfaccia legacy. Se si esce dalla modalità di testo dopo la creazione di questi tipi di istruzioni, potrebbe essere generato un messaggio di avviso.

1. (Facoltativo) Fai clic su **Applica** per applicare il filtro all’elenco e visualizzare i risultati.

   Se il filtro non produce risultati, l’elenco sarà vuoto.

1. Fai clic su **Salva come nuovo** per salvare il filtro per un utilizzo futuro.

   ![Assegnare un nome e salvare il filtro](assets/save-as-untitled-filter-ui-nwe.png)

1. Seleziona **Filtro senza titolo** e digitare il nome del nuovo filtro.

   >[!TIP]
   >
   >Assicurati di denominare il filtro in modo da poterlo trovare in un secondo momento. Se il filtro non viene denominato, verrà denominato Filtro senza titolo nel sistema.

1. Seleziona un’icona per il nuovo filtro dal **Icona** menu a discesa.

   ![Seleziona un’icona per il filtro](assets/new-filter-select-icon.png)

1. (Facoltativo) Aggiungi una descrizione per il filtro per indicare l’elemento univoco. La descrizione viene visualizzata sotto il nome del filtro nell’elenco dei filtri.

   >[!TIP]
   >
   >Clic **Annulla** in qualsiasi momento ti riporta all&#39;area di costruzione del filtro.

1. Fai clic su **Salva**. Il filtro viene salvato nell’elenco Salvati e applicato all’elenco di elementi.
1. (Facoltativo) Per spostare un filtro nell’elenco Preferiti, posiziona il cursore del mouse su un filtro nel cassetto del filtro e fai clic sull’icona Preferito . ![Icona preferita](assets/favorites-icon-small.png).

   Oppure

   Passa il puntatore del mouse su un filtro nel cassetto del filtro e fai clic sul menu Altro ![Menu Altro](assets/more-icon-spectrum.png)e fai clic su **Preferito**.

1. (Facoltativo) Fai clic sul pulsante **Filtri di stack** per attivare i filtri sovrapposti. Questa opzione consente di applicare più di un filtro salvato. Le regole di filtro vengono applicate nell’ordine in cui sono state selezionate.

   >[!TIP]
   >
   >Non esiste un limite al numero di filtri che è possibile selezionare.
   >
   >Quando selezioni più filtri, tutte le loro condizioni devono essere soddisfatte contemporaneamente per visualizzare i risultati corrispondenti.

   ![Stack di filtri](assets/new-filter-stack-filters.png)

   Il numero di filtri selezionati viene visualizzato accanto all’icona del filtro nella parte superiore dell’elenco di elementi.

   ![Numero di filtri selezionati](assets/number-of-filters-selected.png)

1. (Facoltativo) Effettua una delle seguenti operazioni:

   * Condividere il filtro con altri utenti o renderlo disponibile a livello di sistema. Per ulteriori informazioni, consulta [Condividere un filtro, una visualizzazione o un raggruppamento](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

   * Elimina il filtro se non è più valido o se è un duplicato. Puoi eliminare solo i filtri di tua proprietà. Puoi rimuovere i filtri condivisi con te. Per informazioni, consulta [Rimuovere filtri, visualizzazioni e raggruppamenti](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).

## Creare o modificare un filtro nel generatore legacy {#create-filter-in-legacy-builder}

È possibile creare filtri legacy in elenchi e rapporti nei modi seguenti:

* Da zero
* Modificare un filtro esistente e salvarlo come nuovo filtro

Indipendentemente dal metodo utilizzato per creare i filtri, la creazione di un filtro da zero o da un filtro esistente è simile.

1. Passare a un elenco o a un report contenente il filtro che si desidera personalizzare.
1. Fai clic sul pulsante **Filtro** icona ![Icona Filtro](assets/filter-nwepng.png).

   >[!TIP]
   >
   >Per visualizzare l’elenco a discesa Filtro in un rapporto, l’autore del rapporto deve consentire la modifica dei filtri. Il filtro Predefinito per rapporto viene applicato a un rapporto per impostazione predefinita. Il filtro Predefinito rapporto può essere personalizzato solo quando lo si modifica.

   ![Elenco a discesa Filtro](assets/filter-drop-down-expanded-nwe.png)

1. Fai clic su **Nuovo filtro** nella parte superiore dell’elenco dei filtri.

   Oppure

   Passa il puntatore del mouse sul filtro da modificare e fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png).

   Generatore per personalizzare gli avvii del filtro.

1. Effettua una delle seguenti operazioni:

   * Modifica le regole di filtro esistenti facendo clic sulla regola esistente e selezionando una nuova opzione.
   * Aggiungi una regola di filtro facendo clic su **Aggiungi un’altra regola filtro** inizia a digitare il nome dell’opzione per la quale desideri aggiungere una regola nel **Inizia a digitare il nome del campo** quindi fare clic su di essa quando viene visualizzata nell&#39;elenco a discesa.

      I campi associati all’oggetto del filtro sono elencati nella **Inizia a digitare il nome del campo** scatola.

   * Fai clic su **E** o **O** quando si aggiunge una nuova regola di filtro.\
      Quando aggiungi le regole di filtro, utilizza i modificatori di filtro per stabilire la condizione del filtro. Per ulteriori informazioni sui modificatori dei filtri, consulta [Modificatori di filtri e condizioni](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

      >[!NOTE]
      >
      >Quando si collega un gruppo di istruzioni AND da più istruzioni OR, è necessario ripetere i campi che non cambiano tra le istruzioni OR per ciascun gruppo di istruzioni.
      >
      >![Istruzioni di filtro collegate](assets/filters-and-statements-connected-by-or-statements-builder-ui-old-filters-2022.png)
      >
      >Quando si crea un filtro per le attività che contengono la parola &quot;marketing&quot; e si trovano in progetti con stato Corrente o Pianificazione, è necessario disporre delle seguenti regole di filtro:
      >
      >`Task: Name Contains Marketing`
      >`AND`
      >`Project: Status Equals Current`
      >`OR`
      >`Task: Name Contains Marketing`
      >`AND`
      >`Project: Status Equals Planning`
      >
      >Anche se attività: Nome Contiene &quot;marketing&quot; non cambia tra i due gruppi di filtri AND, deve essere ripetuto nel secondo gruppo.

   * Elimina una regola di filtro esistente facendo clic sull&#39;icona &quot;X&quot;.

1. (Facoltativo) Fai clic su **Passa alla modalità testo** per aggiungere un filtro utilizzando l’interfaccia Modalità testo .

   Per ulteriori informazioni sulla creazione di un filtro tramite l’interfaccia della modalità testo, consulta [Modificare un filtro utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

1. Fai clic su **Salva filtro** per creare un nuovo filtro o sostituire quello selezionato con le modifiche apportate.

   Oppure

   Fai clic su **Salva come nuovo filtro** per creare un nuovo filtro da quello selezionato.

   Il nuovo filtro viene visualizzato nell’elenco dei filtri e viene applicato automaticamente all’elenco o al rapporto selezionato.

1. (Facoltativo) Effettua una delle seguenti operazioni:

   * Condividi i filtri creati con altri utenti o rendili disponibili a livello di sistema. Per informazioni, consulta [Condividere un filtro, una visualizzazione o un raggruppamento](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
   * Rimuovere i filtri che non si desidera più visualizzare nell’elenco. Per informazioni, consulta [Rimuovere filtri, visualizzazioni e raggruppamenti](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).


