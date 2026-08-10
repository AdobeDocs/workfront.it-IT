---
title: Utilizza collaboratori attività
content-type: reference
description: Scopri come utilizzare i collaboratori attività, i collaboratori IA che possono essere assegnati alle attività di Workfront.
author: Becky
feature: Work Management, Tasks
source-git-commit: a05312fa1def1db593743e5e6d385da0b393d5d4
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 3%

---

# Utilizza collaboratori attività

{{highlighted-preview-article-level}}

I collaboratori attività sono collaboratori IA che possono essere assegnati direttamente alle attività di Workfront, oltre al collaboratore IA di tipo revisore esistente utilizzato per le revisioni di documenti e risorse. Come altri collaboratori AI, i collaboratori attività sono configurati nell’area Configura e assegnati alle attività proprio come un utente.

I collaboratori attività si connettono agli agenti configurati, come in un server MCP.

Per informazioni e istruzioni sulla creazione di un collaboratore attività in Workfront, vedere [Configurare un collaboratore attività](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) nell&#39;articolo Configurare i collaboratori IA.

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

* È necessario configurare un agente in Copilot, Claude o Writer.ai prima di poterlo utilizzare come collaboratore di attività.

## Panoramica di Collaboratore attività

I collaboratori task sono un modo per assegnare agenti MCP a task specifici in Workfront. Puoi configurare l’agente in un’app come Copilot Studio, Claude o Writer.ai, quindi collegare l’agente a Workfront come Collaboratore attività. È quindi possibile assegnarla alle attività come se si trattasse di un utente.

Alcuni flussi di lavoro di esempio possono includere:

* Rileva le immagini caricate su un’attività, genera varianti in base ai criteri forniti all’agente e carica le nuove immagini nell’attività.
* Generazione della copia da una descrizione dell&#39;attività, esame della copia in base alle linee guida configurate nell&#39;agente e registrazione della copia nel flusso di aggiornamento.
* Lettura dei dettagli di un evento, identificazione dei dettagli mancanti e pubblicazione nel flusso di aggiornamento di domande sui dettagli mancanti.

>[!NOTE]
>
>* Dettagli specifici sulle responsabilità e sulle capacità di un agente sono configurati nell’applicazione in cui viene creato l’agente, non in Workfront.
>* I collaboratori attività supportano attualmente gli agenti creati in Copilot Studio, Claude e Writer.ai.
>* Durante la configurazione di un agente in Copilot Studio, è necessario impostare la protezione su **Nessuna autenticazione**.
>* Per informazioni e istruzioni sulla creazione di un collaboratore attività in Workfront, vedere [Configurare un collaboratore attività](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) nell&#39;articolo Configurare i collaboratori IA.

## Trigger di avvio di Collaborator attività

Quando un collaboratore di task viene assegnato a un task, inizia a lavorare quando si verifica una delle seguenti situazioni:

* Il Collaboratore attività è assegnato a un&#39;attività pronta per l&#39;avvio. Se ad esempio l&#39;attività ha predecessori, questi ultimi saranno completati.
* Il Collaboratore task e un utente vengono assegnati a un task e il Collaboratore task viene assegnato per primo.
* Un&#39;attività a cui è già assegnato un Collaboratore attività diventa pronta per l&#39;avvio. Se ad esempio l&#39;attività ha predecessori, questi ultimi saranno completati.
* Un task a cui sono già assegnati un collaboratore e un utente diventa pronto per iniziare. Se ad esempio l&#39;attività ha predecessori, questi ultimi saranno completati.
* Un utente e un Collaboratore attività vengono assegnati a un&#39;attività e l&#39;utente viene rimosso.
* A un task vengono assegnati un utente e un collaboratore task e il collaboratore task viene impostato come assegnatario principale del task.

Le situazioni seguenti non determinano l&#39;inizio del lavoro del task da parte di Collaboratore task:

* Un Collaboratore attività viene assegnato a un&#39;attività a cui è già stato assegnato un utente.
* Un Collaboratore attività è @mentioned in un&#39;attività.
* Un Collaboratore attività viene assegnato a un&#39;attività a cui è già stato assegnato un Collaboratore attività. In questo caso, solo il primo Collaboratore attività assegnato inizia a lavorare sull&#39;attività.
* Un Collaboratore attività viene assegnato a un&#39;attività che non è pronta per l&#39;avvio. Ad esempio, se l&#39;attività ha predecessori, questi non sono ancora completi.

## Assegnare un collaboratore a un task

I collaboratori delle attività vengono assegnati alle attività nello stesso modo in cui vengono assegnati gli utenti.

Quando si cerca un Collaboratore attività nell&#39;elenco degli assegnatari disponibili, il nome del Collaboratore attività è solo un nome.

Per istruzioni, vedere [Assegnare attività](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).
