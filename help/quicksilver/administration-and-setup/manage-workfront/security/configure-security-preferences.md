---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurare le preferenze di sistema
description: In qualità di amministratore di Adobe Workfront, puoi configurare le preferenze per il tuo sistema Workfront, incluse le preferenze di sicurezza.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: d4ebdcc942f119dc229e2a3216dbe82b3d701cba
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 5%

---

# Configurare le preferenze di sistema

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

{{important-admin-console-onboard}}

In qualità di amministratore di Adobe Workfront, puoi configurare le preferenze per il tuo sistema Workfront, tra cui:

* Accesso a Workfront da app per dispositivi mobili e altre applicazioni integrate
* Regole per incorporare Workfront in un iframe

Le modifiche apportate nelle preferenze del sistema hanno un impatto su tutti gli utenti del sistema e sulla loro esperienza in Workfront.

È consigliabile configurare le preferenze di sistema durante l’implementazione di Workfront e rivederle solo occasionalmente in seguito.

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
   <td><p>Nuovo: Standard</p>
   <p>oppure</p>
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare le preferenze di sistema

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Sistema** > **Preferenze**.

1. Seleziona uno dei campi seguenti per definire le impostazioni per la tua organizzazione:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Abilita processo di rilascio rapido</p> </td> 
      <td>Consente di abilitare i rilasci mensili di Workfront per la tua organizzazione invece dei rilasci trimestrali.</p><p>Per ulteriori informazioni sul processo di rilascio rapido, vedere <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">Abilitare o disabilitare i rilasci rapidi per l'organizzazione</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Consenti l’incorporamento di Workfront in un iframe</p> </td> 
      <td>Consente di incorporare Workfront in un iframe.<p>Questa opzione è disabilitata per impostazione predefinita.</p><p><b>IMPORTANTE</b>: la visualizzazione di un'applicazione basata sul Web in un iframe rende l'applicazione vulnerabile a una vulnerabilità di sicurezza di tipo click-jacking.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti l'autenticazione SAML 2.0 nei componenti aggiuntivi di Office 365</td> 
      <td> <p>Consente di incorporare Workfront in un iframe solo per i componenti aggiuntivi di Office 365 quando Workfront è integrato con una soluzione Single Sign-On SAML 2.0. </p> <p>Questa opzione è attivata per impostazione predefinita.</p> <p><b>NOTA</b>: se abiliti l'opzione precedente, <strong>Consenti incorporamento di Workfront in un iframe</strong>, l'opzione <strong>Consenti autenticazione SAML 2.0 nei componenti aggiuntivi di Office 365</strong> è abilitata e disabilitata.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abilita l’utilizzo delle informazioni della sessione durante la creazione degli URL delle pagine esterne</td> 
      <td> <p>Consente agli utenti di utilizzare le informazioni ID sessione di un sito quando si aggiunge una pagina esterna a un dashboard.</p> <p>Questa opzione non è sicura e disattivata per impostazione predefinita. Si consiglia invece di utilizzare OAuth per le integrazioni.</p> <p>Per ulteriori informazioni sull'aggiunta di pagine esterne a un dashboard, vedere <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Incorporare una pagina Web esterna in un dashboard</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti l'utilizzo delle applicazioni mobili di Workfront e del componente aggiuntivo di Workfront Outlook</td> 
      <td> <p>Consente agli utenti di accedere alle app per dispositivi mobili (visualizzazione Workfront per iPad e app per telefoni cellulari) e all’app Workfront Outlook.</p> <p>Questa opzione è attivata per impostazione predefinita. </p> <p>Per informazioni sulla visualizzazione Workfront, vedere <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Utilizzare la visualizzazione Adobe Workfront</a>. Per ulteriori informazioni sulle app per dispositivi mobili, vedere <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Utilizzare l'app per dispositivi mobili Adobe Workfront: indice articolo</a>.</p> <p>Per ulteriori informazioni sul plug-in di Outlook, vedere <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Configurare Adobe Workfront per Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Collaborare con persone senza account Workfront utilizzando indirizzi e-mail</p> </td> 
      <td>Consente agli utenti di Workfront di condividere alcuni elementi con persone senza un account Workfront includendo il proprio indirizzo e-mail invece del nome. Gli utenti possono condividere i seguenti elementi con utenti esterni utilizzando il proprio indirizzo e-mail:
       <ul>
        <li>Documento<br></li>
        <li>Richiesta documento<br></li>
        <li>Approvazione documento</li>
        <li>Calendario</li>
       </ul><p>Questa opzione è attivata per impostazione predefinita.</p> <p><b>Importante</b>: se questa opzione è disabilitata, il livello di accesso per gli utenti esterni non è disponibile nell'istanza di Workfront. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Livelli di accesso incorporati</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiedi agli utenti esterni di registrarsi con una password</td> 
      <td> <p>Richiede agli utenti esterni di registrarsi prima di poter visualizzare gli elementi in Workfront. Per impostazione predefinita, questa opzione è disabilitata. Quando abiliti questa opzione, alle persone senza un account Workfront incluse in alcuni aggiornamenti in base al loro indirizzo e-mail verrà richiesto di creare un account prima di poter visualizzare l’elemento in cui sono incluse. In questo modo viene creato un account utente esterno.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disconnetti automaticamente gli utenti dopo</td> 
      <td> Consente di specificare quando un utente viene disconnesso da Workfront dopo un periodo di inattività. Per impostazione predefinita, gli utenti vengono disconnessi dopo 8 ore di inattività. <p>Questa opzione interessa anche i clienti Workfront che utilizzano una soluzione single sign-on.</p> <p>Questa impostazione non è disponibile per le organizzazioni che sono state migrate ad Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Disconnetti automaticamente gli utenti mobili dopo </td> 
      <td>Consente di specificare quando un utente viene disconnesso dall’applicazione Workfront dopo un periodo di inattività. Per impostazione predefinita, gli utenti vengono disconnessi dopo 7 giorni di inattività. <p>Questa opzione interessa anche i clienti Workfront che utilizzano una soluzione single sign-on.</p> <p>Questa impostazione non è disponibile per le organizzazioni che sono state migrate ad Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Help URL</td> 
      <td>Consente di definire un sito di assistenza personalizzato interno in cui l’icona Help (Guida) del Main Menu (Menu principale) può essere visualizzata. Per ulteriori informazioni, vedere <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Configurare un URL della Guida personalizzato</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Gli utenti nel sistema visualizzeranno per impostazione predefinita la nuova esperienza Home </td> 
      <td>Consente di specificare se gli utenti visualizzeranno la nuova esperienza Home per impostazione predefinita. Quando questa opzione è attivata, gli utenti vedranno l’esperienza Nuova home per impostazione predefinita, ma potranno comunque scegliere di abilitare o disabilitare la nuova home su base individuale. Se l'opzione è disabilitata, gli utenti non visualizzeranno il banner che consente loro di passare alla nuova home. Tuttavia, possono comunque passare alla nuova home page immettendo manualmente <code>/home/workspaces</code> alla fine dell'URL dell'istanza. Questa impostazione è attivata per impostazione predefinita.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Abilitare l’elenco di lavoro Priorità </td> 
      <td>Consente di abilitare o disabilitare l’esperienza dell’elenco di lavoro Priorità per i tuoi utenti. Gli utenti continueranno a visualizzare le icone Priorità in Workfront, ma non avranno accesso alla funzionalità. Per ulteriori informazioni sulle priorità, vedere <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Introduzione alle priorità</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Ambienti di prova</td> 
      <td>Consente di accedere agli ambienti di test di Workfront. Per ulteriori informazioni, consulta <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Ambiente Sandbox di anteprima di Adobe Workfront</a>.</p></td> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

   Le modifiche salvate in questa pagina influiscono sull&#39;esperienza di tutti gli utenti di Workfront e di tutti coloro che interagiscono con il sistema come utenti esterni.
