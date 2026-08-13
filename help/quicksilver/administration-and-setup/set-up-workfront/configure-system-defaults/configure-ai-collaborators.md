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
source-git-commit: 1894bbb5ec7f44f93468c202fb9c07fa656a83cf
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 2%

---

# Configurare i collaboratori IA


<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo il rilascio in anteprima, le stesse funzioni sono disponibili mensilmente nell’ambiente di produzione per i clienti che hanno abilitato i rilasci rapidi. </span>


I collaboratori IA sono un modo per integrare gli agenti IA nei progetti e nelle attività. Puoi configurare un Collaboratore IA, quindi assegnarlo come faresti con un utente.

Ad esempio, puoi configurare un collaboratore IA di tipo revisore con le linee guida del brand, quindi assegnare tale collaboratore per rivedere un documento.

I tipi di Collaboratore IA disponibili includono:

* Revisore: crea un collaboratore utilizzando i brand o Adobe Brand Intelligence, quindi assegna il collaboratore come revisore delle risorse.

  Per ulteriori informazioni, vedere [Introduzione a Revisore contenuto Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Collaboratore task: creare un collaboratore utilizzando il copilota o il writer, quindi assegnare il collaboratore a un task per completare il lavoro a livello di task.

  Per ulteriori informazioni, vedere [Utilizzare i collaboratori attività](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).


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
   <td>[!UICONTROL Amministratore di sistema]</td> 
  </tr> 
  </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

### Per i revisori AI:

* La tua organizzazione deve disporre di un contratto Adobe Gen AI firmato.

  Per ulteriori informazioni, consulta [Firmare il contratto di Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) nell&#39;articolo Assistente IA in Workfront.
* È necessario aver configurato un marchio in Workfront prima di poterlo utilizzare per un collaboratore di IA di tipo Revisore.

  Per istruzioni, consulta [Creare e gestire i brand per il revisore dei contenuti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).
* Per utilizzare Adobe Brand Intelligence per un collaboratore di IA per l’analisi dei revisori, l’organizzazione deve utilizzare l’esperienza di revisione e approvazione unificata in Workfront. </span>

  Per ulteriori informazioni, vedere [Introduzione a revisione e approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md). </span>

<div class="preview">

### Per i collaboratori attività

È necessario configurare un agente in Claude, Copilot Studio o Writer prima di poterlo utilizzare come collaboratore di attività.

</div>

## Crea un nuovo Collaboratore IA di tipo Revisore

I collaboratori di IA per l’analisi dei revisori possono essere configurati per utilizzare i marchi Workfront o Adobe Brand Intelligence.

* **Marchi**: i marchi vengono creati in Workfront. Puoi creare marchi in Workfront caricando file PDF che contengono le linee guida per i marchi o immettendo manualmente gli elementi del marchio.
* **Adobe Brand Intelligence**: quando un collaboratore AI rivede una risorsa utilizzando Adobe Brand Intelligence, puoi visualizzare i commenti del revisore in Frame.io.  </span>


{{step-1-to-setup}}

1. Nel menu di navigazione a sinistra, fai clic su **Collaboratori IA**.
1. Fai clic su **Nuovo collaboratore** nell&#39;angolo superiore destro della schermata.
1. Fai clic su **Revisore**, quindi su **Continua**.
1. Nel campo Nome collaboratore immettere un nome per il collaboratore. Questo è il nome visualizzato nell&#39;elenco degli assegnatari disponibili per un&#39;attività.
1. Seleziona se il collaboratore utilizzerà un marchio o Adobe Brand Intelligence per le sue recensioni.
1. (Condizionale) Se il Collaboratore IA utilizza un Brand, seleziona il brand e la linea guida del brand che utilizzerà.
1. Fai clic su **Salva**.

<div class="preview">

## Configurare un collaboratore di attività

I collaboratori attività sono agenti MCP che possono essere assegnati ad attività in Workfront. È possibile configurare Collaboratore task con un nome, un livello di accesso e altri dettagli e assegnarlo a un task come si farebbe con un utente.

Poiché i collaboratori attività sono agenti MCP, le loro azioni e capacità vengono configurate nel punto in cui vengono configurati gli agenti. Attualmente, gli agenti utilizzati come collaboratori task possono essere creati in Copilot Studio, Claude o Writer.

I collaboratori attività possono essere assegnati solo ad attività e non possono essere attualmente assegnati a problemi.

Per un elenco delle procedure consigliate per la creazione di un agente da utilizzare come Collaboratore attività, vedere [Procedure consigliate per la creazione di un agente per un Collaboratore attività](#best-practices-for-creating-an-agent-for-a-task-collaborator).

### Configurare un collaboratore in Workfront

{{step-1-to-setup}}

1. Nel menu di navigazione a sinistra, fai clic su **Collaboratori IA**.
1. Fai clic su **Nuovo collaboratore** nell&#39;angolo superiore destro della schermata.
1. Seleziona **Agenti attività**, quindi fai clic su **Continua**.
1. Nel campo Nome collaboratore IA immettere un nome per il collaboratore. Questo è il nome visualizzato nell&#39;elenco degli assegnatari disponibili per un&#39;attività.
1. Nel campo Descrizione collaboratore AI immettere una descrizione dello scopo del collaboratore o delle azioni eseguite.
1. Nel campo Livello di accesso selezionare un livello di accesso per il collaboratore. Questo livello di accesso controlla ciò che il collaboratore può fare, allo stesso modo un livello di accesso controlla ciò che un utente può fare.
1. Nell&#39;area **Scegli l&#39;origine dell&#39;agente** selezionare se si desidera connettere un agente creato in una piattaforma comune, ad esempio Copilot o Writer, oppure utilizzare un agente personalizzato.
1. (Condizionale) Se utilizzi un agente di una piattaforma comune, inserisci i dettagli di autenticazione per la piattaforma dell’agente:

   | Piattaforma | Autenticazione richiesta |
   |---|---|
   | Copilot Studio | Segreto canale web |
   | Claude Managed Agents | Chiave API antropica<br>ID agente<br>ID ambiente |
   | Autore | Chiave API<br>ID applicazione |

1. Fare clic su **Verifica connessione**. Questo consente di sapere se la connessione è stata configurata correttamente.
1. Nell&#39;area **Al termine del lavoro del collaboratore, è possibile** attivare le azioni che si desidera vengano eseguite dal collaboratore.
1. Fai clic su **Salva**.

Per ulteriori informazioni sui collaboratori attività, tra cui come assegnarli alle attività, vedere [Utilizzare i collaboratori attività](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).


### Procedure consigliate per la creazione di un agente per un collaboratore attività

Le procedure consigliate riportate di seguito sono utili per la creazione di un agente da utilizzare come collaboratore di task in Workfront. Per visualizzare le best practice, fai clic sulla sezione dell’applicazione in cui stai creando l’agente.

+++ Claude

1. Passa alla console Claude all&#39;indirizzo [platform.claude.com](https://platform.claude.com/).
1. Crea una chiave API.
   1. In Chiavi API, fai clic su **Crea chiave** nell&#39;angolo in alto a destra.
   1. Immetti un nome e una data di scadenza.
   1. Copiare la chiave e salvarla in un luogo sicuro. Questa chiave è necessaria per configurare Task Collaborator in Workfront.

1. Creare un ambiente.
   1. In **Agenti gestiti** > **Ambienti**, fai clic su **Crea ambiente** nell&#39;angolo superiore destro.
   1. Specifica un nome e un tipo di hosting, a seconda dei casi.
   1. Configura i pacchetti condivisi e i metadati in base alle esigenze. Gli ambienti possono essere riutilizzati in più agenti e consentire la condivisione di pacchetti e metadati.
      L’ID dell’ambiente viene visualizzato sotto il nome dell’ambiente nell’angolo in alto a sinistra.

1. Crea un agente.
   1. In Agenti gestiti > Agenti fare clic su **Crea agente** nell&#39;angolo superiore destro.
   1. Fornisci un nome, un modello, un prompt del sistema, le abilità e gli strumenti necessari. Essere descrittivi, perché i collaboratori attività trasmettono il contesto dell&#39;attività a questo agente, che quindi esegue il lavoro.
      L&#39;ID agente viene visualizzato sotto il nome dell&#39;agente nell&#39;angolo superiore sinistro.

1. Configurare Collaboratore attività in Workfront.
   1. Immetti la chiave API, l’ID ambiente e l’ID agente
   1. Fai clic su **Verifica connessione** per verificare.

1. Assegnare il Collaboratore task a un task Workfront.
   1. Il Collaboratore attività viene attivato dopo il completamento di tutte le attività predecessori.

+++
<!--
+++ Copilot Studio



+++
-->
+++ Autore

>[!NOTE]
>
> È possibile utilizzare un agente Writer come Collaboratore attività, ma i playbook Writer non possono essere utilizzati come Collaboratori attività.

Quando si crea un agente da utilizzare come collaboratore attività in Writer, si consiglia di eseguire il seguente flusso di lavoro.

Ulteriori informazioni sulla creazione di agenti sono disponibili nella [documentazione di Writer](https://dev.writer.com/no-code/introduction).

1. Crea un’app senza codice in Writer AI Studio.
1. Aggiungere un singolo campo di immissione Testo. È possibile utilizzare il nome predefinito &quot;Input testo&quot;.
1. Aggiungi `@TextInput` alla tua richiesta. Nella sezione Prompts della configurazione di app, accertati che il modello di prompt faccia riferimento alla variabile di input. Senza questo, il modello non vede mai i dati dell’attività.
1. Regola la richiesta per generare l&#39;output immediatamente. Rimuovi eventuali istruzioni che richiedono all’utente chiarimenti o contesto aggiuntivo prima di rispondere. Ad esempio: &quot;Quando ricevi un input, consideralo come una richiesta di generazione di contenuti e generi immediatamente l’output. Non chiedete chiarimenti.&quot;
1. Copia la chiave API e l’ID applicazione. È necessario Collaboratore attività per configurare Collaboratore attività in Workfront.

   * Per istruzioni sulla configurazione di una chiave API in Writer, vedi [Quickstart](https://dev.writer.com/home/quickstart) nella documentazione di Writer.
   * Per istruzioni sulla configurazione di un ID applicazione in Writer, vedere [Richiamare agenti senza codice tramite l&#39;API](https://dev.writer.com/home/applications) nella documentazione di Writer.

1. Configurare Collaboratore attività in Workfront. Come parte della configurazione, immetti la chiave API e l&#39;ID applicazione, quindi fai clic su **Verifica connessione** per verificare.
1. Assegnare il Collaboratore task a un task Workfront. Il collaboratore inizia a lavorare quando tutte le attività predecessore dell&#39;attività sono state completate.

+++

</div>

## Gestisci collaboratori IA

È possibile modificare, copiare ed eliminare i collaboratori IA esistenti.

{{step-1-to-setup}}

1. Nel menu di navigazione a sinistra, fai clic su **Collaboratori IA**.
1. (Condizionale) Per modificare un collaboratore, fare clic sul nome del collaboratore che si desidera modificare, apportare le modifiche desiderate nella finestra Modifica collaboratore e fare clic su **Salva**.
1. (Condizionale) Per copiare un collaboratore, fare clic sull&#39;icona Copia ![icona Copia](assets/copy-ai-collaborator.png) nella riga del collaboratore AI che si desidera copiare, fare clic sul nome della copia, apportare le modifiche desiderate nella finestra Modifica collaboratore e fare clic su **Salva**.
1. (Condizionale) Per eliminare un collaboratore, fare clic sull&#39;icona Elimina ![icona Elimina](assets/delete-collaborator-icon.png) nella riga del collaboratore AI che si desidera eliminare, quindi fare clic su **Elimina**.
