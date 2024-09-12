---
title: Registri di controllo
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: In qualità di amministratore di Adobe Workfront, puoi tenere traccia delle modifiche utente attivate nel sistema negli ultimi 90 giorni utilizzando i registri di audit.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 3%

---

# Registri di audit

<!--Audited: 01/2024-->

In qualità di amministratore di Adobe Workfront, puoi tenere traccia delle modifiche utente attivate nel sistema negli ultimi 90 giorni utilizzando i registri di audit descritti di seguito.

Per istruzioni su come visualizzare e filtrare ciò che si desidera visualizzare in questi registri di controllo, vedere [Visualizzare ed esportare i registri di controllo](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Informazioni disponibili in un registro di audit

In ogni voce del registro di controllo vengono registrati i campi riportati di seguito.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Data e Ora</td> 
   <td>Quando si è verificata l’azione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo di accesso</td> 
   <td>Tipo di registro di controllo, ad esempio Livello di accesso o Modulo personalizzato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome utente</td> 
   <td> <p>Nome dell’utente che ha eseguito l’azione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Azione</td> 
   <td> Azioni eseguite dall'utente, ad esempio Modifica, Crea ed Elimina. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Oggetto</td> 
   <td> Nome dell’oggetto interessato dall’azione. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dettagli</td> 
   <td>Dettagli aggiuntivi sull’azione. Passa il puntatore del mouse sul testo per leggere il messaggio completo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Indirizzo IP</td> 
   <td> <p>Indirizzo IP dell’utente che ha eseguito l’azione al momento dell’azione.</p> <p>L'indirizzo IP non è disponibile per alcune azioni di sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipi di registro di controllo e azioni che li attivano

* [Livello d&#39;Accesso](#access-level)
* [Regole aziendali](#business-rules)
* [Società](#company)
* [Condizione](#condition)
* [Campo personalizzato](#custom-field)
* [Modulo personalizzato](#custom-forms)
* [Sezione personalizzata](#custom-section)
* [Tasso di cambio](#exchange-rate)
* [Gruppo](#group)
* [Ruoli](#job-roles)
* [Tentativo di accesso](#login-attempt)
* [Priorità](#priority)
* [Preferenza progetto](#project-preference)
* [Gravità](#severity)
* [Stato](#status)
* [Preferenze attività e problemi](#tasks-issues-preferences)
* [Utente](#user)

### Livello di accesso {#access-level}

Il sistema genera una voce di registro del livello di accesso quando un utente esegue una delle seguenti operazioni:

* Crea un livello di accesso
* Elimina un livello di accesso
* Modifica un livello di accesso:

   * Modifica il tipo di licenza
   * Modifica le autorizzazioni per progetti, attività, problemi, Portfoli, programmi, report, documenti, utenti o modelli

     >[!NOTE]
     >
     >Il sistema non registra alcuna modifica delle autorizzazioni per Financial Data o all&#39;interno dei seguenti tipi di accesso: Visualizza e Modifica.
     >
     >Ad esempio, se un utente modifica il tipo di accesso Planner da Vista a Modifica, il sistema non visualizza le informazioni contenute nel menu a discesa Ottimizza impostazioni.

### Regole aziendali

Le regole business sono disponibili solo per i clienti che hanno acquistato un piano Workfront Ultimate. Per ulteriori informazioni, vedere [Creare e modificare le regole business](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

Il sistema genera una voce del registro di controllo Regola aziendale quando un utente esegue una delle operazioni seguenti:

* Crea una regola business
* Modifica una regola business:

   * Rinomina
   * Aggiunge o rimuove espressioni
   * Modifica un trigger

* Elimina una regola business

### Azienda {#company}

Il sistema genera una voce del registro di audit aziendale quando un utente effettua una delle seguenti operazioni:

* Crea una società
* Cambia una società:

   * Rinomina
   * Aggiunge o rimuove membri
   * Aggiunge, modifica o elimina il valore nel relativo campo Gruppo
   * Aggiunge o modifica una tariffa di fatturazione della società per una mansione
   * Rimuove una tariffa di fatturazione della società per una mansione
   * Imposta la società come società principale per l&#39;organizzazione
   * Allega o rimuove un modulo personalizzato

* Elimina una società

Per ulteriori informazioni sugli stati, vedere [Panoramica sugli stati](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Condizione {#condition}

Il sistema genera una voce del registro di controllo Condizione quando un utente esegue una delle seguenti operazioni:

* Crea una condizione
* Modifica una condizione:

   * Modifica il nome
   * Cambia il colore
   * Imposta come predefinito
   * Modifica o rimuove la descrizione della condizione
   * Nasconde o mostra la condizione

* Elimina una condizione

Per ulteriori informazioni sulla configurazione delle mansioni, vedere [Creare o modificare una condizione personalizzata](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### Campo personalizzato {#custom-field}

Il sistema genera una voce del registro di controllo del campo personalizzato quando un utente esegue una delle seguenti operazioni:

* Crea un campo personalizzato
* Modifica un campo personalizzato:

   * Modifica il nome, l&#39;etichetta, le istruzioni o il formato
   * Modifica il tipo di visualizzazione

     Questa opzione è disponibile solo se il campo è di uno dei tipi seguenti: riga singola, paragrafo, elenco a discesa, casella di controllo, pulsante di opzione

   * Modifica le dimensioni del campo

     Questa opzione è disponibile solo se il campo è di uno dei tipi seguenti: riga singola, paragrafo, testo con formattazione

   * Aggiunge, rimuove o nasconde una scelta di campo.
   * Modifica un&#39;etichetta o un valore di scelta del campo
   * Configura la scelta del campo da selezionare o meno per impostazione predefinita
   * Configura un campo a discesa per consentire più selezioni o una singola selezione
   * Configura un campo data per visualizzare o meno l’ora del giorno
   * Modifica il collegamento ipertestuale o modifica il valore in un campo di testo descrittivo

* Elimina un campo personalizzato
* Condivide un campo personalizzato

### Modulo personalizzato {#custom-form}

Il sistema genera una voce del registro di controllo di Forms personalizzato quando un utente esegue una delle seguenti operazioni:

* Crea un modulo personalizzato
* Modifica un modulo personalizzato:

   * Modifica il nome o la descrizione
   * Abilita o disabilita è attivo
   * Aggiunge o rimuove un campo o una sezione
   * Per una sezione personalizzata, modifica un’impostazione in Impostazioni aggiuntive
   * Modifica un campo in obbligatorio o non obbligatorio
   * Modifica un calcolo in un campo personalizzato
   * Nasconde o visualizza la formula associata a un campo calcolato nel testo delle istruzioni al passaggio del mouse
   * Attiva o disattiva Aggiorna calcoli precedenti
   * Aggiunge o modifica la logica di salto o di visualizzazione.

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Elimina un modulo personalizzato
* Condivide un modulo personalizzato

### Sezione personalizzata {#custom-section}

Il sistema genera una voce del registro di controllo Sezione personalizzata quando un utente esegue una delle seguenti azioni in un modulo personalizzato:

* Crea una sezione personalizzata
* Modifica il nome o la descrizione di una sezione personalizzata
* Elimina una sezione personalizzata

Per informazioni sulle sezioni personalizzate nei moduli personalizzati, vedere [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Tasso di cambio {#exchange-rate}

Il sistema genera una voce del registro di controllo Tasso di cambio quando un utente esegue una delle seguenti operazioni:

* Crea un tasso di cambio
* Modifica un tasso di cambio:

   * Aggiunge una valuta
   * Modifica il tasso di cambio per la valuta
   * Imposta la valuta come valuta di base (predefinita) per tutti i progetti e i report nel sistema

* Elimina un tasso di cambio

Per ulteriori informazioni sulla configurazione dei tassi di cambio, vedere [Impostare i tassi di cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Gruppo {#group}

Il sistema genera una voce del registro di controllo Gruppo quando un utente esegue una delle seguenti operazioni:

* Crea un gruppo
* Elimina un gruppo
* Modifica un gruppo:

   * Aggiunge o rimuove utenti
   * Aggiunge o rimuove sottogruppi

### Ruoli {#job-roles}

Il sistema genera una voce del registro di controllo Ruoli processo quando un utente esegue una delle seguenti operazioni:

* Crea una mansione
* Cambia una mansione:

   * Modifica il nome
   * Aggiunge, modifica o rimuove la descrizione.
   * Aggiunge, modifica o rimuove il costo orario (Costo orario).
   * Aggiunge, modifica o rimuove la tariffa di fatturazione (Fatturazione oraria).

* Elimina una mansione

Per ulteriori informazioni sulla configurazione dei ruoli, vedere [Creare e gestire i ruoli](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### Tentativo di accesso {#login-attempt}

Il sistema genera una voce del registro di controllo Tentativo di accesso quando un utente esegue una delle seguenti operazioni:

* Effettua l’accesso, esce o non riesce dopo un tentativo di accesso in Workfront (in un browser e nell’app mobile).
* Effettua l’accesso, si disconnette o non riesce dopo un tentativo di accesso nell’integrazione con Workfront (ad esempio Workfront per Slack e Workfront per Salesforce).
* Accedi o esce dall’API Workfront

I registri dei tentativi di accesso non vengono registrati quando un amministratore di Workfront utilizza la funzione Accedi come.

>[!NOTE]
>
>Questa opzione non è disponibile se l’organizzazione è stata integrata in Adobe Admin Console. Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

### Priorità {#priority}

Il sistema genera una voce del registro di controllo Priority quando un utente esegue una delle seguenti operazioni:

* Crea una priorità
* Modifica una priorità:

   * Modifica il nome
   * Cambia il colore
   * Imposta come predefinito
   * Aggiunge, modifica o rimuove la descrizione della priorità
   * Nasconde o mostra la priorità

* Elimina una priorità

Per ulteriori informazioni sulla configurazione delle priorità, vedere [Creare e personalizzare le priorità](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### Preferenza di progetto {#project-preference}

Il sistema genera una voce del registro di controllo Preferenze progetto quando un utente esegue una delle seguenti operazioni:

* Crea un trimestre personalizzato
* Modifica le preferenze di un progetto:

   * Blocca o sblocca
   * Modifica una delle impostazioni
   * Abilita, disabilita o modifica l&#39;elemento
   * Modifica un calcolo della sequenza temporale

* Elimina un trimestre personalizzato

Per ulteriori informazioni sulle preferenze del progetto, vedere [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### Gravità {#severity}

Il sistema genera una voce del registro di controllo Gravità quando un utente esegue una delle seguenti operazioni:

* Crea una gravità del problema
* Modifica la gravità di un problema:

   * Modifica il nome
   * Cambia il colore
   * Imposta come predefinito
   * Modifica o rimuove la descrizione della gravità
   * Nasconde o mostra la gravità

* Elimina la gravità di un problema

Per ulteriori informazioni sulla configurazione delle mansioni, vedere [Creare o personalizzare le gravità dei problemi](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### Stato {#status}

Il sistema genera una voce del registro di controllo dello stato quando un utente esegue una delle seguenti operazioni:

* Crea uno stato a livello di sistema o di gruppo
* Modifica uno stato a livello di sistema o di gruppo:

   * Rinomina
   * Imposta lo stato predefinito
   * Blocca o sblocca
   * Nasconde o rivela
   * Modifica il colore o la descrizione

* Elimina uno stato a livello di sistema o di gruppo

Per ulteriori informazioni sugli stati, vedere [Panoramica sugli stati](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Preferenze attività e problemi {#tasks-issues-preferences}

Il sistema genera una voce del registro di controllo Preferenze attività e problemi quando un utente modifica una preferenza Attività e problemi in uno dei seguenti modi:

* Blocca o sblocca una preferenza
* Modifica l&#39;impostazione di una preferenza
* Modifica un&#39;impostazione di accesso per attività, problemi o richieste

Per ulteriori informazioni sulle preferenze per attività e problemi, vedere [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Utente {#user}

Il sistema genera una voce del registro di controllo utente quando un utente esegue una delle seguenti operazioni:

* Crea un utente

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >Questa opzione non è disponibile se l’organizzazione è stata integrata in Adobe Admin Console. Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

* Elimina un utente
* Modifica il livello di accesso, la società, il team o il gruppo di un utente
* Attiva un utente
* Disattiva un utente
