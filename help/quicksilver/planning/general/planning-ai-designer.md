---
title: Guida introduttiva di Adobe Workfront Planning Designer
description: Puoi utilizzare Adobe Planning Designer basato sull’intelligenza artificiale per configurare facilmente le aree di lavoro e le strutture di dati. Il Designer di Planning supporta tutte le operazioni, dalla creazione e configurazione delle aree di lavoro alla definizione di campi e formule, alla gestione dei record, alla revisione della cronologia delle modifiche e alla creazione di viste personalizzate. Sia che venga utilizzato direttamente o tramite l'Assistente di intelligenza artificiale, Planning Designer offre un ambiente flessibile e potente per la creazione e la manutenzione di informazioni strutturate e connesse.
recommendations: noDisplay, noCatalog
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
exl-id: ba7a4b04-5faa-41b6-86d0-4d0ce946ad1e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YZRzcl8ymUo85jplCgKOx-qI83Gqa4CUI6saxfijtec
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 184cff4f2ebf8a1343d784936f10c902e350c134
workflow-type: tm+mt
source-wordcount: 1386
ht-degree: 6%

---

# Introduzione a Adobe Workfront Planning Designer

<!--remove the Beta tags in the screen shots on this page when this is released to GA - maybe March 2, 2026-->

>[!IMPORTANT]
>
>Il Designer di Planning è attualmente disponibile per tutti i clienti in uno stato Beta.
>
>Le informazioni contenute in questo articolo si riferiscono alla Pianificazione di Adobe Workfront, una funzionalità aggiuntiva di Adobe Workfront.
>
>Per un elenco dei requisiti per accedere alla Pianificazione di Workfront, consulta [Panoramica dell’accesso alla Pianificazione di Adobe Workfront](/help/quicksilver/planning/access/access-overview.md).
> 
>Per informazioni generali su Workfront Planning, vedere [Introduzione ad Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Puoi utilizzare Adobe Planning Designer basato sull’intelligenza artificiale per configurare facilmente le aree di lavoro e le strutture di dati. Il Designer di Planning supporta tutte le operazioni, dalla creazione e configurazione delle aree di lavoro alla definizione di campi e formule, alla gestione dei record, alla revisione della cronologia delle modifiche e alla creazione di viste personalizzate.

Sia che venga utilizzato direttamente o tramite l&#39;Assistente di intelligenza artificiale, Planning Designer offre un ambiente flessibile e potente per la creazione e la manutenzione di informazioni strutturate e connesse.

Per informazioni su Workfront Planning, vedere gli articoli seguenti:

* [Indice articolo e informazioni generali per Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Introduzione alla Pianificazione di Adobe Workfront](/help/quicksilver/planning/general/planning-overview.md)
* [Panoramica sull’accesso a Pianificazione di Adobe Workfront](/help/quicksilver/planning/access/access-overview.md)


## Requisiti di accesso <!--edit theses??-->

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetti Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront e Planning</p>
<p>Qualsiasi pacchetto di Workflow e Planning</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Standard</p> 
   <p>L'amministratore di sistema deve abilitare Planning Designer per l'organizzazione</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  
   </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Abilitare Planning Designer per l&#39;organizzazione

In qualità di amministratore di sistema, è possibile attivare Planning Beta per l&#39;organizzazione. Dopo l&#39;attivazione di questa impostazione, tutti gli utenti dell&#39;istanza di Workfront potranno visualizzare le funzionalità di Planning Designer nella propria area Planning.

1. Accedi come amministratore Workfront in Workfront.
1. Fai clic sull&#39;icona **Main Menu** ![Main Menu](assets/main-menu-shell.png), quindi fai clic su **Setup**.
1. Vai a **Sistema** > **Preferenze** > **Preferenze AI**.
1. Attiva **Abilita IA**<!--and ensure you have a signed Gen AI Agreement with Adobe-->.
   <!--1. Turn on the **Opt in to AI Beta** setting.-->
1. Attivare l&#39;impostazione **Planning Designer**.
   <!-- add new screenshot-->
   ![Impostazione di Planning Designer nelle preferenze di sistema](assets/planning-designer-toggle-in-system-preferences.png)

1. Fai clic su **Salva**.

   Le funzionalità di Planning Designer per la creazione o la modifica delle aree di lavoro sono ora disponibili per tutti gli utenti dell&#39;organizzazione che possono accedere a Planning.

<!--

## Turn off the Planing Designer for your organization

After your Workfront administrator accepts the AI Assistant agreement, the Planning Designer is turned on for everyone in your organization, by default. 

To turn it off: 

1. Log in to Workfront as a System Administrator. 
1. Click **Main Menu** ![Main menu icon](assets/main-menu-shell.png) in the upper-left corner of the screen, then click **Setup**.
1. Click **System** >  in the left panel, then go to the **AI preferences** area.
1. Turn off the **Planning Onboarding** setting.
1. Click **Save**.

    This removes the Planning Designer for all users in the system.

-->

<!--

## Enroll in the Closed Beta program for the Planning Designer

Currently, you can request to participate in the Closed Beta program for the Planning Designer by sending us an email to sargism@adobe.com.

After we receive the email, our Engineering team will turn on the Planning Designer in your Workfront instance. 

>[!IMPORTANT]
>
>Your company must first accept the AI Assistant agreement before the Planning Designer is available in your system. 

-->

## Invia feedback sul Designer di Planning

È possibile inviare un feedback sul Designer di pianificazione durante il programma beta.

1. Accedi a Workfront, quindi fai clic sull&#39;icona **Main Menu** ![Lines main menu](assets/lines-main-menu.png) in alto a sinistra, quindi fai clic su **Planning**.

   Verrà aperta l&#39;area **Planning**.

1. Fai clic su **Crea con IA**. <!--update this tag name when they change it-->

   Viene visualizzata la finestra **Planning Designer**.

1. Fai clic **Invia feedback qui** nella parte inferiore della pagina.
1. Aggiungi il tuo feedback nello spazio fornito, quindi fai clic su **Invia**.
Il tuo feedback viene inviato ai team tecnici e di prodotto.

## Considerazioni sul Designer di Planning

* Non è necessario abilitare il contratto di intelligenza artificiale prima di poter accedere al Designer di Planning.

<!--* You must sign the Beta agreement to access the Planning Designer.-->

<!--
Sargis and Ashot  said these are not required: 

* To use the Planning Designer, you first need to enable AI for your organization. The following must be in place for the AI features to be available to everyone in your organization:

    * Workfront must make the AI features available for your organization.

        For details, see [Prerequisites to AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).
    * After Workfront makes the AI features available for your organization, the main Workfront administrator can access it. 

        For information, see [Configure basic information for your system](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md). 
    * The Workfront administrator must accept the Gen AI agreement, and then turn on AI and the Planning Designer for your organization. 

        For more information, see [Enable or disable AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md). 

-->

* L&#39;amministratore di Workfront deve attivare il Designer di Planning per l&#39;organizzazione. In seguito, il Designer di Planning sarà disponibile per tutti gli utenti per impostazione predefinita.
* Le azioni eseguite dal Designer di Planning possono essere eseguite anche dall&#39;Assistente IA, quando lo si utilizza nell&#39;area Pianificazione, se l&#39;organizzazione ha firmato il contratto di IA.
* Le azioni eseguite dall&#39;Assistente IA nell&#39;area Pianificazione o quelle eseguite dal Designer di pianificazione si trovano nel contesto delle autorizzazioni di Workfront Planning e del livello di accesso a Workfront.

  Per ulteriori informazioni, consulta:

  * [Panoramica delle autorizzazioni di condivisione in Pianificazione di Adobe Workfront](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Panoramica del tipo di licenza durante l’utilizzo di Pianficazione di Adobe Workfront](/help/quicksilver/planning/access/license-type-overview.md)

* Le modifiche apportate dall&#39;Assistente AI o dal Designer di Planning per conto dell&#39;utente vengono registrate nel pannello della cronologia del record.

* Le azioni eseguite dal Designer di pianificazione sono permanenti e potrebbero essere irreversibili. L’eliminazione di un campo, ad esempio, non può essere annullata. Rivedi tutte le azioni proposte da Designer prima di accettarle.

  >[!IMPORTANT]
  >
  >Durante la creazione, l&#39;aggiornamento o l&#39;eliminazione di un oggetto tramite il Designer di Planning, il prompt richiede una conferma solo per le azioni irreversibili. Ad esempio, l’eliminazione di un tipo di record o di un’area di lavoro è irreversibile. L&#39;eliminazione di un record non è. Il Designer di Planning richiederà conferma solo quando si tenta di eliminare un tipo di record o un&#39;area di lavoro.

* Quando si creano aree di lavoro e tipi di record mediante Planning Designer, vengono creati automaticamente anche le viste e i campi.

## Funzionalità attualmente disponibile per Planning Designer

È possibile utilizzare Planning Designer o l&#39;Assistente IA per eseguire una delle azioni seguenti:

* Creare e configurare le aree di lavoro

<!--On March 2: * Edit workspaces-->

* Creare tipi di record, inclusa la definizione e l&#39;aggiunta di tipi di record globali alle aree di lavoro

* Progettare campi o campi formula

* Creare, eliminare, duplicare e ripristinare record

* Modificare, aggiornare e aggiungere un campo in un record

* Collega record ad altri record

* Cronologia modifiche record di accesso

* Creare viste personalizzate

* Creare record importando un documento

  È ad esempio possibile caricare un&#39;immagine di un organigramma della società e il Designer di Planning può creare un&#39;area di lavoro basata su tale immagine.

  La creazione di oggetti da un documento importato è disponibile solo in Planning Designer e non nell&#39;Assistente IA.

  >[!IMPORTANT]
  >
  >Sebbene supportino i tipi di file XLSX, non possono essere utilizzati per l&#39;importazione di record su larga scala tramite Planning Designer.
  >Se in questo momento è necessario importare un numero considerevole di record, è consigliabile utilizzare le funzionalità manuali disponibili in Planning.
  >
  >Per ulteriori informazioni, vedere [Creare record importando informazioni da un file CSV o Excel](/help/quicksilver/planning/records/import-file-to-create-records.md).
  >Per informazioni sulle limitazioni relative al tipo di file, vedere la sezione &quot;Ottieni suggerimenti in base a un documento caricato&quot; in [Utilizzare il riempimento modulo basato su IA per compilare una richiesta utilizzando prompt o documenti](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).


  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Creazione o aggiornamento di oggetti mediante Planning Designer

È possibile creare o aggiornare oggetti in Workfront Planning utilizzando il Designer di Planning o l&#39;Assistente IA, salvo diversa indicazione.

1. Accedi a Workfront, quindi fai clic sull&#39;icona **Main Menu** ![Lines main menu](assets/lines-main-menu.png) in alto a sinistra, quindi fai clic su **Planning**.

   Verrà aperta l&#39;area **Planning**. <!--update screen shot when they change the name of the button-->

   ![Pulsante Progettazione con IA nella pagina Aree di lavoro](assets/design-with-ai-button-on-workspaces-page.png)

1. Fai clic su **Crea con IA** o su **Crea area di lavoro**, quindi utilizza la finestra di richiesta nella parte superiore per indicare il tipo di area di lavoro che desideri creare. <!--update this when they change it to Generate with AI-->

   Viene visualizzata la finestra **Planning Designer**. <!--remove the Beta tag here when this removes from Beta-->

   ![Finestra di Planning Designer](assets/planning-designer-window.png)

1. Nello spazio disponibile, inizia a digitare i prompt per l’Assistente AI, quindi al termine fai clic su Invio.

   <!--add screen shot-->

   È ad esempio possibile digitare prompt simili a quelli riportati di seguito:

   * Creare e configurare un’area di lavoro con cinque tipi di record per gestire le campagne

   * Crea campagne di marketing per ogni mese dell’anno corrente

   * Aggiungere un campo campagna per lo stato dell&#39;area di lavoro Progettazione marketing

   * Elimina tutti i record con lo stato Non aggiornato

   * Aggiorna tutte le campagne Planning con lo stato Attivo

   * Collegare le campagne a utenti tipo nell’area di lavoro Progettazione marketing

   * Visualizza la cronologia modifiche per la campagna &quot;San Valentino&quot;

   * Creare una visualizzazione timeline per le campagne nell’area di lavoro Progettazione marketing

   * Creare record importando un documento. La creazione di record da un documento importato è disponibile solo in Planning Designer e non nell&#39;Assistente IA.

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

1. Dopo aver ricevuto una risposta corretta, segui i collegamenti forniti nell’area dei prompt per creare, aggiornare o rivedere l’oggetto della richiesta.

   Quando si accetta di creare gli oggetti, le modifiche vengono visualizzate a destra dell&#39;area del prompt.

   È possibile visualizzare aree di lavoro, tipi di record, campi, visualizzazioni e record nell&#39;area di anteprima a destra del prompt.

   >[!TIP]
   >
   >Alcuni oggetti vengono creati immediatamente, senza necessità di conferma.

1. (Facoltativo) Immettete ulteriori richieste per modificare ulteriormente gli oggetti.
1. (Facoltativo) Fai clic sull&#39;icona **Mostra o nascondi la schermata di anteprima** ![Nascondi o mostra l&#39;icona della schermata di anteprima](assets/hide-show-preview-screen-in-planning-designer.png) per aprire o chiudere la schermata di anteprima a destra.
1. Fai clic sull&#39;icona **Apri area di lavoro in una nuova scheda** ![Apri area di lavoro in una nuova scheda](assets/open-workspace-on-new-tab-icon.png) per aprire l&#39;area di lavoro che stai aggiornando in una nuova scheda.
1. Fare clic sull&#39;icona **Chiudi** **X** per chiudere Planning Designer e aprire l&#39;area Aree di lavoro.
1. (Facoltativo) Per modificare un&#39;area di lavoro, effettuate una delle seguenti operazioni:

   * Apri l’area di lavoro e apporta manualmente le modifiche. Per informazioni, consulta [Modificare le aree di lavoro](/help/quicksilver/planning/architecture/edit-workspaces.md).
   * Fai clic su **Modifica con IA**. Verrà aperto Planning Designer. Ripeti i passaggi precedenti per utilizzare l’intelligenza artificiale e apportare ulteriori modifiche all’area di lavoro.


