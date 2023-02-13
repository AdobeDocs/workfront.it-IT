---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurare le informazioni di base per il sistema
description: Per configurare il sistema Adobe Workfront, puoi gestire i dettagli dell’organizzazione nella sezione Informazioni di base della pagina Informazioni cliente .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 2%

---

# Configurare le informazioni di base per il sistema

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Per configurare il sistema Adobe Workfront, puoi gestire i dettagli dell’organizzazione nella sezione Informazioni di base della pagina Informazioni cliente .

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> <col> 
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
   <td> <p>Devi essere un amministratore Workfront. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Accedere alle informazioni sul cliente

Il cliente rappresenta l’istanza Workfront per la tua organizzazione. Le opzioni in quest&#39;area sono uniche per te, come cliente di Workfront.

Per accedere alla pagina Informazioni cliente:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Sistema** > **Informazioni cliente**.

   A seconda del piano Workfront acquistato, alcune sezioni potrebbero mancare nella pagina Informazioni cliente . Contatta il rappresentante commerciale di riferimento per scoprire quale piano Workfront utilizza la tua organizzazione.

   Le sezioni disponibili nell&#39;area Informazioni cliente sono:

   * **Informazioni di base**

      Per informazioni sulla configurazione delle informazioni di base in Workfront, consulta [Configurare le informazioni di base](#configure-basic-info).

   * **Impostazioni chiavi API**

      Per informazioni sulle impostazioni delle chiavi API, vedi [Gestire le chiavi API](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **Elenco IP consentiti**

      Per informazioni sull’aggiunta degli indirizzi IP al tuo inserire nell&#39;elenco Consentiti per sapere dove gli utenti possono accedere a Workfront, consulta [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **Licenza**

      Per informazioni sulle licenze, vedi [Gestione delle licenze disponibili nel sistema](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## Configurare le informazioni di base {#configure-basic-info}

All’interno dell’area Informazioni di base della pagina Informazioni cliente, alcuni dettagli sul cliente sono configurati da Workfront e vengono visualizzati in modalità di sola lettura. Puoi configurare altri dettagli da te. Tutte le opzioni modificabili in questa area hanno un effetto globale su tutti gli utenti di Workfront.

Per configurare la sezione Informazioni di base nell&#39;area Informazioni cliente:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Sistema** > **Informazioni cliente**.

1. In **Informazioni di base** nella parte superiore della sezione **Informazioni cliente** trova le seguenti informazioni sull’istanza con Workfront:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td>Il nome della tua organizzazione, che corrisponde anche al nome della tua azienda. Questo viene aggiunto da Workfront e non può essere modificato.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cluster Setup </td> 
      <td>Il numero del cluster per l'istanza.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">E-mail ammin.</td> 
      <td> <p>L’indirizzo e-mail del tuo amministratore Workfront. Puoi modificare questo campo in modo che corrisponda all’indirizzo e-mail di uno dei tuoi amministratori di Workfront. L’utente associato a questo indirizzo e-mail è considerato l’amministratore principale di Workfront del sistema Workfront. Qualsiasi comunicazione a livello di sito da Workfront viene indirizzata a questo indirizzo e-mail, quindi è importante mantenerlo aggiornato.</p> <p><b>NOTA</b>: Non puoi disattivare, eliminare o modificare il livello di accesso dell’utente associato all’e-mail di amministrazione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dominio</td> 
      <td> <p>Il dominio viene impostato da Workfront al momento della creazione dell’account.</p> <p>Il dominio identifica il sottodominio univoco dell’URL utilizzato per accedere a Workfront.<p>Ad esempio, se alla tua organizzazione è stato assegnato il dominio "mycompany", l’URL che utilizzi per accedere a Workfront è <i>https://mycompany.my.workfront.com.</i></p><p>Non puoi modificare il dominio da solo. Se desideri modificare il dominio, puoi contattare l’Assistenza clienti Workfront. Per ulteriori informazioni su come contattare l’Assistenza clienti Workfront, consulta <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contatta l’Assistenza clienti</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Time Zone</td> 
      <td> <p>Questo è il fuso orario predefinito dell’istanza Workfront. Puoi modificare questo campo in modo che corrisponda al fuso orario della posizione Workfront principale. Il fuso orario selezionato determina quanto segue: </p> 
       <ul> 
        <li>Data e ora visualizzate nelle e-mail in uscita</li> 
        <li>Fuso orario predefinito per i nuovi utenti al momento della creazione</li> 
       </ul> <p>Gli utenti possono modificare il fuso orario per la propria istanza Workfront sotto il proprio profilo. Quando gli utenti modificano il loro fuso orario, la data e l’ora nelle e-mail da Workfront corrispondono alle loro preferenze di profilo. Per ulteriori informazioni sulla modifica delle preferenze del profilo utente, consulta <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurare le impostazioni personali</a>. Viene selezionato come fuso orario predefinito al momento della creazione di una nuova pianificazione. Per ulteriori informazioni sulla creazione delle pianificazioni, consulta <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>.</p> <p>Per informazioni sull'utilizzo delle pianificazioni per aiutare gli utenti a collaborare in Workfront in diversi fusi orari, vedi <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Utilizzo di fusi orari diversi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zona</td> 
      <td>Controlla la lingua, la data e il formato del numero utilizzati nei messaggi e-mail in uscita. Le impostazioni internazionali selezionate in questo caso sono le impostazioni internazionali predefinite al momento della creazione dei nuovi utenti. Gli utenti possono modificare le impostazioni internazionali nel proprio profilo utente. Quando gli utenti modificano le impostazioni internazionali, la lingua, la data e il formato dei numeri nei loro messaggi e-mail da Workfront corrispondono alle loro preferenze di profilo. Per ulteriori informazioni sulla modifica delle preferenze del profilo, consulta <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurare le impostazioni personali</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quota archivio</td> 
      <td> <p>Si tratta della quantità di spazio di archiviazione dei documenti disponibile nell'istanza Workfront.<br>La quota contiene i documenti caricati direttamente in Workfront.<br>Non include:</p> 
       <ul> 
        <li>Documenti collegati a Workfront da qualsiasi altro provider di servizi di terze parti (SharePoint, Google Drive, Webdam, Box, Dropbox, qualsiasi altro provider di gestione delle risorse dei documenti).</li> 
        <li>Dati di Workfront (progetti, attività, problemi, utenti e così via).</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versione prodotto</td> 
      <td>Questo è il tipo di istanza Workfront che ti viene assegnato. La versione di prodotto per la maggior parte dei clienti Workfront è <strong>Enterprise</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.
