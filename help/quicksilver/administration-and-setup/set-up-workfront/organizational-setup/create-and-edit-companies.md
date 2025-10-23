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
source-git-commit: e25ea757129e9645f7b5f0729cd498d5947f49f2
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# Creare e modificare le aziende

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambiente Sandbox di anteprima ed è in fase di rilascio in un rollout graduale in produzione.</span>

Un&#39;azienda è un&#39;unità organizzativa in [!DNL Adobe Workfront] che può rappresentare l&#39;organizzazione, un reparto all&#39;interno dell&#39;organizzazione o un cliente con cui si lavora. È possibile aggiungere società a [!DNL Workfront] e utilizzarle a scopo di pianificazione finanziaria, reporting, definire autorizzazioni per gli oggetti e mantenere riservate le informazioni.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] pacchetto</p> </td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurazione del livello di accesso</td> 
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Il livello di accesso [!UICONTROL Amministratore di sistema], che consente di modificare qualsiasi società del sistema.</p> </li> 
     <li> <p>Accesso amministrativo per gestire le società, che consente di modificare qualsiasi società nel sistema.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>Puoi anche gestire le aziende associate a qualsiasi gruppo a cui sei assegnato come amministratore di gruppo.</p> </li> 
      <li> <p>Per aggiungere e rimuovere utenti dal sistema [!DNL Workfront], è necessario disporre di uno dei seguenti elementi:</p> 
       <ul> 
        <li> <p>Livello di accesso [!UICONTROL System Administrator]. </p> </li> 
        <li> <p>Impostazione di <b>[!UICONTROL Utenti]</b> nel livello di accesso configurato per l'accesso <b>[!UICONTROL Modifica]</b>, con <b>[!UICONTROL Crea]</b> e almeno una delle due opzioni di <b>[!UICONTROL Amministratore utenti]</b> abilitate in <b>[!UICONTROL Ottimizza le impostazioni]</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Di queste due opzioni, se <b>[!UICONTROL User Admin (Group Users)]</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Aziende]**.

   Viene visualizzato un elenco di aziende.

1. Se stai aggiungendo una società, fai clic su **[!UICONTROL Nuova società]**.

   Oppure

   Se stai modificando una società esistente, selezionala e fai clic sull&#39;icona **[!UICONTROL Modifica]** ![Modifica icona](assets/edit-icon.png) nella parte superiore dell&#39;elenco delle società.

1. Aggiorna le seguenti informazioni nella sezione **Informazioni di base**:

   * **Nome società**<span class="preview"> o **Nome**</span>: digitare un nome per la società.
   * **È attivo**: quando questa opzione è abilitata, gli utenti possono trovare la società e allegarla ai progetti che creano e modificano. Una società inattiva non può essere collegata a progetti. Questa opzione è attivata per impostazione predefinita.
   * **Questa è la società principale**<span class="preview"> o **è la società principale**</span>: assegna la società come società principale della tua organizzazione. L’azienda principale in genere rappresenta l’account Workfront dove lavora la maggior parte degli utenti.

     È possibile che una sola azienda o nessuna azienda sia designata come società principale, ma non è possibile che più aziende siano designate come società principali. Per ulteriori informazioni, vedere [Creare e modificare livelli di accesso personalizzati](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

     >[!NOTE]
     >
     >Modificando i rispettivi livelli di accesso, è possibile limitare la visualizzazione agli altri utenti: solo nella società principale oppure nella società associata e nella società principale. Per informazioni sul funzionamento della società principale con i livelli di accesso degli utenti, vedere [Creare e modificare livelli di accesso personalizzati](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   * **Gruppo**: se è presente un gruppo che conduce affari con la società, è possibile aggiungere il nome del gruppo qui. Questo è utile per gli amministratori di gruppi che devono segnalare e gestire tutte le aziende con cui i loro gruppi intrattengono rapporti commerciali.

     Se non si associa il gruppo che lavorerà con questa società, gli amministratori del gruppo non potranno accedere alla società a meno che non abbiano accesso amministrativo alle società nel loro livello di accesso. Per informazioni sulle modalità di concessione dell&#39;accesso, vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

     Iniziate a digitare il nome del gruppo, quindi selezionatelo quando viene visualizzato.

     Quando si assegna un gruppo a una società, gli amministratori del gruppo ottengono l&#39;accesso Gestisci alla società. Per ulteriori informazioni, consulta [Amministratori di gruppi e società](#group-administrators-and-companies) in questo articolo.

   * **Membri società**: aggiungi utenti esistenti alla società. In questo modo, si associano questi utenti a questa azienda.

     Inizia a digitare il nome di un utente, quindi selezionalo quando viene visualizzato.

     Non esiste un limite al numero di utenti associati a una società, ma un utente non può essere associato a più società.

1. Aggiungere o aggiornare moduli personalizzati nella sezione **Forms personalizzato**.

   Se sono presenti campi che si desidera aggiungere alla società e che non sono disponibili in Workfront, è possibile creare un modulo personalizzato e associarlo alla società.

   Per allegare il modulo alla società, selezionarlo dal menu a discesa. Nel menu sono elencati solo i moduli personalizzati attivi.

   >[!NOTE]
   >
   >Le funzioni avanzate dei moduli personalizzati, ad esempio i campi di ricerca esterni e i campi nativi di Workfront, sono disponibili solo quando si apre il record aziendale nella pagina dei dettagli e non nella finestra di dialogo Modifica società. Dall’elenco delle aziende, fai clic sul nome della società per aprire i dettagli.

   Per informazioni sulla creazione di moduli personalizzati, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Condizionale) Se stai creando una società, fai clic su **[!UICONTROL Crea società]**<span class="preview">o **&#x200B; Salva &#x200B;**.</span>

   Oppure

   Se stai modificando una società esistente, fai clic su **[!UICONTROL Salva modifiche]**<span class="preview">o **&#x200B; Salva &#x200B;**.</span>

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

<!-- OLD HTML TABLE
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] section</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Type a name for the company.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>: When this option is enabled, users can find the company and attach it to projects that they create and edit. An inactive company cannot be attached to projects. This option is enabled by default.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Assigns the company as your organization's primary company. The primary company typically represents your [!DNL Workfront] account where most of your users work.</p> <p>You can have one company or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p><b>NOTE</b>: By modifying their access levels, you can restrict users to see other users: only in their primary company, or in their associated company and the primary company. For information about how the primary company works with users' access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: If there is a group that conducts business with the company, you can add the name of the group here. This is useful for group administrators who need to report on and manage all the companies that their groups do business with.</p> <p><b>IMPORTANT</b>: If you don't associate the group that will be working with this company, administrators for the group can't access the company unless they have administrative access to companies in their access level. For information about how this access is granted, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Start typing the name of the group, then press <strong>[!UICONTROL Enter]</strong> when it appears.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">When you assign a group to a company, the group administrators for the group gain [!UICONTROL Manage] access to the company. For more information, see <a href="#group-administrators-and-companies" class="MCXref xref">Group administrators and companies</a> in this article.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Add existing users to the company. By doing this, you are associating these users with this company.</p> <p>There is no limit to how many users you associate with one company, but a user cannot be associated with more than one company.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] section</td> 
      <td> <p>If there are fields that you want to add to your company that are not available in [!DNL Workfront], you can build a custom form and associate it with your company. </p> <p>You can attach this form to your company by selecting it from the drop-down menu. Only active custom forms are listed in the menu.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the company record on the details page, not on the Edit Company dialog. (From the list of companies, click the company name to open the details.)</p> <p> For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>
   -->
