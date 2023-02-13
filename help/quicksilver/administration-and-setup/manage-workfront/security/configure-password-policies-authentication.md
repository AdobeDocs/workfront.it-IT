---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurare i criteri password per l'autenticazione
description: In qualità di amministratore di Adobe Workfront, puoi configurare le opzioni relative ai criteri per le password per personalizzare l’esperienza di autenticazione nel sistema Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 1%

---

# Configurare i criteri password per l&#39;autenticazione

{{important-admin-console-onboard}}

In qualità di amministratore di Adobe Workfront, puoi configurare le opzioni relative ai criteri per le password per personalizzare l’esperienza di autenticazione nel sistema Workfront.

È consigliabile configurare le preferenze di autenticazione durante l’implementazione di Workfront e solo occasionalmente rivisitarle successivamente.

Le funzionalità di gestione delle password migliorate saranno presto disponibili o potrebbero già essere disponibili per la tua organizzazione. Utilizza una delle sezioni seguenti, a seconda che l’organizzazione abbia accesso o meno alla nuova esperienza di autenticazione.

## Requisiti di accesso

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare l’autenticazione (disponibile per tutti i clienti) {#configure-authentication-available-for-all-customers}

Vengono visualizzate le opzioni di autenticazione per tutti i clienti. Le funzionalità di gestione delle password migliorate saranno presto disponibili o potrebbero già essere disponibili per la tua organizzazione, come descritto nella sezione [Configurare l’autenticazione avanzata (disponibile a breve)](#configure-enhanced-authentication-coming-soon) in questo articolo.

Per configurare le preferenze di autenticazione:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** > **Autenticazione**.

1. Seleziona uno dei campi seguenti per stabilire le impostazioni di autenticazione per la tua organizzazione:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Impone agli utenti di reimpostare la password ogni <em>&lt;value&gt;</em> giorni</td> 
      <td>Questo stabilisce l'intervallo di tempo entro il quale gli utenti possono reimpostare la propria password Workfront. Per impostazione predefinita, questa opzione è disabilitata. Quando lo abiliti, puoi scegliere tra 30, 60, 90, 120, 180 giorni. Il valore predefinito è 30 giorni.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non consentire agli utenti di impostare la stessa password di una qualsiasi delle loro precedenti <em>&lt;value&gt;</em> password</td> 
      <td> <p>Questo campo impedisce agli utenti di riutilizzare le password per un determinato numero di reinsiemi. Per impostazione predefinita, questo campo è disabilitato. Se lo si abilita, è possibile impostare questo valore su 5, 10 o 15 reinsiemi prima che una password possa essere riutilizzata.</p> <p>Quando questa opzione è selezionata, gli utenti non possono reimpostare le password più di una volta al giorno</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Se una password errata viene immessa cinque volte consecutive, bloccare l'account per <em>&lt;value&gt;</em> minuti: </td> 
      <td> <p>Seleziona per quanto tempo un utente verrà bloccato fuori da Workfront dopo aver inserito una password errata cinque volte consecutive. Per impostazione predefinita, questa opzione è attivata e il tempo di attesa è di 10 minuti. È possibile bloccare gli account per 10 minuti, 30 minuti, 1 ora, 8 ore o 24 ore. </p> <p>Il ripristino manuale della password per l’utente sostituisce questo valore di attesa predefinito. <br>Gli utenti possono reimpostare le proprie password quando vengono bloccati tramite la schermata di accesso. Per ulteriori informazioni su come reimpostare la password, se l'hanno dimenticata, consulta <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Ripristino della password</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le password devono contenere almeno <em>&lt;value&gt;</em> diversi tipi di caratteri:</td> 
      <td> <p>Determina il livello di sicurezza delle password utente grazie alla possibilità di selezionare il numero di diversi tipi di caratteri richiesti nelle password.</p> <p>Impossibile utilizzare una parola dizionario riconoscibile come password.<br>Per impostazione predefinita, Workfront richiede che almeno 2 dei seguenti caratteri siano presenti nelle password (è inoltre possibile richiedere che 3 di questi caratteri siano presenti per una password valida): </p> 
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

## Configurare l’autenticazione avanzata (disponibile a breve) {#configure-enhanced-authentication-coming-soon}

Questa sezione descrive l’esperienza di autenticazione avanzata, che potrebbe non essere ancora disponibile per la tua organizzazione. Se la tua organizzazione non è stata migrata alla nuova esperienza di autenticazione, devi configurare le impostazioni di autenticazione come descritto in [Configurare l’autenticazione (disponibile per tutti i clienti)](#configure-authentication-available-for-all-customers).

Per configurare le preferenze di autenticazione avanzate:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** > **Autenticazione avanzata**.
1. In **Lunghezza password** immettere il numero minimo di caratteri necessari per una password valida.

   Workfront richiede almeno 6 caratteri.

1. (Facoltativo) In **Requisiti per le password** selezionare i tipi di caratteri richiesti nelle password utente.

   È possibile aumentare l&#39;intensità delle password utente richiedendo uno o tutti i tipi di caratteri nella sezione Password Requirements . Sono disponibili le seguenti opzioni:

   | Lettere minuscole | Richiedi almeno una lettera minuscola |
   |---|---|
   | Lettere maiuscole | Richiedi almeno una lettera maiuscola |
   | Numeri | Richiedi almeno un numero |
   | Caratteri speciali | Richiedi almeno un carattere speciale |

   {style=&quot;table-layout:auto&quot;}

1. Fai clic su **Salva**.
