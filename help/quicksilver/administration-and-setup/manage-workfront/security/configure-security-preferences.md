---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurare le preferenze di sicurezza del sistema
description: In qualità di amministratore di Adobe Workfront, puoi configurare le preferenze di protezione per il tuo sistema Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 04cf9d37c681398f5a0e2b9d7d45c0f8b93ab44b
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 5%

---

# Configurare le preferenze di sicurezza del sistema

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

In qualità di amministratore di Adobe Workfront, puoi configurare le preferenze di protezione per il tuo sistema Workfront:

* Accesso a Workfront da app mobili e altre applicazioni integrate
* Regole per incorporare Workfront in un iframe

Le modifiche apportate nelle preferenze di sistema hanno un impatto su tutti gli utenti del sistema e sulla loro esperienza in Workfront.

È consigliabile configurare le preferenze di sicurezza del sistema durante l’implementazione di Workfront e solo occasionalmente rivederle.

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

## Configurare le preferenze di sicurezza del sistema

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Sistema** > **Preferenze**.

1. In **Sicurezza** seleziona uno dei campi seguenti per stabilire le impostazioni di protezione per la tua organizzazione:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Consenti incorporazione di <strong>Workfront</strong> in un iframe</p> </td> 
      <td>Consente di incorporare Workfront in un iframe.<p>Questa opzione è disabilitata per impostazione predefinita.</p><p><b>IMPORTANTE</b>: La visualizzazione di un'applicazione basata su web in un iframe rende l'applicazione suscettibile a una vulnerabilità di sicurezza click-jacking.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti l'autenticazione SAML 2.0 nei componenti aggiuntivi di Office 365</td> 
      <td> <p>Consente di incorporare Workfront in un iframe solo per i componenti aggiuntivi di Office 365 quando Workfront è integrato con una soluzione Single Sign-On SAML 2.0. </p> <p>Questa opzione è attivata per impostazione predefinita.</p> <p><b>NOTA</b>: Se si abilita l'opzione precedente, <strong>Consenti incorporazione di Workfront in un iframe</strong>, l’opzione <strong>Consenti autenticazione SAML 2.0 nei componenti aggiuntivi di Office 365</strong> è attivato e disattivato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abilita l'utilizzo delle informazioni della sessione durante la creazione degli URL delle pagine esterne</td> 
      <td> <p>Consente agli utenti di utilizzare le informazioni ID sessione di un sito quando si aggiunge una pagina esterna a un dashboard.</p> <p>Per ulteriori informazioni sull'aggiunta di pagine esterne a un dashboard, consulta <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Incorporare una pagina web esterna in un dashboard</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consente alle persone di utilizzare le applicazioni mobili Workfront e <strong>Workfront</strong> Componente aggiuntivo di Outlook</td> 
      <td> <p>Consente agli utenti di accedere alle app mobili (Workfront View for iPad and mobile phone apps) e all'app Workfront Outlook.</p> <p>Questa opzione è attivata per impostazione predefinita. </p> <p>Per informazioni su Workfront View, consulta <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Usa visualizzazione Adobe Workfront</a>. Per ulteriori informazioni sulle app per dispositivi mobili, vedi <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Utilizzare l’app mobile Adobe Workfront</a>.</p> <p>Per ulteriori informazioni sul plugin di Outlook, vedere <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Configurare Adobe Workfront per Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Collabora con persone senza account Workfront utilizzando gli indirizzi e-mail</p> </td> 
      <td>Consente agli utenti di Workfront di condividere determinati elementi con persone senza un account Workfront includendo il loro indirizzo e-mail invece del loro nome. Gli utenti possono condividere i seguenti elementi con utenti esterni utilizzando il proprio indirizzo e-mail:
       <ul>
        <li>Documento<br></li>
        <li>Richiesta documento<br></li>
        <li>Approvazione del documento</li>
        <li>Calendario</li>
       </ul><p>Questa opzione è attivata per impostazione predefinita.</p> <p><b>Importante</b>: Il livello di accesso Utente esterno non è disponibile nell'istanza di Workfront se questa opzione è disabilitata. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Livelli di accesso incorporati in Workfront</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiede agli utenti esterni di registrarsi con una password</td> 
      <td> <p>Richiede agli utenti esterni di registrarsi prima di poter visualizzare gli elementi in Workfront. Per impostazione predefinita, questa opzione è disabilitata. Quando abiliti questa opzione, alle persone senza un account Workfront che sono incluse in alcuni aggiornamenti in base al loro indirizzo e-mail verrà richiesto di creare un account prima di poter visualizzare l’elemento su cui sono incluse. Questo crea un account utente esterno per loro.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disconnetti automaticamente gli utenti dopo</td> 
      <td> Consente di specificare quando un utente si disconnette da Workfront dopo un periodo di inattività. Per impostazione predefinita, gli utenti vengono disconnessi dopo 8 ore di inattività. <p>Questa opzione interessa anche i clienti Workfront che utilizzano una soluzione single sign-on.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disconnetti automaticamente gli utenti mobili dopo </td> 
      <td>Consente di specificare quando un utente viene disconnesso dall’applicazione Workfront dopo un periodo di inattività. Per impostazione predefinita, gli utenti vengono disconnessi dopo 7 giorni di inattività. <p>Questa opzione interessa anche i clienti Workfront che utilizzano una soluzione single sign-on.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

   Le modifiche salvate qui influiscono sull’esperienza di tutti gli utenti in Workfront e di tutti coloro che interagiscono con loro come utenti esterni.
