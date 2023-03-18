---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Panoramica della sezione Aggiornamenti
description: La sezione Aggiornamenti mostra fino a 200 degli ultimi aggiornamenti effettuati negli ultimi 90 giorni.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 6%

---

# Panoramica della sezione Aggiornamenti

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the Updates section of an object. You can access the new design by enabling the commenting Beta. 
Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new commenting  experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

Nella sezione Aggiornamenti di un oggetto vengono visualizzati i commenti degli utenti relativi all’oggetto o agli aggiornamenti di sistema che tengono traccia delle modifiche apportate all’oggetto.

## Panoramica della sezione Aggiornamenti

<!--drafted for the commenting beta for issues: 
The information is organized differently in the Updates section, depending on which environment you access it from. 

###  Overview of the current Updates section 
-->

La sezione Aggiornamenti di un oggetto mostra fino a 200 degli aggiornamenti più recenti effettuati negli ultimi 90 giorni.

<!--drafted for the commenting beta for issues: 
The current Updates section shows the following information:

************** AND REMOVE THE SENTENCE BELOW WHEN MAKING THIS LIVE:
-->

La sezione Aggiornamenti mostra le seguenti informazioni:

* Osservazioni degli utenti e risposte a tali osservazioni.
* Aggiornamenti di sistema, ovvero messaggi informativi creati da Workfront per registrare determinati eventi su un oggetto. Ad esempio, è possibile acquisire le modifiche di stato, nome o campi personalizzati con gli aggiornamenti di sistema. L’amministratore di Workfront o di gruppo può abilitare gli aggiornamenti di sistema per gli oggetti. Per ulteriori informazioni, consulta [Configurare gli aggiornamenti di sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Viene visualizzata la sezione Aggiornamenti per i seguenti oggetti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Documenti</li> 
     <li>Obiettivi</li> 
     <li>Problemi</li> 
     <li>Iterazioni</li> 
     <li>Progetti</li> 
     <li>Programmi</li> 
     <li>Portfolio</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Storie</li> 
     <li>Attività</li> 
     <li>Modelli</li> 
     <li>Attività modello</li> 
     <li>Schede orario</li> 
     <li>Utenti</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted for the commenting beta for issues: 
###  Overview of the Updates section in the Beta commenting experience

The Updates section displays information in the following tabs in the Beta commenting experience: 

* **Updates**: Displays comments made by users and replies to those comments. 
* **System Activity**: Displays system updates which are informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your ojects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Currenlty, you can make comments and reply to updates using the Beta commenting experience on the following objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Goals</li> 
     </ul> </td> 
   <td> 
    <ul> 
     <li><span class="preview">Issues</span></li> 
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>The commenting experience Beta is the default current experience for goals. You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

## Aggiornamenti che vengono visualizzati anche su oggetti di rango più elevato

Come illustrato nella tabella seguente, anche le risposte agli aggiornamenti su alcuni oggetti vengono visualizzate nella sezione Aggiornamenti di oggetti di livello superiore.

Ad esempio, quando si aggiunge un aggiornamento a un&#39;attività, l&#39;aggiornamento viene visualizzato nella sezione Aggiornamenti dell&#39;attività e nella sezione Aggiornamenti del progetto contenente l&#39;attività.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Oggetto in cui è stato aggiunto l’aggiornamento originale</strong> </th> 
   <th> <p><strong>Oggetto con classificazione più elevata in cui viene visualizzato anche l’aggiornamento originale</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Problema</td> 
   <td>Progetto</td> 
  </tr> 
  <tr> 
   <td>Attività</td> 
   <td>Progetto</td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>Programma, Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Documento </td> 
   <td>Oggetto in cui è allegato il documento, Project </td> 
  </tr> 
  <tr> 
   <td>Programma</td> 
   <td>Portfolio</td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td>Team</td> 
  </tr> 
  <tr> 
   <td>Scheda orario</td> 
   <td>Utente, Team</td> 
  </tr> 
  <tr> 
   <td>Attività modello</td> 
   <td>Modello</td> 
  </tr> 
  <tr> 
   <td>Storia</td> 
   <td>Iterazione, Team</td> 
  </tr> 
  <tr> 
   <td>Iterazione</td> 
   <td>Team</td> 
  </tr>

<tr> 
   <td>Obiettivi</td> 
   <td>Risultato, attività</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Le risposte aggiunte agli aggiornamenti di sistema non vengono riportate all&#39;oggetto principale. Solo le risposte dirette su un oggetto secondario e le risposte aggiunte agli aggiornamenti esistenti vengono riportate agli oggetti principali.
>
>Per informazioni sulla gerarchia degli oggetti in Adobe Workfront, consulta [Comprendere gli oggetti in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

<!-- drafted for the new commenting experience for issues in beta: Add this paragraph to the note above: 
><span class="preview"> It is not possible to reply to system updates in the new commenting experience Beta. For more information, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).</span> -->

## Limitazioni della sezione Aggiornamenti

### Limitazioni per utenti e team

Non è possibile eseguire aggiornamenti sui team. La sezione Aggiornamenti per i team viene compilata dagli aggiornamenti immessi nei seguenti oggetti:

* Utenti
* Schede orario
* Storie
* Iterazioni

Nella sezione Aggiornamenti per utenti e team, puoi visualizzare gli aggiornamenti immessi negli ultimi 90 giorni.

Se desideri visualizzare tutti gli aggiornamenti effettuati su un utente o un team, oltre il limite di 90 giorni, puoi creare un rapporto per le note. Il rapporto non deve avere un filtro temporale che mostri tutti gli aggiornamenti effettuati per utenti o team. Per ulteriori informazioni, consulta [Creare un rapporto personalizzato](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Limitazioni per l’inserimento di commenti per conto di un altro utente

Gli amministratori di Adobe Workfront e gli amministratori di gruppo possono accedere come altri utenti ed eseguire azioni in Workfront, ad esempio inserire commenti. (Per informazioni, consulta [Accedi come altro utente](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).) Le osservazioni formulate per conto di un altro utente sono indicate nel commento.

Un amministratore di gruppo può commentare per conto di un&#39;altra persona ma non può eliminare tale commento. Solo un amministratore di Adobe Workfront può eliminare un commento che ha effettuato per conto di un altro utente.

## Visualizza gli aggiornamenti di sistema sugli elementi di lavoro con il rapporto Scrittura contabile

Il rapporto Scrittura contabile consente di visualizzare gli aggiornamenti del sistema dall&#39;area Aggiornamenti di progetti, attività e problemi.

Il rapporto ti consente di visualizzare:

* Quante modifiche di stato si sono verificate
* Quando un&#39;attività o un problema è stato eliminato
* Modifica dei valori in importanti campi personalizzati nel corso di un progetto
* Quali date importanti sono cambiate nel corso di un progetto?
* Se la priorità è cambiata nel corso di un progetto
* Se il proprietario di un progetto è cambiato

Per ulteriori informazioni, consulta [Rapporto sull’area Aggiornamenti](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
