---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Panoramica della scheda Aggiornamenti
description: La scheda Aggiornamenti mostra fino a 200 degli aggiornamenti più recenti effettuati negli ultimi 90 giorni.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 19872953e847921c0fee6d383026641c05012ead
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 7%

---

# Panoramica della scheda Aggiornamenti

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only for a limited number of objects when you opt in to the new commenting experience Beta.</span> -->

<!-- for preview commenting beta: at the release of commenting beta: change the title to: Updates section overview - also update ALL articles from which this is linked-->

La scheda Aggiornamenti mostra fino a 200 degli aggiornamenti più recenti effettuati negli ultimi 90 giorni.

È possibile commentare e rispondere agli aggiornamenti sui seguenti oggetti:

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

## Aggiornamenti che vengono visualizzati anche su oggetti di rango più elevato

Come illustrato nella tabella seguente, le risposte agli aggiornamenti su alcuni oggetti vengono visualizzate anche nella scheda Aggiornamenti di oggetti di livello superiore.

Ad esempio, quando si aggiunge un aggiornamento a un’attività, l’aggiornamento viene visualizzato nella scheda Aggiornamenti dell’attività e nella scheda Aggiornamenti del progetto contenente l’attività.

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

## Limitazioni della scheda Aggiornamenti

### Limitazioni per utenti e team

Non è possibile eseguire aggiornamenti sui team. La scheda Aggiornamenti per i team viene compilata dagli aggiornamenti immessi nei seguenti oggetti:

* Utenti
* Schede orario
* Storie
* Iterazioni

Nella scheda Aggiornamenti per utenti e team, puoi visualizzare gli aggiornamenti immessi negli ultimi 90 giorni.

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
