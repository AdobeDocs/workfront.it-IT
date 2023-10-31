---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurare le preferenze di sicurezza del sistema
description: In qualità di amministratore di Adobe Workfront, puoi configurare le preferenze di sicurezza per il tuo sistema Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 20e806b1a4face80488bf32fda677f730baed41a
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 6%

---

# Configurare le preferenze di sistema

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

In qualità di amministratore di Adobe Workfront, puoi configurare le preferenze per il tuo sistema Workfront:

* Accesso a Workfront da app per dispositivi mobili e altre applicazioni integrate
* Regole per incorporare Workfront in un iframe

Le modifiche apportate nelle preferenze del sistema hanno un impatto su tutti gli utenti del sistema e sulla loro esperienza in Workfront.

È consigliabile configurare le preferenze di sistema durante l’implementazione di Workfront e rivederle solo occasionalmente in seguito.

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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare le preferenze di sistema

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Sistema** > **Preferenze**.

1. Seleziona uno dei campi seguenti per definire le impostazioni per la tua organizzazione:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Abilita processo di revisione rapida</p> </td> 
      <td>Consente di abilitare i rilasci mensili di Workfront per la tua organizzazione invece dei rilasci trimestrali.</p><p>Per ulteriori informazioni sul processo di rilascio rapido, consulta <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Abilitare o disabilitare le versioni rapide per la tua organizzazione</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Consenti incorporamento di <strong>Workfront</strong> in un iframe</p> </td> 
      <td>Consente di incorporare Workfront in un iframe.<p>Questa opzione è disabilitata per impostazione predefinita.</p><p><b>IMPORTANTE</b>: la visualizzazione di un’applicazione basata sul web in un iframe rende l’applicazione vulnerabile a una vulnerabilità di sicurezza dovuta al click-jacking.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti l'autenticazione SAML 2.0 nei componenti aggiuntivi di Office 365</td> 
      <td> <p>Consente di incorporare Workfront in un iframe solo per i componenti aggiuntivi di Office 365 quando Workfront è integrato con una soluzione Single Sign-On SAML 2.0. </p> <p>Questa opzione è attivata per impostazione predefinita.</p> <p><b>NOTA</b>: se abiliti l’opzione precedente, <strong>Consenti l’incorporamento di Workfront in un iframe</strong>, l’opzione <strong>Consenti autenticazione SAML 2.0 nei componenti aggiuntivi di Office 365</strong> è attivato e oscurato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abilita l'utilizzo delle informazioni della sessione durante la creazione degli URL delle pagine esterne</td> 
      <td> <p>Consente agli utenti di utilizzare le informazioni ID sessione di un sito quando si aggiunge una pagina esterna a un dashboard.</p> <p>Per ulteriori informazioni sull'aggiunta di pagine esterne a un dashboard, vedere <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Incorporare una pagina web esterna in una dashboard</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consentire alle persone di utilizzare le applicazioni mobili di Workfront e <strong>Workfront</strong> Componente aggiuntivo per Outlook</td> 
      <td> <p>Consente agli utenti di accedere alle app per dispositivi mobili (visualizzazione Workfront per iPad e app per telefoni cellulari) e all’app Workfront Outlook.</p> <p>Questa opzione è attivata per impostazione predefinita. </p> <p>Per informazioni sulla visualizzazione Workfront, consulta <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Utilizza la vista Adobe Workfront</a>. Per ulteriori informazioni sulle app per dispositivi mobili, consulta <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Utilizzare l’app mobile di Adobe Workfront</a>.</p> <p>Per ulteriori informazioni sul plug-in di Outlook, vedere <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Configurare Adobe Workfront per Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Collaborare con persone senza account Workfront utilizzando indirizzi e-mail</p> </td> 
      <td>Consente agli utenti di Workfront di condividere alcuni elementi con persone senza un account Workfront includendo il proprio indirizzo e-mail invece del nome. Gli utenti possono condividere i seguenti elementi con utenti esterni utilizzando il proprio indirizzo e-mail:
       <ul>
        <li>Documento<br></li>
        <li>Richiesta documento<br></li>
        <li>Approvazione documento</li>
        <li>Calendario</li>
       </ul><p>Questa opzione è attivata per impostazione predefinita.</p> <p><b>Importante</b>: se questa opzione è disabilitata, il livello di accesso per gli utenti esterni non è disponibile nell’istanza di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Livelli di accesso incorporati in Workfront</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiede agli utenti esterni di registrarsi con una password</td> 
      <td> <p>Richiede agli utenti esterni di registrarsi prima di poter visualizzare gli elementi in Workfront. Per impostazione predefinita, questa opzione è disabilitata. Quando abiliti questa opzione, alle persone senza un account Workfront incluse in alcuni aggiornamenti in base al loro indirizzo e-mail verrà richiesto di creare un account prima di poter visualizzare l’elemento in cui sono incluse. In questo modo viene creato un account utente esterno.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disconnetti automaticamente gli utenti dopo</td> 
      <td> Consente di specificare quando un utente viene disconnesso da Workfront dopo un periodo di inattività. Per impostazione predefinita, gli utenti vengono disconnessi dopo 8 ore di inattività. <p>Questa opzione interessa anche i clienti Workfront che utilizzano una soluzione single sign-on.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disconnetti automaticamente gli utenti mobili dopo </td> 
      <td>Consente di specificare quando un utente viene disconnesso dall’applicazione Workfront dopo un periodo di inattività. Per impostazione predefinita, gli utenti vengono disconnessi dopo 7 giorni di inattività. <p>Questa opzione interessa anche i clienti Workfront che utilizzano una soluzione single sign-on.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gli utenti nel sistema visualizzeranno per impostazione predefinita la nuova esperienza Home </td> 
      <td>Consente di specificare se gli utenti visualizzeranno la nuova esperienza Home per impostazione predefinita. Quando questa opzione è attivata, gli utenti vedranno l’esperienza Nuova home per impostazione predefinita, ma potranno comunque scegliere di abilitare o disabilitare la nuova home su base individuale. Se l'opzione è disattivata, gli utenti non visualizzeranno il banner che consente loro di passare alla nuova home, ma potranno comunque passare alla nuova home page immettendo manualmente <code>/home/workspaces</code> alla fine dell’URL dell’istanza. Questa impostazione è attivata per impostazione predefinita.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

   Le modifiche salvate qui influiscono sull&#39;esperienza di tutti gli utenti in Workfront e di chiunque interagisca con loro come utente esterno.
