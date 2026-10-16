---
title: Usa agenti di lavoro
content-type: reference
description: Scopri come utilizzare agenti di lavoro, collaboratori IA che possono essere assegnati ad attività, problemi e richieste di Workfront.
author: Becky
feature: Work Management, Tasks
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 18b3d84862352792e094738269e4307e2f6006bf
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 2%
---
# Usa agenti di lavoro

{{preview-fast-release-general}}

Gli agenti di lavoro sono collaboratori AI che possono essere assegnati direttamente ad attività, problemi e richieste di Workfront. Come altri collaboratori AI, gli agenti di lavoro sono configurati nell’area Configura e assegnati agli elementi di lavoro proprio come un utente.

Gli agenti di lavoro si connettono agli agenti configurati in Copilot Studio, Claude, <span class="preview">OpenAI o IBM. </span>

>[!IMPORTANT]
>
>Writer ha dichiarato obsoleto il loro uso di agenti. Gli agenti di lavoro configurati utilizzando gli agenti Writer non funzionano più dopo il 9 ottobre. 2026.
>
>Per informazioni sull&#39;elemento deprecato, vedere [Migrazione e deprecazione della libreria agenti](https://support.writer.com/articles/8335689949-migrating-no-code-agents) nella documentazione di Writer.

Per informazioni e istruzioni sulla creazione di un agente di lavoro in Workfront, vedere [Configurare un agente di lavoro](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent) nell&#39;articolo Configurare i collaboratori di IA.

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

* È necessario configurare un agente in Copilot, Claude, OpenAI o IBM prima di poterlo utilizzare come agente di lavoro in Workfront.

## Panoramica dell’agente di lavoro

Gli agenti di lavoro sono un modo per assegnare agenti ad attività specifiche in Workfront. Puoi configurare l’agente in un’app come Copilot Studio o Claude.ai, quindi collegare l’agente a Workfront come agente di lavoro. È quindi possibile assegnarla alle attività come se si trattasse di un utente.

Alcuni flussi di lavoro di esempio possono includere:

* Generazione della copia dai dettagli dell&#39;attività e dai documenti basati su testo allegati, quindi registrazione dell&#39;output nel flusso di aggiornamento o caricamento come documento basato su testo.
* Generazione della copia da una descrizione dell&#39;attività, esame della copia in base alle linee guida configurate nell&#39;agente e registrazione della copia nel flusso di aggiornamento.
* Lettura dei dettagli di un evento, identificazione dei dettagli mancanti e pubblicazione nel flusso di aggiornamento di domande sui dettagli mancanti.

>[!NOTE]
>
>* Dettagli specifici sulle responsabilità e sulle capacità di un agente sono configurati nell’applicazione in cui viene creato l’agente, non in Workfront.
>* Non è necessario aggiungere il server MCP di Workfront all&#39;agente utilizzato come agente di lavoro e non è necessario connettersi affinché l&#39;agente di lavoro funzioni.
>* Gli agenti di lavoro supportano attualmente gli agenti creati in Copilot Studio, Claude, <span class="preview">OpenAI e IBM. </span>
>* Durante la configurazione di un agente in Copilot Studio, è necessario impostare la protezione su **Nessuna autenticazione**.
>* Per informazioni e istruzioni sulla creazione di un agente di lavoro in Workfront, vedere [Configurare un agente di lavoro](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent) nell&#39;articolo Configurare i collaboratori di IA.

## Informazioni lette da un agente di lavoro

Quando un agente di lavoro inizia a lavorare su un’attività, legge automaticamente come contesto le seguenti informazioni sull’attività:

* Titolo attività
* Descrizione attività
* Commenti nel flusso di aggiornamento dell&#39;attività
* Informazioni in qualsiasi modulo personalizzato allegato all’attività
* <span class="preview">Documenti basati su testo allegati, ad esempio file DOC e PDF</span>
* <span class="preview">Campi progetto, se sono configurati nella configurazione dell&#39;agente di lavoro</span>

Queste informazioni vengono sempre lette e non sono configurabili come impostazioni di Workfront.

>[!TIP]
>
>Per ottenere risultati ottimali, consigliamo di:
>
>* Includere tutte le informazioni di sfondo che si desidera vengano utilizzate direttamente dall&#39;agente nella descrizione dell&#39;attività o in un campo modulo personalizzato appropriato.
>* Assicurati che l’attività corrisponda a quanto il tuo agente è istruito a fare. Ad esempio, se il tuo agente è istruito a tradurre il testo dall’inglese al francese, includi il testo che desideri tradurre nella descrizione dell’attività.

## Azioni che un agente di lavoro può intraprendere

A seconda della configurazione dell’agente di lavoro in Workfront, dopo il completamento del lavoro può eseguire le azioni seguenti:

* Scrivi campi attività, se configurati
* Carica documenti basati su testo
* Contrassegna l&#39;attività come completata

## Attivatori avvio agente di lavoro

Quando un agente di lavoro viene assegnato a un&#39;attività <span class="preview">o a un problema</span>, inizia a funzionare quando si verifica una delle seguenti situazioni:

<!--update wording to include issues when this goes to production-->

* L&#39;agente di lavoro viene assegnato a un&#39;attività pronta per l&#39;avvio. Se ad esempio l&#39;attività ha predecessori, questi ultimi saranno completati.
* L’agente di lavoro e un utente vengono assegnati a un’attività e l’agente di lavoro viene assegnato per primo.
* Un&#39;attività a cui è già assegnato un agente di lavoro come diventa pronta per l&#39;avvio e l&#39;agente di lavoro è l&#39;unico o principale assegnatario. Se ad esempio l&#39;attività ha predecessori, questi ultimi saranno completati.
* Un&#39;attività a cui un agente di lavoro e un utente sono già assegnati diventa pronta per l&#39;avvio e l&#39;agente di lavoro è stato assegnato per primo o è l&#39;assegnatario principale. Se ad esempio l&#39;attività ha predecessori, questi ultimi saranno completati.
* Un utente e un agente di lavoro vengono assegnati a un’attività e l’utente viene rimosso.
* Un utente e un agente di lavoro vengono assegnati a un&#39;attività e l&#39;agente di lavoro viene impostato come assegnatario principale per l&#39;attività.

Le situazioni seguenti non determinano l&#39;inizio del lavoro dell&#39;agente sull&#39;attività:

* Un agente di lavoro viene assegnato a un&#39;attività a cui è già stato assegnato un utente.
* Un agente di lavoro è @mentioned in un&#39;attività.
* Un agente di lavoro viene assegnato a un&#39;attività a cui è già stato assegnato un agente di lavoro. In questo caso, il primo agente di lavoro assegnato avrà già avviato il lavoro e il secondo agente di lavoro non farà nulla.
* Un agente di lavoro viene assegnato a un&#39;attività che non è pronta per l&#39;avvio. Ad esempio, se l&#39;attività ha predecessori, questi non sono ancora completi.

## Assegnare un agente di lavoro a un’attività, un problema o una richiesta

Gli agenti di lavoro vengono assegnati ad attività, problemi o richieste nello stesso modo in cui vengono assegnati gli utenti.

Quando si cerca un agente di lavoro nell&#39;elenco degli assegnatari disponibili, il nome dell&#39;agente di lavoro è solo un nome.

Per istruzioni, vedere [Assegnare attività](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) e [Gestire le richieste di lavoro e team](/help/quicksilver/people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

>[!NOTE]
>
>Gli agenti di lavoro non possono essere assegnati per rivedere o approvare un documento.

## Risoluzione dei problemi degli agenti di lavoro

Se l’agente di lavoro non restituisce una risposta o un output, verifica quanto segue:

* Assicurati che l’agente sia pubblicato sul lato provider della piattaforma di intelligenza artificiale.
* Assicurati di disporre di crediti di intelligenza artificiale sufficienti con la piattaforma del tuo agente.
* Verificare che l&#39;azione eseguita sull&#39;attività non richieda un livello di accesso specifico.
* Se utilizzi Copilot come provider di agenti, assicurati di utilizzare l’impostazione &quot;no authentication&quot; (Nessuna autenticazione).
* Se utilizzi Copilot, assicurati che l’agente sia configurato in un ambiente globale. La funzionalità agente di lavoro non supporta attualmente le versioni regionali di Copilot Studio.
* Assicurarsi che Collaborator sia l&#39;assegnatario principale dell&#39;attività.
* Verificare che l&#39;attività assegnata all&#39;agente di lavoro possa iniziare. Ad esempio, verificare che tutti i predecessori dell&#39;attività siano completi.

>[!TIP]
>
>Puoi anche passare alla piattaforma del provider di agenti e chiedere all’agente di eseguire l’attività all’interno della piattaforma. Se l’agente non è in grado di eseguire l’attività all’interno della piattaforma, l’agente di lavoro riscontrerà dei problemi anche in Workfront.
