---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Condividere un problema
description: L’amministratore di Adobe Workfront consente agli utenti di visualizzare o modificare i problemi quando assegnano i livelli di accesso. Per ulteriori informazioni su come concedere l’accesso ai problemi, consulta Concedere l’accesso ai problemi.
author: Courtney
feature: Get Started with Workfront
exl-id: 91ee72e0-20a9-4b06-9f80-a343dd4fbe06
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 4%

---

# Condividere un problema

L’amministratore di Adobe Workfront consente agli utenti di visualizzare o modificare i problemi quando assegnano i livelli di accesso. Per ulteriori informazioni sulla concessione dell&#39;accesso ai problemi, vedere [Concedere l&#39;accesso ai problemi](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md).

Oltre al livello di accesso concesso agli utenti, è possibile concedere loro le autorizzazioni per visualizzare, contribuire o gestire problemi specifici a cui si ha accesso per la condivisione. Per ulteriori informazioni sui livelli di accesso e sulle autorizzazioni, vedere [Funzionamento dei livelli di accesso e delle autorizzazioni](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile eseguire su tale elemento.


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

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
   <p>Lavoro o superiore</p> 
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

## Considerazioni sulla condivisione dei problemi

Oltre alle considerazioni riportate di seguito, vedere anche [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Un amministratore di Workfront può aggiungere o rimuovere autorizzazioni per qualsiasi elemento del sistema, per tutti gli utenti, senza esserne il proprietario.

* Per impostazione predefinita, l’autore di un problema dispone delle autorizzazioni di gestione relative a tale problema.
* È possibile condividere i problemi singolarmente o più problemi contemporaneamente. I problemi di condivisione sono identici agli altri elementi di Workfront. Per ulteriori informazioni sulla condivisione di elementi in Workfront, vedere [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Puoi concedere le seguenti autorizzazioni a un problema: 

   * Visualizzazione
   * Contribuisci
   * Gestisci

* Quando condividi un problema, tutti i documenti allegati al problema ereditano le stesse autorizzazioni.

  L&#39;amministratore di Workfront può specificare se i documenti devono ereditare le autorizzazioni da oggetti di livello superiore nel livello di accesso dell&#39;utente. Per ulteriori informazioni sulla limitazione delle autorizzazioni ereditate sui documenti, vedere [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* È possibile rimuovere le autorizzazioni ereditate da un problema. Per ulteriori informazioni, vedere [Rimuovere le autorizzazioni dagli oggetti](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Modi per condividere un problema

* Manuale, simile alla condivisione di qualsiasi altro oggetto in Workfront.
* Automaticamente, effettuando una delle seguenti operazioni:

   * Specifica le autorizzazioni per uno qualsiasi degli oggetti principali del problema: progetto, programma o portfolio. I problemi ereditano le autorizzazioni dai loro oggetti principali. Per informazioni sulla visualizzazione delle autorizzazioni ereditate sugli oggetti, vedere [Visualizzare le autorizzazioni ereditate sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Aggiungere entità alla condivisione di progetto in un modello utilizzato per creare il progetto in cui si trova il problema. Per informazioni sulla condivisione di progetti da modelli, vedere [Condividere un modello](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Specifica le autorizzazioni per tutti i problemi in un progetto quando lo modifichi. Per informazioni sulla gestione dell&#39;accesso a problemi o richieste sul progetto in base alle autorizzazioni di un utente per il progetto, vedere la sezione [](../../manage-work/projects/manage-projects/edit-projects.md#access) nell&#39;articolo [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >Se non si specifica il problema di autorizzazioni che gli utenti devono avere quando sono assegnati ai problemi del progetto, per impostazione predefinita ricevono le stesse autorizzazioni che hanno sul progetto.

   * Specifica le autorizzazioni che gli utenti ricevono in caso di problemi inviati in una coda di richieste durante la creazione di una coda di richieste. Per informazioni, vedere [Creare una coda di richieste](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

     >[!IMPORTANT]
     >
     >Le autorizzazioni vengono concesse in modo diverso a seconda che il progetto sia pubblicato o meno come coda di richieste:
     >
     >   
     >   
     >   * Quando un utente invia una richiesta a un progetto pubblicato come coda di richieste, agli utenti Contatto principale e Immesso da viene concessa l’autorizzazione specificata.
     >   * Quando un utente invia una richiesta a un progetto non pubblicato come coda di richieste, al contatto principale (se diverso dall’utente Inserito da) viene concessa l’autorizzazione specificata e all’utente Inserito da vengono concesse le autorizzazioni Gestione del problema.
     >   
     >

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue at the project level</h2>
<p>(NOTE: this info duplicates in Edit projects - linked there instead (above).)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are added to a project.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2"> Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. </li>
<li value="3">In the <strong>Edit Project</strong> box that displays, click <strong>Access</strong>.</li>
<li value="4">In the <strong>When someone is assigned to an ISSUE</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><strong>Manage</strong><br>Now, when someone is assigned to an issue on the selected project, they are granted the specified permissions to the issue.&nbsp;</li>
</ul></li>
<li value="5">(Optional) Select the <strong>Also grant ... access to the project</strong> field to also grant View, Contribute, or Manage permissions to the projects to the user assigned to the issue</li>
<li value="6">In the <strong>When someone submits a REQUEST ...</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><p><strong>Manage</strong></p><note type="important">
<p>Permissions are granted differently depending on whether or not the project is published as a request queue:</p>
<ul>
<li>When a user submits a request to a project published as a request queue, the Primary Contact and Entered By users are granted the permission specified.</li>
<li>When a user submits a request to a project not published as a request queue, the Primary Contact (if different from Entered By user) is granted the permission specified, and the Entered By user is granted Manage permissions to the issue.</li>
</ul>
</note></li>
</ul></li>
<li value="7"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong> field.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="8">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue in request queues</h2>
<p>(NOTE: drafted because it's duplicated from Create a Request Queue which is linked above)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are submitted to a request queue.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2">Click <strong>Edit Project</strong>.</li>
<li value="3">Click <strong>More</strong> then click <strong>Queue Setup</strong>. </li>
<li value="4"> <p>On the <strong>Queue Details</strong> sub-tab, in the drop-down menu under <strong>When someone makes a request, automatically grant</strong>, select from the following permissions levels:</p>
<ul>
<li><strong>View Access</strong> </li>
<li><strong>Contribute Access</strong> </li>
<li> <p><strong>Manage Access</strong> </p> </li>
</ul> <p>Now, when someone submits a request to the selected project, they are granted the specified permissions to the request.</p> </li>
<li value="5"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong>.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Condividere un problema

1. Individua il problema da condividere.

1. A destra del nome del problema, fai clic su **Condividi**. Viene visualizzata la finestra di dialogo **Condividi [Nome problema]**.

   ![Pulsante Condividi problema](assets/share-issue-button.png)

1. Nel campo **Concedi l&#39;accesso al problema**, inizia a digitare il nome dell&#39;utente, del team, della mansione, del gruppo o della società con cui vuoi condividere il problema, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   >
   >Puoi condividere un problema solo con utenti attivi, team, ruoli o aziende.


1. (Facoltativo) Seleziona l&#39;elenco a discesa **Chi ha accesso** e seleziona il livello di accesso del problema:

   * **Solo gli utenti invitati possono accedere a:** Solo gli utenti invitati possono accedervi (impostazione predefinita).
   * **Tutti nel sistema possono visualizzare**: tutti gli utenti del sistema possono visualizzare il problema senza un invito.

1. Fai clic sull’elenco a discesa a destra del nome dell’utente e seleziona il relativo livello di autorizzazione per questo problema:

   * **Visualizza**: l&#39;utente può esaminare e condividere il problema.
   * **Contributo**: l&#39;utente può apportare aggiornamenti, registrare informazioni, apportare modifiche minori e condividere il problema (include anche tutte le autorizzazioni di visualizzazione).
   * **Gestisci**: l&#39;utente ha accesso completo al problema senza diritti amministrativi, concessi a livello di accesso (include anche tutte le autorizzazioni di visualizzazione e di contributo).

1. (Facoltativo) Fai clic sull’icona delle opzioni avanzate accanto al livello di autorizzazione concesso per configurare autorizzazioni specifiche sul problema.

   ![Opzioni di autorizzazione avanzate configurate](assets/advanced-permission-options.png)

1. (Facoltativo) Per condividere rapidamente il problema utilizzando un collegamento, fare clic su **Copia collegamento** e quindi inoltrarlo al destinatario.

1. Fai clic su **Salva**.

## Condividi problemi in blocco

1. Passa al progetto contenente i problemi da condividere.

1. Nella scheda **Problemi** della pagina del progetto, seleziona la casella a sinistra di ciascun problema che desideri condividere, quindi fai clic sull&#39;icona **Condividi** ![Condividi icona](assets/share-icon.png) nella parte superiore della pagina. Viene visualizzata la finestra modale di condivisione.

   ![Problemi di condivisione in blocco](assets/bulk-share-issues.png)

1. Nel campo **Concedi l&#39;accesso al problema**, inizia a digitare il nome dell&#39;utente, del team, della mansione, del gruppo o della società con cui desideri condividere i problemi, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   >
   >Puoi condividere i problemi solo con utenti attivi, team, ruoli o aziende.


1. (Facoltativo) Seleziona l&#39;elenco a discesa **Chi ha accesso** e il livello di accesso dei problemi:

   * **Solo gli utenti invitati possono accedere a:** Solo gli utenti invitati possono accedervi (impostazione predefinita).
   * **Tutti gli utenti del sistema possono visualizzare**: tutti gli utenti del sistema possono visualizzare i problemi senza un invito.


1. Fai clic sull’elenco a discesa a destra del nome dell’utente e seleziona il relativo livello di autorizzazione per i problemi:

   * **Visualizza**: l&#39;utente può esaminare e condividere i problemi.
   * **Contributo**: l&#39;utente può apportare aggiornamenti, registrare informazioni, apportare modifiche minori e condividere i problemi (include anche tutte le autorizzazioni di visualizzazione).
   * **Gestisci**: l&#39;utente dispone dell&#39;accesso completo ai problemi senza diritti amministrativi, concessi a livello di accesso (include anche tutte le autorizzazioni di visualizzazione e di contributo).

1. (Facoltativo) Fai clic sull’icona delle opzioni avanzate accanto al livello di autorizzazione concesso per configurare autorizzazioni specifiche sui problemi.

   ![Opzioni di autorizzazione avanzate configurate](assets/advanced-permission-options.png)

1. Fai clic su **Salva**.

## Autorizzazioni problema

Nella tabella seguente vengono visualizzate le autorizzazioni che è possibile concedere agli utenti quando si consente loro di visualizzare, contribuire o gestire un problema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Azioni</strong> </td> 
   <td><strong>Gestisci</strong> </td> 
   <td><strong>Contribuisci</strong> </td> 
   <td><strong>Visualizza</strong> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiungi problemi</p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Elimina </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Allega modulo personalizzato</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifica campi personalizzati</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Approva problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Aggiungere Un Processo Di Approvazione</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aggiungi documenti</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Copia problema*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Sposta problema</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Registra ore</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Converti in progetto*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Accetta assegnazione</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aggiornamenti/commenti</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Modifica date pianificate</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Fai le assegnazioni</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Condividi</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Condividi a livello di sistema</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Controllato dai livelli di accesso e dalle autorizzazioni per il progetto.
