---
title: Condividi campi Workfront Planning
description: È possibile condividere il campo di un record di Workfront Planning con altri utenti per garantire la collaborazione quando si utilizza Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: b529b3aded4ab92015683a0ddccd152bc2cc798c
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 3%
---

# Condividere i campi di Workfront Planning

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

È possibile condividere il campo di un record di Workfront Planning con altri utenti per garantire la collaborazione quando si utilizza Adobe Workfront Planning.

La condivisione dei campi consente agli amministratori dell’area di lavoro di controllare l’accesso a un singolo campo. Ogni campo di un tipo di record dispone di una propria finestra di dialogo di condivisione in cui l&#39;accesso può essere impostato su Nessun accesso, Visualizza valori di campo o Gestisci valori di campo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->



<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi Workfront o flusso di lavoro con un pacchetto Planning</p> 
Oppure
<p>Qualsiasi pacchetto di prodotti Workfront Planning come unità autonoma</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Qualsiasi</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Planning</p></td> 
   <td><p>Qualsiasi</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>È necessario aggiungere sia un flusso di lavoro che un tipo di licenza Planning al livello di accesso quando si dispone sia di un flusso di lavoro che di un pacchetto Planning</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td><p>Gestire le autorizzazioni per un campo per modificare i valori del campo</p>  
   <p>Contribuire o concedere autorizzazioni superiori a un tipo di record per ereditare le autorizzazioni Manage per il campo</p>  
   </td> 
  </tr>
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulla condivisione dei campi

* Puoi condividere i campi con utenti, mansioni, gruppi, team o aziende.
* È possibile condividere i campi solo dalla vista tabella di un tipo di record.
* Non puoi condividere i seguenti tipi di campi:

  * Campi di sistema (ad esempio Creato da, ID record)
  * Campi principali
  * Campi di ricerca. Ereditano sempre le autorizzazioni dei campi oggetto di origine.
* L’accesso a un campo proviene dalla combinazione delle seguenti impostazioni:

  * **Autorizzazioni ereditate**: per impostazione predefinita, un campo eredita lo stesso accesso di un utente sul tipo di record. È possibile disattivare le autorizzazioni ereditate e concedere agli utenti un accesso al campo inferiore a quello di cui dispongono per il tipo di record.
  * **Tutti nell&#39;area di lavoro possono visualizzare** o **Solo gli invitati possono accedere alla selezione**. Puoi consentire a tutti coloro che dispongono delle autorizzazioni per l’area di lavoro di visualizzare il campo o concedere le autorizzazioni solo a singole entità.

  Se più regole si applicano alla stessa persona, questa riceve l’autorizzazione più elevata disponibile da una delle regole.

* A seconda delle autorizzazioni per il tipo di record, gli utenti possono ricevere le seguenti autorizzazioni per i campi:

  * Le autorizzazioni di visualizzazione del tipo di record consentono a un utente di visualizzare i valori dei campi
  * Le autorizzazioni Contribute (Contribute) o Manage (Manage) per i tipi di record consentono a un utente di gestire i valori dei campi

* Solo i proprietari e i responsabili dell&#39;area di lavoro possono modificare le autorizzazioni dei campi. I manager di Workspace mantengono sempre l&#39;accesso Gestisci a tutti i campi e questo non può essere ridotto.
* La condivisione dei campi controlla l&#39;accesso ai valori, non alle impostazioni dei campi. Solo i responsabili del workspace possono modificare la configurazione di un campo.
* L&#39;aggiunta di un utente all&#39;elenco di condivisione di un campo non consente l&#39;accesso all&#39;area di lavoro o al tipo di record. Se non dispongono di tale accesso, un&#39;icona di avviso indica che l&#39;autorizzazione avrà effetto solo dopo essere state aggiunte al tipo di record.
* I campi con autorizzazioni limitate vengono applicati ovunque venga visualizzato il campo. Ciò include tutte le visualizzazioni, le pagine dei dettagli dei record, i moduli di richiesta, le connessioni e i campi di ricerca, le dashboard di Canvas, gli strumenti API e MCP.
* Le visualizzazioni pubbliche rimangono completamente visibili e di sola lettura per chiunque possa accedervi.
  <!--Not sure if this is right - right now, it allows me to duplicate with the values in the new record - checking with Lilit: * When you duplicate a record, the restricted values are not copied to the new records.-->
* Le modifiche al valore del campo con restrizioni non vengono registrate nella cronologia di un record.
* Le modifiche delle autorizzazioni per i campi non attivano le notifiche.
* Per i tipi di record globali, le autorizzazioni del campo si applicano a tutte le aree di lavoro secondarie e non possono essere regolate localmente.

<!--
From Claude: 
Additional permissions for fields - maybe add this to the Overview article for all of the sharing?? - help/quicksilver/planning/access/sharing-permissions-overview.md 

Here's how record type / workspace access maps to field-level access in the document:

Field permission levels (only two, plus none):

No Access – field is completely hidden
View field values – can see the value, can't edit
Manage field values – can view and edit

Default inheritance from record type role

Record type / workspace access    Default field permission
View    View field values
Contribute    Manage field values
Manage (workspace manager)    Manage field values (locked — cannot be reduced)

So by default, a field simply mirrors whatever role someone has on the record type — Viewers get read-only, Contributors and Managers get edit rights. Workspace managers are a special case: whenever they're added to a field's sharing list, "Manage field values" is pre-selected and the "View field values" option is disabled, since their edit access can never be taken away.

Wildcard (fallback) setting
Separate from inheritance, each field has a wildcard default:

Everyone in the workspace can view (default)
Only invited people can access

How the final permission is calculated

If inherited permissions are enabled: a person's access = the highest of (inherited from record type, wildcard, individually granted permission).
If inherited permissions are disabled: a person's access = the highest of (wildcard, individually granted permission) — record type role no longer factors in.
If inheritance is disabled, wildcard is "Only invited people can access," and the person isn't individually added → they get No Access.

Other permission notes

Individually granting access to someone doesn't grant them workspace/record-type access — it just sits inactive (with a warning icon) until they're separately added to the workspace.
For Global Record Types, field permissions are set once and apply to all secondary workspaces; secondary/team workspace managers cannot override them locally.

-->

## Condividi campi

In qualità di manager dell&#39;area di lavoro, puoi modificare le autorizzazioni per i singoli campi.

{{step1-to-planning}}

1. Aprire l&#39;area di lavoro, quindi il tipo di record di cui si desidera condividere i campi.

1. Dalla vista tabella, passa il puntatore del mouse sul nome dell&#39;intestazione di colonna di un campo, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Condividi campo**.

   Viene visualizzata la casella **Condividi**.

1. (Facoltativo) Nell&#39;area **Concedi accesso**, l&#39;opzione **Tutti nell&#39;area di lavoro possono visualizzare** è selezionata per impostazione predefinita. Tutti gli utenti con autorizzazioni **Visualizza** o superiori per l&#39;area di lavoro e il tipo di record dispongono delle stesse autorizzazioni per il campo.

1. (Facoltativo) Fai clic sugli avatar degli utenti nell&#39;opzione **Autorizzazioni ereditate da** per visualizzare utenti, team, gruppi, aziende o ruoli che ereditano le autorizzazioni dall&#39;area di lavoro.

   Le autorizzazioni dell&#39;utente per il tipo di record vengono visualizzate quando si espandono le autorizzazioni ereditate.

   >[!TIP]
   >
   >Non è possibile rimuovere singole entità dall&#39;elenco delle autorizzazioni ereditate. Vengono elencati gli utenti di team, gruppi, aziende o mansioni anziché le entità a cui erano associati quando l’area di lavoro e il tipo di record sono stati condivisi con loro.

1. (Facoltativo e condizionale) Se si desidera condividere il campo con entità specifiche e concedere loro un accesso al campo diverso da quello già disponibile per il tipo di record, eseguire le operazioni seguenti:

   1. Deseleziona l&#39;opzione **Attivato** da **Autorizzazioni ereditate**. È selezionata per impostazione predefinita.

      L&#39;opzione diventa **Disattivata**.

      >[!TIP]
      >
      >I manager di Workspace continuano a disporre delle autorizzazioni di gestione per il tipo di record e il campo.

   1. Nella casella **Concedi l&#39;accesso**, aggiungi gli utenti, i team, i gruppi, le aziende o le mansioni a cui desideri concedere un livello di autorizzazione diverso da quello che hanno per l&#39;area di lavoro o il tipo di record.

      Quando condividi un campo con un utente, anche la mansione principale e l’e-mail vengono visualizzate nel campo. Per poter visualizzare l&#39;e-mail dell&#39;utente, è necessario che l&#39;impostazione Visualizza informazioni di contatto sia abilitata per l&#39;oggetto Users nel proprio livello di accesso.

   1. Scegliere uno dei seguenti livelli di autorizzazione:

      * Visualizza valori dei campi
      * Gestisci valori dei campi

      >[!IMPORTANT]
      >
      ><!-- * If users have Contribute or Manage permissions to the workspace and the record type, you can give them Manage permissions to the field. The View permission is dimmed.-->
      >* Non è possibile concedere agli utenti un&#39;autorizzazione inferiore per il campo se dispongono di Contribute o di un&#39;autorizzazione superiore per il tipo di record.
      >
      >* Non puoi concedere autorizzazioni a utenti che non si trovano nell’area di lavoro. Gli utenti che non dispongono di autorizzazioni per l’area di lavoro e il tipo di record non possono accedere a nessuno dei campi. Potranno accedere ai campi quando ottengono le autorizzazioni per l’area di lavoro e i tipi di record.

1. Fai clic su **Salva**.

   Il campo ora è condiviso con altri utenti.

   <!--
    Not possible for fields: 
    The users you shared the field with receive both an in-app and email notification about having been given permissions to the field.
    For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md).
    -->

## Rimuovere le autorizzazioni per un campo

Puoi rimuovere le autorizzazioni degli utenti da un campo. Tuttavia, manterranno almeno le autorizzazioni View (Visualizzazione) per l’area di lavoro e il tipo di record, che concedono loro almeno le autorizzazioni View (Visualizzazione) per il campo.

È necessario rimuoverne l&#39;accesso dall&#39;area di lavoro se si desidera che non dispongano di autorizzazioni per i tipi di record o i campi nell&#39;area di lavoro.

Non è possibile rimuovere un utente dalle autorizzazioni ereditate.

{{step1-to-planning}}

1. Aprire l&#39;area di lavoro di cui si desidera interrompere la condivisione dei campi, quindi fare clic su una scheda del tipo di record. Verrà aperta la pagina del tipo di record.
1. Dalla vista tabella, passa il puntatore del mouse sul nome dell&#39;intestazione di colonna di un campo, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Condividi campo**.

   Viene visualizzata la casella **Condividi**.
1. Individuare l&#39;utente, il gruppo, il team, la società o la mansione che si desidera rimuovere, espandere il menu a discesa delle autorizzazioni a destra del nome, quindi fare clic su **Rimuovi**.

1. Fai clic su **Salva**.

   Le persone non dispongono più delle autorizzazioni indicate per il campo. Tuttavia, dispongono ancora delle autorizzazioni per il tipo di record e l’area di lavoro, a meno che non vengano rimosse anche da tali autorizzazioni.

   Agli utenti che sono stati rimossi dall’accesso al campo non viene notificato di non disporre più di queste autorizzazioni.
