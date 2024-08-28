---
title: "Panoramica dell’Assistente AI"
content-type: reference
description: Panoramica dell’Assistente AI
author: Becky
feature: Get Started with Workfront
source-git-commit: 09c05db7c6a5db7db74dd95ca323415f4318489d
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Panoramica dell’Assistente AI

L’Assistente AI di Workfront ti aiuta a svolgere il tuo lavoro offrendo informazioni e suggerimenti in-app in una conversazione in linguaggio naturale. L’Assistente AI può offrirti un’esperienza di lavoro più fluida grazie a

* Riepilogo di elementi di lavoro o documenti
* Ricerca di istruzioni o materiale di riferimento per i processi di lavoro
* Generazione o controllo di formule per i campi calcolati

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td><p>Nuovo: Qualsiasi</p>
       <p>oppure</p>
       <p>Corrente: non disponibile</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>oppure</p>
       <p>Corrente: non disponibile</p></td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).## Prerequisiti per l&#39;Assistente IA

## Prerequisiti per l’Assistente IA

Per abilitare l&#39;Assistente IA per la tua organizzazione, **tutti** i seguenti elementi devono essere applicati:

* La tua organizzazione deve aver eseguito la migrazione ad Adobe IMS (Identity Management System)
* L’esperienza unificata di Adobe deve essere abilitata
* La tua organizzazione deve disporre di un piano Select, Prime o Ultimate Workfront
* L&#39;Adobe deve disporre di un accordo Adobe Gen AI firmato nel file

  Per ulteriori informazioni sulla firma del contratto, consulta [Firmare il contratto di IA per l&#39;analisi dell&#39;Adobe](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) in questo articolo.

## Considerazioni sull’Assistente IA

* L’Assistente IA è sensibile al contesto per la pagina aperta. Ad esempio, l’immissione di &quot;Riepiloga questo progetto&quot; nell’Assistente IA in una pagina di progetto restituisce un riepilogo di tale progetto specifico.
* L’amministratore di Workfront deve abilitare l’Assistente IA per gli utenti dell’organizzazione. L’Assistente AI è abilitato tramite i livelli di accesso.

  Per ulteriori informazioni, vedere [Attivare o disattivare l&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* L&#39;Assistente di Workfront Planning AI dispone di funzioni diverse dall&#39;Assistente di Workfront AI.

  Per ulteriori informazioni sull&#39;Assistente di IA in Workfront Planning, vedere [Panoramica dell&#39;Assistente di IA di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).


## Funzionalità disponibile in AI Assistant

L’Assistente AI offre attualmente le seguenti funzionalità:

* Riepilogo di progetti, attività, problemi o documenti.

  Per ulteriori informazioni, vedere [Riepilogare utilizzando l&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Fornire istruzioni o informazioni di riferimento ricavate dalla documentazione di Workfront su Adobe Experience League.

  Per ulteriori informazioni, vedere [Ottenere assistenza dall&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Genera o perfeziona formule per i campi personalizzati calcolati.

  >[!NOTE]
  >
  >Questa funzionalità è disponibile solo per le organizzazioni che utilizzano Prime o Ultimate Workfront.

  Per ulteriori informazioni, vedere [Generare o modificare formule di campi calcolati con Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

## Accedi all’Assistente di AI

1. Nella parte superiore di qualsiasi pagina di Workfront, fare clic sull&#39;icona Assistente AI ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Digita la domanda o il prompt nel pannello a destra della schermata.

   Se non riesci a digitare in questo pannello, la tua organizzazione non dispone di un accordo Adobe Gen AI firmato su file.

1. Se l’assistente AI non fornisce la risposta necessaria, perfeziona la richiesta e riprova.

## Firma l&#39;accordo Adobe Gen AI

Se l’organizzazione non dispone di un accordo Adobe Gen AI firmato su file, l’Assistente AI non può essere abilitato per l’organizzazione.

Se un utente tenta di utilizzare l’Assistente IA quando il contratto di Adobe Gen AI non è stato firmato, visualizza un messaggio:

* Utenti: gli utenti vengono informati che l’Assistente IA non è stato abilitato per la loro organizzazione e che possono contattare il proprio amministratore Workfront per richiederlo per la loro organizzazione.
* Amministratori: gli amministratori vengono informati che non esiste un contratto Adobe Gen AI firmato e possono richiedere l’invio di una copia del contratto per la firma.

Per richiedere l&#39;accordo Adobe Gen AI:

1. In qualità di amministratore di Workfront, fare clic sull&#39;icona Assistente IA ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Inizia a digitare nel pannello Assistente AI.
1. Quando viene visualizzato il messaggio del contratto di Adobe Gen AI, fare clic su **Rivedi contratto**.
1. Immetti il nome e l’indirizzo e-mail della persona dell’organizzazione che firmerà l’accordo Adobe Gen AI.

   Il contratto verrà inviato a questa persona per la firma. Dopo la firma e la restituzione, l’Assistente IA viene abilitato per la tua organizzazione.


