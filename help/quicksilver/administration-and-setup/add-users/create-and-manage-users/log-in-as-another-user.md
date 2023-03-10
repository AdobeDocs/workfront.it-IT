---
title: Accedi come altro utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: In qualità di amministratore di Adobe Workfront, a volte potrebbe essere necessario accedere a Workfront per conto di un altro utente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# Accedi come altro utente

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate in Adobe Admin Console. Se l’organizzazione è stata caricata in Adobe Admin Console, questa azione non è disponibile.
>
>Per un elenco delle procedure che variano a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

In qualità di amministratore di Adobe Workfront, a volte potrebbe essere necessario accedere a Workfront per conto di un altro utente.

In alternativa, in qualità di amministratore di gruppo, potrebbe essere necessario accedere a Workfront per conto di un utente membro di un gruppo gestito.

Ad esempio, se un&#39;attività non può avanzare finché un utente in vacanza non esegue una determinata azione, è possibile accedere come tale utente ed eseguire l&#39;azione.

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
>Poiché un’integrazione di un documento può connettersi a file personali privati, gli amministratori non possono accedere alle integrazioni di documenti quando hanno effettuato l’accesso come un altro utente.
>
>Per ulteriori informazioni sulle integrazioni di documenti, consulta [Configurare le integrazioni di documenti](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Con il livello di accesso amministratore di sistema, puoi accedere come chiunque altro. Per informazioni su questo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> <p>Con un livello di accesso Planner, puoi accedere come utente con un livello di licenza inferiore se il <b>Utenti</b> nel livello di accesso è configurata per <b>Modifica</b> accesso, con <b>Crea</b> e almeno uno dei due <b>Amministratore utente</b> opzioni attivate in <b>Ottimizzare le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>NOTA</b>: Di queste due opzioni, se Utente <b>Amministratore (utenti del gruppo)</b> è abilitato, devi essere un amministratore di gruppo di un gruppo in cui l’utente è membro.</p> 
   <p>Per ulteriori informazioni sulla <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Accedi ed esegui azioni come un altro utente

1. Accedi a Workfront come amministratore di Workfront o di gruppo.

   >[!NOTE]
   >
   >* Se sei un amministratore di gruppo, puoi accedere solo come utenti dei gruppi gestiti. Inoltre, l’autorizzazione Amministratore utenti (Utenti gruppo) deve essere abilitata nel livello di accesso:
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  Questa impostazione è disabilitata per impostazione predefinita. Per ulteriori informazioni, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Non è possibile reimpostare la password di un amministratore Workfront.


1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Accedi come**.

1. In **Utenti** nella casella **Accedi come** inizia a digitare il nome dell&#39;utente, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   L’utente deve avere un livello di accesso definito in Workfront. Non è possibile accedere al sistema Workfront come utente che non dispone dei diritti di accesso.

   >[!NOTE]
   >
   >Gli amministratori dei gruppi possono accedere solo quando gli utenti sono membri dei gruppi gestiti. Non possono accedere come amministratore di Workfront.

1. Fai clic su **Accedi.**

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

   Quando hai effettuato l’accesso come un altro utente, nella parte superiore della schermata viene visualizzata una notifica per indicarlo.

1. Dopo aver eseguito le azioni necessarie come utente, fai clic su **Esci.**

## Tracciamento e controllo dell’attività mentre un amministratore ha effettuato l’accesso come un altro utente

Workfront fornisce meccanismi per il tracciamento e il controllo delle attività che si verificano mentre l’amministratore ha effettuato l’accesso come un altro utente.

Quando si effettua l&#39;accesso come un altro utente, l&#39;ultima data di accesso viene modificata per tale utente alla data in cui l&#39;amministratore di sistema o di gruppo effettua l&#39;accesso come utente.

* [Visualizza gli indicatori degli elementi](#view-indicators-on-items)
* [Visualizza informazioni sul controllo di audit](#view-audit-information)

### Visualizza gli indicatori degli elementi {#view-indicators-on-items}

Quando accedi a Workfront come altro utente ed esegui un&#39;azione, Workfront indica chiaramente che qualsiasi azione esegui è eseguita da te a nome dell&#39;utente con cui hai effettuato l&#39;accesso.

Ad esempio, se commentate un elemento durante l’accesso come un altro utente, un’istruzione indica che il commento è stato effettuato da voi per conto dell’utente.

### Visualizza informazioni sul controllo di audit {#view-audit-information}

1. Accedi a Workfront come amministratore Workfront o amministratore di gruppo.
1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Accedi come,** quindi fai clic su **Registro di accesso** scheda .

   Ogni volta che un amministratore di sistema o di gruppo accede a Workfront come un altro utente, l’evento viene registrato nell’audit trail. Inoltre, tutte le azioni verificabili che avvengono durante l&#39;accesso dell&#39;amministratore quando un altro utente ha effettuato l&#39;accesso nell&#39;audit trail.

1. (Facoltativo) Puoi filtrare i risultati visualizzati nella traccia di audit nei seguenti modi:

   * Utente che ha effettuato l&#39;accesso
   * Per utente che ha effettuato l’accesso come
   * Per data
