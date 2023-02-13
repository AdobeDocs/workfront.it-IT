---
product-area: projects
navigation-topic: manage-tasks
title: Sposta attività
description: In Adobe Workfront è possibile spostare le attività in progetti diversi o a diverse attività principali.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 23a08c929b0a227c7a555af70ff731ef2df7a179
workflow-type: tm+mt
source-wordcount: '1360'
ht-degree: 2%

---

# Sposta attività

È possibile spostare le attività in Adobe Workfront tra i seguenti oggetti:

* Attività ad hoc per un progetto.
* Attività da un progetto a un altro progetto.
* Attività di un progetto con un padre diverso in un altro progetto.
* Un&#39;attività all&#39;interno dello stesso progetto in un elemento padre diverso.

È possibile spostare un&#39;attività a livello di attività oppure spostare un&#39;attività da un elenco di attività.

## Requisiti di accesso

Per eseguire le azioni di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso a Attività e Progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività</p> <p>Contribuisci o autorizzazioni superiori per il progetto con la possibilità di aggiungere attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Spostare un&#39;attività in un elenco

Per spostare un&#39;attività visualizzata in un elenco di attività:

1. Passare al progetto contenente l&#39;attività o le attività che si desidera spostare.
1. Fai clic su **Attività** nel pannello a sinistra per visualizzare l’elenco delle attività.
1. Assicurati che **Salvataggio automatico** l&#39;opzione è attivata, quindi selezionare l&#39;attività o le attività che si desidera spostare.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >Non è possibile spostare le attività quando **Salvataggio automatico** l&#39;opzione è disabilitata.

1. (Facoltativo e condizionale) Se desideri spostare le attività selezionate all’interno dello stesso progetto, fai clic sulle attività selezionate, trascinale e rilasciale nel punto in cui desideri spostarle nel progetto.

   Dopo aver rilasciato le attività nella posizione corretta sul progetto, le modifiche apportate alla gerarchia delle attività vengono salvate immediatamente. Tutte le informazioni associate a ciascuna attività vengono spostate insieme alle attività.

1. (Condizionale) Selezionare l&#39;attività o le attività da spostare ed effettuare una delle seguenti operazioni:

   * Fai clic sul pulsante **Altro** menu ![](assets/qs-more-menu.png) in alto nell’elenco delle attività, quindi fai clic su **Sposta a**.
   * Fai clic con il pulsante destro del mouse sulle attività selezionate, quindi fai clic su **Sposta a**.
   * Quando selezioni un’attività, fai clic sul pulsante **Altro** menu ![](assets/more-icon-task-list.png) accanto al nome dell’attività nell’elenco, quindi fai clic su **Sposta a**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   Viene visualizzata la casella Sposta attività

1. Continua a spostare l’attività, come descritto nella sezione . [Spostare un&#39;attività a livello di attività](#move-a-task-at-the-task-level) in questo articolo, a partire dal passaggio 4.

   <!--
   is this still accurate?!
   -->

## Spostare un&#39;attività a livello di attività {#move-a-task-at-the-task-level}

Oltre a spostare le attività da un elenco di attività, è anche possibile spostare un&#39;attività a livello di attività, dopo averla aperta. 

1. Trovare un&#39;attività nel sistema Workfront ricercandola.
1. Fare clic sul nome dell&#39;attività per aprirla.
1. Fai clic sul pulsante **Altro** menu a discesa ![](assets/qs-more-menu.png) accanto al nome dell’attività, quindi fai clic su **Sposta a**. Viene visualizzata la casella Sposta attività .

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. (Facoltativo) Aggiorna **Nome attività**. L&#39;attività viene spostata con il nuovo nome nella nuova posizione. Workfront non registra il nome originale dell&#39;attività.

   >[!TIP]
   >
   >Questo campo è oscurato e non modificabile quando si seleziona per spostare più attività in un elenco. Passa il puntatore del mouse sul campo Nome attività per visualizzare un elenco di tutte le attività selezionate.
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Digita il nome della **Progetto di destinazione** in cui si desidera spostare l&#39;attività nel **Seleziona progetto di destinazione** campo .

   Se si desidera spostare l&#39;attività all&#39;interno dello stesso progetto, digitare il nome del progetto corrente.

   >[!TIP]
   >
   >* Il nome del progetto distingue tra maiuscole e minuscole.
   >* Puoi anche iniziare a digitare il numero di riferimento o l’ID del progetto. Questo potrebbe essere utile per distinguere tra progetti con nomi identici.
   >* Nell’elenco vengono visualizzati solo 100 progetti.


1. (Condizionale) Fai clic su **Richiesta di accesso** per richiedere l’accesso al progetto, se non disponi dell’accesso al progetto selezionato.
1. (Condizionale) Continua a spostare l’attività nel progetto di destinazione selezionato senza richiedere l’accesso se hai accesso per aggiungere attività a una delle attività nel progetto di destinazione.

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Messaggi simili vengono visualizzati se il progetto selezionato è in attesa di approvazione, completato o disattivato, quando l’amministratore di Workfront impedisce l’aggiunta di attività a tali progetti. Per ulteriori informazioni, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Facoltativo) Fai clic su **Opzioni** nel pannello a sinistra

   Oppure

   Scorri verso il basso fino a **Opzioni** nella casella Sposta attività , quindi deseleziona uno degli elementi elencati nella tabella seguente per rimuoverli dalle attività spostate . Tutte le opzioni sono selezionate per impostazione predefinita.

   >[!IMPORTANT]
   Deselezionando gli elementi nell&#39;elenco Opzioni si verifica una perdita di dati. Le informazioni dell&#39;attività esistente verranno rimosse e non possono essere recuperate.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seleziona tutto</td> 
      <td>Deselezionare questa opzione per rimuovere tutte le informazioni dall'attività quando si sposta nella nuova posizione. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vincolo Data</td> 
      <td> <p>Il vincolo dell'attività viene impostato su Il più presto possibile o Il più tardi possibile in base all'impostazione Modalità pianificazione progetto.</p> <p> Se selezionata, il vincolo corrente dell'attività viene trasferito con l'attività. </p> 
      <p><b>NOTA</b>

   Quando si sposta o si copia un&#39;attività con vincoli specifici per la data in un altro progetto e le date dei vincoli dell&#39;attività sono al di fuori delle date del nuovo progetto, il Vincolo attività diventa Il più presto possibile o Il più tardi possibile oppure le date di Inizio pianificato o Completamento pianificato dei progetti vengono modificate.

   Di seguito sono riportati alcuni esempi di vincoli specifici per la data:
   <ul>
      <li> Inizia il</li>
      <li> Deve Finire al</li>
      <li> Iniziare non Prima di</li>
      <li> Iniziare non Dopo di</li>
      </ul>

   Per informazioni sui vincoli delle attività e sulle possibili ripercussioni sui vincoli delle attività o sulle date del progetto, consulta <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sul vincolo di attività</a> e cercare un vincolo specifico.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Assegnazioni</td> 
      <td> <p>Tutte le assegnazioni vengono rimosse dall'attività. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo di approvazione</td> 
      <td>Tutti i processi di approvazione vengono rimossi dall'attività.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Avanzamento</td> 
      <td>Lo stato dell'attività è Nuovo. In caso contrario, lo stato dell'attività esistente viene mantenuto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informazione Finanziaria</td> 
      <td>Le informazioni finanziarie dell'attività vengono rimosse e Workfront aggiorna il tipo di costo dell'attività su Nessun costo e il tipo di ricavi dell'attività su Non fatturabile. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tutti i predecessori</td> 
      <td> <p>Se selezionata, la dipendenza diventa un predecessore tra progetti quando si sposta l’attività in un altro progetto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td> <p>I documenti allegati all'attività non vengono trasferiti all'attività spostata. Ciò include versioni, bozze e documenti collegati.</p> <p>Non sono incluse le approvazioni dei documenti. Le approvazioni dei documenti non possono mai essere spostate quando un'attività viene spostata.</p> 
      <b>NOTA</b>

   Se si sceglie di non spostare i documenti con l&#39;attività, i documenti verranno eliminati e inseriti nel Cestino per 30 giorni. Un amministratore può ripristinarli e ripristinarli nell’attività spostata.

   Se l&#39;attività viene eliminata dopo lo spostamento, i documenti ripristinati verranno inseriti nell&#39;area Documenti della pagina utente dell&#39;amministratore che li ripristina.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td>I promemoria attività non vengono trasferiti all'attività spostata. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td>Le spese registrate nell'attività non vengono trasferite all'attività spostata. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autorizzazioni</td> 
      <td> <p>Workfront rimuove i nomi di tutte le entità visualizzate nell'elenco Condivisione dell'attività. </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. (Facoltativo) Fai clic su **Seleziona padre** nel pannello a sinistra

   Oppure

   Scorri fino a **Seleziona padre** quindi selezionare l&#39;attività nel progetto di destinazione che si desidera diventare padre dell&#39;attività spostata.

   >[!TIP]
   Quando si seleziona per spostare più attività in un elenco, tutte le attività selezionate diventano le attività secondarie dell&#39;elemento padre selezionato.

   Selezionare un padre eseguendo una delle operazioni seguenti:

   * Nell’elenco Attività, selezionare uno degli elementi principali del piano di progetto.
   * Fai clic sull’icona di ricerca ![Icona Ricerca](assets/search-icon.png) e cercare un&#39;attività principale per nome.

   L’attività deve essere visualizzata nell’elenco.

   ![Selezionare l&#39;attività principale quando si sposta un&#39;attività con funzionalità di ricerca ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Selezionare il pulsante di scelta per il padre dopo averlo trovato.

   Se non si seleziona un&#39;attività padre, le attività vengono spostate come attività principali anziché come sottoattività e verranno posizionate alla fine dell&#39;elenco delle attività nel progetto di destinazione.

1. Fai clic su **Sposta attività**

   Oppure

   Fai clic su **Sposta attività** quando si selezionano più attività in un elenco.
Le attività spostate ora si trovano nel progetto specificato e possono essere sottoattività a un&#39;attività principale oppure le ultime attività del progetto.
