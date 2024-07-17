---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurare le informazioni di base per il sistema
description: Durante la configurazione del sistema Adobe Workfront, puoi gestire i dettagli dell’organizzazione nella sezione Informazioni di base della pagina Informazioni cliente.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 1%

---

# Configurare le informazioni di base per il sistema

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Durante la configurazione del sistema Adobe Workfront, puoi gestire i dettagli dell’organizzazione nella sezione Informazioni di base della pagina Informazioni cliente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td>
   <p>Nuovo: Standard</p>
   Oppure
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## Accedi a informazioni cliente

Il cliente rappresenta l’istanza di Workfront per la tua organizzazione. Le opzioni disponibili in quest&#39;area sono specifiche per l&#39;utente, in quanto cliente di Workfront.

Per accedere alla pagina Informazioni cliente:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Sistema** > **Informazioni cliente**.

   A seconda del piano Workfront acquistato, alcune sezioni potrebbero non essere presenti nella pagina Informazioni cliente. Se hai bisogno di sapere quale piano Workfront utilizza la tua organizzazione, contatta il rappresentante del tuo account.

   Le sezioni disponibili nell’area Informazioni cliente sono:

   * **Informazioni di base**

     Per informazioni sulla configurazione delle informazioni di base in Workfront, vedere [Configurare le informazioni di base](#configure-basic-info).

   * **Impostazioni chiave API**

     Per informazioni sulle impostazioni delle chiavi API, vedere [Gestione chiavi API](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **Inserisco nell&#39;elenco Consentiti IP**

     Per informazioni sull&#39;aggiunta degli indirizzi IP al inserisco nell&#39;elenco Consentiti di accesso degli utenti a Workfront, vedere [Configurare il inserisco nell&#39;elenco Consentiti di accesso del firewall all&#39;interno del sistema di gestione delle relazioni con i clienti](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **Licenza**

     Per informazioni sulle licenze, vedere [Gestire le licenze disponibili nel sistema](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## Configura informazioni di base {#configure-basic-info}

Nell’area Informazioni di base della pagina Informazioni cliente, alcuni dettagli sul cliente sono configurati da Workfront e vengono visualizzati in modalità di sola lettura. Puoi configurare altri dettagli. Tutte le opzioni modificabili in quest&#39;area hanno un effetto globale su tutti gli utenti di Workfront.

Per configurare la sezione Informazioni di base nell&#39;area Informazioni cliente:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Sistema** > **Informazioni cliente**.

1. Nella sezione **Informazioni di base** nella parte superiore della pagina **Informazioni cliente**, trova le seguenti informazioni sull&#39;istanza con Workfront:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td>Il nome dell’organizzazione, che corrisponde anche al nome della tua azienda. Questo viene aggiunto da Workfront e non può essere modificato.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cluster Setup </td> 
      <td>Numero del cluster per l'istanza.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">E-mail ammin.</td> 
      <td> <p>Indirizzo e-mail dell’amministratore di Workfront. Puoi modificare questo campo in modo che corrisponda all’indirizzo e-mail di uno dei tuoi amministratori di Workfront. L’utente associato a questo indirizzo e-mail è considerato l’amministratore principale di Workfront del sistema Workfront. Qualsiasi comunicazione a livello di sito da parte di Workfront viene indirizzata a questo indirizzo e-mail, pertanto è importante mantenerlo aggiornato.</p> <p><b>NOTA</b>: non puoi disattivare, eliminare o modificare il livello di accesso dell'utente associato all'e-mail dell'amministratore.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dominio</td> 
      <td> <p>Il dominio viene impostato da Workfront al momento della creazione dell’account.</p> <p>Il dominio identifica il sottodominio univoco dell’URL utilizzato per accedere a Workfront.<p>Ad esempio, se all'organizzazione è stato assegnato il dominio "mycompany", l'URL utilizzato per accedere a Workfront è <i>https://mycompany.my.workfront.com.</i></p><p>Non puoi modificare il dominio da solo. Se desideri modificare il dominio, puoi contattare l’Assistenza clienti Workfront. Per ulteriori informazioni su come contattare l'Assistenza clienti Workfront, vedere <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contattare l'Assistenza clienti</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fuso orario</td> 
      <td> <p>Questo è il fuso orario predefinito dell’istanza Workfront. Puoi modificare questo campo in modo che corrisponda al fuso orario della posizione principale di Workfront. Il fuso orario selezionato determina quanto segue: </p> 
       <ul> 
        <li>Data e ora visualizzate nelle e-mail in uscita</li> 
        <li>Fuso orario predefinito per i nuovi utenti al momento della creazione</li> 
       </ul> <p>Gli utenti possono modificare il fuso orario per la propria istanza di Workfront nel proprio profilo. Quando gli utenti modificano il proprio fuso orario, la data e l’ora nelle e-mail provenienti da Workfront corrispondono alle preferenze del profilo. Per ulteriori informazioni sulla modifica delle preferenze del profilo utente, vedere <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurare le impostazioni personali</a>. Viene selezionato come fuso orario predefinito quando si crea una nuova pianificazione. Per ulteriori informazioni sulla creazione di pianificazioni, vedere <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>.</p> <p>Per informazioni sull'utilizzo delle pianificazioni per consentire agli utenti di collaborare in Workfront con fusi orari diversi, vedere <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Utilizzo con fusi orari diversi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zona</td> 
      <td>Controlla la lingua, la data e il formato numerico utilizzati nei messaggi e-mail in uscita. La lingua selezionata è quella predefinita al momento della creazione di nuovi utenti. Gli utenti possono modificare le proprie impostazioni locali nel proprio profilo utente. Quando gli utenti modificano le impostazioni locali, la lingua, la data e il formato del numero nelle e-mail inviate da Workfront corrispondono alle preferenze del profilo. Per ulteriori informazioni sulla modifica delle preferenze del profilo, vedere <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurare le impostazioni personali</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quota archivio</td> 
      <td> <p>Quantità di spazio di archiviazione dei documenti disponibile nell'istanza di Workfront.<br>La quota contiene documenti caricati direttamente in Workfront.<br>Non include:</p> 
       <ul> 
        <li>Documenti collegati a Workfront da qualsiasi altro provider di servizi di terze parti (SharePoint, Google Drive, Webdam, Box, Dropbox o qualsiasi altro provider di Document Asset Management).</li> 
        <li>I tuoi dati Workfront (progetti, attività, problemi, utenti e così via).</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versione prodotto</td> 
      <td>Questo è il tipo di istanza di Workfront che ti viene assegnata. La versione del prodotto per la maggior parte dei clienti Workfront è <strong>Enterprise</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.
