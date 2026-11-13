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
source-git-commit: 13403cc11448a0611ad0996ed21e1745277e9c05
workflow-type: tm+mt
source-wordcount: '1993'
ht-degree: 2%
---
# Configurare i collaboratori IA

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambiente di anteprima per tutti i clienti.</span>

I collaboratori IA sono un modo per integrare gli agenti IA nei progetti, nelle attività e nei problemi. Puoi configurare un Collaboratore IA, quindi assegnarlo come faresti con un utente.

Ad esempio, puoi configurare un collaboratore IA di tipo revisore con le linee guida del brand, quindi assegnare tale collaboratore per rivedere un documento.

I tipi di Collaboratore IA disponibili includono:

* Revisore IA: crea un collaboratore utilizzando brand o Adobe Brand Intelligence, quindi assegna il collaboratore come revisore delle risorse.

  Per ulteriori informazioni, consulta [Introduzione a Workfront AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Agente di lavoro: crea un collaboratore <span class="preview">con tecnologia Adobe CX Coworker,</span> o connetti un agente da una piattaforma esterna supportata, quindi assegna il collaboratore a un&#39;attività o a un problema per completare gli elementi di lavoro.

  Per ulteriori informazioni, vedere [Utilizzare agenti di lavoro](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

  Per ulteriori informazioni su Adobe CX Enterprise Coworker, vedere [Panoramica di CX Enterprise Coworker in Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

Le licenze utilizzate dai collaboratori AI non vengono fatturate. Se la tua organizzazione dispone di 200 licenze Workfront e crea un Collaboratore AI, sono in uso 201 licenze, ma solo 200 vengono fatturate.

* <span class="preview">Coordinatore progetto: un collaboratore predefinito che controlla lo stato del progetto e invia aggiornamenti al progetto senza dover configurare un agente esterno.</span>

  <span class="preview">Per ulteriori informazioni, vedere [Utilizzare Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).</span>


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
   <td>[!UICONTROL System Administrator] o Group Administrator</span></td> 
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

<span class="preview">I prerequisiti dipendono dall&#39;origine dell&#39;agente:</span>

* <span class="preview">Adobe nativo: l&#39;organizzazione deve avere Adobe CX Coworker abilitato. Non è necessario configurare un agente in una piattaforma esterna o fornire credenziali di piattaforma esterna.</span>
* Piattaforma esterna o agente personalizzato: configura l’agente nella piattaforma che intendi connettere prima di creare l’agente di lavoro in Workfront.

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

<span class="preview">Le seguenti indicazioni di installazione riflettono il supporto nativo di Adobe e il modello di installazione basato sull&#39;origine ancora in anteprima.</span>

Gli agenti di lavoro sono agenti che puoi assegnare ad attività o problemi in Workfront. È possibile configurare l&#39;agente di lavoro con un nome, un livello di accesso e altri dettagli e assegnarlo a un&#39;attività come si farebbe con un utente.

Poiché gli agenti di lavoro sono agenti, le loro azioni e capacità vengono configurate nel punto in cui vengono configurati gli agenti. Gli agenti di lavoro possono essere <span class="preview">Agenti di lavoro nativi che utilizzano Coworker,</span> o possono provenire da una piattaforma esterna supportata, ad esempio Copilot Studio, Claude, OpenAI e IBM.

>Gli agenti di lavoro possono essere assegnati ad attività o problemi.

Le licenze utilizzate dagli agenti di lavoro non sono fatturate. Se la tua organizzazione dispone di 200 licenze Workfront e crea un agente di lavoro, sono in uso 201 licenze, ma solo 200 vengono fatturate.

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
   >Se si è un amministratore di gruppo, in questo campo vengono visualizzati solo i gruppi per i quali si è un amministratore. Gli amministratori dei gruppi devono selezionare almeno un gruppo.

1. Nell&#39;area **Scegli l&#39;origine dell&#39;agente**, seleziona se desideri <span class="preview">utilizzare Adobe Native</span>, connettere un agente creato in una piattaforma comune come Copilot o utilizzare un agente personalizzato.
1. <span class="preview">(Condizionale) Se si seleziona Adobe Native, verificare che Adobe CX Coworker sia abilitato per la propria organizzazione e che si desideri utilizzare l&#39;agente Adobe Native pronto all&#39;uso.</span>
1. (Condizionale) Se utilizzi un agente di una piattaforma comune, inserisci i dettagli di autenticazione per la piattaforma dell’agente:

   | Piattaforma | Autenticazione richiesta |
   |---|---|
   | Copilot Studio | Segreto canale web |
   | Claude Managed Agents | Chiave API antropica<br>ID agente<br>ID ambiente |
   | Agenti OpenAI | Chiave API <br>ID agente |
   | IBM watsonx Orchestrate | URL servizio<br>ID agente chiave API<br> |

1. Fare clic su **Verifica connessione**. Questo consente di sapere se la connessione è stata configurata correttamente.
1. Nell&#39;area **Al termine del lavoro del collaboratore, è possibile** attivare le azioni che si desidera vengano eseguite dal collaboratore.

   * Invia notifica: l’agente inserisce un commento nel flusso di aggiornamento, assegna tag all’utente che ha richiesto il lavoro, gli assegna l’agente o il proprietario del progetto.
   * Carica documenti basati su testo
   * Contrassegna l’attività come completata
   * Scrivi campi attività: selezionare i moduli e i campi che l&#39;agente può scrivere.
   * Scrivi campi progetto: seleziona i moduli e i campi in cui l’agente può scrivere.

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



>[!IMPORTANT]
>
>Writer ha dichiarato obsoleto il loro uso di agenti. Gli agenti di lavoro configurati utilizzando gli agenti Writer non funzionano più dopo il 9 ottobre. 2026.
>
>Per informazioni sull&#39;elemento deprecato, vedere [Migrazione e deprecazione della libreria agenti](https://support.writer.com/articles/8335689949-migrating-no-code-agents) nella documentazione di Writer.


<!--

>[!NOTE]
>
> You can use a Writer agent as a Work Agent, but Writer playbooks cannot be used as Work Agents.

When creating an agent for use as a Work Agent in Writer, we recommend the following workflow.

More detailed information about creating agents can be found in the [Writer documentation](https://dev.writer.com/no-code/introduction).

1. Create a no-code app in Writer AI Studio. 
1. Add a single Text input field. You can use the default name "Text input."
1. Add `@TextInput` to your Prompt. In the Prompts section of your app configuration, make sure your prompt template references the input variable. Without this, the model never sees the task data.
1. Adjust your Prompt to generate output immediately. Remove any instructions that ask the user for clarification or additional context before responding. For example: "When you receive input, treat it as a content generation request and produce the output immediately. Do not ask for clarification."
1. Copy your API key and Application ID. You will need them to configure the Work Agent in Workfront.

   * For instructions on setting up an API key in Writer, see [Quickstart](https://dev.writer.com/home/quickstart) in the Writer documentation.
   * For instructions on setting up an application ID in Writer, see [Invoke no-code agents via the API](https://dev.writer.com/home/applications) in the Writer documentation.
 
1. Configure the Work Agent in Workfront. As part of the configuration, enter your API key and Application ID, then click **Test connection** to verify.
1. Assign the Work Agent to a Workfront task. The Work Agent begins work when all of the task's predecessor tasks are complete.

-->

+++

<div class="preview">

## Configurare un coordinatore del progetto

Il coordinatore del progetto è un collaboratore pronto all’uso che monitora lo stato del progetto e aiuta a mantenere il lavoro sulla strada giusta. A differenza degli agenti di lavoro, Project Coordinator non richiede la configurazione di un agente esterno.

{{step-1-to-setup}}

1. Nel menu di navigazione a sinistra, fai clic su **Collaboratori IA**.
1. Fai clic su **Nuovo collaboratore** nell&#39;angolo superiore destro della schermata.
1. Seleziona **Coordinatore progetto**, quindi fai clic su **Continua**.
1. Nel campo **Nome collaboratore AI** immettere un nome per il coordinatore del progetto. Questo è il nome visualizzato come collaboratore nel progetto.
1. (Facoltativo) Nel campo **Descrizione collaboratore AI** immettere una descrizione delle funzioni o degli scopi del coordinatore del progetto.
1. Nel campo **Livello di accesso**, selezionare un livello di accesso per il coordinatore del progetto. Questo livello di accesso controlla ciò che il collaboratore può fare sui progetti, allo stesso modo in cui un livello di accesso controlla ciò che un utente può fare.
1. (Facoltativo) Nel campo **Gruppi**, seleziona i gruppi a cui sarà associato il coordinatore del progetto.

   >[!NOTE]
   >
   >Se si è un amministratore di gruppo, in questo campo vengono visualizzati solo i gruppi per i quali si è un amministratore. Gli amministratori dei gruppi devono selezionare almeno un gruppo.

1. Nell&#39;area **Azioni coordinatore**, specificare la modalità con cui il coordinatore del progetto invia gli aggiornamenti del progetto. Il coordinatore del progetto deve disporre dell&#39;autorizzazione per eseguire queste azioni. Un coordinatore di progetto può anche commentare il progetto e le sue attività.

   Gli aggiornamenti dei progetti possono includere un riepilogo dello stato di avanzamento, lo stato del progetto, attività o approvazioni scadute o a rischio e campi o assegnazioni mancanti.

   * Nel campo **Cadenza**, seleziona se il coordinatore del progetto invia aggiornamenti ogni giorno o ogni settimana.
   * (Condizionale) Se hai selezionato settimanalmente, nel campo **Giorno**, seleziona il giorno della settimana in cui vengono inviati gli aggiornamenti.
   * Nel campo **Ora**, seleziona l&#39;ora di invio degli aggiornamenti.
   * Nel campo **Fuso orario**, selezionare il fuso orario per l&#39;ora di aggiornamento.
   * Nel campo **Chi riceve l&#39;aggiornamento**, selezionare se l&#39;aggiornamento verrà inviato al proprietario del progetto o alle parti interessate. L&#39;impostazione predefinita è il proprietario del progetto.

1. Fai clic su **Salva**.

Dopo aver salvato il coordinatore del progetto, aggiungi il campo **Coordinatore del progetto** all&#39;intestazione del progetto nei modelli di layout utilizzati dagli utenti. Gli utenti non possono assegnare un coordinatore di progetto a un progetto finché il campo non è disponibile nell’intestazione.

Per istruzioni, vedere [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

Per ulteriori informazioni sul coordinatore del progetto, incluso come assegnarlo ai progetti, vedere [Utilizzare il coordinatore del progetto &#x200B;](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).

</div>

## Gestisci collaboratori IA

È possibile modificare, copiare ed eliminare i collaboratori IA esistenti.

>[!NOTE]
>
>Gli amministratori di gruppi possono visualizzare e interagire solo con i collaboratori IA associati ai gruppi di cui sono amministratori. Se a un determinato collaboratore AI sono associati anche altri gruppi, l’amministratore del gruppo può visualizzarlo ma non modificarlo.

{{step-1-to-setup}}

1. Nel menu di navigazione a sinistra, fai clic su **Collaboratori IA**.
1. (Condizionale) Per modificare un collaboratore, fare clic sul nome del collaboratore che si desidera modificare, apportare le modifiche desiderate nella finestra Modifica collaboratore e fare clic su **Salva**.
1. (Condizionale) Per eliminare un collaboratore, fare clic sull&#39;icona Elimina ![icona Elimina](assets/delete-collaborator-icon.png) nella riga del collaboratore AI che si desidera eliminare, quindi fare clic su **Elimina**.
