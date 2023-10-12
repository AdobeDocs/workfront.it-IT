---
title: Accedi come altro utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: In qualità di amministratore di Adobe Workfront, a volte potresti dover accedere a Workfront per conto di un altro utente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 8be7534dfc0a1227bd2274ad093a88ae19b4691d
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 0%

---

# Accedi come altro utente


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non hanno ancora effettuato l’onboarding in Adobe Admin Console. Se per la tua organizzazione è stato eseguito l’onboarding in Adobe Admin Console, questa azione non è disponibile.
>
>Per un elenco delle procedure che differiscono in base al fatto che la tua organizzazione sia stata onboarding in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

In qualità di amministratore di Adobe Workfront, a volte potresti dover accedere a Workfront per conto di un altro utente.

In alternativa, in qualità di amministratore di gruppo, potrebbe essere necessario accedere a Workfront per conto di un utente membro di un gruppo che gestisci.

Ad esempio, se un&#39;attività non può avanzare fino a quando un utente in vacanza non esegue una determinata azione, è possibile accedere come tale utente ed eseguire l&#39;azione.

<!--
<note type="note">
Some users, such as executives, need to be able to control which administrators can log in to their accounts, and for how long. Working with your organization, Workfront configures settings that allow this control for these users. When a Workfront administrator or group administrator (associated with one of the user's groups) tries to log in as one of these users, an on-screen message prompts the administrator to contact the user for access. From the user profile area, the user can then grant access to the administrator and specify an expiration time for it. For more information on how the user does this, see
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#access" class="MCXref xref">Access</a> in
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.
<span class="PinkDraftNote">[Add a note about this being only for the Enterprise package if they decide to do it that way]</span>
</note>
-->

>[!NOTE]
>
>Poiché un’integrazione di documenti può connettersi a file personali privati, gli amministratori non possono accedere alle integrazioni di documenti quando hanno effettuato l’accesso come altro utente.
>
>Per ulteriori informazioni sulle integrazioni di documenti, consulta [Configurare le integrazioni dei documenti](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Con il livello di accesso Amministratore di sistema, puoi accedere come chiunque. Per informazioni su questo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> <p>Con un livello di accesso Planner, puoi accedere come utente con un livello di licenza inferiore se <b>Utenti</b> l'impostazione nel livello di accesso è configurata su <b>Modifica</b> accesso, con <b>Crea</b> e almeno uno dei due <b>Amministratore utenti</b> opzioni abilitate in <b>Metti a punto le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>NOTA</b>: di queste due opzioni, se Utente <b>Amministratore (utenti gruppo)</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> 
   <p>Per ulteriori informazioni su <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Accedi ed esegui azioni come altro utente

1. Accedi a Workfront come amministratore di Workfront o amministratore di gruppo.

   >[!NOTE]
   >
   >* Gli amministratori di gruppi possono accedere solo come utenti dei gruppi gestiti. Inoltre, l’autorizzazione Amministratore utenti (utenti gruppo) deve essere abilitata nel tuo livello di accesso:
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  Questa impostazione è disabilitata per impostazione predefinita. Per ulteriori informazioni, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Non è possibile reimpostare la password di un amministratore Workfront.

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Accedi come**.

1. In **Utenti** casella sul **Accedi come** , inizia a digitare il nome dell’utente, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.

   L’utente deve disporre di un livello di accesso definito in Workfront. Non è possibile accedere al sistema Workfront come utente che non dispone dei diritti di accesso.

   >[!NOTE]
   >
   >Gli amministratori dei gruppi possono accedere solo come utenti membri dei gruppi che gestiscono. Non possono accedere come amministratori di Workfront.

1. Clic **Accedi.**

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Might come in a future story:</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">click an Access period and then click Request to ask the user for access to log as him or her for the specified period of time. Continue these steps after the user grants access. Specify somewhere here that this is only for the Enterprise package if they decide on that</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Or </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a prompt appears indicating that the user has restricted access to their account, contact the user to request access.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The user can then can grant you "Log in as" access in their user profile. They can also specify an expiration date and time for the access period. </p>
   -->

   <!--
   This triggers an email to let you know that you have access to log in as the user, depending on how your event notifications are enabled. For more information, see <a href="../../../workfront-basics/using-notifications/event-notifications.md" class="MCXref xref">Event notifications</a>.
   </div>
   -->

   Quando hai effettuato l’accesso come altro utente, nella parte superiore dello schermo viene visualizzata una notifica per indicare che si tratta di un’operazione.

1. Dopo aver eseguito le azioni necessarie come utente, fai clic su **Disconnetti.**

## Attività di tracciamento e controllo durante l’accesso di un amministratore come altro utente

Workfront fornisce meccanismi per il tracciamento e il controllo dell’attività che ha luogo mentre l’amministratore è connesso come altro utente.

Quando si effettua l&#39;accesso come altro utente, la data dell&#39;ultimo accesso per l&#39;utente viene modificata alla data in cui l&#39;amministratore di sistema o di gruppo effettua l&#39;accesso come tale utente.

* [Visualizza indicatori su articoli](#view-indicators-on-items)
* [Visualizzare le informazioni di audit](#view-audit-information)

### Visualizza indicatori su articoli {#view-indicators-on-items}

Quando accedi a Workfront come altro utente ed esegui un’azione, Workfront indica chiaramente che l’azione eseguita è stata eseguita da te per conto dell’utente che hai effettuato l’accesso come.

Ad esempio, se si commenta un elemento durante l&#39;accesso come altro utente, un&#39;istruzione indica che il commento è stato creato dall&#39;utente per conto dell&#39;utente.

<!--remove the note below when we bring this back to Prod: -->

>[!NOTE]
>
>Quando si utilizza la nuova esperienza di commento, il commento viene aggiunto come utente che ha effettuato l’accesso come altro utente e non vi è alcuna indicazione che stia aggiungendo un commento per conto di un altro utente.
>
>Ad esempio, se un amministratore di Workfront effettua l’accesso come altro utente, l’utente associato al commento è l’amministratore di Workfront. Per ulteriori informazioni, consulta [Nuova esperienza di commento](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


### Visualizzare le informazioni di audit {#view-audit-information}

1. Accedere a Workfront come amministratore di Workfront o amministratore di gruppo.
1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **Accedi come,** quindi fai clic su **Registro degli accessi** scheda.

   Ogni volta che un amministratore di sistema o di gruppo accede a Workfront come altro utente, l’evento viene registrato nell’audit trail. Inoltre, tutte le azioni controllabili che si verificano durante l’accesso dell’amministratore come altro utente vengono registrate nell’audit trail.

1. (Facoltativo) Puoi filtrare i risultati visualizzati nell’audit trail nei seguenti modi:

   * Per utente che ha effettuato l’accesso
   * Per utente che ha effettuato l’accesso come
   * Per data
