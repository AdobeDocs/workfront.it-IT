---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creare e modificare i modelli di progetto di un gruppo
description: Quando visualizzi un gruppo che gestisci nell’area Gruppi, puoi visualizzare e utilizzare i modelli di progetto associati al gruppo e ai relativi sottogruppi.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1281'
ht-degree: 1%

---

# Creare e modificare i modelli di progetto di un gruppo

Quando visualizzi un gruppo che gestisci nell’area Gruppi, puoi visualizzare e utilizzare i modelli di progetto associati al gruppo e ai relativi sottogruppi.

Se ci sono gruppi al di sopra del gruppo, gli amministratori possono eseguire queste operazioni anche per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di visualizzazione o versione successiva sui modelli che si desidera visualizzare e utilizzare</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Visualizzare, utilizzare e creare modelli per il gruppo dall&#39;area Gruppi

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![Gruppi](assets/groups-icon.png).

1. Fare clic sul nome del gruppo per il quale si desidera creare o modificare i modelli.
1. Nel pannello a sinistra, fai clic su **Modelli** per elencare i modelli associati al gruppo e ai suoi eventuali sottogruppi.

   È necessario disporre dell&#39;accesso di visualizzazione a un modello per visualizzarlo in questo elenco. Per informazioni su questo accesso, vedere [Concedere l&#39;accesso ai modelli](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Effettua una delle seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aggiungi un modello</td> 
      <td> <p>Fai clic su <strong>Nuovo modello</strong>, quindi configuralo utilizzando le opzioni disponibili. Per informazioni su queste opzioni, vedere <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Creare un modello di progetto</a>.</p> <p>Il modello viene associato automaticamente al gruppo.</p> <p>Per informazioni sulle modalità di applicazione delle preferenze di gruppo ai nuovi modelli, vedere <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">Modalità di applicazione delle preferenze ai modelli e alle attività modello</a> in questo articolo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modifica uno o più modelli</td> 
      <td> <p>Selezionare almeno un modello, fare clic sull'icona Modifica <img src="assets/edit-icon.png">, quindi utilizzare una delle opzioni disponibili per configurarlo. Per informazioni su queste opzioni, vedere <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Modifica modelli di progetto</a>.</p> <p>L’icona Modifica è disponibile solo se disponi dell’accesso Modifica per tutti i modelli selezionati. Per informazioni su questo accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concedere l'accesso ai modelli</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Elimina uno o più modelli</td> 
      <td> <p>Selezionare almeno un modello, quindi fare clic sull'icona Elimina <img src="assets/delete.png">.</p> <p>Questa icona è disponibile solo se si dispone dell'accesso di modifica a tutti i modelli selezionati. Per informazioni su questo accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concedere l'accesso ai modelli</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condividere uno o più modelli</td> 
      <td> <p>Selezionare almeno un modello, fare clic sull'icona Condividi <img src="assets/share-icon.png">, quindi scegliere una delle opzioni seguenti nel menu a discesa:</p> 
       <ul> 
        <li> <p><strong>Modello</strong>: nella casella <strong>Accesso al modello</strong> visualizzata, aggiungi dei nomi per specificare chi desideri avere accesso al modello stesso.</p> <p>Per ulteriori informazioni, vedere la sezione <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Condividere un modello</a> nell'articolo <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Condividere modelli di progetto</a>.</p> </li> 
        <li><strong>Progetto</strong>: nella casella <strong>Project Access</strong> visualizzata, aggiungi dei nomi per specificare chi desideri avere accesso ai progetti creati dal modello</li> 
       </ul> <p>L’icona Condividi è disponibile solo se disponi dell’accesso Condividi per tutti i modelli selezionati. Per informazioni su questo accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concedere l'accesso ai modelli</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esporta l’elenco dei modelli</td> 
      <td>Fai clic su <strong>Esporta</strong> <img src="assets/export.png">, quindi seleziona il formato di file desiderato per l'elenco esportato.</td> 
     </tr> 
    </tbody> 
   </table>

## Applicare le preferenze ai modelli e alle attività modello {#how-preferences-apply-to-templates-and-template-tasks}

Quando si crea un modello di progetto, le impostazioni elencate nelle tabelle seguenti vengono configurate automaticamente in base a una preferenza di progetto o attività correlata.

>[!NOTE]
>
>Un modello di progetto o una preferenza di attività a livello di gruppo o di sistema influisce su un modello di progetto, a seconda che il modello sia stato associato o meno a un gruppo al momento della creazione.
>
>Se è stata associata a un gruppo, viene applicata la preferenza a livello di gruppo. Ciò si verifica nei seguenti scenari:
>
>* Crea il modello dall’area Gruppi, come spiegato in questo articolo
>* Specificare un gruppo quando si crea il modello utilizzando un file Kick-Start
>* Quando crei il modello utilizzando l’API, specifica un gruppo
>
>Se il nuovo modello non è stato associato a un gruppo, viene applicata la preferenza a livello di sistema. Ciò si verifica negli scenari seguenti. Se in seguito si assegna un gruppo all&#39;attività modello o modello, le preferenze del gruppo non hanno effetto su di esso.
>
>* Il modello viene creato dall&#39;area Modelli
>* Non si specifica un gruppo quando si crea il modello utilizzando un file Kick-Start
>* Non si specifica un gruppo durante la creazione del modello utilizzando l’API
>

* [Impostazioni modello di progetto configurate dalle preferenze progetto e attività](#project-template-settings-configured-by-project-and-task-preferences)
* [Impostazioni attività modello configurate dalle preferenze attività](#template-task-settings-configured-by-task-preferences)

### Impostazioni dei modelli di progetto configurate dalle preferenze per progetto e attività {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Metodo indice prestazioni</p> </td> 
   <td> <p>Configurato dalla preferenza di progetto a livello di gruppo "Metodo indice prestazioni" se si associa il nuovo modello a un gruppo o dalla stessa preferenza di progetto a livello di sistema in caso contrario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo di condizione</p> </td> 
   <td> <p>Configurato dalla preferenza di progetto a livello di gruppo "Imposta automaticamente la condizione del progetto in base allo stato di avanzamento" se si associa il nuovo modello a un gruppo o dalla stessa preferenza di progetto a livello di sistema in caso contrario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Pianifica da</p> </td> 
   <td> <p>Configurato dalla preferenza di progetto a livello di gruppo "Pianifica da" se si associa il nuovo modello a un gruppo o dalla stessa preferenza di progetto a livello di sistema in caso contrario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Indisponibilità utente</p> </td> 
   <td> <p>Configurato dalla preferenza di progetto a livello di gruppo "Indisponibilità utente" se si associa il nuovo modello a un gruppo o dalla stessa preferenza di progetto a livello di sistema in caso contrario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo di aggiornamento</p> </td> 
   <td> <p>Configurato dalla preferenza di progetto a livello di gruppo "Le sequenze temporali del progetto verranno ricalcolate automaticamente" se si associa il nuovo modello a un gruppo o dalla stessa preferenza di progetto a livello di sistema in caso contrario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Impostazioni sezione di accesso</p> </td> 
   <td> <p>Configurato dalle preferenze per le attività a livello di gruppo nella sezione "Accesso" se si associa il nuovo modello a un gruppo o dalla stessa preferenza per il progetto a livello di sistema in caso contrario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni sulle preferenze di progetto elencate in questa tabella, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Per informazioni sull&#39;attività e sulle preferenze relative ai problemi, vedere [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* Se si modifica il gruppo associato a un modello di progetto esistente, le impostazioni del modello rimangono invariate.
>* Se si sposta un&#39;attività modello esistente in un altro modello, le impostazioni seguenti rimangono invariate nell&#39;attività modello, indipendentemente dal gruppo associato al nuovo modello:>
>   * Tipo di Durata
>   * Tipo di Reddito
>   * Tipo Cst
>
>  Tuttavia, l’attività modello è interessata dall’impostazione &quot;Quando a un utente viene assegnata un’attività&quot; nel nuovo modello. Per ulteriori informazioni, vedere la sezione [Accesso](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) nell&#39;articolo [Modifica modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* Quando un amministratore salva un progetto come modello, tutte le impostazioni del modello vengono ereditate dal progetto, incluso il gruppo.
>
>  Quando un amministratore converte un’attività o un problema in un progetto utilizzando un modello, tutte le impostazioni del modello sono determinate da ciò che è già stato salvato nel modello.
>

### Impostazioni attività modello configurate dalle preferenze attività {#template-task-settings-configured-by-task-preferences}

Quando si crea un&#39;attività modello, alcune delle relative impostazioni vengono configurate automaticamente da una preferenza dell&#39;attività correlata. Queste impostazioni sono elencate nella tabella seguente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Tipo di Durata </p> </td> 
   <td> <p>Configurato dalla preferenza "Tipo di durata" per le attività a livello di gruppo, se si associa il modello a un gruppo, oppure dalla stessa preferenza per attività e problemi a livello di sistema, in caso contrario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo di Reddito</p> </td> 
   <td> <p>Configurato dalla preferenza "Tipo di retribuzione" per le attività a livello di gruppo, se si associa il modello a un gruppo, oppure dalla stessa preferenza per attività e problemi a livello di sistema, in caso contrario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tipo Cst </p> </td> 
   <td> <p> Configurato dalla preferenza dell'attività a livello di gruppo "Tipo di costo" se si associa il modello a un gruppo oppure dalla stessa attività a livello di sistema e dalla stessa preferenza del problema in caso contrario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni sulle preferenze per le attività elencate in questa tabella, vedere [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
