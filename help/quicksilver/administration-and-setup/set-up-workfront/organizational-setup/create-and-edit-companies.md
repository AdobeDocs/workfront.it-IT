---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Creare e modificare le società
description: È possibile aggiungere società a  [!DNL Adobe Workfront]  e utilizzarle a scopo di pianificazione finanziaria, reporting, definire autorizzazioni per gli oggetti e mantenere riservate le informazioni.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1472'
ht-degree: 0%

---

# Creare e modificare le società

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Un&#39;azienda è un&#39;unità organizzativa in [!DNL Adobe Workfront] che può rappresentare l&#39;organizzazione, un reparto all&#39;interno dell&#39;organizzazione o un cliente con cui si lavora. È possibile aggiungere società a [!DNL Workfront] e utilizzarle a scopo di pianificazione finanziaria, reporting, definire autorizzazioni per gli oggetti e mantenere riservate le informazioni.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per gestire le società in [!DNL Workfront] è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] piano</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td><p>Corrente: [!UICONTROL Plan]</p>
   Oppure
   <p>Nuovo: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Il livello di accesso [!UICONTROL Amministratore di sistema], che consente di modificare qualsiasi società del sistema. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
     <li> <p>Accesso amministrativo per gestire le società, che consente di modificare qualsiasi società nel sistema. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md">Concedere agli utenti l'accesso amministrativo ad alcune aree</a>.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>Puoi anche gestire le aziende associate a qualsiasi gruppo a cui sei assegnato come amministratore di gruppo.</p> </li> 
      <li> <p>Per aggiungere e rimuovere utenti dal sistema [!DNL Workfront], è necessario disporre di uno dei seguenti elementi:</p> 
       <ul> 
        <li> <p>Livello di accesso [!UICONTROL System Administrator]. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
        <li> <p>Nel livello di accesso, è necessario selezionare [!UICONTROL Edit] per l'impostazione [!UICONTROL Users]. Inoltre, per l'impostazione [!UICONTROL Users], in [!UICONTROL Ottimizza le impostazioni] <img src="assets/gear-icon-in-access-levels.png">, è necessario abilitare l'opzione [!UICONTROL Create] e almeno una delle due opzioni [!UICONTROL User Admin]. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Se si utilizza l'opzione [!UICONTROL User Admin (Group Users)], è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> </li> 
       </ul> <p>Per informazioni sull'impostazione Utenti in un livello di accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l'accesso agli utenti</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sulle configurazioni di piano, tipo di licenza o livello di accesso disponibili, contattare l&#39;amministratore [!DNL Workfront]. Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vantaggi dell’aggiunta di utenti a un’azienda {#benefits-of-adding-users-to-a-company}

* È possibile creare un organigramma aziendale associando gli utenti ai referenti diretti. Solo gli utenti della stessa azienda possono essere aggiunti come report diretti di un altro utente della stessa azienda.
* In qualità di project manager, puoi identificare le risorse disponibili all’interno della stessa azienda.
* È possibile mantenere private le informazioni tra società scegliendo una o tutte le impostazioni seguenti:

   * Gli utenti della stessa azienda possono vedere le richieste degli altri.

     Per ulteriori informazioni su come un amministratore di [!DNL Workfront] può concedere un accesso simile alle richieste in base alla società degli utenti, vedere la sezione [Configurare le preferenze per attività e problemi per tutti gli utenti di  [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) nell&#39;articolo [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Per ulteriori informazioni su come un amministratore di gruppo può concedere un accesso simile alle richieste in base alla società degli utenti, vedi [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Gli utenti possono visualizzare solo le code di richieste associate alle proprie società. Per ulteriori informazioni sulla limitazione della visibilità di una coda di richieste, vedere [Fornire accesso alle code di richieste](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Puoi limitare gli utenti affinché vedano solo gli utenti della loro azienda o della loro azienda e dell’azienda principale. Per informazioni sulle funzionalità aziendali principali relative alla privacy degli utenti, vedere [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Gli utenti possono limitare gli aggiornamenti che apportano agli elementi affinché siano visibili solo agli utenti della propria azienda. Per ulteriori informazioni su un aggiornamento privato per un&#39;azienda, vedere [Aggiorna lavoro](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Crea o modifica una società in [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Non esiste alcun limite al numero di aziende che è possibile aggiungere. Tuttavia, si consiglia di limitare il numero di aziende utilizzate a causa di problemi che possono verificarsi con le autorizzazioni degli oggetti. Una frammentazione eccessiva potrebbe interferire con la visibilità degli utenti agli elementi di lavoro.

Per impostazione predefinita, la società associata all&#39;istanza di [!DNL Workfront] è già creata nel sistema [!DNL Workfront] ed è la società principale della tua organizzazione. Ha lo stesso nome del nome del cliente. Per ulteriori informazioni sulle informazioni sui clienti in [!DNL Workfront], vedere [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Per aggiungere o modificare una società:

{#step-1-to-setup}

1. Fai clic su **[!UICONTROL Aziende]**.

   Viene visualizzato un elenco di aziende.
1. Se stai aggiungendo una società, fai clic su **[!UICONTROL Nuova società]**.

   Oppure

   Se stai modificando una società esistente, selezionala e fai clic su **[!UICONTROL Modifica]** in alto nell&#39;elenco delle società.

1. Aggiorna le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sezione [!UICONTROL Informazioni di base]</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Nome società]</b>: digitare un nome per la società.</p> </li> 
        <li> <p><b>[!UICONTROL è attivo]</b>: quando questa opzione è abilitata, gli utenti possono trovare la società e allegarla ai progetti che creano e modificano. Una società inattiva non può essere collegata a progetti. Questa opzione è attivata per impostazione predefinita.</p> </li> 
        <li> <p><b>[!UICONTROL Questa è la società principale]</b>: assegna la società come società principale della tua organizzazione. La società principale rappresenta in genere l'account [!DNL Workfront] in cui lavora la maggior parte degli utenti.</p> <p>È possibile che una sola azienda o nessuna azienda sia designata come società principale, ma non è possibile che più aziende siano designate come società principali. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> <p><b>NOTA</b>: modificando i livelli di accesso, è possibile limitare la visualizzazione ad altri utenti: solo nella società principale o nella società associata e nella società principale. Per informazioni sul funzionamento della società principale con i livelli di accesso degli utenti, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: se è presente un gruppo che conduce affari con la società, è possibile aggiungere il nome del gruppo qui. Questo è utile per gli amministratori di gruppi che devono segnalare e gestire tutte le aziende con cui i loro gruppi intrattengono rapporti commerciali.</p> <p><b>IMPORTANTE</b>: se non si associa il gruppo che lavorerà con questa società, gli amministratori del gruppo non potranno accedere alla società a meno che non abbiano accesso amministrativo alle società nel loro livello di accesso. Per informazioni sulle modalità di concessione dell'accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo ad alcune aree</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Inizia a digitare il nome del gruppo, quindi premi <strong>[!UICONTROL Invio]</strong> quando viene visualizzato.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Quando si assegna un gruppo a una società, gli amministratori del gruppo del gruppo ottengono l'accesso [!UICONTROL Gestisci] alla società. Per ulteriori informazioni, consulta <a href="#group-administrators-and-companies" class="MCXref xref">Amministratori di gruppi e società</a> in questo articolo.</p> </li> 
        <li> <p><b>[!UICONTROL Membri società]</b>: aggiungi utenti esistenti alla società. In questo modo, si associano questi utenti a questa azienda.</p> <p>Non esiste un limite al numero di utenti associati a una società, ma un utente non può essere associato a più società.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Sezione [!UICONTROL Custom Forms]</td> 
      <td> <p>Se sono presenti campi che si desidera aggiungere alla società non disponibili in [!DNL Workfront], è possibile creare un modulo personalizzato e associarlo alla società. </p> <p>Per allegare il modulo alla società, selezionarlo dal menu a discesa. Nel menu sono elencati solo i moduli personalizzati attivi.</p> <p><strong>Nota:</strong> le caratteristiche avanzate dei moduli personalizzati, ad esempio i campi di ricerca esterna e i campi nativi di Workfront, sono disponibili solo quando si apre il record della società nella pagina dei dettagli e non nella finestra di dialogo Modifica società. Dall’elenco delle aziende, fai clic sul nome della società per aprire i dettagli.</p> <p> Per informazioni sulla creazione di moduli personalizzati, vedere <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>

1. (Condizionale) Se stai creando una società, fai clic su **[!UICONTROL Crea società]**.

   Oppure

   Se stai modificando una società esistente, fai clic su **[!UICONTROL Salva modifiche]**.

## Gestire le appartenenze a società

Per informazioni sulla gestione delle appartenenze per una società esistente, vedere [Gestire le appartenenze a società](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Gestione tariffe di fatturazione

Per informazioni sulla sostituzione delle tariffe di fatturazione a livello aziendale, vedere [Sostituire le tariffe di fatturazione dei ruoli a livello aziendale](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Panoramica sulla condivisione di oggetti con le aziende

Alcune autorizzazioni sono disponibili per gli utenti associati a un&#39;azienda, come spiegato nella sezione [Vantaggi dell&#39;aggiunta di utenti a un&#39;azienda](#benefits-of-adding-users-to-a-company). Oltre a queste autorizzazioni, è possibile consentire agli utenti di visualizzare, contribuire o modificare oggetti in [!DNL Workfront] condividendo l&#39;oggetto con la propria società.

Anziché condividere un oggetto con un singolo utente alla volta, è possibile condividerlo con l&#39;intera azienda. Ogni utente dell’azienda dispone delle stesse autorizzazioni per tale oggetto.

Per ulteriori informazioni sulla condivisione degli oggetti, vedere [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Amministratori di gruppi e società {#group-administrators-and-companies}

Quando un amministratore [!DNL Workfront] assegna un gruppo a una società, gli amministratori del gruppo ottengono l&#39;accesso [!UICONTROL Gestione] alla società in [!UICONTROL Configurazione]. Ciò include l&#39;accesso alla pagina [!UICONTROL Aziende] in [!UICONTROL Configurazione], in cui possono visualizzare e gestire la società associata al loro gruppo.

Con questo accesso alla pagina [!UICONTROL Società], un amministratore di gruppo può assegnare un gruppo a una società, ma deve trattarsi di una società creata dall&#39;amministratore del gruppo. Se il livello di accesso dell&#39;amministratore del gruppo non è configurato con accesso amministrativo alle società, il campo [!UICONTROL Gruppo] è obbligatorio quando l&#39;amministratore del gruppo crea la società. Il titolo in grassetto indica quanto segue:

![Modifica società](assets/group-admin-add-company.png)

Per informazioni su come gli utenti ottengono l&#39;accesso amministrativo alle aziende nel loro livello di accesso, vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Per informazioni sulla gestione di una società nell&#39;area [!UICONTROL Configurazione], vedere [Creare o modificare una società in [!DNL Workfront]](#create-or-edit-a-company-in-workfront) in questo articolo.
