---
product-area: projects
navigation-topic: manage-issues
title: Assegnare i problemi
description: Puoi assegnare i problemi a utenti, ruoli e team per indicare chi è responsabile del completamento dei problemi. Per informazioni generali sull'assegnazione dei problemi, vedere la panoramica Modifica assegnazione dei problemi.
author: Alina
feature: Work Management
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '1405'
ht-degree: 0%

---

# Assegnare i problemi

Puoi assegnare i problemi a utenti, ruoli e team per indicare chi è responsabile del completamento dei problemi. Per informazioni generali sull’assegnazione dei problemi, consulta [Modifica della panoramica delle assegnazioni dei problemi](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>È possibile assegnare più utenti, ruoli o team. È possibile assegnare solo utenti attivi, ruoli e team.
>
>Se un utente, un ruolo o un team è stato assegnato prima della disattivazione, rimangono assegnati all&#39;elemento di lavoro. In questo caso, si consiglia quanto segue:
>
>* Riassegna l&#39;elemento di lavoro alle risorse attive.
>* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.


Oltre a questo articolo, ti consigliamo di leggere i seguenti articoli per ulteriori informazioni sull’assegnazione dei problemi:

* [Modifica della panoramica delle assegnazioni dei problemi](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [Modifica dei problemi](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Modificare le assegnazioni utente per più problemi in un elenco](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [Creazione di assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Esecuzione di assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Panoramica delle assegnazioni intelligenti](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Panoramica dell’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

Puoi assegnare un problema a una o più risorse a livello di singolo problema, oppure puoi assegnare più risorse a più problemi contemporaneamente.

L’assegnazione di problemi e attività è simile in Adobe Workfront. Per informazioni generali sull&#39;assegnazione delle attività, vedere [Panoramica sulla modifica delle assegnazioni di attività](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica accesso ai problemi</p> <p>Visualizza o consente un accesso più elevato a progetti e attività</p> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull'accesso ai problemi relativi al livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concedere l’accesso ai problemi</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni al problema</p> <p>Autorizzazioni di Contribute per l'elemento in cui si copia il problema con la possibilità di aggiungere problemi.</p> <p> Per informazioni sulla concessione delle autorizzazioni per i problemi, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a></p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Considerazioni relative a più assegnazioni a ruoli, team e utenti del processo

Quando si assegnano più risorse a un elemento di lavoro, tenere presente quanto segue:

* Gli utenti possono avere più di un ruolo di lavoro associato al loro profilo. Per informazioni sull’associazione degli utenti ai ruoli di lavoro, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Le attività o i problemi vengono solitamente assegnati per la prima volta a uno o più ruoli o team di lavoro. Quando i progetti sono pronti per essere avviati, potrebbe essere necessario assegnarli anche agli utenti.

   Se un’attività o un problema viene assegnato a uno o più ruoli e poi si assegna anche un utente, Adobe Workfront decide quale ruolo di lavoro associare all’utente aggiuntivo (se presente) in base alle regole seguenti:

   * Se è assegnato un solo ruolo di lavoro e corrisponde al ruolo principale dell&#39;utente, l&#39;attività o il problema viene assegnato solo all&#39;utente che svolge il ruolo primario.
   * Se sono assegnati più ruoli e almeno uno dei ruoli corrisponde ai ruoli secondari dell&#39;utente, l&#39;attività o il problema viene assegnato all&#39;utente che esegue uno dei loro Altri ruoli, che Workfront seleziona in modo casuale in presenza di più corrispondenze, nonché a eventuali ruoli aggiuntivi assegnati.
   * Se sono assegnati uno o più ruoli di lavoro e non vi sono corrispondenze con i ruoli dell&#39;utente, l&#39;attività o il problema viene assegnato sia al ruolo o ai ruoli che all&#39;utente.

* Se un&#39;attività o un problema viene assegnato a un team e si assegna anche un utente, l&#39;attività o il problema rimane assegnato sia al team che all&#39;utente.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<h2>Considerations about removing assignments from issues</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to Modify issue assignments overview article)</p>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Modify user assignments for multiple issues in a list</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

## Assegnare un singolo problema

1. Passa a un problema che desideri assegnare.
1. Fai clic su **Assegna a** nell’angolo in alto a destra dell’intestazione del problema, nella sezione **Assegnazioni** area

   Oppure

   Fare clic sul nome delle assegnazioni correnti, se il problema è già assegnato.

   ![](assets/nwe-assign-to-button-in-header-350x77.png)

1. Esegui una delle operazioni seguenti:

   * Iniziare a digitare il nome di un utente, un ruolo o un team che si desidera assegnare, quindi fare clic su di esso quando viene visualizzato nell&#39;elenco.

      ![](assets/nwe-assignments-expanded-in-task-header-350x259.png)

   * (Condizionale) Fai clic su uno dei nomi nel **Assegnazioni suggerite** elenco
   * Fai clic su **Assegnami** per assegnarlo a se stessi
   * Fai clic su **Avanzate**

      La creazione di assegnazioni avanzate è simile per le attività e i problemi. Per informazioni su come effettuare assegnazioni avanzate, vedere [Creazione di assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

      >[!TIP]
      >
      >Quando aggiungi un&#39;assegnazione utente, osserva l&#39;avatar, il ruolo principale dell&#39;utente o il relativo indirizzo e-mail per distinguere tra utenti con nomi identici. Gli utenti devono essere associati ad almeno un ruolo di lavoro per visualizzarlo durante l&#39;aggiunta.


1. Fai clic su **Salva** per completare l’assegnazione del problema.
1. (Facoltativo) Fai clic sul pulsante **Icona X** accanto al nome delle assegnazioni nell&#39;area Assegnazioni nell&#39;intestazione del problema per rimuovere un&#39;assegnazione.

## Assegnare un problema in un elenco

È possibile assegnare problemi in un elenco o in un rapporto quando uno dei campi delle assegnazioni è visibile nella visualizzazione dell&#39;elenco. Questo è il modo più veloce per assegnare i problemi.

A seconda del campo visibile nella visualizzazione, è possibile assegnare le seguenti entità al problema:

| Opzione | Entità assegnate |
|---|---|
| **Assegna a** | Assegnare un utente |
| **Assgnt** | Assegnare un utente |
| **Assegnazioni** | Assegna utenti, ruoli o team. |

Per assegnare i problemi in un elenco:

1. Vai a un elenco dei problemi che presentano i campi Assegnato a, Assegnato o Assegnazioni nella visualizzazione.
1. Per assegnare i problemi, effettua una delle seguenti operazioni:

   * Fai clic all’interno del **Assegnato a** o **Assegnato** campi e inizia a digitare il nome di un utente attivo che desideri assegnare al problema, quindi fai clic su di esso quando viene visualizzato nell’elenco.

      ![](assets/assigned-to-field-task-list-nwe.png)

   * Fai clic all’interno del **Assegnazioni** e inizia a digitare il nome di un utente attivo, di un ruolo di lavoro o di un team attivo che si desidera assegnare al problema, quindi fai clic su di esso quando viene visualizzato nell&#39;elenco.

      ![](assets/assignments-field-task-list-nwe.png)
   >[!TIP]
   >
   >Quando aggiungi un&#39;assegnazione utente, osserva l&#39;avatar, il ruolo principale dell&#39;utente o il relativo indirizzo e-mail per distinguere tra utenti con nomi identici. Gli utenti devono essere associati ad almeno un ruolo di lavoro per visualizzarlo durante l&#39;aggiunta.


1. (Condizionale) Se visibile nel campo Assegnazioni, fai clic sul pulsante **Icona Persone** ![](assets/teams.png) nell&#39;angolo superiore destro della casella assegnazioni per aprire la casella Assegnazioni avanzate e creare assegnazioni avanzate. Per ulteriori informazioni, consulta [Creazione di assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Non è possibile effettuare assegnazioni avanzate dai campi Assegnato a o Assegnato.

1. Dopo aver aggiunto gli assegnatari al problema, premi Invio o fai clic in un punto qualsiasi della pagina per salvare le modifiche.

## Assegnare i problemi in blocco

1. Vai a un elenco dei problemi che desideri assegnare in blocco.
1. Seleziona diversi problemi nell’elenco.
1. Fai clic sul pulsante **Icona Modifica** ![](assets/qs-edit-icon.png).

   La **Modifica problemi** viene visualizzata la finestra di dialogo.

1. In **Assegnazioni** area, selezionare **Assegnatario** quindi iniziare a digitare il nome di un utente, di un ruolo o di un team da assegnare a tutti i problemi.

   >[!IMPORTANT]
   >
   >Se uno dei problemi è già assegnato, le risorse indicate vengono aggiunte ai problemi invece di sostituire le risorse esistenti sui problemi.

1. (Facoltativo) Seleziona il pulsante di scelta nel **Proprietario del problema** per indicare quale risorsa è l’assegnatario principale o il proprietario del problema, quando si assegnano più risorse al problema. Non disponibile per i team.
1. (Facoltativo) Seleziona un ruolo che l’utente deve svolgere sul problema dal **Scegli un ruolo** nel menu a discesa **Ruolo dell&#39;assegnatario** quando assegni gli utenti a problemi. Se non selezioni un ruolo, Workfront seleziona automaticamente il ruolo principale dell’utente.

1. (Facoltativo) Se desideri rimuovere gli assegnatari esistenti da tutti i problemi, effettua una delle seguenti operazioni:

   1. Inizia a digitare il nome di un utente, un ruolo o un team da rimuovere dal problema, quindi selezionalo quando viene visualizzato nell’elenco e fai clic su **Rimuovi assegnatario** per aggiungere altri assegnatari da rimuovere.
   1. Fai clic su **Rimuovi tutti gli assegnatari esistenti** per rimuovere tutti gli assegnatari da tutti i problemi selezionati.

1. Fai clic su **Salva modifiche**.
1. (Facoltativo e condizionale) Quando i campi Assegnato a o Assegnazioni vengono visualizzati nell’elenco dei problemi, fai clic all’interno di una di queste colonne per un problema, quindi fai clic sul pulsante **Icona X** accanto al nome di un assegnatario per rimuoverlo dal problema.
