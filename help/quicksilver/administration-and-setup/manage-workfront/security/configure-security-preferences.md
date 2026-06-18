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
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/46D3BBajFk39FP-dMDk0SuSSGM5nYPKas11Bs159R9Y
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1e6380b0422efdd98449ab1e74cadb4f330917f1
workflow-type: tm+mt
source-wordcount: 1155
ht-degree: 10%

---

# Configurare le preferenze di sistema

{{preview-fast-release-general}}

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

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Standard</p><p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
      <td role="rowheader">Consenti l'utilizzo delle applicazioni mobili di Workfront</td> 
      <td> <p>Consente agli utenti di accedere alle app mobili (Visualizzazione Workfront per iPad e app per telefoni cellulari)</p> <p>Questa opzione è attivata per impostazione predefinita. </p> <p>Per informazioni sulla visualizzazione Workfront, vedere <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Utilizzare la visualizzazione Adobe Workfront</a>. Per ulteriori informazioni sulle app per dispositivi mobili, vedere <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Utilizzare l'app per dispositivi mobili Adobe Workfront: indice articolo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Collaborare con persone senza account Workfront utilizzando indirizzi e-mail</p> </td> 
      <td>Consente agli utenti di Workfront di condividere alcuni elementi con persone senza un account Workfront includendo il proprio indirizzo e-mail invece del nome. Gli utenti possono condividere i seguenti elementi con utenti esterni utilizzando il proprio indirizzo e-mail:
       <ul>
        <li>Documento<br></li>
        <li>Richiesta documento<br></li>
        <li>Approvazione documento</li>
        <li>Calendario</li>
       </ul><p>Questa opzione è attivata per impostazione predefinita.</p> <p><b>IMPORTANTE</b>: se questa opzione è disabilitata, il livello di accesso per gli utenti esterni non è disponibile nell'istanza di Workfront. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Livelli di accesso incorporati</a>.</p> </td> 
     </tr> 
     <!--
     <tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr>
     -->
     <tr> 
      <td role="rowheader">Help URL</td> 
      <td>Consente di definire un sito di assistenza personalizzato interno in cui l’icona Help (Guida) del Main Menu (Menu principale) può essere visualizzata. Per ulteriori informazioni, vedere <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Configurare un URL della Guida personalizzato</a>.</p></td> 
     </tr>
    <tr> 
      <td role="rowheader">Disabilita l’aggiornamento automatico nei Livelli di accesso</td> 
      <td>È possibile disattivare il processo di aggiornamento automatico per i livelli di accesso Collaboratore. Quando questa impostazione è selezionata, l’amministratore deve aggiornare manualmente a una nuova licenza gli utenti con licenza Collaboratore che hanno superato il limite di decisioni di approvazione.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Abilitare l’elenco di lavoro Priorità </td> 
      <td>Consente di abilitare o disabilitare l’esperienza dell’elenco di lavoro Priorità per i tuoi utenti. Gli utenti continueranno a visualizzare le icone Priorità in Workfront, ma non avranno accesso alla funzionalità. Per ulteriori informazioni sulle priorità, vedere <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Introduzione alle priorità</a>.</td> 
     </tr>
     <tr>
      <td><span class="preview">Applica sempre i campi obbligatori nella modifica in blocco</span></td>
      <td><span class="preview"><p>Consente di scegliere se obbligare gli utenti a immettere le informazioni nei campi obbligatori durante la modifica in blocco di oggetti.</p> <p>Quando questa opzione è selezionata, i campi obbligatori devono avere dei valori prima di essere salvati in modalità di modifica collettiva. Se nel campo obbligatorio manca un valore per almeno un oggetto selezionato in blocco, il salvataggio non è consentito.</p> <p>Se questa opzione non è selezionata, i campi obbligatori vengono applicati solo quando un utente modifica il campo. Se un campo non viene modificato, viene considerato facoltativo e non convalidato.</p></span></td>
     </tr>
     <tr> 
      <td role="rowheader">Preferenze archiviazione </td> 
      <td>In questa sezione puoi abilitare le preferenze cloud di Adobe. Consente di abilitare o disabilitare l’archiviazione cloud di Adobe per l’intera organizzazione o per gruppi specifici. 
      <p>Aggiorna le seguenti informazioni:</p>
      <ul><li><b>Predefinito</b>: scegli l'archiviazione legacy Workfront o l'archiviazione cloud Adobe</li>
      <li><b>Consenti agli utenti di selezionare il provider di archiviazione</b>: consente agli utenti di scegliere tra i due tipi di archiviazione durante la creazione di oggetti Workfront.</li>
      <li><b>Si applica a</b>: scegliere se le impostazioni predefinite si applicano all'intera organizzazione o a gruppi specifici</li>
      <li><b>Seleziona i portfolio da convertire nell'archiviazione cloud Adobe</b>: seleziona i portfolio che desideri convertire automaticamente dall'archiviazione legacy di Workfront all'archiviazione cloud Adobe. I portfolio vengono convertiti quando si salvano le preferenze di sistema.</li></ul>     
    Per ulteriori informazioni sull'archiviazione cloud Adobe, consulta <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md">Abilitare l'archiviazione cloud Adobe per la tua organizzazione</a>.</td></tr>
    <tr> 
      <td role="rowheader">Seleziona i portfolio da convertire in Adobe Cloud Storage </td> 
      <td>Consente di convertire i portfolio di archiviazione Workfront legacy esistenti in archiviazione cloud Adobe. Per ulteriori informazioni, consulta <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md">Convertire i portfolio legacy in Adobe Cloud Storage</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Abilita IA </td> 
      <td>Attivando le impostazioni nell’area Preferenze AI, puoi abilitare AI, incluso AI Assistant. <p><b>NOTA</b>: l'organizzazione deve soddisfare requisiti specifici per abilitare l'intelligenza artificiale. Per ulteriori informazioni sull'intelligenza artificiale, inclusi i requisiti, vedere <a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">Panoramica dell'Assistente intelligenza artificiale</a>.</p></td> 
     </tr>
    <tr> 
      <td role="rowheader">Compilazione modulo IA </td> 
      <td>Consenti agli utenti di utilizzare Compilazione modulo con IA per compilare automaticamente un modulo di richiesta. Per ulteriori informazioni, consulta <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md">Utilizzare il riempimento del modulo basato su IA per compilare una richiesta utilizzando prompt o documenti</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Completamento automatico intelligente nei moduli di richiesta </td> 
      <td>Consente di abilitare la possibilità di completare automaticamente i moduli di richiesta in base ai dati di richiesta precedenti. Per ulteriori informazioni sul completamento automatico del modulo, vedere <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">Compilazione automatica di una richiesta dai dati precedenti</a>.</td> 
     </tr>
    <tr> 
      <td role="rowheader">Designer pianificazione</td> 
      <td>Questa opzione è disponibile solo per i clienti che hanno acquistato un pacchetto Workfront Planning. L'attivazione di questa impostazione consente agli utenti di creare e modificare le aree di lavoro utilizzando Planning Designer. Per informazioni, vedere <a href="/help/quicksilver/planning/general/planning-ai-designer.md">Introduzione ad Adobe Workfront Planning Designer</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Consenso alle versioni Beta dell’IA </td> 
      <td>Consente di abilitare le funzioni di intelligenza artificiale attualmente in Beta. Se abiliti questa opzione, puoi quindi selezionare le funzioni di AI Beta da abilitare. Per ulteriori informazioni su ciascuna funzione di AI Beta, fai clic sull'icona delle informazioni accanto a tale funzione.</td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Strumenti MCP in sola lettura</span></td> 
      <td><span class="preview">Consente al server MCP di Workfront di eseguire operazioni di lettura sui dati di Workfront, ad esempio la ricerca o l'elenco di progetti, attività o altri elementi. Questa opzione è attivata per impostazione predefinita.<p>Per ulteriori informazioni sul server Workfront MCP, vedere <a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">Configurare il server Adobe Workfront MCP</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Scrivi strumenti MCP</span></td> 
      <td><span class="preview">Consente al server MCP di Workfront di eseguire azioni di creazione, aggiornamento ed eliminazione sui dati di Workfront. Questa opzione è disabilitata per impostazione predefinita.<p>Per ulteriori informazioni sul server Workfront MCP, vedere <a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">Configurare il server Adobe Workfront MCP</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader">Ambienti di prova</td> 
      <td>Consente di accedere agli ambienti di test di Workfront. Per ulteriori informazioni, consulta <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Ambiente sandbox di anteprima di Adobe Workfront</a>.</p></td> 
    </tbody> 
   </table>

1. Fai clic su **Salva**.

   Le modifiche salvate in questa pagina influiscono sull&#39;esperienza di tutti gli utenti di Workfront e di tutti coloro che interagiscono con il sistema come utenti esterni.
