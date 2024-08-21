---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurare i criteri password per l’autenticazione
description: In qualità di amministratore di Adobe Workfront, puoi configurare le opzioni dei criteri per le password per personalizzare l’esperienza di autenticazione per il tuo sistema Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 2%

---

# Configurare i criteri password per l’autenticazione

{{important-admin-console-onboard}}

In qualità di amministratore di Adobe Workfront, puoi configurare le opzioni dei criteri per le password per personalizzare l’esperienza di autenticazione per il tuo sistema Workfront.

È consigliabile configurare le preferenze di autenticazione durante l’implementazione di Workfront e rivederle solo occasionalmente in seguito.

Le funzionalità di gestione delle password migliorate saranno presto disponibili o potrebbero già essere disponibili per la tua organizzazione. Utilizza una delle sezioni seguenti, a seconda che l’organizzazione abbia accesso o meno alla nuova esperienza di autenticazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configura autenticazione (disponibile per tutti i clienti) {#configure-authentication-available-for-all-customers}

Le opzioni di autenticazione vengono visualizzate per tutti i clienti. Le funzionalità di gestione delle password migliorate saranno presto disponibili o potrebbero già essere disponibili per la tua organizzazione, come descritto nella sezione [Configurare l&#39;autenticazione avanzata)](#configure-enhanced-authentication-coming-soon) in questo articolo.

Per configurare le preferenze di autenticazione:

{{step-1-to-setup}}

1. Fare clic su **Sistema** > **Autenticazione**.

1. Selezionare uno dei campi seguenti per definire le impostazioni di autenticazione per l&#39;organizzazione:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Obbliga gli utenti a reimpostare la password ogni <em>&lt;valore&gt;</em> giorni</td> 
      <td>Questo stabilisce l'intervallo di tempo per la reimpostazione della password Workfront da parte degli utenti. Per impostazione predefinita, questa opzione è disabilitata. Quando lo abiliti, puoi scegliere tra 30, 60, 90, 120, 180 giorni. Il valore predefinito è 30 giorni.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non consentire agli utenti di impostare la stessa password di una delle precedenti <em>&lt;valore&gt;</em> password</td> 
      <td> <p>Questo campo impedisce agli utenti di riutilizzare le password per un numero impostato di ripristini. Per impostazione predefinita, questo campo è disabilitato. Quando viene abilitata, è possibile impostare questo valore su 5, 10 o 15 ripristini prima di poter riutilizzare una password.</p> <p>Quando questa opzione è selezionata, gli utenti non possono reimpostare le password più di una volta in un dato giorno</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Se viene immessa una password non corretta per cinque volte consecutive, bloccare l'account per <em>&lt;valore&gt;</em> minuti: </td> 
      <td> <p>Seleziona per quanto tempo un utente verrà bloccato fuori da Workfront dopo aver inserito una password errata per cinque volte consecutive. Per impostazione predefinita, questa opzione è abilitata e il tempo di attesa è di 10 minuti. Puoi bloccare gli account per 10 minuti, 30 minuti, 1 ora, 8 ore o 24 ore. </p> <p>Il ripristino manuale della password dell’utente esclude questo valore di attesa predefinito. <br>Gli utenti possono reimpostare le proprie password quando vengono bloccate tramite la schermata di accesso. Per ulteriori informazioni su come reimpostare la password, vedere <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Reimpostare la password</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le password devono contenere almeno <em>&lt;valore&gt;</em> tipi diversi di caratteri:</td> 
      <td> <p>Determina la forza delle password utente consentendo di selezionare il numero di tipi diversi di caratteri richiesti nelle password.</p> <p>Impossibile utilizzare una parola del dizionario riconoscibile come password.<br>Per impostazione predefinita, Workfront richiede che almeno due dei seguenti caratteri siano presenti nelle password (è inoltre possibile richiedere che tre di questi caratteri siano presenti per una password valida): </p> 
       <ul> 
        <li>Caratteri maiuscoli</li> 
        <li>Caratteri minuscoli</li> 
        <li>Numeri</li> 
        <li>Simboli</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

## Configurare l’autenticazione avanzata{#configure-enhanced-authentication-coming-soon}

Questa sezione descrive l’esperienza di autenticazione avanzata, che potrebbe non essere ancora disponibile per la tua organizzazione. Se nell&#39;organizzazione non è stata eseguita la migrazione alla nuova esperienza di autenticazione, è necessario configurare le impostazioni di autenticazione come descritto in [Configurare l&#39;autenticazione (disponibile per tutti i clienti)](#configure-authentication-available-for-all-customers).

Per configurare le preferenze di autenticazione avanzate:

{{step-1-to-setup}}

1. Fare clic su **Sistema** > **Autenticazione avanzata**.
1. Nella casella **Lunghezza password** immettere il numero minimo di caratteri necessario per una password valida.

   Workfront richiede almeno 6 caratteri.

1. (Facoltativo) Nella sezione **Requisiti password**, seleziona i tipi di caratteri richiesti nelle password utente.

   È possibile aumentare il numero di password utente richiedendo uno o tutti i tipi di caratteri nella sezione Requisito password. Sono disponibili le seguenti opzioni:

   | Lettere minuscole | Richiedi almeno una lettera minuscola |
   |---|---|
   | Lettere maiuscole | Richiedi almeno una lettera maiuscola |
   | Numeri | Richiedi almeno un numero |
   | Caratteri speciali | Richiede almeno un carattere speciale |

   {style="table-layout:auto"}

1. Fai clic su **Salva**.
