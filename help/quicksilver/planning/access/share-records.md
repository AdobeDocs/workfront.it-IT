---
title: Condividi record
description: Puoi condividere i record utilizzando il pulsante Condividi per aumentare la collaborazione in Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 9ffad1aa-3c96-40fa-9c62-7a3e00699f18
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: fdbe3945f59306fc26424d7e88b799d9dcaea4da
workflow-type: tm+mt
source-wordcount: '1700'
ht-degree: 2%

---

<!--update metadata with real information at release-->

# Condividere i record

<!--
this will NOT be available in Preview ever - find a way to add this in this article that is prominent
-->

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>\
<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

In Adobe Workfront Planning è possibile modificare le autorizzazioni delle persone per singoli record di un tipo di record.

È possibile condividere un record di Adobe Workfront Planning nei modi seguenti:

* Condividere un collegamento al record.

  Per ulteriori informazioni, vedere [Condividere record utilizzando un collegamento](/help/quicksilver/planning/records/share-records.md).

* Condividere tutti i record di un&#39;area di lavoro con altri utenti condividendo l&#39;area di lavoro e il tipo di record.

  Per ulteriori informazioni, consulta i seguenti articoli:

   * [Condividere un’area di lavoro](/help/quicksilver/planning/access/share-workspaces.md)

   * [Condividere un tipo di record](/help/quicksilver/planning/access/share-record-types.md)

* Condividi un singolo record o condividi più record in blocco utilizzando l&#39;opzione **Condividi**.

  In questo articolo viene descritto come condividere i record con altri utenti utilizzando l&#39;opzione **Condividi**.

>[!IMPORTANT]
>
>* Gli utenti con accesso a un&#39;area di lavoro ottengono automaticamente almeno le autorizzazioni di visualizzazione per tutti i record dell&#39;area di lavoro.
>* La condivisione delle visualizzazioni non concede agli utenti le autorizzazioni per i record. Solo le aree di lavoro condivise possono concedere agli utenti le autorizzazioni per tipi di record e record.
>
>Per informazioni generali sulla condivisione di oggetti in Workfront Planning, vedere anche [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

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
<p>Qualsiasi pacchetto Workfront e Planning</p> 
Oppure
<p>Qualsiasi pacchetto di Workflow e Planning</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Qualsiasi</p> 
   <p><b>NOTA</b></p>
   <p>Solo le persone con una licenza Standard possono ottenere le autorizzazioni di gestione per i record. Tutte le altre licenze possono disporre solo delle autorizzazioni di visualizzazione e l’opzione Gestisci non è attiva.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>  <p>Gestire le autorizzazioni per un'area di lavoro, un tipo di record e il record</p>  
   <p><b>IMPORTANTE</b></p>
   <p>Solo gli utenti con le autorizzazioni di gestione di un'area di lavoro possono condividere un record</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> Agli utenti con una licenza Light o Contributor deve essere assegnato un modello di layout che includa Planning.
   <p>Per impostazione predefinita, le aree Pianificazione sono attivate dagli utenti standard e dagli amministratori di sistema.</p></div></li></ul>
</td>
  </tr>

</tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni durante la condivisione dei record

<!--
maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information
-->

<!--checking on the below with Lilit-->

* Puoi condividere i record con le seguenti entità: persone, gruppi, team, aziende o mansioni.
* Se si limitano le autorizzazioni a un record, gli utenti non visualizzano più il record e i valori dei relativi campi di ricerca in qualsiasi punto del sistema in cui viene visualizzato il record.
* Workfront controlla le autorizzazioni dei record nelle connessioni fino a 5 record in profondità, garantendo agli utenti di visualizzare solo i record condivisi con loro.
* È possibile concedere a un record i livelli di autorizzazione seguenti:

   * Visualizzazione
   * Gestione
* Per impostazione predefinita, quando si condivide un&#39;area di lavoro e un tipo di record con gli utenti, questi ultimi ricevono anche le stesse autorizzazioni per i record nell&#39;area di lavoro.
Quando gli utenti dispongono delle autorizzazioni Contribute per un&#39;area di lavoro o un tipo di record, ricevono le autorizzazioni Manage (Gestione) per i record di quel tipo.
* Quando rimuovi un’entità da un’area di lavoro, tutte le autorizzazioni di condivisione vengono rimosse dai tipi di record e da tutti i record in essa contenuti.
* Non è possibile condividere un record con un utente che non dispone di autorizzazioni per l&#39;area di lavoro o il tipo di record.
* L’accesso di un utente al record è determinato dalla combinazione delle tre impostazioni seguenti:

   * Le relative autorizzazioni ereditate dal tipo di record e dall’area di lavoro
   * Autorizzazioni aggiunte singolarmente nella casella di condivisione dei record
   * L&#39;impostazione **Everyone nell&#39;area di lavoro può visualizzare**.

     In questo modo il record sarà visibile a tutti gli utenti dell&#39;area di lavoro

     <!--
      Cannot do this on a record: 
      * **Only invited people can access**: This is selected by default and allows restricting access to the record to specific people. 
      -->

* Per impostazione predefinita, quando si condivide un record con un utente, questi vengono aggiunti con la stessa autorizzazione disponibile per il tipo di record.

  Ad esempio:

   * Se dispongono delle autorizzazioni di visualizzazione per il tipo di record, ottengono le autorizzazioni di visualizzazione per il record
   * Se dispongono delle autorizzazioni Contribuisci o Gestisci per il tipo di record, ottengono le autorizzazioni Gestione per il record

* Quando un utente dispone delle autorizzazioni Gestisci o Contribuisci per l’area di lavoro e il tipo di record e li aggiungi alle autorizzazioni del record, le autorizzazioni Visualizza vengono disattivate. Mantengono le stesse autorizzazioni del record di quelle del tipo di record e non è possibile concedere loro autorizzazioni inferiori.

* È possibile disabilitare le autorizzazioni ereditate per un singolo record, nel qual caso è possibile assegnare a determinati utenti le autorizzazioni per singoli record oppure ottenere le autorizzazioni se appartengono all&#39;area di lavoro, a causa dell&#39;opzione **Tutti nell&#39;area di lavoro possono visualizzare**.

* Se più autorizzazioni di condivisione si applicano allo stesso utente, quest&#39;ultimo riceve l&#39;autorizzazione più elevata.

  Ad esempio, se un record viene condiviso con un utente con autorizzazioni di visualizzazione e il relativo gruppo con l&#39;accesso Gestisci, questi riceveranno le autorizzazioni di gestione per il record.

* Se un campo formula o un campo di ricerca di un record connesso è basato su un campo di un record per il quale non si dispone di autorizzazioni, verrà visualizzato il calcolo corretto per i fattori del record ai quali non è possibile accedere in altro modo.

  <!--
   Not possible: 
   * As a workspace manager, you can share a record with a user that does not have permissions to the record type or the workspace. In this case, there is a warning next to the added entity notifying you that they don't have access to the workspace or the record type.  You can continue adding the user to the record which will also add them to the record type and workspace, or cancel the sharing.
   -->

  <!--
   ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too
   -->

<!--
Lilit is checking on this, it is not working correctly
-->

<!--
   check on this: I cannot disable inherited permissions when this setting is ON and this documented in a TIP below: When they have View permissions to the workspace or the record type, they retain View permissions to the records. You can grant them Manage permissions to the record by disabling Inherited permissions and selecting the Only invited people can access setting.
   -->

<!-- 
   not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.
   -->

<!--
   Too granular??
   If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 
   If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions 
   -->

<!--
   not sure if any of the Share record types points might match here - ask Lilit??
   -->

## Condividere i record

In qualità di manager dell&#39;area di lavoro, è possibile modificare le autorizzazioni per singoli record.

{{step1-to-planning}}

1. Aprire l&#39;area di lavoro, quindi il tipo di record di cui si desidera condividere i record.

1. Esegui una delle operazioni seguenti:

   * Nella vista tabella, passa il puntatore del mouse sul nome di un record e fai clic sul menu **Altro** ![Altro](assets/more-menu.png), quindi fai clic su **Condividi**.
   * Nella vista a tabella, seleziona uno o più record, quindi fai clic su **Condividi** nella barra degli strumenti blu in fondo all&#39;elenco.
   * Da qualsiasi visualizzazione, fai clic sul nome di un record, quindi fai clic su **Condividi** nell&#39;angolo superiore destro della pagina dei dettagli del record.

   Viene visualizzata la casella **Condividi**.

   ![Autorizzazioni per i record con autorizzazioni ereditate su](assets/permissions-for-records-with-inherited-permissions-on.png)

   >[!WARNING]
   >
   >Non è possibile condividere le autorizzazioni con record aggiunti in aree di lavoro diverse. Quando si condividono record in blocco, tutti i record devono essere creati nella stessa area di lavoro.

1. (Facoltativo) Nell&#39;area **Chi ha accesso**, l&#39;opzione **Tutti nell&#39;area di lavoro possono visualizzare** è selezionata per impostazione predefinita.  Tutti gli utenti con autorizzazioni **View** o superiori per l&#39;area di lavoro e il tipo di record dispongono delle stesse autorizzazioni per il record.

1. (Facoltativo) Fai clic sugli avatar degli utenti nell&#39;opzione **Autorizzazioni ereditate da** per visualizzare utenti, team, gruppi, aziende o ruoli che ereditano le autorizzazioni dall&#39;area di lavoro. <!--logged bug to move "Permissions" to lowercase-->

   Le autorizzazioni dell&#39;utente per il tipo di record vengono visualizzate quando si espandono le autorizzazioni ereditate.

   >[!TIP]
   >
   >Non è possibile rimuovere singole entità dall&#39;elenco delle autorizzazioni ereditate. Vengono elencati gli utenti di team, gruppi, aziende o mansioni anziché le entità a cui erano associati quando l’area di lavoro e il tipo di record sono stati condivisi con loro.

1. (Facoltativo e condizionale) Se si desidera condividere il record con entità specifiche e concedere loro un accesso diverso al tipo di record rispetto a quello già disponibile per l&#39;area di lavoro, eseguire le operazioni seguenti:

   1. Deseleziona l&#39;opzione **Attivato** da **Autorizzazioni ereditate**. È selezionata per impostazione predefinita.

      L&#39;opzione diventa **Disattivata**.

      >[!TIP]
      >
      >I responsabili di Workspace e i creatori di record continuano a disporre delle autorizzazioni di gestione per il tipo di record e il record.

      <!-- 
      This is no longer possible for a record: 
      (Optional) Select **Only invited people can access** from the **Who has access** area. You must indicate individual users, groups, teams, or companies to share the records with. 
      >[!TIP]
      >
      >You cannot disable or enable Inherited permissions when this setting is selected.
      -->

   1. Nel campo **Concedi l&#39;accesso a questo record**, aggiungi gli utenti, i team, i gruppi, le aziende o le mansioni a cui desideri concedere un livello di autorizzazione diverso da quello che hanno per l&#39;area di lavoro o il tipo di record.

      Quando condividi un record con un utente, anche la mansione principale e l’e-mail vengono visualizzate nel campo. Per poter visualizzare l&#39;e-mail dell&#39;utente, è necessario che l&#39;impostazione Visualizza informazioni di contatto sia abilitata per l&#39;oggetto Users nel proprio livello di accesso.

   1. Scegliere uno dei seguenti livelli di autorizzazione:

      * Visualizzazione
      * Gestione

      >[!IMPORTANT]
      >
      >* Se gli utenti dispongono delle autorizzazioni Contribute (Contribuisci) o Manage (Gestisci) per l&#39;area di lavoro e il tipo di record, potete assegnare loro le autorizzazioni Manage (Gestisci) per il record. L’autorizzazione Visualizzazione è disabilitata.
      >* Non potete concedere agli utenti un&#39;autorizzazione minore per il record se dispongono di Contribute o di una versione successiva per il tipo di record.
      >Per ulteriori informazioni, vedere [Panoramica sulle autorizzazioni di condivisione in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
      >* Non puoi concedere autorizzazioni a utenti che non si trovano nell’area di lavoro. Gli utenti che non dispongono delle autorizzazioni per l&#39;area di lavoro e il tipo di record non possono accedere a nessuno dei record.

   <!--   
   Not possible:
   1. To give users who do not have permissions to the workspace access to view a record, in the **Grant access to this view** field, start typing the name of a user, a group, team, company, or job role, then click it when it displays in the list. 
      The entity you selected is added to the record and also to the record type and the workspace with **View** permissions. 
      System administrators always receive Manage permissions to records shared with them, and there is an indication that a user is a System administrator.
   -->

1. (Facoltativo) Fai clic su **Copia collegamento** per copiare un collegamento al record negli Appunti e condividerlo con altri utenti. Il collegamento apre la pagina dei dettagli del record.
1. Fai clic su **Salva**.

   Il record è ora condiviso con altri utenti.

   Gli utenti con cui hai condiviso il record ricevono una notifica in-app e una notifica e-mail relativa alle autorizzazioni concesse al record.

   <!--
   not possible anymore: 
   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them.
   -->

   Per informazioni, vedere [Notifiche di Adobe Workfront Planning: indice articolo](/help/quicksilver/planning/notifications/notifications-information.md).


1. (Facoltativo) Condividi il collegamento copiato con altri utenti.

   Gli utenti che ricevono il collegamento devono essere utenti attivi e accedere a Workfront per poter accedere alla pagina del tipo di record e visualizzarla nella visualizzazione selezionata.

   Per visualizzarlo, è necessario disporre delle autorizzazioni per il tipo di record.

   Per ulteriori informazioni, vedere anche [Condividere record utilizzando un collegamento](/help/quicksilver/planning/records/share-records.md).


## Rimuovere le autorizzazioni da un record

È possibile rimuovere le autorizzazioni degli utenti da un record. Tuttavia, manterranno almeno le autorizzazioni View (Visualizzazione) per l&#39;area di lavoro, che assegnano loro almeno le autorizzazioni View (Visualizzazione) per il tipo di record.

È necessario rimuoverne l&#39;accesso dall&#39;area di lavoro se si desidera che non dispongano di autorizzazioni per i tipi di record o i record nell&#39;area di lavoro.

Non è possibile rimuovere un utente dalle autorizzazioni ereditate.

{{step1-to-planning}}

1. Aprire l&#39;area di lavoro di cui si desidera interrompere la condivisione dei record, quindi fare clic su una scheda del tipo di record. Verrà aperta la pagina del tipo di record.
1. Esegui una delle operazioni seguenti:

   * Nella vista tabella, passa il puntatore del mouse sul nome di un record e fai clic sul menu **Altro** ![Altro](assets/more-menu.png), quindi fai clic su **Condividi**.
   * Nella vista a tabella, seleziona uno o più record, quindi fai clic su **Condividi** nella barra degli strumenti blu in fondo all&#39;elenco.

     È necessario selezionare i record creati nello stesso workspace.
   * Da qualsiasi visualizzazione, fai clic sul nome di un record, quindi fai clic su **Condividi** nell&#39;angolo superiore destro della pagina dei dettagli del record.

   Viene visualizzata la casella **Condividi**.
1. Individuare l&#39;utente, il gruppo, il team, la società o la mansione che si desidera rimuovere, espandere il menu a discesa delle autorizzazioni a destra del nome, quindi fare clic su **Rimuovi**.

   ![Rimuovi le autorizzazioni dal record](assets/remove-option-on-record-sharing-drop-down.png)

1. Fai clic su **Salva**.

   Gli utenti non dispongono più delle autorizzazioni indicate per il record. Tuttavia, dispongono ancora delle autorizzazioni per il tipo di record e l’area di lavoro, a meno che non vengano rimosse anche da tali autorizzazioni.

   Agli utenti che sono stati rimossi dall’accesso al record non viene notificato che non dispongono più di queste autorizzazioni.
