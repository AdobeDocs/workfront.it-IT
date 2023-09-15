---
content-type: release-notes
navigation-topic: product-releases-archive
title: Anteprima R1 5
description: Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con la versione R1 Preview 5. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima il 16 marzo 2017.
author: Luke
feature: Product Announcements
exl-id: 4fba14b5-6c5a-4b03-99a7-f0e6f75807c3
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1281'
ht-degree: 13%

---

# Anteprima R1 5

Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con la versione R1 Preview 5. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima il 16 marzo 2017.

Per un elenco di tutte le modifiche apportate in R1, vedere [Panoramica dell’attività sulla versione R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## Tracciare l&#39;avanzamento del progetto con un report Utilizzo

Ora un utente con accesso Gestisci a un progetto può monitorare l’avanzamento del progetto con un rapporto sull’utilizzo.

Il rapporto sull&#39;utilizzo consente di mantenere il progetto entro i limiti del budget, consentendo di vedere rapidamente come vengono registrate le ore effettive rispetto alle ore preventivate o pianificate per una data settimana o mese o per il progetto complessivo. Inoltre, è possibile visualizzare informazioni dettagliate sul numero di ore in ciascuna categoria (preventivata, pianificata ed effettiva), suddivise per mansione o singolo utente.

Per ulteriori informazioni sul tracciamento dell’utilizzo in un progetto, consulta [Panoramica del rapporto Utilizzo risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

In qualità di amministratore di sistema, puoi specificare se la scheda Utilizzo è disponibile per gli utenti. Per impostazione predefinita, la scheda Utilizzo si trova nel menu a discesa Altro all’interno di un progetto. È possibile spostare la scheda Utilizzo in un&#39;altra posizione oppure nasconderla completamente. Se hai definito modelli di layout personalizzati per gli utenti dell’organizzazione, devi aggiungere manualmente la scheda Utilizzo ai modelli di layout personalizzati.

Per ulteriori informazioni sulla configurazione della posizione della scheda Utilizzo, vedere &quot;Personalizzare le schede&quot; in &quot;Creazione e gestione dei modelli di layout&quot;.

## Modifica di un processo di approvazione globale esistente per un singolo oggetto

Ora è possibile modificare un processo di approvazione globale esistente quando si associa tale processo a un oggetto. Le modifiche apportate vengono applicate solo al processo di approvazione dell&#39;oggetto a cui si sta associando l&#39;oggetto.

Per ulteriori informazioni, consulta [Associa un processo di approvazione nuovo o esistente al lavoro](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) in [Associa un processo di approvazione nuovo o esistente al lavoro](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)

## Configurazione dei rapporti per visualizzare il nuovo diagramma di Gantt per impostazione predefinita

È possibile configurare i report relativi al progetto e alle attività creati in modo da visualizzare il nuovo diagramma di Gantt per impostazione predefinita con la nuova opzione &quot;Mostra report in visualizzazione Gantt per impostazione predefinita&quot;.

Per ulteriori informazioni sulla configurazione dei rapporti per visualizzare il nuovo diagramma di Gantt, consulta [Modificare le impostazioni dei rapporti](../../../../reports-and-dashboards/reports/creating-and-managing-reports/edit-report-settings.md).

Per ulteriori informazioni sulla visualizzazione del diagramma di Gantt nei report di progetto e nei report di attività, vedere [Visualizzare le informazioni nel diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)&quot; in [Visualizzare le informazioni nel diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

## Miglioramento Cestino: le attività e le sottoattività vengono ripristinate nell&#39;ordine precedente

Ora, quando si ripristina un&#39;attività o una sottoattività dopo che è stata eliminata, l&#39;attività o la sottoattività viene ripristinata nella posizione precedente (nell&#39;elenco delle attività o sotto l&#39;attività padre), nello stesso ordine in cui era visualizzata prima dell&#39;eliminazione.

Prima di questa modifica, le attività e le sottoattività ripristinate venivano sempre ripristinate come ultima attività (nell&#39;elenco delle attività o sotto l&#39;attività padre), indipendentemente dall&#39;ordine in cui erano visualizzate prima di essere eliminate.

Per ulteriori informazioni sul ripristino di oggetti in Workfront, vedere [Ripristina elementi eliminati](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Miglioramenti alla vista Milestone

Sono ora disponibili i seguenti miglioramenti quando si visualizza un elenco di progetti o un rapporto di progetto nella vista Milestone (Attività cardine):

* **Configura se lo stato di avanzamento e la percentuale di completamento sono visualizzati nella vista:** È disponibile una nuova opzione che consente di configurare la visualizzazione delle icone di stato di avanzamento nella vista Milestone. Inoltre, puoi anche configurare la visualizzazione delle informazioni sulla percentuale di completamento in relazione ai progetti e alle attività.\
  Per ulteriori informazioni, consulta [Utilizzare la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [Utilizzare la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Modifica la percentuale di completamento direttamente dalla vista Milestone:** Ora è possibile modificare la percentuale di completamento dei progetti e delle attività direttamente dalla vista Milestone.\
  Per ulteriori informazioni, consulta [Utilizzare la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [Utilizzare la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md). 

## È stato aggiornato il look and feel di diverse pagine di configurazione del sistema

Sono stati aggiornati l’aspetto delle seguenti pagine del menu Sistema dell’area Configura (la funzionalità rimane la stessa):

* Diagnostiche
* Single Sign-On (SSO) che include:

   * Active Directory
   * LDAP
   * SAML 1.1
   * SAML 2.0

* Aggiorna utenti per l&#39;SSO

## Raggruppamenti di notifiche di eventi aggiornati nell’area di configurazione e-mail

Le intestazioni organizzative delle Notifiche eventi nell’area Configurazione e-mail ora corrispondono alle intestazioni di sezione utilizzate nell’area delle impostazioni del profilo utente.

Per ulteriori informazioni sulle notifiche degli eventi, consulta  [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Rinuncia a notifiche istantanee: configurazione riepilogo in contesto

Le seguenti opzioni sono ora disponibili nelle notifiche e-mail istantanee. Queste opzioni sono disponibili solo per le notifiche istantanee che hanno anche una controparte di riepilogo giornaliera:

* &quot;Aggiungi a un digest giornaliero&quot;
* &quot;Interrompi le e-mail di questo tipo&quot;

Ora, quando ricevi una notifica e-mail istantanea, puoi aggiungerla a una notifica con riepilogo giornaliero, oppure puoi annullare completamente l’abbonamento a tale notifica.

Queste opzioni sono disponibili all’interno della notifica e-mail. Per ulteriori informazioni sulla ricezione delle notifiche e-mail, consulta [Notifiche Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md)

## Varie notifiche e-mail sono state spostate dalla sezione &quot;Azione richiesta&quot; ad altre sezioni correlate al progetto

Sono state spostate diverse notifiche dalla sezione &quot;Azione richiesta&quot; della pagina del profilo utente ad altre sezioni, come segue:

Per ulteriori informazioni sulla configurazione delle notifiche e-mail, consulta [Modifica le tue notifiche e-mail](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)

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
   <td>Viene aggiunto un problema a un progetto di cui sono proprietario</td> 
   <td> <p> Azione richiesta </p> </td> 
   <td>   <p>Informazioni sui progetti di cui sono proprietario</p></td> 
  </tr> 
  <tr> 
   <td>Viene aggiunto un problema a un progetto a cui collaboro</td> 
   <td>   <p>Azione richiesta</p><p> </p></td> 
   <td> <p> Informazioni sui progetti di cui sono proprietario </p>   </td> 
  </tr> 
  <tr> 
   <td>Un problema non assegnato viene aggiunto a un progetto di cui sono proprietario</td> 
   <td>   <p>Azione richiesta</p></td> 
   <td>   <p>Informazioni sui progetti di cui sono proprietario</p></td> 
  </tr> 
  <tr> 
   <td> <p> Un problema non assegnato viene aggiunto a un progetto a cui partecipo </p> </td> 
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
   <td> <p> Modifica dello stato per un attività a cui sono stato assegnato </p>   </td> 
   <td> <p> Azione richiesta </p>   </td> 
   <td> <p> Informazioni sul lavoro assegnato a me </p>   </td> 
  </tr> 
 </tbody> 
</table>

## Nuova funzionalità di pianificazione delle risorse (non disponibile in produzione in R1)

>[!NOTE]
>
>Questa funzionalità è attualmente disponibile nell’ambiente di anteprima. Verrà rimosso dall’ambiente di anteprima circa un mese prima della versione R1 in produzione. Verrà quindi reintrodotto nell&#39;ambiente di anteprima in R2 Preview 1.

 

Sono state aggiunte le seguenti modifiche per supportare la futura funzionalità di pianificazione delle risorse:

* La scheda &quot;Pianificazione delle risorse&quot; corrente è stata rinominata &quot;Pianificazione delle risorse legacy&quot; nell’area Persone. 
* Nell’area Persone è stata introdotta una nuova scheda &quot;Pianificazione delle risorse&quot; in cui verranno sviluppate le nuove funzionalità.\
  Per ulteriori informazioni sulla nuova scheda Pianificazione risorse, vedere [Introduzione alla pianificazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planning.md) 

* L&#39;oggetto corrente &quot;Pool di risorse&quot; è stato rinominato &quot;Pool di risorse legacy&quot;.\
  Per ulteriori informazioni sulla creazione dei nuovi gruppi di risorse basati sull&#39;utente, vedere [Panoramica sui pool di risorse](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

* È stato creato un nuovo oggetto &quot;Pool di Risorse&quot; per supportare i nuovi Pool di Risorse (basati sull&#39;utente).

  >[!NOTE]
  >
  >
  >   
  >   
  * Se i rapporti sono attualmente in esecuzione sui gruppi di risorse esistenti, i rapporti esistenti non subiranno modifiche.
  * Se si desidera creare un nuovo rapporto per i gruppi di risorse esistenti (basati su ruolo), è necessario selezionare &quot;Gruppi di risorse esistenti&quot; come oggetto del rapporto.
  * Se desideri creare un nuovo rapporto per i nuovi Pool di Risorse (basati sull&#39;utente), seleziona &quot;Pool di Risorse&quot; come oggetto del rapporto.
  >   
  >
