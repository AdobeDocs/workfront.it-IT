---
product-area: projects
navigation-topic: create-projects
title: Crea un Progetto
description: '(NOTA: è collegato dall’interfaccia utente della sezione Navigazione globale dei progetti in Classic. Non modificare/rimuovere)'
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: e83d4742106bc3cb5adb939040997959315dd1e2
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# Crea un Progetto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is linked from the UI from the Projects global nav section in classic. Do not change/ remove)</p>
-->

I progetti rappresentano una grande quantità di lavoro che deve essere svolto in Adobe Workfront.

## Requisiti di accesso

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull&#39;accesso ai progetti, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concedere l’accesso ai progetti</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Quando crei un progetto ricevi automaticamente le autorizzazioni Gestisci per il progetto </p> <p> Per informazioni sulle autorizzazioni del progetto, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Condivisione di un progetto in Adobe Workfront</a>.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Modalità di creazione dei progetti

Puoi creare un progetto in Workfront utilizzando uno dei seguenti metodi:

* Crea un progetto da zero senza utilizzare un modello. Questo articolo descrive come creare un progetto da zero.

* Copia un progetto esistente.\
   Per ulteriori informazioni sulla copia del progetto, vedi [Copiare un progetto](../../../manage-work/projects/manage-projects/copy-project.md).

* Utilizza un modello.\
   Per ulteriori informazioni sull&#39;utilizzo di un modello per creare un nuovo progetto, consulta [Creare un progetto utilizzando un modello](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Importa un progetto da Progetto Microsoft.\
   Per ulteriori informazioni sull&#39;importazione di un progetto da MS Project, vedere [Importare un progetto da un progetto Microsoft](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importa un progetto utilizzando le fasi di avvio.

   In qualità di amministratore di Workfront, puoi importare i progetti con una procedura di avvio rapido.

   Per informazioni sull&#39;importazione di dati con i avvii di avvio in Workfront, vedi [Importare dati in Adobe Workfront utilizzando un modello Click-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md) .

   Per informazioni sull’importazione di progetti tramite i Avvio rapido, vedi [Scenario Kick-Starts: preparazione semplice di progetti e operazioni di importazione](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md) .

* Pubblica un&#39;iniziativa da uno scenario in Adobe Workfront Scenario Planner. Il planner scenario richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedi [Panoramica di Scenario Planner](../../../scenario-planner/scenario-planner-overview.md). Per informazioni sulla creazione di progetti da iniziative di pubblicazione, vedi  [Aggiornare o creare progetti pubblicando iniziative nel Planner scenario](../../../scenario-planner/publish-scenarios-update-projects.md).

## Prerequisiti

Prima di iniziare, assicurati che

* L’amministratore di sistema o di gruppo ha abilitato la preferenza &quot;Consenti agli utenti di creare progetti senza utilizzare un modello&quot; nell’area Configurazione.

   Per ulteriori informazioni, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Nuove impostazioni predefinite del progetto

Quando crei un progetto, Workfront applica un set di impostazioni predefinite. Ad esempio, le modalità Stato, Gruppo o Pianificazione sono predefinite quando crei un progetto.

Considera quanto segue:

* In qualità di amministratore di Workfront o di gruppo, è possibile configurare le impostazioni predefinite per un nuovo progetto durante la configurazione di Preferenze progetto.
* Workfront applica le impostazioni del gruppo, se presenti, prima di applicare quelle impostate dall’amministratore di Workfront.
* Se crei un progetto utilizzando un modello, le impostazioni del modello hanno la precedenza sulle impostazioni stabilite dall’amministratore di Workfront o di gruppo.

>[!NOTE]
>
>Lo stato predefinito per un nuovo progetto è Planning. Quando apporti modifiche al nuovo progetto, le notifiche non vengono attivate dagli utenti assegnati al progetto.

Per ulteriori informazioni sull’impostazione dello stato predefinito e di altre impostazioni predefinite per un nuovo progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).



## Crea un progetto da zero

1. Esegui una delle operazioni seguenti:

   * Fai clic sul pulsante **Menu principale** ![](assets/main-menu-icon.png), fai clic su **Progetti**, quindi espandi **Nuovo progetto**.
   * Passa a un portfolio, quindi espandi **Nuovo progetto**.

      >[!TIP]
      >
      >Quando crei un progetto utilizzando un modello di un portfolio, il campo Portfolio del nuovo progetto viene aggiornato per visualizzare il portfolio da cui hai scelto di creare il progetto. Questo sovrascrive il campo Portfolio sul modello, se specificato.

   * Vai a un programma, quindi espandi **Nuovo progetto**.

      >[!TIP]
      >
      >Quando crei un progetto utilizzando un modello di un programma, il campo Programma dei nuovi progetti viene aggiornato per visualizzare il programma da cui hai scelto di creare il progetto. Il campo Portfolio del modello viene aggiornato per visualizzare il portfolio del programma da cui hai scelto di creare il progetto. Questo sovrascrive i campi Programma e Portfolio nel modello, se specificati.

   * Gli amministratori di gruppo possono creare un progetto anche nella sezione Progetti di un gruppo gestito. Per ulteriori informazioni, consulta [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

      >[!TIP]
      >
      >Quando crei un progetto utilizzando un modello di un gruppo, il gruppo da cui crei il progetto viene visualizzato nel campo Gruppo del nuovo progetto solo quando il campo Gruppo del modello non è specificato. Se il campo Gruppo modello è specificato, il campo Gruppo del nuovo progetto è quello del modello.
   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Fai clic su **Nuovo progetto** per creare un progetto da zero.
1. Inserisci un nome per il progetto. Premere Invio per salvare il nome.

   ![](assets/untitled-project-rename-new-project-nwe-350x127.png)

   L’intestazione della pagina del progetto presenta una rapida panoramica dello stato attuale e dell’avanzamento di un progetto. Le informazioni nell’intestazione del progetto cambiano quando vengono aggiornate le informazioni del progetto.

1. Fai clic su **Aggiungi** **Attività**.

   Oppure

   Fai clic su **Nuova attività** per aggiungere attività al progetto e assegnare loro risorse.\
   Per ulteriori informazioni sull’aggiunta di attività a un progetto, consulta [Creazione di attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Modifica i dettagli del progetto facendo clic sul pulsante **Menu Altro** e poi **Modifica** ![](assets/qs-edit-icon.png) accanto al nome del progetto.

   La **Modifica progetto** viene visualizzata la finestra di dialogo.

   Per ulteriori informazioni sulla modifica di un progetto, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

1. (Facoltativo) Dopo aver configurato le impostazioni del progetto e aggiunto le attività, puoi modificare lo stato del progetto in **Corrente**.

   Questo indica che il progetto è ora pronto per essere avviato e che gli utenti assegnati alle attività possono ora iniziare a lavorarci.

   Per ulteriori informazioni sugli stati del progetto, consulta [Accedere all’elenco degli stati del progetto di sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
