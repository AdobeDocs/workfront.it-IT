---
user-type: administrator
product-area: system-administration;setup
navigation-upperic: configure-locations
title: Configurare i collaboratori IA
description: In qualità di amministratore di Adobe Workfront, puoi configurare i collaboratori IA e assegnarli a progetti e attività.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 3cf7495f827156fabac1214b38a104ed826d558c
workflow-type: tm+mt
source-wordcount: '1577'
ht-degree: 2%
---
# Configurare i collaboratori IA

{{preview-fast-release-general}}

I collaboratori IA sono un modo per integrare gli agenti IA nei progetti, nelle attività e nei problemi. Puoi configurare un Collaboratore IA, quindi assegnarlo come faresti con un utente.

Ad esempio, puoi configurare un collaboratore IA di tipo revisore con le linee guida del brand, quindi assegnare tale collaboratore per rivedere un documento.

I tipi di Collaboratore IA disponibili includono:

* Revisore IA: crea un collaboratore utilizzando brand o Adobe Brand Intelligence, quindi assegna il collaboratore come revisore delle risorse.

  Per ulteriori informazioni, consulta [Introduzione a Workfront AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Agente di lavoro: crea un collaboratore utilizzando una piattaforma di intelligenza artificiale standard come Claude, OpenAI, Copilot o Writer, quindi assegna il collaboratore a un’attività o a un problema per completare gli elementi di lavoro.

  Per ulteriori informazioni, vedere [Utilizzare agenti di lavoro](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

<!--
* <span class="preview">Project Coordinator: An out-of-the-box collaborator that monitors project status and follows up on overdue tasks automatically, without needing to configure an external agent.</span>

   <span class="preview">For more information, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).</span>
-->


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Seleziona, Prime o Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema] <span class="preview">o Amministratore di gruppo</span></td> 
  </tr> 
  </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

* [Per i revisori AI](#for-ai-reviewers)
* [Per agenti di lavoro](#for-work-agents)

### Per i revisori AI:

* La tua organizzazione deve disporre di un contratto Adobe Gen AI firmato.

  Per ulteriori informazioni, consulta [Firmare il contratto di Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) nell&#39;articolo Assistente IA in Workfront.
* Prima di poter utilizzare un marchio per un revisore di intelligenza artificiale, devi averlo configurato in Workfront.

  Per istruzioni, consulta [Creare e gestire i brand per il revisore di IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).
* Per utilizzare Adobe Brand Intelligence per un revisore di IA, la tua organizzazione deve utilizzare l’esperienza di revisione e approvazione unificata in Workfront.

  Per ulteriori informazioni, vedere [Introduzione alla revisione e all&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

### Per agenti di lavoro

È necessario configurare un agente in Claude, Copilot Studio, Writer, OpenAI o IBM prima di poterlo utilizzare come agente di lavoro.

>[!NOTE]
>
>Il nostro obiettivo è quello di connetterci con qualsiasi provider di agenti, quindi se il provider in uso non è al momento compatibile con gli agenti di lavoro, contatta il team del tuo account per assistenza.

## Crea un nuovo revisore di IA

I revisori AI possono essere configurati per utilizzare i marchi Workfront o Adobe Brand Intelligence.

* **Marchi**: i marchi vengono creati in Workfront. Puoi creare marchi in Workfront caricando file PDF che contengono le linee guida per i marchi o immettendo manualmente gli elementi del marchio.
* **Adobe Brand Intelligence**: quando un collaboratore IA esamina una risorsa utilizzando Adobe Brand Intelligence, puoi visualizzare i commenti del revisore IA in Frame.io.


{{step-1-to-setup}}

1. Nel menu di navigazione a sinistra, fai clic su **Collaboratori IA**.
1. Fai clic su **Nuovo collaboratore** nell&#39;angolo superiore destro della schermata.
1. Fai clic su **Revisore**, quindi su **Continua**.
1. Nel campo Nome collaboratore immettere un nome per il collaboratore. Questo è il nome visualizzato nell&#39;elenco degli assegnatari disponibili per un&#39;attività.
1. Seleziona se il collaboratore utilizzerà un marchio o un Adobe Brand Intelligence per le sue recensioni.
1. (Condizionale) Se il Collaboratore IA utilizza un Brand, seleziona il brand e la linea guida del brand che utilizzerà.
1. Fai clic su **Salva**.

## Configurare un agente di lavoro

Gli agenti di lavoro sono agenti che puoi assegnare ad attività o problemi in Workfront. È possibile configurare l&#39;agente di lavoro con un nome, un livello di accesso e altri dettagli e assegnarlo a un&#39;attività come si farebbe con un utente.

Poiché gli agenti di lavoro sono agenti, le loro azioni e capacità vengono configurate nel punto in cui vengono configurati gli agenti. Attualmente, gli agenti utilizzati come agenti di lavoro possono essere creati in Copilot Studio, Claude o Writer, OpenAI e IBM.

Gli agenti di lavoro possono essere assegnati ad attività o problemi.

Per un elenco delle best practice per la creazione di un agente che possa funzionare come agente di lavoro, vedere [Best practice per la creazione di un agente per un agente di lavoro](#best-practices-for-creating-an-agent-for-a-work-agent).

* [Configurare un agente di lavoro in Workfront](#configure-a-work-agent-in-workfront)
* [Best practice per la creazione di un agente per un agente di lavoro](#best-practices-for-creating-an-agent-for-a-work-agent)

### Configurare un agente di lavoro in Workfront

{{step-1-to-setup}}

1. Nel menu di navigazione a sinistra, fai clic su **Collaboratori IA**.
1. Fai clic su **Nuovo collaboratore** nell&#39;angolo superiore destro della schermata.
1. Seleziona **Agenti di lavoro**, quindi fai clic su **Continua**.
1. Nel campo Nome collaboratore IA immettere un nome per il collaboratore. Questo è il nome visualizzato nell&#39;elenco degli assegnatari disponibili per un&#39;attività.
1. Nel campo Descrizione collaboratore AI immettere una descrizione dello scopo del collaboratore o delle azioni eseguite.
1. Nel campo Livello di accesso selezionare un livello di accesso per il collaboratore. Questo livello di accesso controlla ciò che il collaboratore può fare, allo stesso modo un livello di accesso controlla ciò che un utente può fare.
1. (Facoltativo) Nel campo Gruppi, selezionare i gruppi a cui l&#39;agente di lavoro sarà associato.

   >[!NOTE]
   >
   ><span class="preview">Se si è un amministratore di gruppo, in questo campo vengono visualizzati solo i gruppi per i quali si è un amministratore. Gli amministratori del gruppo devono selezionare almeno un gruppo.</span>

1. Nell&#39;area **Scegli l&#39;origine dell&#39;agente** selezionare se si desidera connettere un agente creato in una piattaforma comune, ad esempio Copilot o Writer, oppure utilizzare un agente personalizzato.
1. (Condizionale) Se utilizzi un agente di una piattaforma comune, inserisci i dettagli di autenticazione per la piattaforma dell’agente:

   | Piattaforma | Autenticazione richiesta |
   |---|---|
   | Copilot Studio | Segreto canale web |
   | Claude Managed Agents | Chiave API antropica<br>ID agente<br>ID ambiente |
   | Agente di scrittura | Chiave API<br>ID applicazione |
   | <span class="preview">Agenti OpenAI</span> | <span class="preview">Chiave API <br>ID agente</span> |
   | <span class="preview">IBM watsonx Orchestrate</span> | <span class="preview">URL servizio<br>Chiave API<br> ID agente</span> |

1. Fare clic su **Verifica connessione**. Questo consente di sapere se la connessione è stata configurata correttamente.
1. Nell&#39;area **Al termine del lavoro del collaboratore, è possibile** attivare le azioni che si desidera vengano eseguite dal collaboratore.

   * <span class="preview">Invia notifica: l&#39;agente inserisce un commento nel flusso di aggiornamento, assegna tag all&#39;utente che ha richiesto il lavoro, ha assegnato l&#39;agente o è il proprietario del progetto. </span>
   * <span class="preview">Carica un documento</span>
   * <span class="preview">Contrassegna attività come completata</span>
   * Scrivi campi attività: selezionare i moduli e i campi che l&#39;agente può scrivere.

1. Fai clic su **Salva**.

Per ulteriori informazioni sugli agenti di lavoro, tra cui come assegnarli alle attività, vedere [Utilizzare agenti di lavoro](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

### Best practice per la creazione di un agente per un agente di lavoro

Le seguenti best practice potrebbero essere utili per la creazione di un agente da utilizzare come agente di lavoro in Workfront. Per visualizzare le best practice, fai clic sulla sezione dell’applicazione in cui stai creando l’agente.

+++ Claude

1. Passa alla console Claude all&#39;indirizzo [platform.claude.com](https://platform.claude.com/).
1. Crea una chiave API.
   1. In Chiavi API, fai clic su **Crea chiave** nell&#39;angolo in alto a destra.
   1. Immetti un nome e una data di scadenza.
   1. Copiare la chiave e salvarla in un luogo sicuro. Questa chiave è necessaria per configurare l’agente di lavoro in Workfront.

1. Creare un ambiente.
   1. In **Agenti gestiti** > **Ambienti**, fai clic su **Crea ambiente** nell&#39;angolo superiore destro.
   1. Specifica un nome e un tipo di hosting, a seconda dei casi.
   1. Configura i pacchetti condivisi e i metadati in base alle esigenze. Gli ambienti possono essere riutilizzati in più agenti e consentire la condivisione di pacchetti e metadati.
      L’ID dell’ambiente viene visualizzato sotto il nome dell’ambiente nell’angolo in alto a sinistra.

1. Crea un agente.
   1. In Agenti gestiti > Agenti fare clic su **Crea agente** nell&#39;angolo superiore destro.
   1. Fornisci un nome, un modello, un prompt del sistema, le abilità e gli strumenti necessari. Essere descrittivi, perché gli agenti di lavoro trasmettono il contesto dell’attività a questo agente, che quindi esegue il lavoro.
      L&#39;ID agente viene visualizzato sotto il nome dell&#39;agente nell&#39;angolo superiore sinistro.

1. Configurare l’agente di lavoro in Workfront.
   1. Immetti la chiave API, l’ID ambiente e l’ID agente
   1. Fai clic su **Verifica connessione** per verificare.

1. Assegnare l&#39;agente di lavoro a un&#39;attività di Workfront.
   1. L&#39;agente di lavoro viene attivato dopo il completamento di tutte le attività predecessore.

+++
<!--
+++ Copilot Studio



+++
-->
+++ Autore

>[!NOTE]
>
> È possibile utilizzare un agente Writer come agente di lavoro, ma i playbook Writer non possono essere utilizzati come agenti di lavoro.

Quando si crea un agente da utilizzare come agente di lavoro in Writer, si consiglia di eseguire il seguente flusso di lavoro.

Ulteriori informazioni sulla creazione di agenti sono disponibili nella [documentazione di Writer](https://dev.writer.com/no-code/introduction).

1. Crea un’app senza codice in Writer AI Studio.
1. Aggiungere un singolo campo di immissione Testo. È possibile utilizzare il nome predefinito &quot;Input testo&quot;.
1. Aggiungi `@TextInput` alla tua richiesta. Nella sezione Prompts della configurazione di app, accertati che il modello di prompt faccia riferimento alla variabile di input. Senza questo, il modello non vede mai i dati dell’attività.
1. Regola la richiesta per generare l&#39;output immediatamente. Rimuovi eventuali istruzioni che richiedono all’utente chiarimenti o contesto aggiuntivo prima di rispondere. Ad esempio: &quot;Quando ricevi un input, consideralo come una richiesta di generazione di contenuti e generi immediatamente l’output. Non chiedete chiarimenti.&quot;
1. Copia la chiave API e l’ID applicazione. Saranno necessarie per configurare l’agente di lavoro in Workfront.

   * Per istruzioni sulla configurazione di una chiave API in Writer, vedi [Quickstart](https://dev.writer.com/home/quickstart) nella documentazione di Writer.
   * Per istruzioni sulla configurazione di un ID applicazione in Writer, vedere [Richiamare agenti senza codice tramite l&#39;API](https://dev.writer.com/home/applications) nella documentazione di Writer.

1. Configurare l’agente di lavoro in Workfront. Come parte della configurazione, immetti la chiave API e l&#39;ID applicazione, quindi fai clic su **Verifica connessione** per verificare.
1. Assegnare l&#39;agente di lavoro a un&#39;attività di Workfront. L&#39;agente di lavoro inizia a lavorare quando tutte le attività predecessore dell&#39;attività sono state completate.

+++

<div class="preview">

<!--
## Configure a Project Coordinator

The Project Coordinator is an out-of-the-box collaborator that monitors project status and helps keep work on track. Unlike Work Agents, the Project Coordinator does not require you to configure an external agent.

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Select **Project Coordinator**.
1. In the **AI Collaborator name** field, enter a name for the Project Coordinator. This is the name that appears as the collaborator in your project.
1. In the **AI Collaborator description** field, enter a description of what the Project Coordinator does or its purpose.
1. In the **Access level** field, select an access level for the Project Coordinator. This access level controls what the collaborator can do on projects.
1. (Optional) In the **Send project updates** section, toggle **Allow** to enable project update notifications, then specify update details.
   * In the **Cadence** field, select whether the Coordinator sends updates daily or weekly.
   * If the Coordinator sends updates weekly, in the **Day of week** field, select the day of the week that updates are sent.
   * In the **Time (MST)** field, select the time to send updates.
   * In the **How to send** field, select whether the Coordinator sends updates as an update on the project, or as an email
   * In the **Who gets the update** field, select whether the update is sent only to the project owner, or to all project stakeholders.
   * (Optional) Check **Send additional update immediately when coordinator is assigned** to notify on assignment.
   * (Optional) Check **Send additional update when a date is missed** to send notifications when dates are missed.
1. (Optional) In the **Notify task assignees** section, toggle **Allow** to enable task notifications, then check the boxes for the situations that you want to notify assignees about.
1. (Optional) In the **Remind reviewers and approvers** section, toggle **Allow** to enable reminders for reviewers, then check the boxes for the situations that you want to remind reviewers and approvers about.
1. (Optional) In the **Update the content of project and task fields** section, toggle **Allow** to enable the coordinator to update project and task field values.
1. Click **Save**.

For more information on the Project Coordinator, including how to assign it to projects, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).
-->

</div>

## Gestisci collaboratori IA

È possibile modificare, copiare ed eliminare i collaboratori IA esistenti.

>[!NOTE]
>
><span class="preview">Gli amministratori di gruppi possono visualizzare e interagire solo con i collaboratori IA associati ai gruppi di cui sono amministratori. Se a un determinato collaboratore AI sono associati anche altri gruppi, un amministratore di gruppo può visualizzarlo ma non modificarlo.</span>

{{step-1-to-setup}}

1. Nel menu di navigazione a sinistra, fai clic su **Collaboratori IA**.
1. (Condizionale) Per modificare un collaboratore, fare clic sul nome del collaboratore che si desidera modificare, apportare le modifiche desiderate nella finestra Modifica collaboratore e fare clic su **Salva**.
1. (Condizionale) Per eliminare un collaboratore, fare clic sull&#39;icona Elimina ![icona Elimina](assets/delete-collaborator-icon.png) nella riga del collaboratore AI che si desidera eliminare, quindi fare clic su **Elimina**.
