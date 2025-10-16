---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront
description: È possibile collegare i progetti agli obiettivi per indicare il modo in cui l'obiettivo progredisce, in base all'effettivo avanzamento del progetto. Il progetto diventa un indicatore di avanzamento per l’obiettivo.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 1%

---

# Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront

<!--Audited for P&P only: 10/2025-->

È possibile collegare i progetti agli obiettivi per indicare il modo in cui l&#39;obiettivo progredisce, in base all&#39;effettivo avanzamento del progetto. Il progetto diventa un indicatore di avanzamento per l’obiettivo.

Collegando i progetti agli obiettivi è possibile collegare la pianificazione strategica (obiettivi) dell&#39;organizzazione al lavoro effettivo che il personale sta svolgendo e completando ogni giorno (progetti).

>[!IMPORTANT]
>
>Gli obiettivi a livello di progetto creati nell’area Caso di business di un progetto non sono collegati agli obiettivi strategici creati negli Obiettivi di Workfront. Per informazioni sugli obiettivi del progetto del caso di business, vedere [Creare gli obiettivi del caso di business](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Requisiti di accesso

>[!NOTE]
>
>La tua azienda potrebbe scegliere di continuare a utilizzare gli obiettivi di Adobe Workfront se ha acquistato questo pacchetto in passato. Per ulteriori dettagli, rivolgiti al rappresentante del tuo account.
>
>Adobe Workfront Goals non è più disponibile per l’acquisto.

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Pacchetto Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licenza Adobe Workfront</td>
 <td>
 <p>Collaboratore o versione successiva</p>
<p>Richiedi o superiore</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configurazione del livello di accesso</td>
 <td> <p>Modifica accesso agli obiettivi</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorizzazioni oggetto</td>
 <td>
  <div>
  <p>Visualizza o autorizzazioni superiori per l’obiettivo per visualizzarlo</p>
  <p>Gestire le autorizzazioni per l’obiettivo per modificarlo</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di sistema, deve essere assegnato un modello di layout che includa l'area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Considerazioni sulla connessione dei progetti agli obiettivi

* Puoi aggiungere a un obiettivo un progetto che soddisfi i seguenti criteri:

   * Devi disporre almeno delle autorizzazioni necessarie per visualizzarlo.

     >[!NOTE]
     >
     >Se perdi le autorizzazioni di visualizzazione del progetto dopo aver associato il progetto all’obiettivo, puoi ancora visualizzare le informazioni del progetto sull’obiettivo, ma non puoi più accedere al progetto.

   * Lo stato del progetto non può essere Inattivo.

* È possibile associare più progetti a un obiettivo.
* È possibile associare lo stesso progetto a più obiettivi.
* Non è possibile aggiornare manualmente l’avanzamento di un progetto dall’obiettivo a cui è associato il progetto. Al contrario, Workfront calcola la percentuale di completamento del progetto e Workfront Goals calcola l’avanzamento dell’obiettivo utilizzando questa percentuale di completamento. Questo aggiorna l’obiettivo in tempo reale dopo gli aggiornamenti della percentuale del progetto.
* La durata del progetto può essere al di fuori del periodo di tempo di un obiettivo. Se un progetto dura più a lungo della scadenza dell’obiettivo, puoi comunque chiudere l’obiettivo e considerarlo completato, ma la percentuale di completamento dell’obiettivo non sarà del 100%. La percentuale di completamento del progetto non viene più aggiornata in base all’obiettivo.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![Goal closed](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Quando elimini un progetto associato a un obiettivo, il progetto viene eliminato anche dall’obiettivo.

  >[!CAUTION]
  >
  >Se l’obiettivo era attivo prima dell’eliminazione del progetto e non sono presenti altri indicatori di avanzamento sull’obiettivo, l’obiettivo diventa inattivo.


## Aggiungere progetti agli obiettivi

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu](assets/main-menu-icon.png) (crea bozza per Shell: oppure fai clic sulle **Main Menu** ![Main Menu lines](assets/three-line-main-menu-icon.png) nell&#39;angolo superiore sinistro, se disponibile.) , quindi su **Goals**.
1. Nell&#39;elenco Obiettivo fare clic sul nome di un obiettivo per aprire la pagina obiettivo.
1. Fai clic su **Indicatori di avanzamento** nel pannello a sinistra.
1. Dal menu a discesa **Nuovo indicatore di avanzamento**, fare clic su **Aggiungi progetto esistente**.

   Viene visualizzata la casella Aggiungi progetti all’obiettivo.
1. (Facoltativo) Aggiorna **Visualizza**, **Filtra** o **Raggruppamento** facendo clic sulle rispettive icone nell&#39;angolo superiore destro dell&#39;elenco per modificare la modalità di visualizzazione dell&#39;elenco dei progetti.
1. (Facoltativo) Fai clic sull&#39;icona **Ricerca** ![Icona Ricerca](assets/search-icon.png) e inizia a digitare il nome di un progetto per trovarlo rapidamente nell&#39;elenco.
1. Seleziona i progetti da aggiungere all&#39;obiettivo, quindi fai clic su **Aggiungi**.

   I progetti selezionati vengono aggiunti all&#39;obiettivo e visualizzati nella sezione Indicatori di avanzamento della pagina dell&#39;obiettivo, nel raggruppamento **Progetto**.

   Dopo aver attivato l’obiettivo, l’avanzamento dell’obiettivo viene aggiornato automaticamente quando si aggiorna l’avanzamento di un progetto. Per informazioni sull&#39;attivazione di un obiettivo, vedere [Attivare gli obiettivi negli Obiettivi di Adobe Workfront](../goal-management/activate-goals.md).

## Individuare le informazioni del progetto sugli obiettivi

<p>
Le seguenti informazioni sul progetto sono visibili a livello di obiettivo nella sezione Indicatori di avanzamento della pagina di un obiettivo:

</p>

<table>
  <tr>
   <td>Nome progetto
   </td>
   <td>Eventuali modifiche al nome del progetto si riflettono anche nel progetto connesso.
   </td>
  </tr>
  <tr>
   <td>Proprietario progetto
   </td>
   <td>Eventuali modifiche apportate al proprietario del progetto si riflettono anche nel progetto connesso.
   </td>
  </tr>
    <tr>
   <td>Avanzamento corrente
   </td>
   <td> <p>La percentuale di completamento del progetto. Non è possibile aggiornare manualmente la percentuale di completamento del progetto dall’obiettivo. Workfront la calcola automaticamente in base alla percentuale di completamento delle attività. </p>
   </td>
  </tr>
  <tr>
   <td>Avanzamento
   </td>
   <td>La percentuale di completamento del progetto rappresentata da una barra. Qualsiasi modifica nella percentuale di completamento del progetto aggiorna automaticamente l’avanzamento dell’obiettivo, a meno che l’obiettivo non venga chiuso.
   </td>
  </tr>

</table>

## Individuare le informazioni sull’obiettivo nei progetti

In un elenco o report di progetti sono visibili le seguenti informazioni sull’obiettivo:

| Informazioni sugli obiettivi | Descrizione |
|---|---|
| Obiettivi | Un elenco di tutti gli obiettivi a cui è associato un progetto. |
| Gerarchia obiettivi | Gerarchia a cui appartiene un obiettivo. In questo campo vengono visualizzati solo i padri dell’obiettivo e l’obiettivo. Gli obiettivi secondari non vengono visualizzati. |
| Numero di obiettivi collegati | Il numero di obiettivi collegati a un progetto. |
