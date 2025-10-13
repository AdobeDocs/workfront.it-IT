---
title: Configurare le funzionalità tra aree di lavoro diverse per i tipi di record
description: È possibile abilitare un tipo di record per l'aggiunta a un'altra area di lavoro o per la connessione da un'altra area di lavoro.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 393f858ba3711b367cf06ad846ea60be0d6d9034
workflow-type: tm+mt
source-wordcount: '1230'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************REPLACE THE "ADVANCED SETTINGS" SECTION IN THE "EDIT RECORD TYPES" ARTICLE WITH A LINK TO THIS ARTILE INSTEAD AND REMOVE THE STEPS FROM THE "EDIT RECORD TYPES" ARTICLE ON HOW TO ALLOW CROSS-WORKSPACE SETTINGS FOR RECORD TYPES*************-->


<!--this article is linked to the UI - do not delete or change the URL-->

<!--THIS MIGHT ALREADY BE ADDED TO THE "OVERVIEW" ARTICLE, BUT CHECK: add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# Configurare le funzionalità tra aree di lavoro diverse per i tipi di record

<!--this is linked to the UI in the info icon when you enable a record to be either global or connectable-->

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

È possibile configurare i tipi di record in modo che funzionino in più aree di lavoro.

Di seguito sono riportate le funzionalità dei tipi di record in più aree di lavoro:

* È possibile designare un tipo di record come globale. Gli utenti possono aggiungere tipi di record globali ad altre aree di lavoro che possono gestire.
* È possibile designare un tipo di record come collegabile. Gli utenti possono connettersi a questo tipo di record da altre aree di lavoro.

È necessario innanzitutto definire le funzionalità di un tipo di record in più aree di lavoro prima che i responsabili dell&#39;area di lavoro possano collegarlo o aggiungerlo ad altre aree di lavoro.

Quando si crea o si modifica un tipo di record, è possibile definire le funzionalità di un tipo di record in più aree di lavoro.

Per informazioni, vedere uno degli articoli seguenti:

* [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md)
* [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr>

</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<ul><li><p>Qualsiasi pacchetto Workfront</p></li>
<p>E</p>
<li><p>Qualsiasi pacchetto Planning per la creazione di tipi di record collegabili</p></li>
<li><p>Pacchetto Planning Plus per la creazione di tipi di record globali</p></li>
</ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Configurare i tipi di record globali

<!--this is a UI term; don't change the title of this section-->

In qualità di responsabile dell&#39;area di lavoro, è possibile configurare un tipo di record come tipo di record globale. È possibile aggiungere un tipo di record globale ad altre aree di lavoro.

Un gestore dell&#39;area di lavoro può aggiungere un tipo di record globale a un&#39;area di lavoro gestita. Vengono aggiunti anche i campi originali del tipo di record.

Gli utenti possono aggiungere record a un tipo di record globale da qualsiasi area di lavoro per cui dispongono delle autorizzazioni Contribute e in cui viene aggiunto il tipo di record globale, inclusa l&#39;area di lavoro originale. Possono visualizzare i record dall’area di lavoro a cui dispongono solo delle autorizzazioni di visualizzazione.

Per ulteriori informazioni, vedere [Panoramica sui tipi di record tra aree di lavoro](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

Per configurare un tipo di record come globale:

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera configurare i tipi di record come globali.

   Viene visualizzata la pagina dell&#39;area di lavoro e i tipi di record.
1. Esegui una delle operazioni seguenti:

   * Passa il puntatore del mouse sulla scheda di un tipo di record e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro della scheda del tipo di record

     ![Altre opzioni di menu dalla scheda del tipo di record](assets/more-menu-options-from-record-type-card.png)

   * Fai clic su una scheda del tipo di record per aprire la pagina del tipo di record, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record.
1. Fai clic su **Modifica** o **Impostazioni**.

   >[!TIP]
   >
   >Quando un tipo di record viene aggiunto a un&#39;altra area di lavoro, viene visualizzato come tipo di record globale in tale area di lavoro. In questo caso, le opzioni Modifica e Impostazioni sono disattivate.

1. (Condizionale) Se hai fatto clic su **Modifica**, nella casella **Modifica tipo di record**, fai clic sulla scheda **Impostazioni per più aree di lavoro**

   Oppure, se hai fatto clic su **Impostazioni**, vai alla sezione **Impostazioni per più aree di lavoro** nel pannello a sinistra.
1. Abilita l&#39;impostazione **Consenti l&#39;aggiunta di questo tipo di record ad altre aree di lavoro**.

   ![Modifica impostazioni tra aree di lavoro del tipo di record con l&#39;opzione Aggiungi ad altre aree di lavoro abilitata](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >Dopo aver aggiunto un tipo di record globale a un&#39;altra area di lavoro, questa impostazione non può più essere disabilitata.

1. Nel campo **Selezionare gli utenti che possono aggiungere questo tipo di record alle aree di lavoro che gestiscono**, aggiungere le entità che si desidera consentire di aggiungere questo tipo di record alle aree di lavoro che gestiscono.

   Il tuo nome viene aggiunto automaticamente nel campo.

   È possibile aggiungere singoli utenti o gruppi, team, mansioni o società di cui si desidera consentire l&#39;aggiunta di questo tipo di record alle aree di lavoro che gestiscono.

   È possibile modificare questo campo dopo aver salvato il tipo di record.

1. (Facoltativo) Rimuovi il tuo nome dal campo **Seleziona gli utenti che possono aggiungere questo tipo di record alle aree di lavoro che gestiscono**.

   >[!TIP]
   >
   >È necessario designare almeno un&#39;entità (utente, team, gruppo, mansione o società) per abilitare questa impostazione.


1. (Condizionale) Fai clic su **Salva** nella casella **Modifica tipo di record** oppure fai clic sulla freccia indietro a sinistra di **Impostazioni** nell&#39;intestazione della pagina per salvare le modifiche.

   Si verificano le seguenti situazioni:

   * Il tipo di record e i relativi campi sono ora disponibili per essere aggiunti a un&#39;altra area di lavoro dalle persone designate.

   >[!NOTE]
   >
   >È possibile modificare l&#39;aspetto e le impostazioni del tipo di record e i relativi campi originali solo dall&#39;area di lavoro originale.

   * Nella scheda del tipo di record viene visualizzata l&#39;icona globale ![Icona del tipo di record globale](assets/global-icon.png) per indicare che il tipo di record è disponibile per l&#39;aggiunta ad altre aree di lavoro.
   * Un campo **Workspace** generato dal sistema viene aggiunto alla vista tabella del tipo di record e dei relativi dettagli.

     Nel campo Workspace viene visualizzata l&#39;area di lavoro da cui viene creato ogni record.

     Questo campo è di sola lettura e non può essere eliminato.
1. (Facoltativo) Passare a un&#39;altra area di lavoro e creare un tipo di record utilizzando un tipo di record esistente. Selezionare il tipo di record abilitato nei passaggi precedenti.

   Per informazioni, vedere [Aggiungere tipi di record esistenti da un&#39;altra area di lavoro](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

## Configura tipi di record collegabili

<!--this is a UI term; don't change the title of this section-->

È possibile configurare un tipo di record per la connessione da altre aree di lavoro quando si crea o si modifica il tipo di record.

Per configurare un tipo di record come collegabile:

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera configurare i tipi di record come collegabile.

   Viene visualizzata la pagina dell&#39;area di lavoro e i tipi di record.
1. Esegui una delle operazioni seguenti:

   * Passa il puntatore del mouse sulla scheda di un tipo di record e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro della scheda del tipo di record

     ![Altre opzioni di menu dalla scheda del tipo di record](assets/more-menu-options-from-record-type-card.png)

   * Fai clic su una scheda del tipo di record per aprire la pagina del tipo di record, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record.
1. Fai clic su **Modifica** o **Impostazioni**.

1. (Condizionale) Se hai fatto clic su **Modifica**, nella casella **Modifica tipo di record**, fai clic sulla scheda **Impostazioni per più aree di lavoro**

   Oppure, se hai fatto clic su **Impostazioni**, vai alla sezione **Impostazioni per più aree di lavoro** nel pannello a sinistra.

1. Abilita l&#39;impostazione **Consenti la connessione a questo tipo di record in altre aree di lavoro**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Modifica tipo di record Scheda Impostazioni area di lavoro incrociata con connessione da altre aree di lavoro abilitata](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Se attivato, il tipo di record è accessibile e può essere connesso ad altre aree di lavoro.

1. Scegliere le aree di lavoro da cui è possibile accedere al tipo di record. Scegli una delle seguenti opzioni:

   * **A livello di sistema**: gli utenti possono connettersi a questo tipo di record da tutte le aree di lavoro per le quali dispongono delle autorizzazioni di gestione.
   * **Aree di lavoro specifiche**: aggiungere i nomi delle aree di lavoro a cui i responsabili area di lavoro possono connettersi a questo tipo di record.
1. (Condizionale) Fai clic su **Salva** nella casella **Modifica tipo di record** oppure fai clic sulla freccia indietro a sinistra di **Impostazioni** nell&#39;intestazione della pagina per salvare le modifiche.

   Si verificano le seguenti situazioni:

   * Il tipo di record e i relativi campi sono ora disponibili per la connessione alle aree di lavoro specificate.
   * Nella scheda del tipo di record viene visualizzata l&#39;icona di connessione tra più aree di lavoro ![Icona di connessione tra aree di lavoro](assets/connect-from-other-workspaces-icon.png) per indicare che il tipo di record è disponibile per la connessione da qualsiasi area di lavoro designata nella configurazione.

   Il tipo di record diventa disponibile per la connessione alle aree di lavoro specificate.
1. (Facoltativo) Vai a un’altra area di lavoro e aggiungi una connessione al tipo di record abilitato per la connessione tra aree di lavoro diverse nei passaggi precedenti.

   Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).









