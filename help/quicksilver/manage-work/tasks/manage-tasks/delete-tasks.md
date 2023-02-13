---
product-area: projects
navigation-topic: manage-tasks
title: Elimina attività
description: È possibile eliminare le attività che potrebbero essere duplicate o che sono state create per errore.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

---

# Elimina attività

È possibile eliminare le attività che potrebbero essere duplicate o che sono state create per errore.

Per le attività che contengono informazioni cronologiche (aggiornamenti, modifiche della pianificazione, dello stato o altri campi), è consigliabile chiuderle o contrassegnarle come morte, anziché eliminarle. In questo modo puoi conservare le informazioni storiche dei tuoi progetti.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l'accesso a Attività e Progetti con accesso a Elimina</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull'accesso alle attività, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Concedere l’accesso alle attività</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute per il progetto con la possibilità di aggiungere attività o versioni successive</p> <p>Quando crei un'attività, riceverai automaticamente le autorizzazioni di gestione per l'attività</p> <p> Per informazioni sulle autorizzazioni delle attività, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Condividere un’attività </a>. </p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Comprendere il processo di eliminazione delle attività

* [Limitazioni per l&#39;eliminazione delle attività](#limitations-for-deleting-tasks)
* [Impatto dell&#39;eliminazione delle attività](#the-impact-of-deleting-tasks)

### Limitazioni per l&#39;eliminazione delle attività  {#limitations-for-deleting-tasks}

* Quando un progetto ha lo stato Completa , è possibile eliminare le attività solo se l’amministratore di Workfront o un amministratore di gruppo lo ha consentito nell’area Preferenze progetto. Per informazioni sulla configurazione delle preferenze del progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se l’attività ha registrato ore, l’amministratore di Workfront o di gruppo deve consentire l’eliminazione di tali attività configurando le preferenze relative a attività e problemi nell’istanza Workfront. Questo vale anche quando tenti di eliminare progetti che hanno attività con ore registrate su di essi.

   <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

   Per ulteriori informazioni sull&#39;abilitazione dell&#39;eliminazione delle attività in cui vengono registrate le ore, consulta la sezione &quot;Eliminazione&quot; in [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Impatto dell&#39;eliminazione delle attività {#the-impact-of-deleting-tasks}

Quando si elimina un&#39;attività, si hanno effetti sugli altri oggetti collegati all&#39;attività.

Quando si elimina un’attività, vengono eliminati anche i seguenti oggetti associati a un’attività:

* Documenti

   Impossibile eliminare un&#39;attività a cui è associato un documento estratto. Per ulteriori informazioni sull&#39;estrazione dei documenti, vedere [Estrarre documenti](../../../documents/managing-documents/check-out-documents.md).

* Problemi
* Sottoattività
* Note
* Approvazioni

A seconda di come l&#39;amministratore Workfront configura le preferenze di eliminazione di progetti, attività o problemi nelle preferenze della scheda attività e ora dell&#39;istanza Workfront, le ore registrate per le attività vengono gestite in uno dei modi seguenti durante l&#39;eliminazione di un&#39;attività:

* Passa al progetto e non verrà ripristinato sull&#39;attività, se l&#39;attività viene successivamente ripristinata.
* Vengono eliminati e verranno ripristinati nell&#39;attività, se l&#39;attività viene successivamente ripristinata.

   Questo vale anche quando tenti di eliminare progetti che hanno attività con ore registrate su di essi.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

   Per ulteriori informazioni sulla configurazione delle preferenze di eliminazione per le ore di accesso ai problemi, vedi [Configurare le preferenze relative a schede attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Le spese relative all’attività passeranno al progetto.

* Gli utenti assegnati all&#39;attività o all&#39;approvazione dell&#39;attività rimangono nel team di progetto.

   Per ulteriori informazioni sui team di progetto, consulta [Panoramica del team di progetto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Elimina attività

* [Eliminare più attività contemporaneamente in un progetto](#delete-multiple-tasks-in-a-project-simultaneously)
* [Eliminare una singola attività](#delete-a-single-task)

### Eliminare più attività contemporaneamente in un progetto  {#delete-multiple-tasks-in-a-project-simultaneously}

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Progetti**.
1. Fare clic sul nome del progetto contenente le attività da eliminare.
1. Fai clic su **Attività** nel pannello a sinistra.
1. Esegui una delle operazioni seguenti:

   1. (Condizionale) Quando **Salvataggio automatico** l&#39;interruttore è abilitato:

      1. Selezionare le attività da eliminare, quindi fare clic su **Altro**
      1. Fai clic su **Elimina**, quindi **Sì, Elimina** per confermare l’eliminazione.

         Le attività vengono eliminate.
   1. (Condizionale) Fai clic sul pulsante **Modalità piano** e seleziona **Salvataggio manuale** per annullare le modifiche apportate all&#39;elenco delle attività.

      ![](assets/nwe-autosave-off-manual-highlighted-350x58.png)

      Effettua le seguenti operazioni:

      1. Selezionare le attività da eliminare.
      1. Fai clic su **Elimina**.
      1. (Facoltativo) Fai clic su **Annulla** per annullare la modifica e non eliminare le attività.
      1. Fai clic su **Ripeti** se si desidera mantenere la modifica ed eliminare l&#39;attività.
      1. Fai clic su **Salva** per eliminare le attività.

         Le attività vengono eliminate solo dopo il salvataggio delle modifiche.


### Eliminare una singola attività {#delete-a-single-task}

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Progetti**.
1. Fare clic sul nome del progetto contenente l&#39;attività da eliminare.
1. Fai clic su **Attività** nel pannello a sinistra.
1. Fare clic sul nome dell&#39;attività da eliminare.
1. Fai clic sul pulsante **Altro** icona ![](assets/qs-more-menu.png)nell&#39;angolo in alto a destra.

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. Fai clic su **Elimina attività**.
1. Se l&#39;eliminazione è consentita, fai clic su **Sì, eliminalo**.

   L’amministratore di Workfront o l’amministratore di gruppo potrebbe non consentire l’eliminazione delle attività in cui vengono registrate ore.

   Per ulteriori informazioni sull&#39;accesso e le autorizzazioni necessarie per eliminare un&#39;attività, consulta la sezione [Limitazioni per l&#39;eliminazione delle attività](#limitations-for-deleting-tasks) in questo articolo.

## Ripristinare le attività eliminate

Un amministratore di Workfront o di gruppo può ripristinare le attività entro 30 giorni dalla loro eliminazione, come descritto in [Ripristina elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
