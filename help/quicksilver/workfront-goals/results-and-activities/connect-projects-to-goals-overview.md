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
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 1%

---

# Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

È possibile collegare i progetti agli obiettivi per indicare il modo in cui l&#39;obiettivo progredisce, in base all&#39;effettivo avanzamento del progetto. Il progetto diventa un indicatore di avanzamento per l’obiettivo.

Collegando i progetti agli obiettivi è possibile collegare la pianificazione strategica (obiettivi) dell&#39;organizzazione al lavoro effettivo che il personale sta svolgendo e completando ogni giorno (progetti).

>[!IMPORTANT]
>
>Gli obiettivi a livello di progetto creati nell’area Caso di business di un progetto non sono collegati agli obiettivi strategici creati negli Obiettivi di Workfront. Per informazioni sugli obiettivi del progetto del caso di business, vedere [Creare gli obiettivi del caso di business](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> 
   <p>Per il nuovo piano e la nuova struttura delle licenze:
  <ul><li>Un piano Ultimate </li></ul>
   </p>
<p>Per il piano corrente e la struttura delle licenze: 
<ul><li> A Pro o superiore </li>
  <li>Una licenza Adobe Workfront Goals oltre a una licenza Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licenza Adobe Workfront*</td>
 <td>
 <p>Nuova licenza: Collaboratore o versione successiva</p>
 Oppure
 <p>Licenza corrente: richiesta o successiva</p> <p>Per ulteriori informazioni, vedere <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica delle licenze di Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Prodotto*</td>
 <td>
 <p> Nuovo requisito del prodotto, uno dei seguenti: </p>
<ul>
<li>Un piano Select o Prime Adobe Workfront e un’ulteriore licenza Adobe Workfront Goals.</li>
<li>Un piano Workfront di Ultimate che include gli obiettivi di Workfront per impostazione predefinita. </li></ul>
 <p>Oppure</p>
 <p>Fabbisogno di prodotto corrente: un piano Workfront e una licenza aggiuntiva per gli obiettivi Adobe Workfront. </p> <p>Per informazioni, vedere <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Livello di accesso</td>
 <td> <p>Modifica accesso agli obiettivi</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorizzazioni oggetto</td>
 <td>
  <div>
  <p>Visualizza o autorizzazioni superiori per l’obiettivo per visualizzarlo</p>
  <p>Gestire le autorizzazioni per l’obiettivo per modificarlo</p>
  <p>Per informazioni sulla condivisione degli obiettivi, vedere <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l’area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
