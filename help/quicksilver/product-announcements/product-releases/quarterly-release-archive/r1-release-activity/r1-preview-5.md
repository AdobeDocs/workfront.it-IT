---
content-type: release-notes
navigation-topic: product-releases-archive
title: Anteprima R1 5
description: Questa pagina descrive tutte le modifiche disponibili nell'ambiente Preview con la versione R1 Preview 5. La funzionalità di questa pagina è stata resa disponibile nell’ambiente Anteprima il 16 marzo 2017.
author: Luke
feature: Product Announcements
exl-id: 4fba14b5-6c5a-4b03-99a7-f0e6f75807c3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1283'
ht-degree: 13%

---

# Anteprima R1 5

Questa pagina descrive tutte le modifiche disponibili nell&#39;ambiente Preview con la versione R1 Preview 5. La funzionalità di questa pagina è stata resa disponibile nell’ambiente Anteprima il 16 marzo 2017.

Per un elenco di tutte le modifiche apportate in R1, vedi [Panoramica dell’attività di rilascio di R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## Tracciare l’avanzamento del progetto con un rapporto sull’utilizzo

Ora un utente con accesso Gestione a un progetto può tenere traccia dell’avanzamento del progetto con un rapporto di utilizzo.

Il rapporto di utilizzo consente di mantenere il progetto entro il budget, consentendo di vedere rapidamente come le ore effettive vengono tracciate rispetto alle ore previste o alle ore pianificate in budget per una determinata settimana o mese o per il progetto complessivo. Inoltre, puoi visualizzare informazioni dettagliate sul numero di ore in ciascuna categoria (in budget, pianificate e effettive), suddivise per ruolo o per singolo utente.

Per ulteriori informazioni sul tracciamento dell’utilizzo in un progetto, consulta [Panoramica del rapporto Utilizzo risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

In qualità di amministratore di sistema, puoi configurare se la scheda Utilizzo è disponibile per gli utenti. Per impostazione predefinita, la scheda Utilizzo si trova nel menu a discesa Altro all’interno di un progetto. È possibile spostare la scheda Utilizzo in un&#39;altra posizione oppure nasconderla completamente. Se sono stati definiti modelli di layout personalizzati per gli utenti dell&#39;organizzazione, è necessario aggiungere manualmente la scheda Utilizzo ai modelli di layout personalizzati.

Per ulteriori informazioni sulla configurazione della posizione della scheda Utilizzo, vedere &quot;Personalizza schede&quot; in &quot;Creazione e gestione di modelli di layout&quot;.

## Modificare un processo di approvazione globale esistente per un singolo oggetto

Ora è possibile modificare un processo di approvazione globale esistente associando tale processo di approvazione globale a un oggetto. Le modifiche apportate vengono applicate solo al processo di approvazione dell&#39;oggetto in cui lo si sta associando.

Per ulteriori informazioni, consulta [Associa un processo di approvazione nuovo o esistente al lavoro](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) in [Associa un processo di approvazione nuovo o esistente al lavoro](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)

## Configurare i rapporti per visualizzare il nuovo diagramma di Gantt per impostazione predefinita

È possibile configurare i rapporti relativi al progetto e alle attività creati per visualizzare il nuovo diagramma di Gantt per impostazione predefinita con la nuova opzione &quot;Mostra il rapporto in una visualizzazione Gantt per impostazione predefinita&quot;.

Per ulteriori informazioni sulla configurazione dei rapporti per visualizzare il nuovo diagramma di Gantt, vedere [Modificare le impostazioni dei rapporti](../../../../reports-and-dashboards/reports/creating-and-managing-reports/edit-report-settings.md).

Per ulteriori informazioni sulla visualizzazione del diagramma di Gantt nei rapporti sui progetti e nei rapporti sulle attività, vedere [Visualizzazione delle informazioni nel diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)&quot; [Visualizzazione delle informazioni nel diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

## Miglioramento Cestino: Le attività e le sottoattività vengono ripristinate in base all&#39;ordine precedente

Ora, quando si ripristina un&#39;attività o una sottoattività dopo l&#39;eliminazione, l&#39;attività o la sottoattività viene ripristinata nella posizione precedente (nell&#39;elenco delle attività o sotto l&#39;attività principale), nello stesso ordine in cui era apparsa prima di essere eliminata.

Prima di questa modifica, le attività e le sottoattività ripristinate venivano sempre ripristinate come ultima attività (nell&#39;elenco delle attività o sotto l&#39;attività principale), indipendentemente dall&#39;ordine in cui erano visualizzate prima di essere eliminate.

Per ulteriori informazioni sul ripristino degli oggetti in Workfront, vedere [Ripristina elementi eliminati](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Miglioramenti alla vista Milestone

I seguenti miglioramenti sono ora disponibili quando si visualizza un elenco di progetti o un rapporto di progetto nella vista Milestone:

* **Configura se nella visualizzazione vengono visualizzati lo stato di avanzamento e la percentuale di completamento:** È disponibile una nuova opzione che consente di configurare la visualizzazione delle icone Stato di avanzamento nella vista Milestone. Inoltre, è possibile configurare la visualizzazione delle informazioni sulla percentuale di completamento relative a progetti e attività.\
   Per ulteriori informazioni, consulta [Utilizzare la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [Utilizzare la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Modifica la percentuale di completamento direttamente dalla vista Milestone:** Ora è possibile modificare la percentuale di completamento di progetti e attività direttamente dalla vista Milestone.\
   Per ulteriori informazioni, consulta [Utilizzare la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [Utilizzare la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md). 

## Aspetto e sensazione aggiornati di diverse pagine di configurazione del sistema

L&#39;aspetto delle pagine seguenti nel menu Sistema dell&#39;area Configurazione è stato aggiornato (la funzionalità rimane invariata):

* Diagnostiche
* Single Sign-On (SSO) che include:

   * Active Directory
   * LDAP
   * SAML 1.1
   * SAML 2.0

* Aggiorna utenti per l&#39;SSO

## Gruppi di notifiche degli eventi aggiornati nell&#39;area di configurazione e-mail

Le intestazioni organizzative delle notifiche degli eventi nell’area Impostazione e-mail ora corrispondono alle intestazioni della sezione utilizzate nell’area delle impostazioni del profilo utente.

Per ulteriori informazioni sulle notifiche degli eventi, vedi  [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Rifiuto delle notifiche istantanee: Configurazione digest in-Context

Le seguenti opzioni sono ora disponibili nelle notifiche e-mail istantanee. Queste opzioni sono disponibili solo per le notifiche istantanee che hanno anche una controparte digest giornaliera:

* “Aggiungi a un digest giornaliero”
* &quot;Interrompi e-mail di questo tipo&quot;

Ora, quando ricevi una notifica e-mail istantanea, puoi aggiungere tale notifica a una notifica digest giornaliera oppure puoi annullare completamente l’iscrizione a tale notifica.

Queste opzioni sono disponibili all’interno della notifica e-mail. Per ulteriori informazioni sulla ricezione delle notifiche e-mail, consulta [Notifiche Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md)

## Varie notifiche e-mail sono state spostate dalla sezione &quot;Azione necessaria&quot; ad altre sezioni correlate ai progetti

Diverse notifiche sono state spostate dalla sezione &quot;Azione necessaria&quot; della pagina del profilo utente ad altre sezioni, come segue:

Per ulteriori informazioni sulla configurazione delle notifiche e-mail, consulta [Attivare o disattivare le notifiche degli eventi personali](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Notifica</strong> </th> 
   <th><strong>Sezione precedente</strong> </th> 
   <th><strong>Nuova sezione</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Quando si aggiunge una Issue, invia email al Proprietario del progetto</td> 
   <td> <p> Azione richiesta </p> </td> 
   <td>   <p>Informazioni sui progetti di cui sono proprietario</p></td> 
  </tr> 
  <tr> 
   <td>Quando si aggiunge una Issue, invia una Email alla squadra</td> 
   <td>   <p>Azione richiesta</p><p> </p></td> 
   <td> <p> Informazioni sui progetti di cui sono proprietario </p>   </td> 
  </tr> 
  <tr> 
   <td>Quando si aggiunge una Issue non assegnata, invia una Email al Proprietario del progetto.</td> 
   <td>   <p>Azione richiesta</p></td> 
   <td>   <p>Informazioni sui progetti di cui sono proprietario</p></td> 
  </tr> 
  <tr> 
   <td> <p> Quando si aggiunge una Issue non assegnata, invia una Email alla Squadra. </p> </td> 
   <td> <p> Azione richiesta </p>   </td> 
   <td> <p> Informazioni sui progetti di cui sono proprietario </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> Modifiche della data di conferma per un'attività su uno dei miei progetti </p> </td> 
   <td>   <p>Azione richiesta</p></td> 
   <td>   <p>Informazioni sui progetti di cui sono proprietario</p></td> 
  </tr> 
  <tr> 
   <td> <p> Modifiche della data di conferma per un problema su uno dei miei progetti </p>   </td> 
   <td>   <p>Azione richiesta</p></td> 
   <td> <p> Informazioni sui progetti di cui sono proprietario </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> Le modifiche della data di scadenza su un'attività a cui sono assegnato </p> </td> 
   <td>   <p>Azione richiesta</p></td> 
   <td>   <p>Informazioni sul lavoro assegnato a me</p></td> 
  </tr> 
  <tr> 
   <td> <p> Le modifiche della data di scadenza su un problema al quale sono assegnato </p> </td> 
   <td> <p> Azione richiesta </p>   </td> 
   <td>   <p>Informazioni sul lavoro assegnato a me</p></td> 
  </tr> 
  <tr> 
   <td> <p> Le modifiche stato su un'attività a cui sono assegnato </p>   </td> 
   <td> <p> Azione richiesta </p>   </td> 
   <td> <p> Informazioni sul lavoro assegnato a me </p>   </td> 
  </tr> 
 </tbody> 
</table>

## Nuova funzionalità di pianificazione delle risorse (non disponibile in produzione in R1)

>[!NOTE]
>
>Questa funzionalità è attualmente disponibile nell’ambiente Anteprima. Verrà rimosso dall’ambiente Preview circa un mese prima della versione R1 in Produzione. Verrà quindi reintrodotto nell&#39;ambiente Preview in R2 Preview 1.

 

Sono state aggiunte le seguenti modifiche per supportare la futura funzionalità di pianificazione delle risorse:

* La scheda &quot;Pianificazione risorse&quot; corrente è stata rinominata in &quot;Pianificazione risorse legacy&quot; nell&#39;area Persone. 
* È stata introdotta una nuova scheda &quot;Pianificazione risorse&quot; nell’area Persone in cui verrà sviluppata la nuova funzionalità.\
   Per ulteriori informazioni sulla nuova scheda Pianificazione delle risorse, vedere [Guida introduttiva alla pianificazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planning.md) 

* L&#39;oggetto &quot;Pool di risorse&quot; corrente è stato rinominato in &quot;Pool di risorse legacy&quot;.\
   Per ulteriori informazioni sulla creazione dei nuovi pool di risorse basati sull&#39;utente, vedi [Panoramica dei pool di risorse](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

* È stato creato un nuovo oggetto &quot;Pool di risorse&quot; per supportare i nuovi pool di risorse (basati sull’utente).

   >[!NOTE]
   * Se attualmente esegui rapporti sui pool di risorse legacy esistenti, i rapporti esistenti non verranno modificati.
   * Se desideri creare un nuovo rapporto per i pool di risorse legacy esistenti (basati sui ruoli del lavoro), dovrai selezionare &quot;Pool di risorse legacy&quot; come oggetto del rapporto.
   * Se desideri creare un nuovo rapporto per i nuovi pool di risorse (basati sull’utente), dovrai selezionare &quot;Pool di risorse&quot; come oggetto per il rapporto.

  >   
