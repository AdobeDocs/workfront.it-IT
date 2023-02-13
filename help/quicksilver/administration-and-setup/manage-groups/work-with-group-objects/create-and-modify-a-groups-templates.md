---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creare e modificare i modelli di progetto di un gruppo
description: Quando visualizzi un gruppo gestito nell’area Gruppi, puoi visualizzare e utilizzare i modelli di progetto associati al gruppo e a uno dei relativi sottogruppi.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 1%

---

# Creare e modificare i modelli di progetto di un gruppo

Quando visualizzi un gruppo gestito nell’area Gruppi, puoi visualizzare e utilizzare i modelli di progetto associati al gruppo e a uno dei relativi sottogruppi.

Se ci sono gruppi al di sopra del gruppo, i loro amministratori possono fare queste cose anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>È necessario essere un amministratore del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza accesso o superiore ai modelli che desideri visualizzare e utilizzare</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Visualizza, utilizza e crea modelli per il gruppo dall’area Gruppi

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fare clic sul nome del gruppo per il quale si desidera creare o modificare i modelli.
1. Nel pannello a sinistra, fai clic su **Modelli** per elencare i modelli associati al gruppo e a eventuali sottogruppi.

   Per visualizzarlo in questo elenco, è necessario disporre dell’accesso Visualizza a un modello. Per informazioni su questo accesso, vedi [Concedere l’accesso ai modelli](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Effettua una delle seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aggiungi un modello</td> 
      <td> <p>Fai clic su <strong>Nuovo modello</strong>, quindi configuralo utilizzando le opzioni disponibili. Per informazioni su queste opzioni, consulta <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Creare un modello di progetto</a>.</p> <p>Il modello viene associato automaticamente al gruppo.</p> <p>Per informazioni su come applicare le preferenze di gruppo ai nuovi modelli, consulta <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">Applicazione delle preferenze ai modelli e alle attività dei modelli</a> in questo articolo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modificare uno o più modelli</td> 
      <td> <p>Seleziona almeno un modello e fai clic sull’icona Modifica <img src="assets/edit-icon.png">, quindi utilizza una qualsiasi delle opzioni disponibili per configurarla. Per informazioni su queste opzioni, consulta <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Modificare i modelli di progetto</a>.</p> <p>L’icona Modifica è disponibile solo se si dispone dell’accesso Modifica a tutti i modelli selezionati. Per informazioni su questo accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concedere l’accesso ai modelli</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eliminare uno o più modelli</td> 
      <td> <p>Seleziona almeno un modello, quindi fai clic sull’icona Elimina <img src="assets/delete.png">.</p> <p>Questa icona è disponibile solo se disponi dell’accesso Modifica a tutti i modelli selezionati. Per informazioni su questo accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concedere l’accesso ai modelli</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condividere uno o più modelli</td> 
      <td> <p>Seleziona almeno un modello e fai clic sull’icona Condividi <img src="assets/share-icon.png">, quindi fai clic su una delle seguenti opzioni nel menu a discesa:</p> 
       <ul> 
        <li> <p><strong>Modello</strong>: In <strong>Accesso a modelli</strong> in cui viene visualizzato, aggiungi i nomi per specificare gli utenti a cui si desidera accedere al modello stesso.</p> <p>Per ulteriori informazioni, consulta la sezione . <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Condividere un modello</a> nell'articolo <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Condividere i modelli di progetto</a>.</p> </li> 
        <li><strong>Progetto</strong>: In <strong>Accesso al progetto</strong> che viene visualizzata, aggiungi i nomi per specificare gli utenti a cui desideri accedere per i progetti creati dal modello</li> 
       </ul> <p>L’icona Condividi è disponibile solo se disponi dell’accesso Condividi a tutti i modelli selezionati. Per informazioni su questo accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concedere l’accesso ai modelli</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esportare l’elenco dei modelli</td> 
      <td>Fai clic su <strong>Esporta</strong> <img src="assets/export.png">, quindi selezionare il formato di file desiderato per l’elenco esportato.</td> 
     </tr> 
    </tbody> 
   </table>

## Applicazione delle preferenze ai modelli e alle attività dei modelli {#how-preferences-apply-to-templates-and-template-tasks}

Quando si crea un modello di progetto, le impostazioni elencate nelle tabelle seguenti vengono configurate automaticamente da una preferenza di progetto o attività corrispondente.

>[!NOTE]
>
>Una preferenza a livello di gruppo, di sistema o di progetto o di attività influisce su un modello di progetto, a seconda che il modello sia associato o meno a un gruppo al momento della creazione.
>
>Se lo si associa a un gruppo, la preferenza a livello di gruppo ha effetto. Questo si verifica nei seguenti scenari:
>
>* Il modello viene creato dall&#39;area Gruppi, come spiegato in questo articolo
>* Puoi specificare un gruppo quando crei il modello utilizzando un file Kickstart
>* Quando crei il modello utilizzando l’API, specifica un gruppo
>
>Se non si associa il nuovo modello a un gruppo, la preferenza a livello di sistema ha effetto. Questo si verifica quando negli scenari seguenti. Se successivamente assegni un gruppo all&#39;attività modello o modello, le preferenze del gruppo non lo influiscono.
>
>* È possibile creare il modello dall&#39;area Modelli
>* Non si specifica un gruppo quando si crea il modello utilizzando un file Kickstart
>* Non specifichi un gruppo quando crei il modello utilizzando l’API
>


* [Impostazioni del modello di progetto configurate dalle preferenze del progetto e dell&#39;attività](#project-template-settings-configured-by-project-and-task-preferences)
* [Impostazioni delle attività del modello configurate dalle preferenze delle attività](#template-task-settings-configured-by-task-preferences)

### Impostazioni del modello di progetto configurate dalle preferenze del progetto e dell&#39;attività {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Metodo Indicizzazione Performance</p> </td> 
   <td> <p>Configurata dalla preferenza di progetto a livello di gruppo "Metodo indice prestazioni" se si associa il nuovo modello a un gruppo oppure, in caso contrario, dalla stessa preferenza di progetto a livello di sistema.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo di Condizione</p> </td> 
   <td> <p>Configurato dalla preferenza di progetto a livello di gruppo "Imposta automaticamente la condizione del progetto in base allo stato di avanzamento" se si associa il nuovo modello a un gruppo oppure, in caso contrario, la stessa preferenza di progetto a livello di sistema.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Pianificazione da</p> </td> 
   <td> <p>Configurata dalla preferenza di progetto a livello di gruppo "Pianificazione da" se si associa il nuovo modello a un gruppo oppure dalla stessa preferenza di progetto a livello di sistema, in caso contrario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tempo di inattività dell'utente</p> </td> 
   <td> <p>Configurato dalla preferenza di progetto a livello di gruppo "User time off" (Tempo utente disattivato) se si associa il nuovo modello a un gruppo oppure dalla stessa preferenza di progetto a livello di sistema, in caso contrario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo di aggiornamento</p> </td> 
   <td> <p>Configurata dalla preferenza del progetto a livello di gruppo "Le timeline del progetto verranno ricalcolate automaticamente" se si associa il nuovo modello a un gruppo oppure, in caso contrario, la stessa preferenza del progetto a livello di sistema.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Accedere alle impostazioni della sezione</p> </td> 
   <td> <p>Configurato dalle preferenze dell'attività a livello di gruppo nella sezione "Accesso" se si associa il nuovo modello a un gruppo, o la stessa preferenza di progetto a livello di sistema, in caso contrario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni sulle preferenze del progetto elencate in questa tabella, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Per informazioni sull&#39;attività e sulle preferenze relative al problema, vedi [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* Se modifichi il gruppo associato a un modello di progetto esistente, le impostazioni del modello rimangono le stesse.
>* Se si sposta un&#39;attività modello esistente in un altro modello, le seguenti impostazioni rimangono invariate nell&#39;attività modello, indipendentemente dal gruppo associato al nuovo modello:>
   >   * Tipo di Durata
   >   * Tipo di Reddito
   >   * Tipo Cst
>
>  Tuttavia, l&#39;attività del modello è influenzata dall&#39;impostazione &quot;Quando un utente viene assegnato a un&#39;attività&quot; sul nuovo modello. Per ulteriori informazioni, consulta la sezione . [Accesso](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) nell&#39;articolo [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* Quando un amministratore salva un progetto come modello, tutte le impostazioni per il modello vengono ereditate dal progetto, incluso il gruppo.
>
>  Quando un amministratore converte un’attività o un problema in un progetto utilizzando un modello, tutte le impostazioni del modello sono determinate da ciò che è già stato salvato nel modello.

### Impostazioni delle attività del modello configurate dalle preferenze delle attività {#template-task-settings-configured-by-task-preferences}

Quando si crea un&#39;attività modello, alcune delle relative impostazioni vengono configurate automaticamente da una preferenza corrispondente. Queste impostazioni sono elencate nella tabella seguente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Tipo di Durata </p> </td> 
   <td> <p>Configurato dalla preferenza per l'attività a livello di gruppo "Tipo di durata" se si associa il modello a un gruppo, oppure dalla stessa attività a livello di sistema e dalla stessa preferenza per il problema in caso contrario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo di Reddito</p> </td> 
   <td> <p>Configurata dalla preferenza attività a livello di gruppo "Tipo di ricavi" se si associa il modello a un gruppo, oppure dalla stessa attività a livello di sistema e dalla stessa preferenza di problema, in caso contrario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo Cst </p> </td> 
   <td> <p> Configurato dalla preferenza attività a livello di gruppo "Tipo di costo" se si associa il modello a un gruppo, oppure dalla stessa attività a livello di sistema e dalla stessa preferenza relativa al problema, in caso contrario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni sulle preferenze delle attività elencate in questa tabella, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
