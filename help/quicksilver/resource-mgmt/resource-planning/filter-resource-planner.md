---
product-area: resource-management
navigation-topic: resource-planning
title: Filtrare le informazioni nel planner risorse
description: '''(AL:*Itera su questo articolo: filtro per dati personalizzati. Altri miglioramenti? I caratteri speciali avvertenze potrebbero cambiare - seguire la storia per sapere quando. Originariamente è arrivato in Beta 3 17.3.)"'
author: Alina
feature: Resource Management
exl-id: 7186cae5-1e16-421e-b26d-afb50aa7f6eb
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '2442'
ht-degree: 0%

---

# Filtrare le informazioni nel planner risorse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(AL:*Iterate on this article: filtering by custom data. Other enhancements? Special characters caveat might change - follow the story to know when. It originally came in Beta 3 17.3.)</p>
-->

Utilizzando i filtri, è possibile modificare le informazioni visualizzate nel Planner risorse da tutte le informazioni memorizzate nel sistema.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro e superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a progetti, utenti e gestione risorse </p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza autorizzazioni o versioni successive per progetti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Panoramica dei filtri di pianificazione delle risorse

Per ridurre al minimo la quantità di informazioni visualizzate nel planner risorse, Adobe Workfront fornisce un filtro predefinito con criteri preconfigurati. Per informazioni sul filtro predefinito, consulta la sezione . [Panoramica del filtro predefinito nel planner risorse](#overview-of-the-default-filter-in-the-resource-planner) in questo articolo.

Puoi anche creare filtri personalizzati. Per informazioni sulla personalizzazione dei filtri nel planner risorse, consulta la sezione . [Creare filtri di pianificazione delle risorse](#create-resource-planner-filters) in questo articolo.

Quando si utilizzano filtri nel planner risorse, tenere presente quanto segue:

* I filtri creati sono visibili solo a te. Puoi condividere i filtri per renderli disponibili ad altri utenti.
* In qualità di amministratore di Workfront, puoi visualizzare solo i filtri creati o condivisi con te.
* I risultati filtrati non cambiano quando si seleziona una visualizzazione diversa per il Planner risorse.\
   Per ulteriori informazioni sulla modifica della visualizzazione nel Planner risorse, vedere la sezione di selezione &quot;Progetto/Ruolo/Visualizzazione utente&quot; in [Panoramica sulla navigazione in planner risorse](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

* L’applicazione di un filtro non modifica i dati di allocazione e disponibilità nel Planner risorse per progetti, ruoli o utenti. Un filtro modifica solo il numero di oggetti visualizzati nel Planner risorse.
* Il filtro si applica a tutti gli oggetti visualizzati contemporaneamente nel Planner risorse. Ad esempio, se si applica un filtro per un utente specifico, in Planner risorse vengono visualizzati solo i risultati seguenti:

   * Progetti in cui l’utente fa parte del pool di risorse (per le visualizzazioni Progetto e Ruolo) o dispone di un’assegnazione nel progetto (per la visualizzazione Utente)
   * Ruoli associati all’utente in tali progetti\
      Gli altri ruoli o utenti dei progetti a cui è associato l’utente non vengono visualizzati.

## Panoramica del filtro predefinito nel planner risorse {#overview-of-the-default-filter-in-the-resource-planner}

Quando si apre il Planner risorse per la prima volta, Workfront applica il filtro Predefinito. Puoi modificare il filtro Predefinito per filtrare solo gli elementi che desideri visualizzare. Per informazioni sulla modifica di un filtro, consulta la sezione . [Modificare un filtro nel planner risorse](#edit-a-filter-in-the-resource-planner) in questo articolo.

Quando utilizzi il filtro Predefinito , considera quanto segue:

* Il filtro predefinito recupera le informazioni solo dai progetti con i seguenti elementi:

   * Data completamento pianificata successiva alla prima data del mese corrente
   * Una data di inizio pianificata che si verifica prima dell&#39;ultimo giorno del quarto mese dalla data corrente
   * Uno stato di corrente o pianificazione

   >[!IMPORTANT]
   >
   >Il filtro Predefinito recupera le informazioni dai progetti che si verificano sempre entro quattro mesi a partire dal primo giorno del mese corrente, indipendentemente dall&#39;intervallo temporale selezionato per la visualizzazione nel Planner risorse.

* Nella visualizzazione utente vengono visualizzati tutti gli utenti del sistema, ma solo gli utenti associati ai progetti filtrati mostrano le informazioni relative all’ora.
* È possibile modificare le informazioni nel filtro Predefinito senza salvare il filtro.
* Puoi duplicare e modificare una copia del filtro Predefinito, modificare i criteri desiderati, quindi salvarlo come nuovo filtro.
* Non è possibile eliminare o condividere il filtro Predefinito.

   ![RP_new_default_fitler_criteria__1_.PNG](assets/rp-new-default-fitler-criteria--1--301x547.png)

## Creare filtri di pianificazione delle risorse {#create-resource-planner-filters}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: **^ This section is somewhat duplicated (format more than content) from the "Filtering Utilization Information" section in "Viewing Utilization Information for Projects, Programs, and Portfolios.")</p>
-->

La creazione di un filtro nel Planner risorse è identica per tutte le visualizzazioni.

Prima di creare un filtro, verificare che siano presenti i prerequisiti per la visualizzazione delle informazioni corrette nel Planner risorse.\
Per informazioni su come soddisfare i prerequisiti necessari per utilizzare il planner risorse, vedere la sezione &quot;Prerequisiti per lavorare nel planner risorse&quot; nella sezione [Panoramica di Resource Planner](../../resource-mgmt/resource-planning/get-started-resource-planner.md) articolo.

Quando crei un filtro, considera quanto segue:

* Non esiste alcun limite al numero di oggetti per i quali è possibile filtrare contemporaneamente.
* I campi disponibili che è possibile aggiungere a una modifica del filtro in base all&#39;oggetto della visualizzazione applicata al planner risorse. Ad esempio, è possibile filtrare i campi Problema o Attività solo nella visualizzazione utente, in quanto questi oggetti vengono visualizzati solo nella visualizzazione utente. Se si crea un filtro per Problemi o Attività nella visualizzazione Utente e lo si applica alle visualizzazioni Progetto o Ruolo, questo viene ignorato perché i campi non esistono nelle visualizzazioni Progetto o Ruolo. In questo caso, il filtro non è disponibile.

Per creare un filtro nel planner risorse:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Risorsa**.

   La **Planner** viene visualizzato per impostazione predefinita.

   Per impostazione predefinita, la prima volta che si accede al Planner risorse, il <strong>Filtro predefinito</strong> viene applicata.<br>Per ulteriori informazioni sul filtro Predefinito, consulta la sezione <a href="#overview-of-the-default-filter-in-the-resource-planner" class="MCXref xref">Panoramica del filtro predefinito nel planner risorse</a> in questo articolo.

1. Nell’angolo in alto a sinistra del , fai clic sul pulsante **Filtro** icona.\
   ![filter_icon.png](assets/filter-icon.png)\
   Oppure\
   Espandi la **Filtro** menu a discesa e fai clic su **Aggiungi nuovo filtro**.\
   ![](assets/rp-filter-dropdown-expanded-with-default-filter-selected-350x283.png)

1. Per creare un filtro utilizzando i criteri incorporati, specifica uno dei campi seguenti:

   * **Portfolio**: Inizia a digitare il nome del portfolio che contiene le informazioni da includere nel Planner risorse, quindi fai clic sul nome quando viene visualizzato nell’elenco.\
      Ripeti questo processo per includere informazioni provenienti da più portfolio.

   * **Stato del progetto**: Espandi il menu a discesa Stato progetto e seleziona uno o più stati di progetto disponibili nell’elenco.
   * **Team**: Inizia a digitare il nome di uno o più team associati agli utenti assegnati alle attività nei progetti da visualizzare.
   * **Ruolo**: Inizia a digitare il nome di uno o più ruoli di lavoro associati agli utenti assegnati alle attività nei progetti che desideri visualizzare.
   * **Piscine**: Inizia a digitare il nome di uno o più pool di risorse associati ai progetti (per la visualizzazione Progetto), agli utenti (per la visualizzazione Utente) o associati ai progetti e agli utenti (per la visualizzazione Ruolo) che desideri visualizzare.
   * **Gruppo**: Inizia a digitare il nome di uno o più gruppi associati agli utenti (nella visualizzazione Utente) o ai progetti (nelle visualizzazioni Progetto e Ruolo) che desideri visualizzare.

1. Fai clic su **Aggiungi regola filtro**, quindi inizia a digitare il nome del campo di cui desideri filtrare in **Tipo per filtrare gli elementi** scatola. Se il campo è disponibile, viene compilato per ciascun oggetto in cui può essere associato.

   >[!IMPORTANT]
   >
   >Quando si fa riferimento a campi personalizzati, è necessario digitare il nome del campo e non l’etichetta del campo. L’etichetta del campo viene visualizzata in un modulo personalizzato associato a un oggetto. Per informazioni sulla differenza tra l’etichetta e il nome di un campo personalizzato, consulta  [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

1. Fai clic sul nome del campo per aggiungerlo al filtro quando viene visualizzato nell’elenco.\
   Per ulteriori informazioni sui campi visualizzati nell’elenco, consulta [Glossario della terminologia di Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. (Facoltativo) Seleziona i modificatori di filtro e condizione per il filtro. I modificatori disponibili sono descritti in [Modificatori di filtri e condizioni](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   È possibile utilizzare caratteri jolly basati su utente o data per filtrare le informazioni associate all&#39;utente connesso.\
   Per informazioni sui caratteri jolly supportati nei filtri, consulta [Variabili filtro caratteri jolly](../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Fai clic su **Salva** per salvare la regola di filtro.
1. (Facoltativo) Fai clic su **Aggiungi regola filtro** per aggiungere una nuova regola per un altro oggetto o campo.
1. Fai clic su **Applica** applicare il filtro senza salvarlo.

   Oppure

   Fai clic su **Salva filtro** per salvare il filtro.\
   ![RP_Apply_or_Save_button_on_filters.png](assets/rp-apply-or-save-buttons-on-filters-320x79.png)

1. (Condizionale) Dopo aver fatto clic su **Salva**, specifica un nome per il filtro nella **Nome filtro** all&#39;interno della **Salva filtro** finestra di dialogo. Questo è un campo obbligatorio.\
   ![RP_new_save_filter_box__with_Save_button__without_apply.png](assets/rp-new-save-filter-box--with-save-button--without-apply-350x175.png)

   >[!NOTE]
   >
   >Se il nome del filtro include caratteri speciali, utilizza solo i seguenti caratteri:
   >
   >* Virgola
   >* Barra
   >* Trattino
   >* Sottolineato


1. Fai clic su **Salva**.

   I risultati nel planner risorse vengono ora filtrati dalle informazioni incluse nelle regole di filtro.

## Applicare un filtro esistente

Quando l&#39;utente o un utente con accesso al planner risorse salva un filtro, questo diventa disponibile a tutti gli utenti che utilizzano il planner risorse.

Per applicare un filtro esistente:

1. Vai al Planner risorse.
1. Nell’angolo in alto a sinistra, espandi la **Filtro** menu a discesa.

   In questo menu puoi vedere i filtri creati o quelli condivisi con te.\
   ![RP_filter_drop_down.png](assets/rp-filter-drop-down-350x152.png)

1. Seleziona un filtro nel menu a discesa. Puoi visualizzare i filtri creati da te o da altri utenti in questo menu.\
   Quando si seleziona un filtro, questo riduce automaticamente la quantità di informazioni visualizzate nel planner risorse.

## Modificare un filtro nel planner risorse {#edit-a-filter-in-the-resource-planner}

È possibile modificare un filtro nel planner risorse eseguendo una delle operazioni seguenti:

* [Rinominare un filtro](#rename-a-filter)
* [Modificare le informazioni in un filtro](#edit-the-information-in-a-filter)
* [Duplicare un filtro](#duplicate-a-filter)

Quando si modifica un filtro, questo viene aggiornato per tutti gli utenti del sistema che hanno accesso al planner risorse.

### Rinominare un filtro {#rename-a-filter}

È possibile modificare il nome di un filtro senza modificarne i criteri. È consigliabile che altri utenti del sistema siano a conoscenza di questa modifica, in quanto i filtri sono visibili ad altri utenti. Questa modifica interessa gli elenchi di filtri per tutti coloro che possono visualizzare il planner risorse.

1. Passa al Planner risorse ed espandi il **Filtro** menu a discesa per selezionare un filtro salvato.
1. Espandi la **Filtro** menu a discesa. Individua il filtro che desideri rinominare e passa il puntatore del mouse sul suo nome.
1. Seleziona la **Rinomina filtro** accanto al nome del filtro.

   ![](assets/rp-filter-options-edit-350x154.png)

1. Specifica un nuovo nome per il filtro nel **Nome filtro** scatola.
1. Fai clic su **Salva**.\
   Le informazioni incluse nel filtro sono le stesse e il nome viene aggiornato.

### Modificare le informazioni in un filtro {#edit-the-information-in-a-filter}

È possibile modificare le informazioni incluse in un filtro senza modificarne il nome. È consigliabile che altri utenti del sistema siano a conoscenza di questa modifica, in quanto i filtri sono visibili. Questa modifica interessa gli elenchi di filtri per tutti coloro che possono visualizzare il planner risorse.

1. Passa al Planner risorse ed espandi il **Filtro** menu a discesa nell&#39;angolo in alto a sinistra.
1. Seleziona un filtro esistente da modificare.
1. Fai clic sul pulsante **Filtro** icona.\
   ![filter_icon.png](assets/filter-icon.png)

1. Aggiungi nuovi campi al filtro.\
   Per informazioni sulla creazione dei filtri, consulta [Creare filtri di pianificazione delle risorse](#create-resource-planner-filters).

1. Passa il puntatore del mouse sui campi esistenti selezionati per il filtro e fai clic sul pulsante **Modifica** per selezionare un altro campo, oppure **Elimina** per eliminare il campo.\
   ![RP_custom_filter_delete_and_edit_icon.png](assets/rp-custom-filter-delete-and-edit-icons-350x169.png)

1. (Facoltativo) Fai clic su **Aggiungi regola filtro** per aggiungere nuovi campi al filtro.\
   Per ulteriori informazioni sulla definizione dei criteri di filtro, consulta [Creare filtri di pianificazione delle risorse](#create-resource-planner-filters).

1. Fai clic su **Applica** applicare il filtro senza salvarlo.

   Oppure

   Fai clic su **Salva** per salvare il filtro.\
   Il filtro viene salvato con lo stesso nome ma con nuovi criteri di filtro.

### Duplicare un filtro {#duplicate-a-filter}

Puoi duplicare un filtro esistente. I criteri di filtro originali rimangono gli stessi nel filtro duplicato ed è possibile salvare il nuovo filtro con un nuovo nome.

1. Passa al Planner risorse ed espandi il **Filtro** menu a discesa nell&#39;angolo in alto a sinistra.
1. Passa il puntatore del mouse sul nome di un filtro salvato da duplicare.
1. Fai clic sul pulsante **Duplica** icona.

   ![](assets/rp-filter-options---duplicate-350x154.png)\
   Viene visualizzata la casella Filtro duplicato.

1. In **Nome filtro** Specifica un nuovo nome per il filtro duplicato.\
   Il nome predefinito del nuovo filtro è *`<Original Filter Name>`(copia)*.

1. Fai clic su **Salva**. Viene creato un nuovo filtro con gli stessi criteri del filtro originale e con un nuovo nome.

   >[!NOTE]
   >
   >Anche se è possibile utilizzare 2 filtri con lo stesso nome e con criteri identici, è consigliabile salvare i filtri con criteri di filtro univoci e nomi nel planner risorse per evitare confusione.

## Eliminare un filtro

È possibile eliminare un filtro quando non è più necessario. Non è possibile eliminare il filtro predefinito.

Per informazioni sul filtro predefinito, consulta la sezione [Panoramica del filtro predefinito nel planner risorse](#overview-of-the-default-filter-in-the-resource-planner) in questo articolo.

Quando elimini un filtro, questo viene eliminato per tutti gli utenti Workfront che hanno accesso al planner risorse. Prima di rimuoverlo, assicurati che il filtro che desideri rimuovere non sia più utilizzato da altri utenti che lavorano nel Planner risorse. Impossibile recuperare un filtro eliminato.

Per rimuovere un filtro:

1. Vai al Planner risorse.
1. Espandi la **Filtro** menu a discesa.
1. Individua il filtro da rimuovere e passa il puntatore del mouse sul nome.
1. Seleziona la **Elimina filtro** accanto al nome del filtro.

   ![](assets/rp-filter-options---delete-350x154.png)

1. Fai clic su **Elimina** in **Elimina filtro** finestra di dialogo.

1. Il filtro viene eliminato e rimosso dal Planner risorse.

## Condivisione di un filtro

Puoi condividere un filtro creato o che puoi condividere con altri utenti. Non è possibile condividere il filtro predefinito, ma è possibile duplicarlo e condividere la copia.

>[!NOTE]
>
>Tutti gli utenti, inclusi gli amministratori di Workfront, possono accedere solo ai filtri creati o condivisi con loro. È possibile condividere un filtro con utenti specifici per rendere disponibile un filtro a tutti gli utenti di Resource Planner.

Per informazioni sul filtro predefinito, consulta la sezione [Panoramica del filtro predefinito nel planner risorse](#overview-of-the-default-filter-in-the-resource-planner) in questo articolo.

Per informazioni sulla duplicazione dei filtri, consulta la sezione [Duplicare un filtro](#duplicate-a-filter) in questo articolo.

1. Vai al Planner risorse.
1. Espandi la **Filtro** menu a discesa.
1. Individua il filtro da condividere e passa il cursore sul nome.
1. Seleziona la **Filtro condivisione** accanto al nome del filtro.

   ![](assets/rp-filter-options---share-350x154.png)

   Viene visualizzata la finestra di dialogo Accesso filtro.

1. (Facoltativo) Per rendere il filtro disponibile a tutti gli utenti di Resource Planner, fai clic sul pulsante **Impostazioni** , quindi seleziona **Rendere visibile il sistema a livello di sistema**.

   ![](assets/make-this-visible-system-wide-350x119.png)

1. In **Assegna l’accesso al filtro del planner risorse a:** inizia a digitare i nomi di utenti, team, ruoli, gruppi o aziende con cui desideri condividere il filtro.
1. Seleziona uno dei seguenti livelli di autorizzazione:

   * Visualizza
   * Gestisci

      Per informazioni sulle autorizzazioni in Workfront, vedi [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

1. (Facoltativo) Fai clic su **Impostazione avanzata** per aggiungere autorizzazioni per ogni livello selezionandoli o rimuovere le autorizzazioni per ogni livello deselezionandole.

   ![](assets/rp-share-filter-manage-advanced-settings-350x271.png)

1. Fai clic su **Salva**.

   Il filtro viene condiviso con le entità selezionate e viene visualizzato nella **Condiviso con me** area.

   ![](assets/rp-shared-with-me-area.png)
