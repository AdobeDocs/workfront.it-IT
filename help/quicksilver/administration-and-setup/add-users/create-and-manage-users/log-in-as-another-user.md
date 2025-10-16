---
title: Accedi come altro utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: In qualità di amministratore di Adobe Workfront, a volte potresti dover accedere a Workfront per conto di un altro utente.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: f8d04790caefd12c9811ea3ed94e1f892311d031
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Accedere come un altro utente

<!--Audited: 5/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

In qualità di amministratore di Adobe Workfront, a volte potresti dover accedere a Workfront per conto di un altro utente. In alternativa, in qualità di amministratore di gruppo, potrebbe essere necessario accedere a Workfront per conto di un utente membro di un gruppo che gestisci.

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
>Per ulteriori informazioni sulle integrazioni dei documenti, vedere [Configurare le integrazioni dei documenti](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td>
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td> 
  </tr>
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Livello di accesso Amministratore di sistema. Questo ti consente di accedere come qualsiasi altro utente.</li> 
     <li> <p>Impostazione di <b>Utenti</b> nel livello di accesso configurato per l'accesso di <b>Modifica</b>, con <b>Crea</b> e almeno una delle due opzioni di <b>Amministratore utenti</b> abilitate in <b>Ottimizza le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. Questo consente di accedere come utente con un livello di licenza inferiore. </p> <p>Di queste due opzioni, se <b>User Admin (Group Users)</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Accedi ed esegui azioni come altro utente

1. Accedere a Workfront come amministratore di Workfront o amministratore di gruppo.

   >[!NOTE]
   >
   >* Gli amministratori di gruppi possono accedere solo come utenti dei gruppi gestiti. Inoltre, l’autorizzazione Amministratore utenti (utenti gruppo) deve essere abilitata nel tuo livello di accesso:
   >   
   >  ![Utente amministratore gruppo](assets/group-admin-user.png)
   >   
   >  Questa impostazione è disabilitata per impostazione predefinita. Per ulteriori informazioni, vedere [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Non è possibile reimpostare la password di un amministratore Workfront.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Accedi come**.

1. Nella casella **Inizia a digitare il nome...** della scheda **Accedi come**, inizia a digitare il nome dell&#39;utente, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.


   >[!NOTE]
   >* L&#39;utente selezionato deve disporre di un livello di accesso definito in Workfront. Non è possibile accedere al sistema Workfront come utente che non dispone dei diritti di accesso.
   >* Gli amministratori dei gruppi possono accedere solo come utenti membri dei gruppi che gestiscono. Non possono accedere come amministratori di Workfront.

1. Fare clic su **Accedi**. Hai effettuato l’accesso come altro utente e nella parte superiore dello schermo viene visualizzata una notifica che indica questo.

   <!--
   <p> Might come in a future story:</p>
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



1. Dopo aver eseguito le azioni necessarie come utente, fai clic su **Disconnetti** nella parte superiore della schermata.

## Attività di tracciamento e controllo durante l’accesso di un amministratore come altro utente

Workfront fornisce meccanismi per il tracciamento e il controllo dell’attività che ha luogo mentre l’amministratore è connesso come altro utente.

Quando si effettua l&#39;accesso come altro utente, la data dell&#39;ultimo accesso per tale utente viene modificata in corrispondenza della data in cui l&#39;amministratore di sistema o di gruppo effettua l&#39;accesso come tale utente.

* [Visualizza indicatori sugli elementi](#view-indicators-on-items)
* [Visualizzare le informazioni di audit](#view-audit-information)

### Visualizza indicatori su articoli {#view-indicators-on-items}

Quando accedi a Workfront come altro utente ed esegui un’azione, Workfront indica chiaramente che l’azione eseguita è stata eseguita da te per conto dell’utente che hai effettuato l’accesso come.

Ad esempio, se si commenta un elemento durante l&#39;accesso come altro utente, un&#39;istruzione indica che il commento è stato fatto da te per conto dell&#39;utente durante la visualizzazione della sezione Aggiornamenti di un oggetto.

### Visualizzare le informazioni di audit {#view-audit-information}

1. Accedere a Workfront come amministratore di Workfront o amministratore di gruppo.
   {{step-1-to-setup}}
   <!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

1. Nel pannello a sinistra, fai clic su **Accedi come**, quindi fai clic sulla scheda **Registro di accesso**.

   >[!NOTE]
   >
   >Ogni volta che un amministratore di sistema o di gruppo accede a Workfront come altro utente, l’evento viene registrato nell’audit trail. Inoltre, tutte le azioni controllabili che si verificano durante l’accesso dell’amministratore come altro utente vengono registrate nell’audit trail.

1. (Facoltativo) Puoi filtrare i risultati visualizzati nell’audit trail nei seguenti modi:

   * Per utente che ha effettuato l’accesso
   * Per utente che ha effettuato l’accesso come
   * Per data e ora
