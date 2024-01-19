---
content-type: overview
navigation-topic: the-new-workfront-experience
title: Panoramica delle intestazioni degli oggetti
description: È possibile visualizzare informazioni sugli oggetti in [!DNL Adobe Workfront] quando ne rivedi l’intestazione. Le informazioni in un'intestazione possono includere il proprietario dell'oggetto, lo stato o la percentuale di completamento.
feature: Get Started with Workfront
exl-id: 76e21df0-9272-4bfb-8a97-c16ae5f4b5dc
source-git-commit: 58dffc8a84c2bcaaf09dfc65c6555d57f0b2eeb4
workflow-type: tm+mt
source-wordcount: '3707'
ht-degree: 0%

---

# Panoramica delle intestazioni degli oggetti

È possibile visualizzare informazioni sugli oggetti in [!DNL Adobe Workfront] quando ne rivedi l’intestazione.

Oltre al nome dell&#39;oggetto, l&#39;intestazione può includere il proprietario dell&#39;oggetto, lo stato o la percentuale di completamento.

[!DNL Workfront] assegna priorità al nome dell&#39;oggetto, allocandovi il maggior spazio possibile nell&#39;intestazione. Quando il nome di un oggetto è troppo lungo, viene troncato. Per visualizzare il nome completo di un oggetto, puoi passare il cursore sopra di esso.

## Accedere all&#39;intestazione di un oggetto

Accesso all’intestazione di un oggetto in [!DNL Workfront] è identico per tutti gli oggetti che lo contengono.

Ad esempio, per accedere all’intestazione di un progetto:

1. Vai a un progetto.\
   L’intestazione viene visualizzata nella parte superiore della pagina e contiene il nome del progetto.

   ![](assets/project-header-350x18.png)

## [!UICONTROL Home] panoramica intestazione

Le seguenti intestazioni sono disponibili in Home:

* Attività: per ulteriori informazioni su come utilizzare questa intestazione, vedi [Panoramica intestazione attività](#task-header-overview) in questo articolo.
* Problema: per ulteriori informazioni su come utilizzare questa intestazione, consulta [Panoramica intestazione problema](#issue-header-overview) in questo articolo.

## Intestazioni personalizzabili

Il tuo [!DNL Workfront]  L’amministratore del gruppo o può personalizzare l’intestazione di progetti, attività e problemi utilizzando un modello di layout.

Questo articolo descrive le intestazioni predefinite per tutti gli oggetti, inclusi i progetti, le attività e i problemi.

Per informazioni sulla personalizzazione delle informazioni sull&#39;intestazione di un oggetto, vedere [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


## Panoramica dell’intestazione del progetto

![](assets/project-header-350x18.png)

Per impostazione predefinita, nell’intestazione del progetto vengono visualizzate le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Breadcrumb con oggetti padre</td> 
   <td>Se il progetto è associato a un programma o a un portfolio, viene visualizzato nella breadcrumb nell’angolo superiore sinistro dell’intestazione. Facendo clic sul nome dell'oggetto padre viene aperto l'oggetto padre.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>L'icona viola [!UICONTROL Project] <img src="assets/nwe-projects-icon.png"> viene visualizzato a sinistra del nome del progetto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del progetto</td> 
   <td>Puoi modificare il nome del progetto nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Il testo "[!UICONTROL PROJECT]" viene visualizzato sopra il nome del progetto nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area azioni dell'attività</td> 
   <td> <p>Accanto al nome del progetto viene visualizzata l’area delle azioni.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percent Complete]</td> 
   <td>Non puoi modificare la percentuale di completamento del progetto nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proprietario Progetto]</td> 
   <td> <p>È possibile modificare [!UICONTROL Project Owner] (Proprietario progetto) nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di completamento Pianificata] </td> 
   <td> <p>Puoi modificare il progetto [!UICONTROL Planned Completion Date] (Data di completamento pianificata) e l’ora nell’intestazione se il progetto è pianificato a partire da [!UICONTROL Completion Date] (Data di completamento pianificata). Se il progetto è pianificato a partire da [!UICONTROL Start Date], queste informazioni vengono aggiornate dalle attività del progetto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Condizione [!UICONTROL] </td> 
   <td> <p>Quando si imposta il tipo di condizione [!UICONTROL] del progetto su Manual, è possibile aggiornare il progetto [!UICONTROL Condition] nell'intestazione.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stato]</td> 
   <td>È possibile modificare il progetto [!UICONTROL Status] nell'intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area [!UICONTROL Approvals]</td> 
   <td> <p>Se sei uno degli approvatori, utilizza le icone seguenti per gestire le approvazioni per il progetto:</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> </img> [!UICONTROL Approva]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> </img> [!UICONTROL rifiuta]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> </img> [!UICONTROL Recall]</p> <p>Se non si è un approvatore, fare clic sull'icona [!UICONTROL Altro] <img src="assets/more-icon-for-approvals-area.png"> per visualizzare informazioni sul passaggio di approvazione corrente.</p> <p>Per ulteriori informazioni sulle approvazioni, consulta <a href="../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Panoramica del processo di approvazione</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Panoramica intestazione attività

![](assets/task-header-350x18.png)

Per impostazione predefinita, l&#39;intestazione dell&#39;attività include le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Breadcrumb con oggetti padre</td> 
   <td> <p>Gli oggetti padre dell’attività vengono visualizzati nella breadcrumb. Facendo clic sul nome dell'oggetto padre viene aperto l'oggetto padre.</p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Panoramica delle breadcrumb</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>L'icona verde [!UICONTROL Task] <img src="assets/nwe-tasks-icon.png"> viene visualizzato a sinistra del nome dell'attività.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome dell’attività</td> 
   <td>Puoi modificare il nome dell’attività nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Il testo "[!UICONTROL TASK]" viene visualizzato sopra il nome dell'attività nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area azioni dell'attività</td> 
   <td> <p>Accanto al nome dell'attività viene visualizzata l'area [!UICONTROL actions].</p> <p> <img src="assets/nwe-dependency-action-area.png"> </p> <p>Se viene visualizzata l'icona Dipendenza, è possibile fare clic su di essa per visualizzare eventuali predecessori o successori dell'attività.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percent Complete]</td> 
   <td>È possibile modificare la percentuale di completamento dell'attività nell'intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assegnazioni]</td> 
   <td>È possibile modificare gli assegnatari di un'attività dall'intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Lavoraci], [!UICONTROL Fine] o pulsante [!UICONTROL Avvia attività]</p> </td> 
   <td> <p>Se l'attività è assegnata a te, puoi fare clic sul [!UICONTROL Lavoraci] <span>o [!UICONTROL Avvia attività]</span> per indicare che si sta lavorando sull'attività oppure il pulsante [!UICONTROL Done] per indicare che l'attività è stata completata.</p> <p><span>Per informazioni sulla sostituzione del pulsante [!UICONTROL Lavoraci] con un pulsante [!UICONTROL Avvia attività], vedere <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Sostituisci il pulsante [!UICONTROL Lavoraci] con un pulsante [!UICONTROL Avvia]</a></span>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di completamento Pianificata]</td> 
   <td> <p>È possibile modificare l'attività [!UICONTROL Data di completamento pianificata] <span>e ora</span> nell’intestazione.</p> <p>Suggerimento: si noti che [!UICONTROL Commit Date] non è visibile nell'intestazione. È possibile visualizzarlo nella pagina [!UICONTROL Details].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stato]</td> 
   <td>È possibile modificare l'attività [!UICONTROL Status] nell'intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area [!UICONTROL Approvals]</td> 
   <td> <p>Quando si è uno degli approvatori, utilizzare le icone seguenti per gestire le approvazioni per l'attività:</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> </img> [!UICONTROL Approva]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> </img> [!UICONTROL rifiuta]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> </img> [!UICONTROL Recall]</p> <p>Se non si è un approvatore, fare clic sull'icona [!UICONTROL Altro] <img src="assets/more-icon-for-approvals-area.png"> per visualizzare informazioni sul passaggio di approvazione corrente.</p> <p>Per ulteriori informazioni sulle approvazioni, consulta <a href="../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Panoramica del processo di approvazione</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Panoramica intestazione problema

![](assets/issue-header-350x19.png)

Per impostazione predefinita, l’intestazione del problema include le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Breadcrumb con oggetti padre</td> 
   <td> <p>Gli oggetti principali del problema vengono visualizzati nella breadcrumb. Facendo clic sul nome dell'oggetto padre viene aperto l'oggetto padre.</p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Panoramica delle breadcrumb</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>L'icona rosa [!UICONTROL Issue] <img src="assets/nwe-issues-icon.png"> viene visualizzato a sinistra del nome del problema.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del problema</td> 
   <td>Puoi modificare il nome del problema nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Il testo "[!UICONTROL ISSUE]" viene visualizzato sopra il nome del problema nell’intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area azioni del problema</td> 
   <td> <p>Accanto al nome del problema viene visualizzata l’area [!UICONTROL actions].</p> <p> <img src="assets/nwe-dependency-action-area.png"> </p> <p>Se viene visualizzata l'icona [!UICONTROL Dependency], è possibile fare clic su di essa per visualizzare eventuali predecessori o successori del problema.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percent Complete]</td> 
   <td> <p>Puoi modificare la percentuale di completamento del problema dall’intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assegnazioni]</td> 
   <td>Puoi modificare gli assegnatari di un problema dall’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lavoraci], [!UICONTROL Fatto], <span>o pulsante [!UICONTROL Avvia problema]</span></td> 
   <td>Se il problema è assegnato a te, puoi fare clic su [!UICONTROL Lavoraci] <span>o [!UICONTROL Start Issue]</span> per indicare che stai lavorando sul problema, oppure il pulsante [!UICONTROL Done] per indicare che il problema è stato completato.<span>Per informazioni sulla sostituzione del pulsante [!UICONTROL Lavoraci] con un pulsante [!UICONTROL Avvia attività], vedere</span> <span href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Sostituisci il pulsante [!UICONTROL Lavoraci] con un pulsante [!UICONTROL Avvia]</a></span><span>.</span></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di completamento Pianificata]</td> 
   <td> <p>È possibile modificare il problema [!UICONTROL Data di completamento pianificata] <span>e ora</span> nell’intestazione.</p> <p>Suggerimento: si noti che [!UICONTROL Commit Date] non è visibile nell'intestazione. È possibile visualizzarlo nella pagina [!UICONTROL Details].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stato]</td> 
   <td>Puoi modificare il problema [!UICONTROL Status] nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area [!UICONTROL Approvals]</td> 
   <td> <p>Se sei uno degli approvatori, utilizza le icone seguenti per gestire le approvazioni per il problema:</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> [!UICONTROL Approva]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> [!UICONTROL rifiuta]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> [!UICONTROL Recall]</p> <p>Se non si è un approvatore, fare clic sull'icona [!UICONTROL Altro] <img src="assets/more-icon-for-approvals-area.png"> per visualizzare informazioni sul passaggio di approvazione corrente.</p> <p>Per ulteriori informazioni sulle approvazioni, consulta <a href="../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Panoramica del processo di approvazione</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Panoramica dell’intestazione del programma

![](assets/program-header-350x18.png)

L’intestazione del programma visualizza le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Breadcrumb con il nome del Portfolio</td> 
   <td> <p>È possibile accedere al Portfolio [!UICONTROL] dall'intestazione del programma [!UICONTROL]. Facendo clic sul nome dell'oggetto padre viene aperto l'oggetto padre.</p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Panoramica delle breadcrumb</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>Icona arancione [!UICONTROL Program] <img src="assets/nwe-programs-icon.png"> viene visualizzato a sinistra del nome del programma.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del programma</td> 
   <td>Puoi modificare il nome del programma nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Se il programma è contrassegnato come [!UICONTROL Attivo], il testo "[!UICONTROL PROGRAMMA]" viene visualizzato sopra il nome del programma nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Stato attivazione</td> 
   <td> <p>Se il programma è disattivato, il testo "[!UICONTROL PROGRAM DEACTIVATED]" viene visualizzato sopra il nome del programma nell’intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Il settore d'azione del programma</td> 
   <td> <p>Accanto al nome del programma, viene visualizzata l'area [!UICONTROL actions].</p> <p> <img src="assets/nwe-general-actions-area.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percent Complete]</td> 
   <td> <p>Impossibile modificare il [!UICONTROL Percent Complete] del programma nell'intestazione. Queste informazioni vengono aggiornate dai progetti nel programma.</p> <p>Suggerimento: per impostazione predefinita, la percentuale di completamento del programma corrisponde alla media dei valori di completamento dei progetti in un [!UICONTROL Current] o [!UICONTROL Approved Status] appartenente al programma.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Manager]</td> 
   <td> <p>È possibile modificare [!UICONTROL Program Manager] nell'intestazione. È lo stesso del [!UICONTROL Proprietario del programma].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data di completamento Pianificata]</td> 
   <td>Non è possibile modificare il programma [!UICONTROL Planned Completion Date] (Data di completamento pianificata) nell'intestazione. Queste informazioni vengono aggiornate dalla [!UICONTROL Planned Completion Date] (Data di completamento pianificata) dei progetti nel programma.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Condizione progetti attivi [!UICONTROL]</td> 
   <td>Questo è un calcolo della percentuale di progetti attivi nel programma per cui la condizione [!UICONTROL] è impostata come [!UICONTROL On Target], [!UICONTROL At Risk] o [!UICONTROL In Trouble].</td> 
  </tr> 
 </tbody> 
</table>

## Panoramica intestazione Portfolio {#portfolio-header-overview}

![](assets/portfolio-header-350x19.png)

L’intestazione del portfolio include le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>L'icona blu [!UICONTROL Portfoli] <img src="assets/nwe-portfolios-icon.png">viene visualizzato a sinistra del nome del portfolio.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del portfolio</td> 
   <td>Puoi modificare il nome del portfolio nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Se il portfolio è contrassegnato come attivo, il testo "[!UICONTROL PORTFOLIO]" viene visualizzato sopra il nome del portfolio nell’intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Stato attivazione</td> 
   <td> <p>Se il portfolio è disattivato, il testo "[!UICONTROL PORTFOLIO DISATTIVATO]" viene visualizzato sopra il nome del portfolio nell’intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">L'area [!UICONTROL actions] del portfolio</td> 
   <td> <p>Accanto al nome del portfolio viene visualizzata l'area [!UICONTROL actions].</p> <p> <img src="assets/nwe-general-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gestione Portfoli]</td> 
   <td>È possibile modificare [!UICONTROL Portfoli Manager] nell'intestazione. Corrisponde al proprietario del Portfolio [!UICONTROL].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL On Time]</td> 
   <td>Questo è un calcolo della percentuale di progetti nel portfolio che sono attualmente in tempo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nel Budget]</td> 
   <td>Si tratta di un calcolo della percentuale di progetti inclusi nel portfolio attualmente nel budget.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Allineato]</td> 
   <td>Si tratta di un calcolo della percentuale di progetti nel portfolio allineati con il portfolio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ROI]</td> 
   <td>Calcolo del [!UICONTROL Return on Investment] per tutti i progetti del portfolio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valore Netto]</td> 
   <td>Calcolo del valore netto di [!UICONTROL] per tutti i progetti nel portfolio.</td> 
  </tr> 
 </tbody> 
</table>

## Panoramica dell’intestazione del modello {#template-header-overview}

![](assets/template-header-350x18.png)

L’intestazione del modello visualizza le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>L'icona verde [!UICONTROL Template] <img src="assets/nwe-templates-icon.png">viene visualizzato a sinistra del nome del modello.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del modello</td> 
   <td>Puoi modificare il nome del modello nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Se il modello è contrassegnato come attivo, il testo "[!UICONTROL TEMPLATE]" viene visualizzato sopra il nome del modello nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Stato attivazione</td> 
   <td> <p>Se il modello è disattivato, il testo "[!UICONTROL TEMPLATE DEACTIVATED]" viene visualizzato sopra il nome del modello nell’intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area azioni del modello</td> 
   <td> <p>Accanto al nome del modello viene visualizzata l’area delle azioni.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proprietario del modello [!UICONTROL]</td> 
   <td>È possibile modificare il campo [!UICONTROL Proprietario modello] nell'intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Duration]</td> 
   <td>La durata del modello. Non puoi modificare questo campo nell’intestazione.</td> 
  </tr> 
 </tbody> 
</table>

## Panoramica dell’intestazione dell’attività modello

![](assets/template-task-header-350x18.png)

Nell&#39;intestazione dell&#39;attività modello vengono visualizzate le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Breadcrumb per oggetti padre</td> 
   <td> <p>Gli oggetti padre dell’attività modello vengono visualizzati nella breadcrumb. Facendo clic sul nome di un oggetto padre, questo viene aperto.</p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Panoramica delle breadcrumb</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>L'icona verde [!UICONTROL Task] <img src="assets/nwe-tasks-icon.png">viene visualizzato a sinistra del nome dell'attività modello.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome dell’attività modello</td> 
   <td>Puoi modificare il nome dell’attività modello nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Il testo "[!UICONTROL TEMPLATE TASK]" viene visualizzato sopra il nome dell'attività modello nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area azioni dell'attività modello</td> 
   <td> <p>Accanto al nome dell’attività modello viene visualizzata l’area delle azioni.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assegnazioni]</td> 
   <td>È possibile modificare le [!UICONTROL Assignments] dell'attività modello nell'intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Completion Day]</td> 
   <td>Questo è il giorno in cui l’attività modello deve essere completata, nella durata del modello.</td> 
  </tr> 
 </tbody> 
</table>

## Panoramica intestazione record fatturazione

![](assets/billing-record-header-nwe-350x19.png)

Nell&#39;intestazione del record fatturazione vengono visualizzate le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Breadcrumb per oggetti padre</td> 
   <td> <p>Gli oggetti padre del record fatturazione vengono visualizzati nella breadcrumb. Facendo clic sul nome di un oggetto padre, questo viene aperto.</p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Panoramica delle breadcrumb</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>Icona blu [!UICONTROL Billing Record] (Fatturazione) <img src="assets/nwe-billing-record-icon-57x55.png" style="width: 57;height: 55;"> viene visualizzato a sinistra del nome del record fatturazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del record fatturazione</td> 
   <td>Puoi modificare il nome del record di fatturazione nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Il testo "[!UICONTROL BILLING RECORD]" viene visualizzato sopra il nome del record di fatturazione nell’intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area azioni del record fatturazione</td> 
   <td> <p>Accanto al nome del record fatturazione, il menu [!UICONTROL Altro] <img src="assets/more-menu.png"> , che consente di selezionare le seguenti opzioni:</p> 
    <ul> 
     <li> <p>[!UICONTROL Modifica]</p> </li> 
     <li> <p> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Totale record fatturazione]</td> 
   <td>Questo è l'importo totale del record fatturazione. Impossibile modificare questo campo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data Fatturazione]</td> 
   <td>Si tratta della data di creazione del record di fatturazione, a meno che non sia stato modificato manualmente al momento della creazione del record di fatturazione. Puoi modificare [!UICONTROL Billing Date] (Data di fatturazione) nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stato]</td> 
   <td> <p>Quando il record fatturazione ha lo stato [!UICONTROL Fatturato], non è più possibile modificarlo.</p> <p>Puoi modificare lo Stato del record di fatturazione nell’intestazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Panoramica dell’intestazione utente

![](assets/user-header-350x20.png)

L’intestazione utente mostra le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Immagine del profilo utente</td> 
   <td>Non è possibile aggiornare l’immagine del profilo nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome dell’utente e titolo</td> 
   <td> <p> Il titolo dell’utente viene visualizzato in lettere maiuscole sopra il nome. Non è possibile modificare il nome dell’utente nell’intestazione.</p> </td> 
  </tr> <!--
   <tr> 
    <td role="rowheader">Name of the object type</td> 
    <td> <p>The name of the object type does not display.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Stato attivazione</td> 
   <td> <p>Se l’utente è stato disattivato, tutto il testo e l’immagine del profilo nell’intestazione vengono oscurati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area azioni dell'utente</td> 
   <td> <p>Accanto al nome dell’utente viene visualizzata l’area delle azioni.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Indirizzo e-mail</td> 
   <td>Non puoi modificare l’indirizzo e-mail nell’intestazione. Di solito si tratta anche del nome utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Numero di telefono</td> 
   <td>Non puoi modificare il numero di telefono nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Team</td> 
   <td> <p>Puoi visualizzare i team a cui appartiene l’utente. Passa il puntatore del mouse su un avatar del team per visualizzarne il nome. Non puoi modificare i team nell’intestazione.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Panoramica dell’intestazione del team

![](assets/team-header-350x23.png)

L’intestazione del team mostra le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>Icona viola [!UICONTROL Team] <img src="assets/nwe-teams-icon.png"> viene visualizzato a sinistra del nome del team.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del team</td> 
   <td>Puoi modificare il nome del team nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Il testo "[!UICONTROL TEAM]" viene visualizzato sopra il nome del team nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">L’area Azioni del team</td> 
   <td> <p>Accanto al nome del team viene visualizzata l'area [!UICONTROL actions].</p> <p> <img src="assets/nwe-switch-team-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Immagini del profilo del membro del team</td> 
   <td>Le immagini del profilo dei membri del team. Passa il puntatore del mouse sopra un'immagine per visualizzarne il nome.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Descrizione</td> 
   <td>Breve descrizione dei membri del team. Non puoi modificare la descrizione del team nell’intestazione.</td> 
  </tr> 
 </tbody> 
</table>

## Panoramica dell’intestazione dell’iterazione

![](assets/iteration-header-350x19.png)

Nell&#39;intestazione dell&#39;iterazione vengono visualizzate le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>Icona arancione [!UICONTROL Iteration] <img src="assets/nwe-iteration-icon-58x58.png" style="width: 58;height: 58;"> viene visualizzato a sinistra del nome dell'iterazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome dell'iterazione</td> 
   <td>Puoi modificare il nome dell’iterazione nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Il testo "[!UICONTROL ITERATION]" viene visualizzato sopra il nome dell'iterazione nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area azioni dell'iterazione</td> 
   <td> <p>Nell’angolo superiore destro dell’intestazione viene visualizzata l’area delle azioni.</p> <p> <img src="assets/nwe-iteration-action-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proprietario</td> 
   <td>Proprietario [!UICONTROL] dell'iterazione. Impossibile modificare [!UICONTROL Owner] nell'intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeline]</td> 
   <td>La sequenza temporale di [!UICONTROL] mostra le date di inizio e di fine dell'iterazione. Impossibile modificare la sequenza temporale [!UICONTROL] nell'intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team]</td> 
   <td>Non è possibile modificare il team dell’iterazione nell’intestazione. Facendo clic sul nome del team viene visualizzata la pagina del team.</td> 
  </tr> 
 </tbody> 
</table>

## Panoramica dell’intestazione del gruppo

![](assets/nwe-group-header-350x20.png)

Nell&#39;intestazione del gruppo vengono visualizzate le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>Icona arancione di [!UICONTROL Group] <img src="assets/nwe-group-icon.png"> viene visualizzato a sinistra del nome del gruppo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del gruppo</td> 
   <td>Puoi modificare il nome del gruppo nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Il testo "[!UICONTROL GROUP]" viene visualizzato sopra il nome del gruppo nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area [!UICONTROL actions] del gruppo</td> 
   <td> <p>Accanto al nome del gruppo, viene visualizzato il menu [!UICONTROL Altro] <img src="assets/more-menu.png"> , che consente di selezionare le seguenti opzioni:</p> 
    <ul> 
     <li> <p>[!UICONTROL Modifica]</p> </li> 
     <li> <p>[!UICONTROL Copy]</p> </li> 
     <li> <p>[!UICONTROL Elimina]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Business Leader]</td> 
   <td>È possibile modificare [!UICONTROL Business Leader] nell'intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Licenses in uso] </td> 
   <td> <p>Nella casella [!UICONTROL Licenses in use] viene visualizzato il numero di utenti di licenze [!UICONTROL Plan] e [!UICONTROL Work] nel gruppo e nei relativi sottogruppi. È possibile fare clic sui numeri per visualizzare queste informazioni per tutti e 5 i tipi di licenza.</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md" class="MCXref xref">Visualizza il numero di licenze allocate e utilizzate in un gruppo nel nuovo [!DNL Adobe Workfront] esperienza</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group Administrators]</td> 
   <td>Puoi modificare gli amministratori di gruppi nell’intestazione.</td> 
  </tr> 
 </tbody> 
</table>

## Panoramica dell’intestazione del documento

![](assets/document-header-350x19.png)

Nell&#39;intestazione del documento vengono visualizzate le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Breadcrumb con oggetti padre</td> 
   <td> <p>Gli oggetti padre del documento vengono visualizzati nel breadcrumb. Facendo clic sul nome di un oggetto padre, questo viene aperto.</p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Panoramica delle breadcrumb</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>L'icona blu [!UICONTROL Document] <img src="assets/nwe-documents-icon-53x50.png" style="width: 53;height: 50;"> viene visualizzato a sinistra del nome del documento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del documento</td> 
   <td>È possibile modificare il nome del documento nell'intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Il testo "[!UICONTROL DOCUMENT]" viene visualizzato sopra il nome del documento nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area azioni del documento</td> 
   <td> <p>Accanto al nome del documento viene visualizzata l'area delle azioni.</p> <p> <img src="assets/nwe-doc-version-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area [!UICONTROL Decision] di approvazione</td> 
   <td> L'area [!UICONTROL Decisions] viene visualizzata nell'angolo superiore destro dell'intestazione del documento. Questa area varia in base alla fase di approvazione e al fatto che si sia un approvatore, un revisore o nessuno dei due. <ul><li> <p>Se si è un approvatore, è possibile utilizzare le icone seguenti per gestire le approvazioni del documento:</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> [!UICONTROL Approva]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> [!UICONTROL Recall]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> [!UICONTROL rifiuta]</p> <p>Per ulteriori informazioni sulle decisioni di approvazione, consulta <a href="../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Approvazione del lavoro</a>.</li><li><p>Se si è un revisore, è possibile fare clic sul pulsante Completa revisione personale per indicare che è stato rivisto il documento.</p><p>Per ulteriori informazioni sulla revisione di un documento, vedere <a href="../../review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-a-document.md" class="MCXref xref">Rivedere un documento</a>.</p></li><li>In caso contrario, quest'area mostra lo stato di revisione e approvazione corrente del documento.</li><ul></p> </td> 
  </tr> 
 </tbody> 
</table>

## Panoramica intestazione società {#company-header-overview}

![](assets/company-header-350x20.png)

L’intestazione dell’azienda mostra le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>L'icona blu [!UICONTROL Company] <img src="assets/nwe-company-icon.png"> viene visualizzato a sinistra del nome della società.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome della società</td> 
   <td>Puoi modificare il nome della società nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Il testo "[!UICONTROL COMPANY]" viene visualizzato sopra il nome della società nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">L’area delle azioni dell’azienda</td> 
   <td> <p>Accanto al nome della società, viene visualizzato il menu [!UICONTROL Altro] <img src="assets/more-menu.png"> , che consente di selezionare le seguenti opzioni:</p> 
    <ul> 
     <li> <p>[!UICONTROL Modifica]</p> </li> 
     <li> <p>[!UICONTROL Elimina società]</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Panoramica dell’intestazione del piano

![](assets/nwe-plan-header-350x34.png)

I piani sono gli oggetti [!DNL Workfront Scenario Planner]. Per informazioni su [!DNL Scenario Planner], vedi [Il [!DNL Scenario Planner] panoramica](../../scenario-planner/scenario-planner-overview.md).

Nell&#39;intestazione del piano vengono visualizzate le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Torna ai piani</td> 
   <td>Facendo clic su questo collegamento si accede all'elenco [!UICONTROL Plans].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>Icona blu [!UICONTROL Plan] <img src="assets/nwe-plan-icon-65x62.png" style="width: 65;height: 62;">viene visualizzato a sinistra del nome del piano.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del piano</td> 
   <td>Puoi modificare il nome del piano nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Il testo "[!UICONTROL PLAN]" viene visualizzato sopra il nome del piano nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">L'area delle azioni del piano</td> 
   <td> <p>Accanto al nome del piano viene visualizzata l'area delle azioni.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Azioni del piano aggiuntive</td> 
   <td> <p>Sotto il nome del piano e l'area delle azioni, è possibile completare le azioni riportate di seguito.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mostra conflitti]</strong>: facendo clic su questa opzione, si mostrano o si nascondono i conflitti nelle iniziative.</p> </li> 
     <li> <p><strong>[!UICONTROL Confronta scenari]</strong>: facendo clic su questo collegamento viene visualizzato un confronto affiancato degli scenari creati.</p> </li> 
     <li> <p><strong>[!UICONTROL Selezione scenario]</strong>: in questo menu a discesa puoi copiare uno scenario o selezionarlo per visualizzarne uno diverso.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Informazioni ruolo</td> 
   <td>Nella casella [!UICONTROL Ruolo] è possibile visualizzare il numero di ruoli disponibili per il piano rispetto al numero di ruoli richiesti. Facendo clic sulla casella è possibile regolare i ruoli disponibili.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Informazioni finanziarie di [!UICONTROL]</td> 
   <td>Nella casella [!UICONTROL Financial] è possibile visualizzare il budget, il costo e la percentuale di utilizzo per il piano. Facendo clic sulla casella è possibile adeguare l'importo del budget e determinare se i costi delle persone sono inclusi nel piano.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valore Netto]</td> 
   <td>Nella casella [!UICONTROL Valore netto] è possibile visualizzare il valore netto del piano in base al budget e ai costi inseriti per il piano.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Informazioni su [!UICONTROL condiviso con]</td> 
   <td>Gli utenti che possono visualizzare o gestire il piano vengono visualizzati nell’angolo superiore destro dell’intestazione. Passando il puntatore del mouse sulle immagini del profilo vengono visualizzati i relativi nomi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vai alla pubblicazione]</td> 
   <td>Quando fai clic su [!UICONTROL Vai a pubblicazione], puoi creare o aggiornare un progetto collegato a un'iniziativa nello scenario che stai visualizzando.</td> 
  </tr> 
 </tbody> 
</table>


## Panoramica intestazione obiettivo

![](assets/goal-header.png)

Puoi creare obiettivi strategici quando la tua azienda ha accesso agli Obiettivi di Workfront. Per ulteriori informazioni su [!DNL Workfront Goals], vedi [Introduzione a [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

L’intestazione dell’obiettivo mostra le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informazioni intestazione</th> 
   <th>Note</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Icona oggetto </td> 
   <td> <p>L'icona viola [!UICONTROL Goal] <img src="assets/goal-icon.png" > viene visualizzato a sinistra del nome dell’obiettivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome dell’obiettivo</td> 
   <td>Puoi modificare il nome dell’obiettivo nell’intestazione.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome del tipo di oggetto</td> 
   <td> <p>Il testo "[!UICONTROL GOAL]" viene visualizzato sopra il nome dell'obiettivo nell'intestazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Area azioni dell’obiettivo</td> 
   <td> <p>Accanto al nome dell’obiettivo viene visualizzata l’area delle azioni.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p>
   Dall’area delle azioni dell’obiettivo puoi eseguire le azioni seguenti:
   <ul><li>[!UICONTROL Modifica]</li>
   <li>[!UICONTROL Copia obiettivo]</li>
   <li>[!UICONTROL Elimina obiettivo]</li>
   <li>[!UICONTROL Share]</li>
   <li>[!UICONTROL Attiva] o [!UICONTROL Disattiva]</li>
   <li>[!UICONTROL Chiudi] o [!UICONTROL Riapri]</li>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Avanzamento]</td> 
   <td>Percentuale dell’obiettivo di avanzamento, che indica la parte dell’obiettivo completata. Non è possibile aggiornare l’avanzamento dell’obiettivo. Workfront lo calcola in base all’avanzamento di ogni indicatore di avanzamento sull’obiettivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proprietario]</td> 
   <td>Questo è il proprietario dell'obiettivo. Puoi aggiornare manualmente il proprietario dell’obiettivo. Utenti, team, gruppi o la tua organizzazione possono essere proprietari di obiettivi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Period]</td> 
   <td>Intervallo di tempo durante il quale l’obiettivo deve essere completato. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Condizione [!UICONTROL]</td> 
   <td>La condizione dell’obiettivo indica se l’obiettivo è sul target da completare in tempo o se è in ritardo </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stato]</td> 
   <td>Indica se l’obiettivo è attivo, nuovo o chiuso. Non è possibile aggiornare manualmente lo stato dell’obiettivo. Per ulteriori informazioni, consulta <a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">Panoramica sullo stato degli obiettivi in [!DNL Adobe Workfront Goals]</a></td> 
  </tr> 
 </tbody> 
</table>