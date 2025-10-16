---
product-area: projects
navigation-topic: manage-issues
title: Copia le Issues
description: È possibile copiare un problema o una richiesta e salvarli nello stesso progetto o in un altro. È inoltre possibile copiare un problema da un’attività a un altro progetto.
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 1%

---

# Copia i problemi

<!--Audited: 08/2025-->

È possibile copiare un problema o una richiesta e salvarli nello stesso progetto o in un altro. È inoltre possibile copiare un problema da un’attività a un altro progetto.

È possibile copiare i problemi dai seguenti oggetti:

* Da un progetto allo stesso progetto (duplicalo sullo stesso progetto)
* Da un&#39;attività alla stessa attività (duplicato se sulla stessa attività)
* Da un progetto a un altro
* Da un&#39;attività a un progetto

>[!TIP]
>
>&quot;Problemi&quot; e &quot;richieste&quot; vengono utilizzati in modo intercambiabile in Workfront. È possibile registrare problemi relativi a progetti e attività per indicare il lavoro imprevisto che deve essere risolto. Puoi anche inviare richieste registrate come problemi in un progetto designato come coda richieste.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <ul><li><p>Collaboratore o versione successiva</p> </li>
   <li><p>Licenza leggera o superiore per copiare un problema nella sezione Problemi di un progetto</p></li></ul>
   Oppure
   <ul><li><p>Richiedente o versione successiva</p> </li>
   <li><p>Revisore o licenza superiore per copiare un problema nella sezione Problemi di un progetto</p></li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p>Accesso di visualizzazione o superiore ai progetti e alle attività</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il problema</p> <p>Concedi le autorizzazioni per l’elemento in cui stai copiando il problema con la possibilità di aggiungere problemi.</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to copy an issue in the Issues section of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are copying the issue to with the ability to Add Issues.</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Considerazioni durante la copia dei problemi

### Considerazioni generali durante la copia dei problemi

Puoi scegliere di copiare alcuni elementi associati al problema nel problema copiato durante il processo di copia. Tuttavia, alcuni elementi vengono trasferiti al nuovo problema per impostazione predefinita, mentre altri no, come descritto negli elenchi seguenti.

I seguenti elementi vengono copiati nel nuovo problema, per impostazione predefinita:

* Contatto principale
* Moduli personalizzati. Le informazioni nei campi personalizzati vengono copiate nel nuovo problema solo quando si seleziona Dati personalizzati nel processo di copia.
* Approvazioni
* Date Pianificate di Inizio e Completamento

Per impostazione predefinita, i seguenti oggetti non vengono copiati nel nuovo problema:

* Ore registrate

### Considerazioni sui problemi associati ai documenti o alle code di richieste

Quando copi problemi che contengono documenti o sono associati a una coda di richieste, tieni presente quanto segue:

* **Quando un problema è associato a una coda di richieste:** Quando si copia un problema in un altro oggetto e il problema è associato a una coda di richieste, il problema copiato non è più associato alla coda originale da cui ha avuto origine il primo problema.
* **Quando un documento è allegato al problema:** Quando si copia un problema in un altro oggetto a cui è associato un documento, anche il documento e le relative versioni passano al nuovo problema. Eventuali bozze o approvazioni associate al documento non vengono spostate.
* **Quando un problema è collegato a un documento o a una cartella:** Quando si copia un problema che include documenti o cartelle collegati a un servizio di terze parti come Google Drive, i collegamenti ai documenti vengono trasferiti al problema copiato.

## Copiare i problemi in un elenco

È possibile copiare uno o più problemi da un elenco di problemi o da un report di problemi.

1. Vai al progetto che contiene il problema o i problemi che desideri copiare.

   Oppure

   Passa a un report sui problemi.

1. Se hai selezionato di passare a un progetto, fai clic su **Problemi** nel pannello a sinistra.
1. Seleziona il problema o i problemi da copiare e fai clic sul **menu Altro** nella parte superiore dell&#39;elenco dei problemi, quindi fai clic su **Copia in**.

   ![Copia problema nell&#39;elenco](assets/copy-issue-in-list-nwe-350x169.png)

1. Continua a copiare il problema, come descritto nella sezione [Copia un singolo problema](#copy-a-single-issue) a partire dal passaggio 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## Copiare un singolo problema {#copy-a-single-issue}

È possibile copiare un problema durante la visualizzazione.

1. Passa al problema da copiare, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-icon.png) a destra del nome del problema, quindi **Copia in**.

   ![Copia a livello di problema](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   Viene visualizzata la casella **Copia problema**.

   ![Copia casella problema](assets/copy-issue-box-nwe-350x285.png)

1. Nella sezione **Seleziona progetto di destinazione**, specifica il nome del progetto in cui desideri copiare i problemi. Il nome del progetto corrente viene visualizzato per impostazione predefinita.

   >[!TIP]
   >
   >Nell’elenco vengono visualizzati solo 100 progetti.

1. (Condizionale) Se non disponi dell&#39;accesso per copiare i problemi nel progetto, fai clic su **richiedi l&#39;accesso**.
1. (Facoltativo) Se disponi dell’accesso per aggiungere problemi a una delle attività nel progetto di destinazione, continua a copiare il problema nel progetto di destinazione selezionato senza richiedere l’accesso.

   ![Copia problema e richiedi accesso](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Messaggi simili vengono visualizzati se il progetto selezionato è in attesa di approvazione, completato o inattivo, quando l’amministratore di Workfront impedisce l’aggiunta di problemi a questi progetti. Per ulteriori informazioni, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Facoltativo) Nella sezione **Opzioni**, deseleziona uno degli elementi elencati nella tabella seguente per rimuoverli dal nuovo problema. Tutte le opzioni sono selezionate per impostazione predefinita.

   >[!NOTE]
   >
   >Questo interessa solo i problemi copiati e non quelli originali.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Assegnazioni</td> 
      <td>Rimuove gli utenti, le mansioni o i team assegnati al problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Avanzamento</td> 
      <td>Rimuove l'eventuale percentuale di completamento del problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td><span style="line-height: 1.5;">Rimuove tutti gli elementi presenti nella scheda documenti, incluse le versioni dei documenti, i documenti collegati e le cartelle.</span> <br>Per impostazione predefinita, le bozze e le approvazioni dei documenti non possono essere copiate in un altro problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autorizzazioni</td> 
      <td>Rimuove le entità con cui è condiviso il problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aggiornamenti</td> 
      <td>Rimuove i commenti dalla sezione Aggiornamenti del problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dati personalizzati</td> 
      <td>Rimuove le informazioni sul problema dal modulo personalizzato, nonché le informazioni sui moduli personalizzati associati ai documenti allegati al problema, se questi vengono copiati anche con il problema. I moduli personalizzati rimarranno allegati ai problemi e ai documenti, ma le informazioni sui moduli non verranno riportate al nuovo problema. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Nella sezione **Seleziona attività**, seleziona l&#39;attività in cui desideri spostare il problema.
1. Se hai selezionato più problemi in un elenco, fai clic su **Copia problema** o **Copia problemi**.

   I problemi copiati vengono aggiunti al progetto specificato.


