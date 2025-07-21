---
title: Configurare le funzionalità tra aree di lavoro diverse per il tipo di record
description: È possibile abilitare un tipo di record per l'aggiunta a un'altra area di lavoro o per la connessione da un'altra area di lavoro.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 943c26efa6f6351abf885dbc5f3aa09c0b0fab05
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->

<!--this is linked to the UI in the info icon of when you create a record type from a global record type-->

# Configurare le funzionalità tra aree di lavoro diverse per i tipi di record

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

È possibile designare un tipo di record da aggiungere a un&#39;altra area di lavoro o da connettere da un&#39;altra area di lavoro in Adobe Workfront Planning.

È necessario innanzitutto definire le funzionalità di un tipo di record in più aree di lavoro prima che i responsabili dell&#39;area di lavoro possano collegarlo o importarlo in altre aree di lavoro.

Quando si crea o si modifica un tipo di record, è possibile definire le funzionalità di un tipo di record in più aree di lavoro.

Per informazioni, vedere uno degli articoli seguenti:

* [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md)
* [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md)

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare l’aggiunta di un tipo di record ad altre aree di lavoro

In qualità di responsabile del workspace, è possibile configurare un tipo di record da aggiungere ad altre aree di lavoro quando si crea o si modifica un tipo di record.

Quando si configura l&#39;aggiunta di un tipo di record ad altre aree di lavoro, un manager area di lavoro può importare il tipo di record e tutte le relative informazioni in una delle aree di lavoro gestite.

Per configurare l&#39;aggiunta di un tipo di record a un&#39;altra area di lavoro quando si modifica il tipo di record:

{{step1-to-planning}}

1. Fare clic sul workspace di cui si desidera modificare i tipi di record.

   Viene visualizzata la pagina dell&#39;area di lavoro e i tipi di record.
1. Esegui una delle operazioni seguenti:

   * Passa il puntatore del mouse sulla scheda di un tipo di record e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro della scheda del tipo di record
Oppure
   * Fai clic su una scheda del tipo di record per aprire la pagina del tipo di record, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record.
1. Fai clic su **Modifica**.

   ![Altre opzioni di menu dalla scheda del tipo di record](assets/more-menu-options-from-record-type-card.png)

1. Nella casella **Modifica tipo di record** selezionare la scheda **Impostazioni avanzate**.
1. Abilita l&#39;impostazione **Consenti l&#39;aggiunta di questo tipo di record ad altre aree di lavoro**.

   ![Modifica impostazioni avanzate tipo di record con Aggiungi ad altre aree di lavoro abilita](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

1. Nel campo **Selezionare gli utenti che possono aggiungere questo tipo di record alle aree di lavoro che gestiscono**, aggiungere gli utenti che si desidera consentire di aggiungere questo tipo di record alle aree di lavoro che gestiscono.

   Il tuo nome viene aggiunto automaticamente nel campo.

   È possibile aggiungere singoli utenti o gruppi, team, mansioni o società di cui si desidera consentire l&#39;aggiunta di questo tipo di record alle aree di lavoro che gestiscono.

   È possibile modificare questo campo dopo aver salvato il tipo di record.
1. (Facoltativo) Rimuovi il tuo nome dal campo **Seleziona gli utenti che possono aggiungere questo tipo di record alle aree di lavoro che gestiscono**.

1. Fai clic su **Salva**.

   Si verificano le seguenti situazioni:

   * Il tipo di record e i relativi campi sono ora disponibili per essere aggiunti a un&#39;altra area di lavoro dalle persone designate.

   >[!NOTE]
   >
   >È possibile modificare il tipo di record e i relativi campi solo dall&#39;area di lavoro originale.

   * Nella scheda del tipo di record viene visualizzata un&#39;icona globale ![Icona del tipo di record globale](assets/global-icon.png) per indicare che il tipo di record è disponibile per essere aggiunto a qualsiasi area di lavoro di cui è stato designato il manager nella configurazione.
   * Al tipo di record è stato aggiunto un campo **Workspace** generato dal sistema.

     Nel campo Workspace viene visualizzata l&#39;area di lavoro da cui è stato creato ogni record.

     Questo campo è di sola lettura e non può essere eliminato.

## Configurare la connessione a un tipo di record da altre aree di lavoro

È possibile configurare un tipo di record a cui connettersi da altre aree di lavoro quando si crea o si modifica il tipo di record.

Per configurare un tipo di record a cui connettersi da altre aree di lavoro quando si modifica il tipo di record:

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera modificare i tipi di record.

   Viene visualizzata la pagina dell&#39;area di lavoro e i tipi di record.
1. Esegui una delle operazioni seguenti:

   * Passa il puntatore del mouse sulla scheda di un tipo di record e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro della scheda del tipo di record, quindi fai clic su **Modifica**
Oppure
   * Fai clic su una scheda del tipo di record per aprire la pagina del tipo di record, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del tipo di record, quindi fai clic su **Modifica**.

   ![Altre opzioni di menu dalla scheda del tipo di record](assets/more-menu-options-from-record-type-card.png)

1. Nella casella **Modifica tipo di record** selezionare la scheda **Impostazioni avanzate**.
1. Abilita l&#39;impostazione **Consenti la connessione a questo tipo di record in altre aree di lavoro**. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Modifica tipo di record Scheda Impostazioni avanzate con connessione da altre aree di lavoro abilitata](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Se attivato, il tipo di record è accessibile e può essere connesso da altre aree di lavoro.

1. Scegliere le aree di lavoro da cui è possibile accedere al tipo di record. Scegli una delle seguenti opzioni:

   * **A livello di sistema**: gli utenti possono connettersi a questo tipo di record da tutte le aree di lavoro in cui dispongono di autorizzazioni di gestione.
   * **Aree di lavoro specifiche**: aggiungere i nomi delle aree di lavoro a cui i responsabili area di lavoro possono connettersi a questo tipo di record.
1. Fai clic su **Modifica**.

   Si verificano le seguenti situazioni:

   * Il tipo di record e i relativi campi sono ora disponibili per la connessione dalle aree di lavoro specificate.
   * Nella scheda del tipo di record viene visualizzata l&#39;icona di connessione tra più aree di lavoro ![Icona di connessione tra aree di lavoro](assets/connect-from-other-workspaces-icon.png) per indicare che il tipo di record è disponibile per la connessione da qualsiasi area di lavoro designata nella configurazione.

   Il tipo di record diventa disponibile per la connessione dalle aree di lavoro specificate.









