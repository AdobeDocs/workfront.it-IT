---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Creare e modificare le società
description: Puoi aggiungere aziende a [!DNL Workfront] e utilizzarli a scopo di pianificazione finanziaria, reporting, definizione di autorizzazioni relative agli oggetti e per mantenere riservate le informazioni.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '1406'
ht-degree: 0%

---

# Creare e modificare le società

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Un’azienda è un’unità organizzativa in [!DNL Adobe Workfront] che può rappresentare la tua organizzazione, un reparto all’interno dell’organizzazione o un cliente con cui lavori. Puoi aggiungere aziende a [!DNL Workfront] e utilizzarli a scopo di pianificazione finanziaria, reporting, definizione di autorizzazioni relative agli oggetti e per mantenere riservate le informazioni.

## Requisiti di accesso

Per gestire le aziende in è necessario disporre dei seguenti elementi [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] piano*</p> </td> 
   <td>[!UICONTROL Team] o versione successiva</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Il livello di accesso [!UICONTROL Amministratore di sistema], che consente di modificare qualsiasi società del sistema. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
     <li> <p>Accesso amministrativo per gestire le società, che consente di modificare qualsiasi società nel sistema. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>Puoi anche gestire le aziende associate a qualsiasi gruppo a cui sei assegnato come amministratore di gruppo.</p> </li> 
      <li> <p>Per aggiungere e rimuovere utenti da [!DNL Workfront] di sistema, è necessario disporre di uno dei seguenti elementi:</p> 
       <ul> 
        <li> <p>Livello di accesso [!UICONTROL System Administrator]. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
        <li> <p>Nel livello di accesso, è necessario selezionare [!UICONTROL Edit] per l'impostazione [!UICONTROL Users]. Inoltre, per l'impostazione [!UICONTROL Users], in [!UICONTROL Ottimizzare le impostazioni] <img src="assets/gear-icon-in-access-levels.png"> , l'opzione [!UICONTROL Create] e almeno una delle due opzioni [!UICONTROL User Admin] devono essere abilitate. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Se si utilizza l'opzione [!UICONTROL User Admin (Group Users)], è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> </li> 
       </ul> <p>Per informazioni sull'impostazione Utenti in un livello di accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sulle configurazioni di piano, tipo di licenza o livello di accesso disponibili, contattare il [!DNL Workfront] amministratore.

## Vantaggi dell’aggiunta di utenti a un’azienda {#benefits-of-adding-users-to-a-company}

* È possibile creare un organigramma aziendale associando gli utenti ai referenti diretti. Solo gli utenti della stessa azienda possono essere aggiunti come report diretti di un altro utente della stessa azienda.
* In qualità di project manager, puoi identificare le risorse disponibili all’interno della stessa azienda.
* È possibile mantenere private le informazioni tra società scegliendo una o tutte le impostazioni seguenti:

   * Gli utenti della stessa azienda possono vedere le richieste degli altri.

     Per ulteriori informazioni su come [!DNL Workfront] L’amministratore può concedere un accesso simile alle richieste in base alla società degli utenti, consulta la sezione [Configurare le preferenze per attività e problemi per tutti gli utenti in [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) nell’articolo [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Per ulteriori informazioni su come un amministratore gruppo può concedere un accesso simile alle richieste in base alla società degli utenti, consulta [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Gli utenti possono visualizzare solo le code di richieste associate alle proprie società. Per ulteriori informazioni sulla limitazione della visibilità di una coda di richieste, consulta [Fornire l’accesso alle code di richieste](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Puoi limitare gli utenti affinché vedano solo gli utenti della loro azienda o della loro azienda e dell’azienda principale. Per informazioni sulla funzionalità aziendale principale relativa alla privacy degli utenti, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Gli utenti possono limitare gli aggiornamenti che apportano agli elementi affinché siano visibili solo agli utenti della propria azienda. Per ulteriori informazioni su come rendere un aggiornamento privato per un’azienda, consulta [Aggiorna lavoro](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Creare o modificare un’azienda in [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Non esiste alcun limite al numero di aziende che è possibile aggiungere. Tuttavia, si consiglia di limitare il numero di aziende utilizzate a causa di problemi che possono verificarsi con le autorizzazioni degli oggetti. Una frammentazione eccessiva potrebbe interferire con la visibilità degli utenti agli elementi di lavoro.

Per impostazione predefinita, l’azienda associata all’istanza di [!DNL Workfront] è già stato creato in [!DNL Workfront] ed è l&#39;azienda principale della tua organizzazione. Ha lo stesso nome del nome del cliente. Per ulteriori informazioni sulle informazioni sui clienti in [!DNL Workfront], vedi [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Per aggiungere o modificare una società:

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Aziende]**.
1. Se stai aggiungendo una società, fai clic su **[!UICONTROL Nuova società]**.

   Oppure

   Se stai modificando una società esistente, selezionala e fai clic su **[!UICONTROL Modifica]**.

1. Utilizza le opzioni visualizzate per configurare le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sezione [!UICONTROL Informazioni di base]</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Nome società]</b>: digita un nome per la società.</p> </li> 
        <li> <p><b>[!UICONTROL È Attivo]</b>: quando questa opzione è abilitata, gli utenti possono trovare la società e allegarla ai progetti che creano e modificano. Una società inattiva non può essere collegata a progetti. Questa opzione è attivata per impostazione predefinita.</p> </li> 
        <li> <p><b>[!UICONTROL È la società principale]</b>: assegna la società come società principale della tua organizzazione. L'azienda principale in genere rappresenta [!DNL Workfront] dell'account in cui lavora la maggior parte degli utenti.</p> <p>È possibile che una sola azienda o nessuna azienda sia designata come società principale, ma non è possibile che più aziende siano designate come società principali. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> <p><b>NOTA</b>: modificando i rispettivi livelli di accesso, puoi limitare la visualizzazione agli altri utenti: solo nella società principale, oppure nella società associata e nella società principale. Per informazioni sul funzionamento della società principale con i livelli di accesso degli utenti, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: se esiste un gruppo che conduce affari con l’azienda, puoi aggiungere il nome del gruppo qui. Questo è utile per gli amministratori di gruppi che devono segnalare e gestire tutte le aziende con cui i loro gruppi intrattengono rapporti commerciali.</p> <p><b>IMPORTANTE</b>: se non associ il gruppo che lavorerà con questa società, gli amministratori del gruppo non possono accedere a meno che non abbiano accesso amministrativo alle società nel loro livello di accesso. Per informazioni sulle modalità di concessione dell’accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo a determinate aree</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Inizia a digitare il nome del gruppo, quindi premi <strong>[!UICONTROL INVIO]</strong> quando viene visualizzato.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Quando si assegna un gruppo a una società, gli amministratori del gruppo del gruppo ottengono l'accesso [!UICONTROL Gestisci] alla società. Per ulteriori informazioni, consulta <a href="#group-administrators-and-companies" class="MCXref xref">Amministratori di gruppi e società</a> in questo articolo.</p> </li> 
        <li> <p><b>[!UICONTROL Membri società]</b>: aggiungi utenti esistenti all’azienda. In questo modo, si associano questi utenti a questa azienda.</p> <p>Non esiste un limite al numero di utenti associati a una società, ma un utente non può essere associato a più società.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Sezione [!UICONTROL Custom Forms]</td> 
      <td> <p>Se sono presenti campi che desideri aggiungere alla tua azienda che non sono disponibili in [!DNL Workfront], è possibile creare un modulo personalizzato e associarlo all'azienda. Per allegare il modulo alla società, selezionarlo dal menu a discesa. Nel menu a discesa sono elencate solo le società attive. Per informazioni sulla creazione di Forms personalizzati, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Se stai creando una nuova società, fai clic su **[!UICONTROL Crea società]**.

   Oppure

   Se stai modificando una società esistente, fai clic su **[!UICONTROL Salva modifiche]**.

## Gestire le appartenenze a società

Per informazioni sulla gestione delle appartenenze per una società esistente, vedere [Gestire le appartenenze a società](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Gestione tariffe di fatturazione

Per informazioni sulla sostituzione delle tariffe di fatturazione a livello aziendale, consulta [Sostituisci le tariffe di fatturazione dei ruoli a livello aziendale](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Informazioni sulla condivisione di oggetti con le aziende

Alcune autorizzazioni sono disponibili per gli utenti associati a un’azienda, come spiegato nella sezione [Vantaggi dell’aggiunta di utenti a un’azienda](#benefits-of-adding-users-to-a-company). Oltre a queste autorizzazioni, puoi consentire agli utenti di visualizzare, contribuire o modificare oggetti in [!DNL Workfront] condividendo l’oggetto con la propria azienda.

Anziché condividere un oggetto con un singolo utente alla volta, è possibile condividerlo con l&#39;intera azienda. Ogni utente dell’azienda dispone delle stesse autorizzazioni per tale oggetto.

Per ulteriori informazioni sulla condivisione degli oggetti, vedere [Panoramica delle autorizzazioni di condivisione sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Amministratori di gruppi e società {#group-administrators-and-companies}

Quando un [!DNL Workfront] l’amministratore assegna un gruppo a una società, gli amministratori del gruppo per il guadagno del gruppo [!UICONTROL Gestisci] accesso all’azienda in [!UICONTROL Configurazione]. Ciò include l&#39;accesso a [!UICONTROL Aziende] pagina in [!UICONTROL Configurazione], in cui possono visualizzare e gestire l’azienda associata al loro gruppo.

Con questo accesso alla [!UICONTROL Aziende] , un amministratore gruppo può assegnare un gruppo a una società, ma deve trattarsi di una società creata dall&#39;amministratore gruppo. Se il livello di accesso dell&#39;amministratore del gruppo non è configurato con l&#39;accesso amministrativo alle società, [!UICONTROL Gruppo] Questo campo è obbligatorio quando l’amministratore del gruppo crea la società: il suo titolo in grassetto indica che:

![](assets/manage-company-group-field-req.jpg)

Per informazioni su come gli utenti ottengono l’accesso amministrativo alle aziende nel loro livello di accesso, consulta [Concedere agli utenti l&#39;accesso amministrativo a determinate aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Per informazioni sulla gestione di un&#39;azienda in [!UICONTROL Configurazione] area, vedi [Creare o modificare un’azienda in [!DNL Workfront]](#create-or-edit-a-company-in-workfront) in questo articolo.
