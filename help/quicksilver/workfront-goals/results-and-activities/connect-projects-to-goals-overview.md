---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront
description: Puoi collegare i progetti agli obiettivi per indicare il progresso dell’obiettivo, in base all’avanzamento effettivo del progetto. Il progetto diventa un indicatore di avanzamento per l’obiettivo.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

Puoi collegare i progetti agli obiettivi per indicare il progresso dell’obiettivo, in base all’avanzamento effettivo del progetto. Il progetto diventa un indicatore di avanzamento per l’obiettivo.

Collegando i progetti agli obiettivi è possibile collegare la pianificazione strategica (obiettivi) dell&#39;organizzazione al lavoro effettivo che le persone stanno eseguendo e completando ogni giorno (progetti).

>[!IMPORTANT]
>
>Gli obiettivi a livello di progetto creati nell’area Business Case di un progetto non sono collegati a obiettivi strategici creati in Obiettivi di Workfront. Per informazioni sugli obiettivi del progetto Business Case, vedi [Creare gli obiettivi del caso aziendale](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Requisiti di accesso

<!--drafted for P&P release: replace the table below with this: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>

-->
Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze di Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td> <p>Devi acquistare una licenza aggiuntiva per la funzionalità Obiettivi di Adobe Workfront per accedere alla descritta in questo articolo. </p> <p>Per informazioni, consulta <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l'accesso agli obiettivi</p> <p><b>NOTA</b>

<p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Concedere l’accesso agli obiettivi di Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> 
    <div> 
     <p>Gestione delle autorizzazioni per l'obiettivo</p> 
     <p>Per informazioni sulla condivisione degli obiettivi, vedi <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

Per ulteriori informazioni sull&#39;accesso agli obiettivi di Workfront, vedi [Requisiti per l&#39;utilizzo degli obiettivi di Workfront](../goal-management/access-needed-for-wf-goals.md).

## Considerazioni sul collegamento di progetti agli obiettivi

* Puoi aggiungere a un obiettivo un progetto che soddisfi i seguenti criteri:

   * Devi disporre almeno delle autorizzazioni per visualizzarlo.

      >[!NOTE]
      >
      >Se si perdono le autorizzazioni per visualizzare il progetto dopo aver collegato il progetto all’obiettivo, è comunque possibile visualizzare le informazioni sul progetto per l’obiettivo, ma non è più possibile accedere al progetto.

   * Il progetto non deve trovarsi in uno stato Morto.

* È possibile associare più progetti a un obiettivo.
* È possibile associare lo stesso progetto a più obiettivi.
* Non puoi aggiornare manualmente l’avanzamento di un progetto dall’obiettivo a cui è associato. Al contrario, Workfront calcola la percentuale di completamento del progetto e obiettivi Workfront calcola l&#39;avanzamento dell&#39;obiettivo utilizzando questa percentuale di completamento. Questo aggiorna l’obiettivo in tempo reale dopo l’aggiornamento della percentuale del progetto.
* La durata del progetto può essere al di fuori del periodo di tempo di un obiettivo. Se un progetto dura più della scadenza dell’obiettivo, puoi comunque chiuderlo e considerarlo completato, ma la percentuale di completamento dell’obiettivo non sarà del 100%. La percentuale di completamento del progetto non viene più aggiornata sull&#39;obiettivo.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Quando elimini un progetto allegato a un obiettivo, anche il progetto viene eliminato dall’obiettivo.

   >[!CAUTION]
   >
   >Se l’obiettivo era attivo prima dell’eliminazione del progetto e non vi sono altri indicatori di avanzamento sull’obiettivo, l’obiettivo diventa Inattivo.


## Aggiungere progetti agli obiettivi

1. Fai clic sul pulsante **Menu principale** ![](assets/main-menu-icon.png) (crea questo progetto per Shell: o fai clic su **Menu principale** ![](assets/three-line-main-menu-icon.png) nell’angolo in alto a sinistra, se disponibile.) , quindi **Obiettivi**.
1. Nell’Elenco obiettivi, fai clic sul nome di un obiettivo per aprire la pagina dell’obiettivo.
1. Fai clic su **Indicatori di progresso** nel pannello a sinistra.
1. Da **Nuovo indicatore di avanzamento** menu a discesa, fai clic su **Aggiungi progetto esistente**.

   Viene visualizzata la casella Aggiungi progetti all’obiettivo .
1. (Facoltativo) Aggiorna **Visualizza**, **Filtro** oppure **Raggruppamento** facendo clic sulle rispettive icone nell’angolo in alto a destra dell’elenco per modificare la modalità di visualizzazione dell’elenco dei progetti.
1. (Facoltativo) Fai clic sul pulsante **Ricerca** icona ![](assets/search-icon.png) inizia a digitare il nome di un progetto per individuarlo rapidamente nell’elenco.
1. Seleziona i progetti da aggiungere all’obiettivo, quindi fai clic su **Aggiungi**.

   I progetti selezionati vengono aggiunti all’obiettivo e vengono visualizzati nella sezione Indicatori di avanzamento della pagina dell’obiettivo, nella sezione **Progetto** raggruppamento.

   Dopo aver attivato l’obiettivo, l’avanzamento dell’obiettivo viene aggiornato automaticamente quando l’avanzamento di un progetto viene aggiornato. Per informazioni sull&#39;attivazione di un obiettivo, vedi [Attivare gli obiettivi in Obiettivi di Adobe Workfront](../goal-management/activate-goals.md).

## Individua informazioni di progetto sugli obiettivi

<p>
Le seguenti informazioni sul progetto sono visibili a livello di obiettivo nella sezione Indicatori di avanzamento della pagina di un obiettivo:

</p>

<table>
  <tr>
   <td>Nome progetto
   </td>
   <td>Eventuali modifiche nel nome del progetto si rifletteranno anche nel progetto connesso.
   </td>
  </tr>
  <tr>
   <td>Proprietario progetto
   </td>
   <td>Eventuali modifiche apportate al proprietario del progetto si rifletteranno anche nel progetto connesso.
   </td>
  </tr>
    <tr>
   <td>Avanzamento corrente
   </td>
   <td> <p>Percentuale di completamento del progetto. Non è possibile aggiornare manualmente la percentuale di completamento del progetto dall'obiettivo. Workfront la calcola automaticamente in base alla percentuale di completamento delle attività. </p>
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

Le seguenti informazioni sull’obiettivo sono visibili in un elenco o in un rapporto di progetto:

| Informazioni sull’obiettivo | Descrizione |
|---|---|
| Obiettivi | Elenco di tutti gli obiettivi a cui è associato un progetto. |
| Gerarchia degli obiettivi | La gerarchia a cui appartiene un obiettivo. Solo i genitori dell&#39;obiettivo e l&#39;obiettivo vengono visualizzati in questo campo. Gli obiettivi dei bambini non vengono visualizzati. |
| Numero di obiettivi collegati | Numero di obiettivi collegati a un progetto. |
