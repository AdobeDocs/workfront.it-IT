---
title: Condividere un progetto
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Il tuo amministratore Adobe Workfront può concederti l’accesso per visualizzare o modificare progetti durante l’assegnazione del livello di accesso. Per ulteriori informazioni, consulta Concedere l’accesso ai progetti.
author: Courtney
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1574'
ht-degree: 7%

---

# Condividere un progetto

<!-- Audited: 1/2024 -->

Il tuo amministratore Adobe Workfront può concederti l’accesso per visualizzare o modificare progetti durante l’assegnazione del livello di accesso. Per ulteriori informazioni, vedere [Concedere l&#39;accesso ai progetti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Oltre al livello di accesso concesso agli utenti, è possibile concedere loro le autorizzazioni per visualizzare, contribuire o gestire progetti specifici a cui si ha accesso per la condivisione.

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile eseguire su tale elemento.


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Work o successiva</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore agli oggetti da condividere</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni o versioni successive per gli oggetti da condividere</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulla condivisione di progetti

Oltre alle considerazioni riportate di seguito, vedere anche [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Per impostazione predefinita, il creatore di un progetto dispone delle autorizzazioni per gestire il progetto ed è anche designato come proprietario del progetto. Se il progetto è assegnato a un altro proprietario, anche tale utente dispone delle autorizzazioni necessarie per gestire il progetto. Quando il creatore del progetto (o il proprietario) condivide il progetto con altri utenti, concede a questi ultimi determinate autorizzazioni per controllare ciò che possono fare mentre lavorano sul progetto.

  Tuttavia, se un proprietario del progetto non dispone di una licenza Pianificazione o Standard, non ha accesso completo alla gestione del progetto. Solo un utente con una licenza Plan o Standard può disporre delle autorizzazioni per gestire un progetto. Per ulteriori informazioni, vedere [Funzionamento dei livelli di accesso e delle autorizzazioni](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

* Puoi condividere i progetti singolarmente, oppure puoi condividerne più di uno alla volta. La condivisione di progetti è identica alla condivisione di altri oggetti. Per ulteriori informazioni sulla condivisione di elementi in Workfront, vedere [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Puoi concedere le seguenti autorizzazioni a un progetto:

   * Visualizzazione
   * Gestione
   * Contribuisci

* Quando si condivide un progetto, tutte le attività, i problemi e i documenti ereditano le stesse autorizzazioni, se non diversamente specificato.

  Per informazioni sulla gestione dell&#39;accesso alle attività e ai problemi del progetto in base alle autorizzazioni di un utente per il progetto, vedere la sezione [](../../manage-work/projects/manage-projects/edit-projects.md#access) nell&#39;articolo [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).

  L&#39;amministratore di Workfront può specificare se i documenti devono ereditare le autorizzazioni da oggetti di livello superiore nel livello di accesso dell&#39;utente. Per ulteriori informazioni sulla limitazione delle autorizzazioni ereditate sui documenti, vedere [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* È possibile rimuovere le autorizzazioni ereditate da un progetto in modo che gli oggetti figlio non le ereditino. Per ulteriori informazioni sulla rimozione delle autorizzazioni ereditate dagli oggetti, vedere [Rimuovere le autorizzazioni dagli oggetti](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Limitazioni per i diversi tipi di licenza

* Gli utenti con una licenza Worker non dispongono delle autorizzazioni necessarie per gestire i progetti. Per i lavoratori, l&#39;autorizzazione di condivisione più elevata è Contribute.
* Gli utenti con una licenza Request possono visualizzare le informazioni sul progetto, ma hanno accesso limitato al progetto.
* Un&#39;eccezione alla modifica dello stato di un progetto si verifica quando un utente con autorizzazioni Visualizza o Contribuisci è incluso anche in un processo di approvazione. Possono approvare il progetto, che modifica lo stato del progetto, ma lo stato è quello predefinito per l’approvazione o per il rifiuto.
* Per poter copiare un progetto, un utente deve anche avere accesso alla creazione di progetti nel proprio Livello di Accesso.

## Modi per condividere un progetto {#ways-to-share-a-project}

Puoi condividere un progetto nei seguenti modi:

* Manualmente, effettuando una delle seguenti operazioni:

   * Aggiunta di utenti al team del progetto. Quando aggiungi utenti al team di progetto, questi ottengono automaticamente le autorizzazioni di visualizzazione per il progetto.\
     Per ulteriori informazioni sull&#39;aggiunta di utenti a un team di progetto, vedere la sezione Aggiunta di utenti a un team di progetto in [Panoramica team di progetto](../../manage-work/projects/planning-a-project/project-team-overview.md).
   * Condivisione singola o in blocco dei progetti quando si utilizza l&#39;opzione **Condivisione**.

* Automaticamente eseguendo una delle operazioni seguenti:

   * Posiziona un progetto in un **Portfolio** o **Programma** già condiviso con altri. Gli utenti ottengono le stesse autorizzazioni al progetto di cui dispongono per il portfolio o il programma.\
     Per informazioni sull&#39;aggiunta di un progetto a un **Portfolio**, vedere [Aggiungere progetti a un portfolio](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).\
     Per informazioni sull&#39;aggiunta di un progetto a un **Programma**, vedere [Aggiungere un progetto a un programma](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).
Per informazioni sulla visualizzazione delle autorizzazioni ereditate per un oggetto, vedere [Visualizzare le autorizzazioni ereditate per gli oggetti](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

   * Aggiungere entità alla condivisione di progetti in un modello utilizzato per creare il progetto. Per informazioni sulla condivisione di progetti da modelli, vedere [Condividere un modello](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).
   * Definire il modello di accesso al progetto.

     >[!TIP]
     >
     >Quando si allega o si salva un modello, è possibile cancellare le regole di condivisione dei progetti dei modelli.

   * Modificare un progetto e definire l&#39;impostazione **Quando a un utente viene concesso l&#39;accesso a questo progetto**.  Per ulteriori informazioni, vedere [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because I created new article and linked it above) </p>
<p>To view what users have inherited the access on the project from a portfolio or a program, do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1">Go to a project whose sharing permissions you want to view. </li>
<li value="2"> Click the <strong>More</strong> menu <img src="assets/more-icon.png">, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>Expand the <strong>Inherited Permissions</strong> list. </p> <p>This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project. </p>  </li>
</ol>
</div>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a project whose sharing permissions you want for all projects you create from scratch. (NOTE: drafted because linked above)  </li>
<li value="2"> Click the More menu, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>In the Project Access box that displays, near the upper-right corner, click the gear icon <img src="assets/gear-icon-settings.png">, then click <strong>Set as my project access template</strong>.</p> <p>The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future.</p> <p> The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level.<br>For more information about specifying sharing defaults for projects in the Access Level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> </li>
<li value="4">Click <strong>Save</strong>.</li>
</ol>
-->

## Condividere un progetto

{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona dall&#39;elenco il progetto che desideri condividere. Viene visualizzata la pagina del progetto.

1. A destra del nome del progetto, fai clic su **Condividi**. Viene visualizzata la finestra di dialogo **Condividi [Nome progetto]**.

   ![Pulsante Condividi progetto](assets/share-project.png)

1. Nel campo **Concedi l&#39;accesso al progetto a**, inizia a digitare il nome dell&#39;utente, del team, della mansione, del gruppo o della società con cui vuoi condividere il progetto, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   >
   >Puoi condividere un progetto solo con utenti attivi, team, ruoli o aziende.


1. (Facoltativo) Seleziona l&#39;elenco a discesa **Chi ha accesso** e seleziona il livello di accesso del progetto:

   * **Solo gli utenti invitati possono accedere a:** Solo gli utenti invitati al progetto possono accedervi (impostazione predefinita).
   * **Tutti gli utenti del sistema possono visualizzare**: tutti gli utenti del sistema possono visualizzare il progetto senza un invito.

1. (Facoltativo) Per applicare automaticamente le impostazioni di accesso al progetto selezionate a tutti i nuovi progetti, fai clic sull&#39;icona **Ingranaggio** ![Seleziona l&#39;icona ingranaggio](assets/gear-icon.png), quindi seleziona la casella in linea con **Imposta come modello di accesso al progetto**.

   >[!NOTE]
   >
   >Il modello di accesso al progetto sostituisce i valori predefiniti di condivisione concessi dall&#39;amministratore di Workfront nel proprio livello di accesso.\
   >Per ulteriori informazioni su come specificare i valori predefiniti di condivisione per i progetti nel Livello d&#39;Accesso, vedere [Concedere l&#39;accesso ai progetti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)

   <!--
   >this note also appears in Understanding Project Permissions-->


1. Fai clic sull’elenco a discesa a destra del nome dell’utente e seleziona il relativo livello di autorizzazione per questo progetto:


   * **Visualizza**: l&#39;utente può rivedere e condividere il progetto.
   * **Contributo**: l&#39;utente può apportare aggiornamenti, registrare informazioni, apportare modifiche minori e condividere il progetto (include anche tutte le autorizzazioni di visualizzazione).
   * **Gestisci**: l&#39;utente ha accesso completo al progetto senza diritti amministrativi, concessi a livello di accesso (include anche tutte le autorizzazioni di visualizzazione e di contributo).

1. (Facoltativo) Fai clic sull’icona delle opzioni avanzate accanto al livello di autorizzazione concesso per configurare autorizzazioni specifiche sul progetto.

   ![Opzioni di autorizzazione avanzate configurate](assets/advanced-permission-options.png)

1. (Facoltativo) Per condividere rapidamente il progetto utilizzando un collegamento, fare clic su **Copia collegamento** e quindi inoltrarlo al destinatario.

1. Fai clic su **Salva**.

## Condivisione di progetti in blocco

{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona la casella a sinistra di ciascun progetto che desideri condividere, quindi fai clic sull&#39;icona **Condividi** ![Condividi icona](assets/share-icon.png) nella parte superiore della pagina. Viene visualizzata la finestra modale di condivisione.

   ![Progetti di condivisione in blocco](assets/bulk-share-icon.png)

1. Nel campo **Concedi l&#39;accesso al progetto a**, inizia a digitare il nome dell&#39;utente, del team, della mansione, del gruppo o della società con cui desideri condividere i progetti, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   >
   >Puoi condividere i progetti solo con utenti attivi, team, ruoli o aziende.


1. (Facoltativo) Seleziona l&#39;elenco a discesa **Chi ha accesso** e il livello di accesso dei progetti:

   * **Solo gli utenti invitati possono accedere a:** Solo gli utenti invitati ai progetti possono accedervi (impostazione predefinita).
   * **Tutti gli utenti del sistema possono visualizzare**: tutti gli utenti del sistema possono visualizzare i progetti senza un invito.


1. Fai clic sull’elenco a discesa a destra del nome dell’utente e seleziona il relativo livello di autorizzazione per i progetti:

   * **Visualizza**: l&#39;utente può esaminare e condividere i progetti.
   * **Contributo**: l&#39;utente può apportare aggiornamenti, registrare informazioni, apportare modifiche minori e condividere i progetti (include anche tutte le autorizzazioni di visualizzazione).
   * **Gestisci**: l&#39;utente ha accesso completo ai progetti senza diritti amministrativi, che sono concessi a livello di accesso (include anche tutte le autorizzazioni Visualizza e Contribuisci).

1. (Facoltativo) Fai clic sull’icona delle opzioni avanzate accanto al livello di autorizzazione concesso per configurare autorizzazioni specifiche sui progetti.

   ![Opzioni di autorizzazione avanzate configurate](assets/advanced-permission-options.png)

1. Fai clic su **Salva**.


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing  the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Access</strong> in the list on the left.</li>
<li value="4"> <p>In the <strong>When someone is given access to this PROJECT</strong> section, select permissions that you want to be available when users are given access to the project via sharing.</p> <p>Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level.</p> <p>To view which permissions are available for each level, see  <a title="Project Permissions" href="#Understanding_Project_Permissions" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <note type="note">
The
<strong>Delete</strong> access in the
<strong>Manage</strong> permission level determines whether users can  delete the project itself. Users with
<strong>Manage</strong> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have
<strong>Manage</strong> permissions to the tasks and issues.  
</note> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## Opzioni di autorizzazione del progetto

Nella tabella seguente sono elencate le autorizzazioni che gli utenti possono concedere quando condividono un progetto. Per ulteriori informazioni sull&#39;accesso degli utenti in base alla licenza, vedere [Concedere l&#39;accesso ai progetti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Azioni</strong> </p> </th> 
   <th> <p><strong>Gestisci</strong> </p> </th> 
   <th> <p><strong>Contribuisci</strong> </p> </th> 
   <th> <p><strong>Visualizza</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aggiungi modulo personalizzato</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiorna campi personalizzati</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungere Un Processo Di Approvazione</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Approvare un progetto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Approva ore</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Crea Un Progetto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungi documenti</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungi problemi</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungi attività</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Copia Progetto</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Cancella Progetto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifica date pianificate</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Condividi progetto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Condividi a livello di sistema</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visualizza Progetto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiornamenti/commenti</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifica stato</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Registra ore</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifica assegnazioni</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gestisci Base Line</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gestione dei rischi*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gestisci dati finanziari*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungi/Modifica spese*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Finanza*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Allega Modello</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Salva come modello</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungi/Modifica Business Case</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifica dettagli progetto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifica assegnazione personale</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Esporta in MS Project</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ricalcola finanza/sequenza temporale*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Imposta proprietà coda</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>    </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modificare un progetto in blocco in un elenco</p> </td> 
   <td> <p>✓</p> </td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Gli utenti che non hanno accesso ai dati finanziari non possono gestire rischi e finanze per i progetti, anche se dispongono dell&#39;accesso in modifica ai progetti. Per informazioni sull&#39;accesso ai dati finanziari, vedere [Concedere l&#39;accesso ai dati finanziari](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
