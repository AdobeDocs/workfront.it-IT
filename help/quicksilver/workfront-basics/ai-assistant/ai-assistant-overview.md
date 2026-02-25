---
title: Assistente IA in Workfront
content-type: reference
description: Scopri l’Assistente IA in Adobe Workfront
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: e8e10f02f77f6c1df9f0af380eb16cc6bbc3b5d1
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 100%

---

# Assistente IA in Workfront

L’Assistente IA di Workfront ti aiuta a svolgere il tuo lavoro offrendo informazioni e suggerimenti in-app tramite una conversazione in linguaggio naturale. L’Assistente IA può offrirti un’esperienza di lavoro più fluida grazie a

* Riepilogo di elementi di lavoro o documenti
* Individuazione di istruzioni o materiale di riferimento per i processi di lavoro
* Generazione o controllo di formule per i campi calcolati

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, devi disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront</td> 
   <td><p>Nuovo: qualsiasi</p>
       <p>oppure</p>
       <p>Corrente: non disponibile</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Nuovo: standard</p>
       <p>oppure</p>
       <p>Corrente: non disponibile</p></td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti per l’Assistente IA

Per abilitare l&#39;Assistente IA per la tua organizzazione, **tutti** i seguenti elementi devono essere applicati:

* L’organizzazione deve aver eseguito la migrazione ad Adobe IMS (Identity Management System)
* Adobe Unified Experience deve essere abilitata
* L’organizzazione deve disporre di un piano Workfront Ultimate, Prime o Select
* Adobe deve disporre di un accordo Adobe Gen AI firmato registrato

  Per ulteriori informazioni sulla firma dell’accordo, consulta [Firmare l’accordo di Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) in questo articolo.

## Considerazioni sull’Assistente IA

* L’Assistente IA agisce in base al contesto della pagina che hai aperto. Ad esempio, l’inserimento di “Riepiloga questo progetto” nell’Assistente IA in una pagina di progetto restituisce un riepilogo di tale progetto specifico.
* L’amministratore di Workfront deve abilitare l’Assistente IA per gli utenti dell’organizzazione. L’Assistente IA è abilitato tramite i livelli di accesso.

  Per ulteriori informazioni, consulta [Abilitare o disabilitare l’Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* L’Assistente IA nella Pianificazione di Workfront dispone di funzioni diverse da quello presente in Workfront.

  Per ulteriori informazioni sull’Assistente IA nella Pianificazione di Workfront, consulta [Panoramica dell’Assistente IA di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

* L’Assistente IA è attualmente disponibile solo in lingua inglese.


## Funzionalità disponibili nell’Assistente IA

L’Assistente IA offre attualmente le seguenti funzionalità:

* Riepilogo di progetti, attività, problemi o documenti.

  Per ulteriori informazioni, consulta [Riepilogare utilizzando l’Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Fornire istruzioni o informazioni di riferimento ricavate dalla documentazione di Workfront su Adobe Experience League.

  Per ulteriori informazioni, consulta [Ottenere aiuto dall’Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Individuazione di elementi specifici in Workfront.

  Per ulteriori informazioni, consulta [Utilizzare l’Assistente IA per lavorare su progetti, attività e problemi](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

* Generazione o ottimizzazione di formule per campi personalizzati calcolati.

  >[!NOTE]
  >
  >Questa funzionalità è disponibile solo per le organizzazioni con piani Workfront Prime o Ultimate.

  Per ulteriori informazioni, consulta [Generare o rivedere formule di campi calcolati con l’Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

* Riepilogo di aggiornamenti, documenti caricati e altre modifiche di rilievo apportate ai progetti entro i seguenti intervalli di tempo: 24 ore, 3 giorni, 7 giorni nelle Priorità.

Per ulteriori informazioni, consulta [Recuperare il lavoro nelle Priorità](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).


## Tipi di oggetto disponibili per l’Assistente IA

L’Assistente IA può eseguire query sui dati associati ai seguenti tipi di oggetto, se l’utente dispone delle autorizzazioni valide in Workfront:

* Portfolio
* Programmi
* Progetti
* Tasks
* Problemi
* Moduli personalizzati
* Utenti
* Record Pianificazione di Workfront


## Accedere all’Assistente IA

1. Nella parte superiore di qualsiasi pagina di Workfront, fai clic sull’icona dell’Assistente IA ![icona Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Digita la domanda o il prompt nel pannello a destra della schermata.

   Se non riesci a digitare in questo pannello, la tua organizzazione non dispone di un accordo Adobe Gen AI firmato registrato.

1. Se l’Assistente IA non fornisce la risposta necessaria, perfeziona il prompt e riprova.

## Firmare l’accordo Adobe Gen AI

Se la tua organizzazione non dispone di un accordo Adobe Gen AI firmato registrato, l’Assistente IA non può essere abilitato per la tua organizzazione.

Se un utente tenta di utilizzare l’Assistente IA quando l’accordo di Adobe Gen AI non è ancora firmato, visualizza un messaggio:

* Utenti: gli utenti vengono informati che l’Assistente IA non è abilitato per la loro organizzazione e che possono contattare il proprio amministratore Workfront per richiederlo.
* Amministratori: gli amministratori vengono informati che non è presente un accordo Adobe Gen AI firmato e possono richiedere l’invio di una copia dell’accordo per la firma.

Per richiedere l’accordo Adobe Gen AI:

1. In qualità di amministratore di Workfront, fai clic sull’icona dell’Assistente IA ![icona Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Inizia a digitare nel pannello dell’Assistente IA.
1. Quando viene visualizzato il messaggio dell’accordo di Adobe Gen AI, fai clic su **Rivedi accordo**.
1. Inserisci il nome e l’indirizzo e-mail della persona dell’organizzazione che firmerà l’accordo Adobe Gen AI.

   L’accordo verrà inviato a tale persona per la firma. Dopo la firma e la restituzione, l’accordo viene rivisto da Adobe, quindi l’Assistente IA viene abilitato per la tua organizzazione.

   >[!NOTE]
   >
   >Attendi 1-3 giorni lavorativi dopo la firma e la restituzione dell’accordo affinché Adobe possa rivedere e abilitare l’Assistente IA.

## Suggerimenti per la creazione di prompt nell’Assistente IA

Utilizza le seguenti parole chiave nei tuoi prompt per fornire contesto e aiutare a individuare le informazioni corrette. Le parole chiave non fanno distinzione tra maiuscole e minuscole.

Quando inserisci il prompt, includi la frase `using (keyword)`.

| Parola chiave | Effetto |
| --- | --- | 
| `workfront` | Interagisce con Workfront. |
| `planning` | Interagisce con Pianificazione di Workfront. |
| `help` | Restituisce informazioni dalla documentazione di Experience League. |
| `formula` | Controlla e restituisce le formule da utilizzare nei moduli personalizzati, Pianificazione o Configurazione. |
| `health` | Controlla lo stato del progetto con Project Health Advisor. |
| `summarize` | Riepiloga gli elementi, ad esempio quando viene caricato un file o riepilogato un progetto. |

>[!NOTE]
>
> Non tutte le parole chiave sono disponibili in tutte le aree.
>
>* La parola chiave `formula` è disponibile solo in Pianificazione, Configurazione e Generatore di moduli personalizzati.
>* La parola chiave `planning` è disponibile solo in Pianificazione di Workfront.





