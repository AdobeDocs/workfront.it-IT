---
title: Registri di controllo
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: In qualità di amministratore di Adobe Workfront, puoi tenere traccia dei cambiamenti utente attivati nel sistema negli ultimi 90 giorni utilizzando i registri di controllo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 4%

---

# Registri di controllo

In qualità di amministratore di Adobe Workfront, puoi tenere traccia dei cambiamenti utente attivati nel sistema negli ultimi 90 giorni utilizzando i registri di controllo descritti di seguito.

Per istruzioni su come visualizzare e filtrare ciò che si desidera visualizzare in questi registri di controllo, vedi [Visualizzare ed esportare i registri di controllo](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Informazioni disponibili in un registro di controllo

I campi seguenti vengono registrati in ogni voce del registro di controllo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Data e ora</td> 
   <td>Quando si è verificata l'azione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo di accesso</td> 
   <td>Tipo del registro di controllo, ad esempio Livello di accesso o Modulo personalizzato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome utente</td> 
   <td> <p>Nome dell’utente che ha eseguito l’azione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Azione</td> 
   <td> Azione eseguita dall’utente, ad esempio Modifica, Crea ed Elimina. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Oggetto</td> 
   <td> Nome dell’oggetto interessato a seguito dell’azione. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dettagli</td> 
   <td>Ulteriori dettagli sull'azione. Passa il puntatore del mouse sul testo per leggere il messaggio completo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Indirizzo IP</td> 
   <td> <p>Indirizzo IP dell’utente che ha eseguito l’azione al momento dell’azione.</p> <p>L'indirizzo IP non è disponibile per alcune azioni del sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipi di log di controllo e azioni che li attivano

* [Livello di accesso](#access-level)
* [Azienda](#company)
* [Condizione](#condition)
* Campo personalizzato [](#custom-field)
* [Moduli personalizzati](#custom-forms)
* [Sezione personalizzata](#custom-section)
* [Tasso di cambio](#exchange-rate)
* [Gruppo](#group)
* [Ruoli](#job-roles)
* [Tentativo di accesso](#login-attempt)
* [Priorità](#priority)
* [Preferenze progetto](#project-preferences)
* [Gravità](#severity)
* [Stato](#status)
* [Preferenze attività e problemi](#tasks-issues-preferences)
* [Utente](#user)

### Livello di accesso {#access-level}

Il sistema genera una voce di registro del livello di accesso quando un utente esegue una delle azioni seguenti:

* Crea un livello di accesso
* Elimina un livello di accesso
* Modifica un livello di accesso:

   * Modifica il tipo di licenza
   * Modifica le autorizzazioni per progetti, attività, problemi, Portfoli, programmi, rapporti, documenti, utenti o modelli

      >[!NOTE]
      >
      >Il sistema non registra alcuna modifica delle autorizzazioni in Dati finanziari o nei seguenti tipi di accesso: Visualizza e modifica.
      >
      >Ad esempio, se un utente modifica il tipo di accesso Planner da Visualizza a Modifica, il sistema non visualizzerà le informazioni contenute nel menu a discesa Ottimizza le impostazioni.

### Azienda {#company}

Il sistema genera una voce del registro di controllo dell&#39;azienda quando un utente effettua una delle seguenti operazioni:

* Crea una società
* Modifica un&#39;azienda:

   * Rinomina
   * Aggiunge o rimuove membri
   * Aggiunge, modifica o elimina il valore nel relativo campo Gruppo
   * Aggiunge o modifica un tasso di fatturazione aziendale per un ruolo di lavoro
   * Rimuove un tasso di fatturazione aziendale per un ruolo di lavoro
   * La imposta come società principale per l&#39;organizzazione
   * Allega o rimuove un modulo personalizzato

* Elimina una società

Per ulteriori informazioni sugli stati, consulta [Panoramica sugli stati](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Condizione {#condition}

Il sistema genera una voce del registro di controllo delle condizioni quando un utente esegue una delle seguenti azioni:

* Crea una condizione
* Modifica una condizione:

   * Cambia il nome
   * Cambia il colore
   * La imposta come predefinita
   * Modifica o rimuove la descrizione della condizione
   * Nasconde o mostra la condizione

* Elimina una condizione

Per ulteriori informazioni sulla configurazione dei ruoli di lavoro, consulta [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### Campo personalizzato {#custom-field}

Il sistema genera una voce del registro di controllo del campo personalizzato quando un utente esegue una delle azioni seguenti:

* Crea un campo personalizzato
* Modifica un campo personalizzato:

   * Modifica il nome, l&#39;etichetta, le istruzioni o il formato
   * Cambia il tipo di visualizzazione

      Questa opzione è disponibile solo se il campo è di uno dei seguenti tipi: riga singola, paragrafo, elenco a discesa, casella di controllo, pulsante di scelta

   * Modifica la dimensione del campo

      Questa opzione è disponibile solo se il campo è di uno dei seguenti tipi: riga singola, paragrafo, testo con formattazione

   * Aggiunge, rimuove o nasconde una scelta di campo
   * Modifica un’etichetta o un valore di scelta del campo
   * Configura la scelta del campo da selezionare o meno per impostazione predefinita
   * Configura un campo a discesa per consentire selezioni multiple o una singola selezione
   * Configura un campo data per visualizzare o meno l’ora del giorno
   * Modifica il collegamento ipertestuale o modifica il valore in un campo di testo descrittivo

* Elimina un campo personalizzato
* Condivide un campo personalizzato

### Moduli personalizzati {#custom-forms}

Il sistema genera una voce di registro di controllo Forms personalizzato quando un utente esegue una delle seguenti azioni:

* Crea un modulo personalizzato
* Modifica un modulo personalizzato:

   * Modifica il nome o la descrizione
   * Abilita o disabilita l&#39;attivazione
   * Aggiunge o rimuove un campo o una sezione
   * Per una sezione personalizzata, modifica un&#39;impostazione in Impostazioni aggiuntive
   * Cambia un campo in obbligatorio o non obbligatorio
   * Modifica un calcolo in un campo personalizzato
   * Nasconde o visualizza la formula associata a un campo calcolato nel testo al passaggio del mouse Istruzioni
   * Abilita o disabilita l&#39;aggiornamento dei calcoli precedenti
   * Aggiunge o modifica una logica di salto o di visualizzazione

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Elimina un modulo personalizzato
* Condivide un modulo personalizzato

### Sezione personalizzata {#custom-section}

Il sistema genera una voce di registro di controllo Sezione personalizzata quando un utente esegue una delle seguenti azioni in un modulo personalizzato:

* Crea una sezione personalizzata
* Modifica il nome o la descrizione di una sezione personalizzata
* Elimina una sezione personalizzata

Per informazioni sulle sezioni personalizzate nei moduli personalizzati, consulta [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

### Tasso di cambio {#exchange-rate}

Il sistema genera una voce del registro di controllo del tasso di cambio quando un utente esegue una delle seguenti azioni:

* Crea un tasso di cambio
* Modifica un tasso di cambio:

   * Aggiunge una valuta
   * Modifica il tasso della valuta
   * Imposta la valuta come valuta di base (predefinita) per tutti i progetti e i rapporti in tutto il sistema

* Elimina un tasso di cambio

Per ulteriori informazioni sulla configurazione dei tassi di cambio, vedere [Imposta i tassi di cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Gruppo {#group}

Il sistema genera una voce del registro di controllo del gruppo quando un utente esegue una delle seguenti azioni:

* Crea un gruppo
* Elimina un gruppo
* Modifica un gruppo:

   * Aggiunge o rimuove utenti
   * Aggiunge o rimuove sottogruppi

### Ruoli {#job-roles}

Il sistema genera una voce del registro di controllo Ruoli processo quando un utente esegue una delle seguenti azioni:

* Crea un ruolo di lavoro
* Modifica un ruolo di lavoro:

   * Cambia il nome
   * Aggiunge, modifica o rimuove la descrizione
   * Aggiunge, modifica o rimuove il costo all’ora (costo/ora)
   * Aggiunge, modifica o rimuove il tasso di fatturazione (Bill/Hr)

* Elimina un ruolo di lavoro

Per ulteriori informazioni sulla configurazione dei ruoli di lavoro, consulta [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### Tentativo di accesso {#login-attempt}

Il sistema genera una voce di registro di controllo del tentativo di accesso quando un utente esegue una delle seguenti azioni:

* Effettua l’accesso, disconnette o non riesce a eseguire un tentativo di accesso in Workfront (in un browser e nell’app mobile)
* Effettua l’accesso, disconnette o non riesce a eseguire un tentativo di accesso in qualsiasi integrazione di Workfront (come Workfront per Slack e Workfront per Salesforce)
* Accedi o disconnette dall’API Workfront

I registri dei tentativi di accesso non vengono registrati quando un amministratore di Workfront utilizza la funzione Accedi come.

>[!NOTE]
>
>Questa opzione non è disponibile se l’organizzazione è stata caricata in Adobe Admin Console. Per ulteriori informazioni, rivolgiti al tuo amministratore di rete o IT.

### Priorità {#priority}

Il sistema genera una voce del registro di controllo delle priorità quando un utente esegue una delle seguenti azioni:

* Crea una priorità
* Modifica una priorità:

   * Cambia il nome
   * Cambia il colore
   * La imposta come predefinita
   * Aggiunge, modifica o rimuove la descrizione della priorità
   * Nasconde o mostra la priorità

* Elimina una priorità

Per ulteriori informazioni sulla configurazione delle priorità, consulta [Creare e personalizzare le priorità](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### Preferenze progetto {#project-preferences}

Il sistema genera una voce del registro di controllo Preferenze progetto quando un utente esegue una delle seguenti azioni:

* Crea un trimestre personalizzato
* Modifica la preferenza di un progetto:

   * Blocca o sblocca
   * Modifica una delle impostazioni
   * Abilita, disabilita o modifica
   * Modifica un calcolo della timeline

* Elimina un trimestre personalizzato

Per ulteriori informazioni sulle preferenze del progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### Gravità {#severity}

Il sistema genera una voce del registro di controllo Gravità quando un utente esegue una delle seguenti azioni:

* Crea una gravità del problema
* Modifica la gravità di un problema:

   * Cambia il nome
   * Cambia il colore
   * La imposta come predefinita
   * Modifica o rimuove la descrizione della gravità
   * Nasconde o mostra la gravità

* Elimina la gravità di un problema

Per ulteriori informazioni sulla configurazione dei ruoli di lavoro, consulta [Creare o personalizzare le gravità dei problemi](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### Stato {#status}

Il sistema genera una voce del registro di controllo dello stato quando un utente esegue una delle seguenti azioni:

* Crea uno stato a livello di sistema o di gruppo
* Cambia uno stato a livello di sistema o gruppo:

   * Rinomina
   * Lo rende uno stato predefinito
   * Blocca o sblocca
   * Lo nasconde o lo nasconde
   * Modifica il colore o la descrizione

* Elimina uno stato a livello di sistema o di gruppo

Per ulteriori informazioni sugli stati, consulta [Panoramica sugli stati](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Preferenze attività e problemi {#tasks-issues-preferences}

Il sistema genera una voce del registro di controllo Preferenze attività e problemi quando un utente modifica una preferenza Attività e problemi in uno dei seguenti modi:

* Blocca o sblocca una preferenza
* Modifica l&#39;impostazione di una preferenza
* Modifica un&#39;impostazione di Access per attività, problemi o richieste

Per ulteriori informazioni sulle preferenze relative a attività e problemi, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Utente {#user}

Il sistema genera una voce del registro di controllo utente quando un utente esegue una delle seguenti azioni:

* Crea un utente

   <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

   >[!NOTE]
   >
   >Questa opzione non è disponibile se l’organizzazione è stata caricata in Adobe Admin Console. Per ulteriori informazioni, rivolgiti al tuo amministratore di rete o IT.

* Elimina un utente
* Modifica il livello di accesso, la società, il team o il gruppo di un utente
* Attiva un utente
* Disattiva un utente
