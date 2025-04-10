---
title: Condividere un’attività
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: L’amministratore di Adobe Workfront può concederti l’accesso per visualizzare o modificare le attività quando assegna i livelli di accesso. Per ulteriori informazioni sulla concessione dell'accesso alle attività, vedere Concedere l'accesso alle attività.
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: b8a2fea8c1eac376f49201dc840f7a4fcc67d759
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 2%

---

# Condividere un’attività

L’amministratore di Adobe Workfront può concederti l’accesso per visualizzare o modificare le attività quando assegna i livelli di accesso. Per ulteriori informazioni sulla concessione dell&#39;accesso alle attività, vedere [Concedere l&#39;accesso alle attività](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

Oltre al livello di accesso concesso agli utenti, è possibile concedere loro le autorizzazioni per visualizzare, contribuire o gestire attività specifiche che si dispone dell&#39;accesso per condividere.

Le autorizzazioni sono specifiche per un elemento in Workfront e definiscono quali azioni è possibile eseguire su tale elemento.

## Considerazioni durante la condivisione di un’attività

Oltre alle considerazioni riportate di seguito, vedere anche [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Per impostazione predefinita, il creatore di un’attività dispone delle autorizzazioni di gestione.
* È possibile condividere le attività singolarmente oppure più attività contemporaneamente in blocco.\
  La condivisione delle attività è identica alla condivisione di altri oggetti. Per ulteriori informazioni sulla condivisione di elementi in Workfront, vedere [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* È possibile concedere le seguenti autorizzazioni a un&#39;attività: 

   * Visualizza
   * Gestire
   * Contribuisci
* Quando si condivide un&#39;attività, per impostazione predefinita gli utenti ereditano le stesse autorizzazioni per tutti gli oggetti figlio associati all&#39;attività. Ad esempio, ereditano le stesse autorizzazioni per le attività, i problemi e i documenti secondari allegati all’attività.\
  Per ulteriori informazioni sulla gerarchia degli oggetti in Workfront, consulta  [Informazioni sugli oggetti in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  L&#39;amministratore di Workfront può specificare se i documenti devono ereditare le autorizzazioni da oggetti di livello superiore nel livello di accesso dell&#39;utente. Per ulteriori informazioni sulla limitazione delle autorizzazioni ereditate sui documenti, vedere [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* È possibile rimuovere le autorizzazioni ereditate da un&#39;attività.\
  Per ulteriori informazioni sulla rimozione delle autorizzazioni ereditate dagli oggetti, vedere  [Rimuovi le autorizzazioni dagli oggetti](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Modalità di condivisione di un&#39;attività

È possibile condividere un&#39;attività nei modi seguenti:

* Manualmente, singolarmente o in blocco. La condivisione manuale delle attività è simile alla condivisione di qualsiasi altro oggetto in Workfront.

  Per ulteriori informazioni sulla condivisione di oggetti in Workfront, vedi  [Condividi un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Automaticamente, eseguendo le operazioni seguenti:

   * Specificare le autorizzazioni per uno qualsiasi degli oggetti padre dell&#39;attività: progetto, programma o portfolio. Le attività ereditano le autorizzazioni dagli oggetti padre. Per informazioni sulla visualizzazione delle autorizzazioni ereditate sugli oggetti, vedere [Visualizzare le autorizzazioni ereditate sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Aggiungere entità alla condivisione di progetto in un modello utilizzato per creare il progetto in cui si trova l&#39;attività. Per informazioni sulla condivisione di progetti da modelli, vedere [Condividere un modello](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Specifica le autorizzazioni per tutte le attività di un progetto quando lo modifichi. Per informazioni sulla gestione dell&#39;accesso alle attività del progetto in base alle autorizzazioni di un utente, vedere la sezione [](../../manage-work/projects/manage-projects/edit-projects.md#access) nell&#39;articolo [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).

  >[!TIP]
  >
  >Se non si specifica quali autorizzazioni di attività si desidera assegnare agli utenti quando vengono assegnati alle attività del progetto, per impostazione predefinita questi ricevono le stesse autorizzazioni di cui dispongono sul progetto.

## Autorizzazioni attività

Nella tabella seguente vengono visualizzate le autorizzazioni che è possibile concedere agli utenti quando si consente loro di visualizzare, contribuire o gestire un&#39;attività:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Azione</strong> </th> 
   <th><strong>Gestisci</strong> </th> 
   <th><strong>Contribuisci</strong> </th> 
   <th><strong>Visualizza</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Aggiungi attività</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aggiungi predecessori</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aggiungi problemi</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Cancella l'Attività</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>Modifica attività generale<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifica stato attività</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifica vincolo attività</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Visualizza l'Attività</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aggiungi documenti</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Copia attività*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Sposta attività*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Registra ore</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifica date pianificate</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Accetta assegnazione</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Crea un'assegnazione</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Allega modulo personalizzato</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modifica campi personalizzati</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Creare un processo di approvazione</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Approva Un'Attività</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Modifica dati finanziari*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aggiungi/Modifica spese</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Visualizza dati finanziari</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aggiornamenti/Commenti</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Condividi</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Condividi a livello di sistema</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Controllato dal livello di accesso e dalle autorizzazioni per il progetto.
