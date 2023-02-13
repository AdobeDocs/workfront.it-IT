---
title: Disattivare o riattivare un utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: In qualità di amministratore di Workfront, puoi disattivare o riattivare un utente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# Disattivare o riattivare un utente

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate nell’Admin Console. Se l’organizzazione è stata configurata per Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Per istruzioni sulla disattivazione di un utente in Adobe Admin Console, consulta la sezione &quot;Rimuovi utenti&quot; nell’articolo [Gestire gli utenti individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) oppure contatta l’amministratore Adobe Admin Console.
>
>Per un elenco delle procedure che variano a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Gli utenti potrebbero lasciare l&#39;organizzazione e potrebbe essere necessario rimuoverli da Adobe Workfront. Non devono rimanere attivi nel sistema perché ciò creerebbe confusione per gli altri utenti quando li aggiungono agli aggiornamenti o li assegnano funzionare. Quando disattivi un utente, gli altri utenti non vedono più il loro nome quando cercano persone nel sistema.

Gli amministratori possono visualizzare gli utenti inattivi nell’area Configurazione.

Puoi riattivare un utente in qualsiasi momento.

>[!IMPORTANT]
>
>È consigliabile disattivare gli utenti che hanno lasciato l’organizzazione anziché eliminarli. Se un utente viene eliminato, tutta la cronologia in Workfront associata a tale utente viene persa. Ciò include le relative assegnazioni di lavoro, l&#39;associazione con note, ore, documenti e tutti gli altri oggetti creati.
>
>La disattivazione di un utente in Workfront rimuove le licenze dell&#39;utente sia su Workfront che su prove digitali. Inoltre, all’utente non può più essere assegnato il lavoro. Quando un utente è disattivato, la licenza Workfront e la licenza di correzione di tale utente diventano disponibili per essere utilizzati da un altro utente; tutte le altre informazioni nel profilo dell’utente disattivato rimangono invariate.
>
>Per ulteriori informazioni sull’impatto dell’eliminazione e sulla disattivazione degli utenti, consulta [Eliminare gli utenti](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Piano </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi disporre di una delle seguenti caratteristiche:</p> 
    <ul> 
     <li> <p>Livello di accesso amministratore di sistema. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> </li> 
     <li> <p><b>Utenti</b> impostazione nel livello di accesso configurato per <b>Modifica</b> accesso, con <b>Crea</b> e almeno uno dei due <b>Amministratore utente</b> opzioni attivate in <b>Ottimizzare le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se Utente <b>Amministratore (utenti del gruppo)</b> è abilitato, devi essere un amministratore di gruppo di un gruppo in cui l’utente è membro.</p> <p>Per ulteriori informazioni sulla <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Disattiva un utente

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).

1. Seleziona un utente e fai clic sull’icona Altro ![](assets/more-icon.png), quindi fai clic su **Disattiva**.

1. Fai clic su **Disattiva** nella casella visualizzata.

## Pianificare gli utenti per la disattivazione

In qualità di responsabile, potresti voler contrassegnare gli utenti per la disattivazione prima che questi effettivamente abbandonino la tua organizzazione. Ad esempio, se lavori con un utente che è vincolato per contratto, il tuo sistema ti offre un periodo di tempo limitato e conosci la data di terminazione. Puoi pianificarle per disattivarle in quella data.

Gli amministratori di Workfront e gli utenti con licenze Pianifica possono visualizzare la data di disattivazione nel loro profilo utente.

Per pianificare la disattivazione di un utente:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).

1. Seleziona il nome dell’utente.

   Oppure

   (Facoltativo) Seleziona più utenti per pianificarli in blocco per la disattivazione.

1. Fai clic sull’icona Modifica ![](assets/edit-icon.png).
1. Nella casella Modifica utente visualizzata, fai clic su **Pianificazione delle risorse** per andare in quella zona.
1. Abilita la **Disattivazione programmata** opzione .

1. Nel calendario visualizzato, specifica la data e l’ora del **Data di disattivazione pianificata**.

   >[!NOTE]
   >
   >* Nella casella Tempo, è possibile selezionare solo incrementi di ore intere, non minuti.
   >* Se selezioni un’ora per il giorno corrente che è passato, Workfront pianifica la disattivazione per il giorno successivo alle 12:00. L’ora selezionata corrisponde al fuso orario del computer dell’utente che pianifica la disattivazione.


1. Fai clic su **Salva modifiche**.

   L’utente viene disattivato il giorno selezionato a volte dopo l’ora selezionata. Se hai selezionato più utenti da disattivare in blocco, tutti gli utenti selezionati vengono disattivati il giorno selezionato a volte dopo l’ora selezionata.

È consigliabile creare un rapporto per gli utenti programmati per la disattivazione, per informarli sugli utenti che verranno disattivati. Non vi è alcuna conferma che la disattivazione si verifichi una volta che gli utenti si sono disattivati.

## Riattivare un utente

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).

1. Seleziona un utente e fai clic sull’icona Altro ![](assets/more-icon.png), quindi fai clic su **Attiva**.

1. Assegnare un nuovo **Livello di accesso** nel menu a discesa .

### Impatto della correzione quando si riattiva un utente

Gli utenti disattivati perdono il ruolo di correzione predefinito assegnato e la relativa licenza di bozza (se ti trovi in un piano legacy di Workfront Premium). Se scegli di riattivare l&#39;utente, devi:

* Riassegna la licenza (se utilizzi un piano legacy di Workfront Premium). Per ulteriori informazioni sui piani di correzione di Workfront, consulta [Accesso alle funzionalità di correzione in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Verifica che abbiano il ruolo di bozza corretto. Agli utenti della bozza riattivata viene assegnato qualsiasi elemento specificato come ruolo di bozza predefinito per i nuovi utenti. Vedi [Configurare i ruoli di correzione predefiniti](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) per ulteriori informazioni.

## Informazioni sulla disattivazione degli amministratori di Workfront e sulla pianificazione degli utenti delle licenze

Prima di disattivare un amministratore Workfront o un utente con una licenza Plan, è importante verificare la presenza di oggetti e attività Workfront che coinvolgono tale persona, quindi associarli a un altro amministratore Workfront o a un utente con licenza Plan, a seconda delle necessità.

Questi oggetti e attività possono includere quanto segue:

* Attività o problemi assegnati all’utente
* Progetti di proprietà dell’utente
* Report configurati per l&#39;esecuzione con i diritti di accesso dell&#39;utente
* Modelli di proprietà dell’utente
* Progetti e modelli in cui l’utente è stato impostato come gestore delle risorse
* Richiedi regole di routing della coda di richiesta in cui l&#39;amministratore di Workfront o l&#39;utente con licenza Piano è l&#39;assegnatario predefinito
* Processi di approvazione che hanno una fase che include l&#39;utente (specialmente se erano l&#39;unico approvatore sulla scena)
* Schede temporali che elencano l’utente come approvatore
* Profili della scheda attività che elencano l&#39;utente come approvatore
* Correzione dei flussi di lavoro automatizzati che includono l’utente

## Impatto sulla pianificazione delle risorse quando si pianifica un utente per la disattivazione

Quando si pianifica la disattivazione di un utente, questo non viene più visualizzato nel Planner risorse come disponibile per le ore di budget. Se rimangono parte dei pool di risorse, vengono visualizzati nel planner risorse, ma la loro disponibilità sarà impostata su zero ore a partire dalla data della loro disattivazione pianificata.

Il Planner risorse tiene conto di tutti i ruoli del lavoro degli utenti e delle date di completamento pianificate delle attività e calcola le risorse di conseguenza.

Per ulteriori informazioni sul planner risorse, vedere [Panoramica di Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
