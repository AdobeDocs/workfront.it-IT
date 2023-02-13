---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Creare e modificare aziende
description: Puoi aggiungere aziende a [!DNL Workfront] e utilizzarli a scopo di pianificazione finanziaria, reporting, per definire le autorizzazioni intorno agli oggetti e per mantenere riservate le informazioni.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# Creare e modificare aziende

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Un&#39;azienda è un&#39;unità organizzativa in [!DNL Adobe Workfront] che può rappresentare la tua organizzazione, un reparto dell&#39;organizzazione o un cliente con cui lavori. Puoi aggiungere aziende a [!DNL Workfront] e utilizzarli a scopo di pianificazione finanziaria, reporting, per definire le autorizzazioni intorno agli oggetti e per mantenere riservate le informazioni.

## Requisiti di accesso

Per gestire le aziende in è necessario disporre dei seguenti elementi [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] piano*</p> </td> 
   <td>Team [!UICONTROL] o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Una delle seguenti opzioni:</p> 
    <ul> 
     <li> <p>Livello di accesso [!UICONTROL System Administrator], che consente di modificare qualsiasi azienda nel sistema. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> </li> 
     <li> <p>Accesso amministrativo alla gestione delle aziende, che consente di modificare qualsiasi azienda nel sistema. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>Puoi anche gestire le società associate a qualsiasi gruppo a cui ti viene assegnato come amministratore di gruppo.</p> </li> 
      <li> <p>Per aggiungere e rimuovere utenti dalla [!DNL Workfront] è necessario disporre di una delle seguenti caratteristiche:</p> 
       <ul> 
        <li> <p>Livello di accesso [!UICONTROL System Administrator]. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> </li> 
        <li> <p>Nel tuo livello di accesso, [!UICONTROL Edit] deve essere selezionato per l’impostazione [!UICONTROL Users]. Inoltre, per l'impostazione [!UICONTROL Users], in [!UICONTROL Ottimizza le impostazioni] <img src="assets/gear-icon-in-access-levels.png"> , l’opzione [!UICONTROL Crea] e almeno una delle due opzioni [!UICONTROL User Admin] devono essere abilitate. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Se utilizzi l’opzione [!UICONTROL User Admin (Group Users)] , devi essere un amministratore di gruppo di un gruppo in cui l’utente è membro.</p> </li> 
       </ul> <p>Per informazioni sull'impostazione Utenti in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o configurazioni del livello di accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Vantaggi dell’aggiunta di utenti a un’azienda {#benefits-of-adding-users-to-a-company}

* Puoi creare un organigramma aziendale associando gli utenti ai rapporti diretti. Solo gli utenti della stessa azienda possono essere aggiunti come rapporti diretti di un altro utente di tale azienda.
* In qualità di project manager, puoi identificare le risorse disponibili all’interno della stessa azienda.
* È possibile mantenere le informazioni private tra le aziende scegliendo una o tutte le seguenti impostazioni:

   * Gli utenti della stessa azienda possono visualizzare le richieste degli altri utenti.

      Per ulteriori informazioni su come [!DNL Workfront] l’amministratore può concedere un accesso simile alle richieste in base all’azienda degli utenti, consulta la sezione . [Configura le preferenze per le attività e i problemi per tutti gli utenti di [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) nell&#39;articolo [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

      Per ulteriori informazioni su come un amministratore di gruppo può concedere un accesso simile alle richieste in base all’azienda degli utenti, consulta [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Gli utenti possono visualizzare solo le code di richiesta associate alle proprie aziende. Per ulteriori informazioni sulla limitazione della visibilità di una coda di richiesta, consulta [Fornire l&#39;accesso alle code di richiesta](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Puoi limitare gli utenti a visualizzare solo gli utenti della loro azienda o della loro azienda e della società principale. Per informazioni sulla funzionalità principale dell&#39;azienda per quanto riguarda la privacy degli utenti, vedi [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Gli utenti possono limitare gli aggiornamenti che apportano agli elementi per renderli visibili solo agli utenti aziendali. Per ulteriori informazioni su come rendere privato un aggiornamento a un&#39;azienda, vedi [Aggiorna lavoro](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Crea o modifica una società in [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Non esiste alcun limite al numero di società che è possibile aggiungere. Tuttavia, consigliamo di limitare il numero di aziende utilizzate a causa di problemi che possono verificarsi con le autorizzazioni per gli oggetti: troppa frammentazione potrebbe interferire con la visibilità degli utenti per gli elementi di lavoro.

Per impostazione predefinita, la società associata alla tua istanza di [!DNL Workfront] è già stato creato nel [!DNL Workfront] ed è l&#39;Azienda principale della tua organizzazione. Ha lo stesso nome del tuo cliente. Per ulteriori informazioni sui clienti in [!DNL Workfront], vedi [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Per aggiungere o modificare un’azienda:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Aziende]**.
1. Se aggiungi una società, fai clic su **[!UICONTROL Nuova società]**.

   Oppure

   Se stai modificando un&#39;azienda esistente, seleziona l&#39;azienda e fai clic su **[!UICONTROL Modifica]**.

1. Utilizza le opzioni visualizzate per configurare le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sezione [!UICONTROL Informazioni di base]</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Nome società]</b>: Digita un nome per la società.</p> </li> 
        <li> <p><b>[!UICONTROL È Attivo]</b>: Quando questa opzione è abilitata, gli utenti possono trovare l’azienda e allegarla ai progetti creati e modificati. Impossibile allegare ai progetti un'azienda inattiva. Questa opzione è attivata per impostazione predefinita.</p> </li> 
        <li> <p><b>[!UICONTROL Questa è l'azienda principale]</b>: Assegna l'azienda come azienda principale dell'organizzazione. La società primaria rappresenta in genere la tua [!DNL Workfront] account in cui lavora la maggior parte degli utenti.</p> <p>Puoi avere una società o nessuna società designata come società primaria, ma non puoi avere più società designate come società primarie. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> <p><b>NOTA</b>: Modificando i rispettivi livelli di accesso, puoi limitare gli utenti alla visualizzazione di altri utenti: solo nella loro società primaria, o nella loro società associata e nella società primaria. Per informazioni sul funzionamento dell’azienda primaria con i livelli di accesso degli utenti, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: Se c'è un gruppo che conduce affari con l'azienda, è possibile aggiungere il nome del gruppo qui. Questo è utile per gli amministratori dei gruppi che devono creare rapporti e gestire tutte le aziende con cui i loro gruppi svolgono attività commerciali.</p> <p><b>IMPORTANTE</b>: Se non associ il gruppo che lavorerà con questa azienda, gli amministratori del gruppo non possono accedervi a meno che non abbiano accesso amministrativo alle aziende nel loro livello di accesso. Per informazioni su come concedere questo accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Inizia a digitare il nome del gruppo, quindi premi <strong>[!UICONTROL Enter]</strong> quando appare.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Quando assegni un gruppo a un'azienda, gli amministratori del gruppo ottengono l'accesso [!UICONTROL Gestisci] all'azienda. Per ulteriori informazioni, consulta <a href="#group-administrators-and-companies" class="MCXref xref">Amministratori di gruppo e aziende</a> in questo articolo.</p> </li> 
        <li> <p><b>[!UICONTROL Società Membri]</b>: Aggiungi utenti esistenti alla società. In questo modo, associ questi utenti a questa azienda.</p> <p>Non vi è alcun limite al numero di utenti che si associano a una società, ma un utente non può essere associato a più di una società.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sezione [!UICONTROL Billing Rates] (Tassi di fatturazione)</td> 
      <td> <p>Puoi sovrascrivere i tassi di fatturazione associati ai ruoli del lavoro a livello aziendale. Per informazioni sulla creazione di ruoli di lavoro e sull'associazione di questi con i tassi di fatturazione, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire ruoli di lavoro</a>.</p> <p>Per ulteriori informazioni sull'override delle tariffe di fatturazione a livello aziendale, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref">Escludere i tassi di fatturazione dei ruoli di lavoro a livello aziendale</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sezione [!UICONTROL Custom Forms]</td> 
      <td> <p>Se esistono campi che desideri aggiungere alla tua azienda che non sono disponibili in [!DNL Workfront], è possibile creare un modulo personalizzato e associarlo all’azienda. Puoi allegare il modulo alla tua azienda selezionandolo dal menu a discesa. Solo le società attive sono elencate nel menu a discesa. Per informazioni sulla creazione di Custom Forms, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Se stai creando una nuova società, fai clic su **[!UICONTROL Crea società]**.

   Oppure

   Se modifichi una società esistente, fai clic su **[!UICONTROL Salva modifiche]**.

## Gestire le iscrizioni aziendali

Per informazioni sulla gestione delle appartenenze per una società esistente, consulta [Gestire le iscrizioni aziendali](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Informazioni sulla condivisione di oggetti con le aziende

Alcune autorizzazioni sono disponibili per gli utenti associati a un&#39;azienda, come spiegato nella sezione . [Vantaggi dell’aggiunta di utenti a un’azienda](#benefits-of-adding-users-to-a-company). Oltre a queste autorizzazioni, puoi consentire agli utenti di accedere alle autorizzazioni per visualizzare, contribuire o modificare oggetti in [!DNL Workfront] condividendo l’oggetto con la propria azienda.

Invece di condividere un oggetto con un singolo utente alla volta, puoi condividerlo con l’intera azienda. Ogni utente della società dispone delle stesse autorizzazioni per quell&#39;oggetto.

Per ulteriori informazioni sulla condivisione degli oggetti, consulta [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Amministratori di gruppo e aziende {#group-administrators-and-companies}

Quando un [!DNL Workfront] l&#39;amministratore assegna un gruppo a una società, gli amministratori del gruppo per il guadagno del gruppo [!UICONTROL Gestisci] accesso alla società in [!UICONTROL Configurazione]. Ciò include l&#39;accesso al [!UICONTROL Aziende] in [!UICONTROL Configurazione], in cui possono visualizzare e gestire l’azienda associata al gruppo.

Con questo accesso al [!UICONTROL Aziende] un amministratore di gruppo può assegnare un gruppo a una società, ma deve essere una società creata dall&#39;amministratore del gruppo. Se il livello di accesso dell&#39;amministratore del gruppo non è configurato con accesso amministrativo alle società, il [!UICONTROL Gruppo] Il campo è obbligatorio quando l&#39;amministratore del gruppo crea l&#39;azienda; il titolo in grassetto indica quanto segue:

![](assets/manage-company-group-field-req.jpg)

Per informazioni su come gli utenti ottengono accesso amministrativo alle aziende nel loro livello di accesso, vedi [Consentire agli utenti l&#39;accesso amministrativo a determinate aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Per informazioni sulla gestione di una società nel [!UICONTROL Configurazione] area, vedere [Crea o modifica una società in [!DNL Workfront]](#create-or-edit-a-company-in-workfront) in questo articolo.
