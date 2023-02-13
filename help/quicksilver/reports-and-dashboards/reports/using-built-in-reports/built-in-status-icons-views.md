---
product-area: reporting
navigation-topic: using-built-in-reports
title: Icone di stato incorporate nelle visualizzazioni
description: Icone di stato incorporate nelle visualizzazioni
author: Nolan
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1291'
ht-degree: 2%

---

# Icone di stato incorporate nelle visualizzazioni

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.) </p>
-->

È possibile aggiungere il campo Icone di stato incorporato come colonna nelle viste per migliorare la visibilità nei punti chiave degli oggetti. Utilizzando le icone di stato, è possibile vedere rapidamente quando sono presenti le seguenti condizioni:

* Un oggetto presenta documenti allegati
* Un oggetto è associato a un processo di approvazione
* A un oggetto sono associate note aggiuntive
* Una spesa è fatturabile o rimborsabile
* Un&#39;attività si trova su un percorso critico
* Un utente appartiene a una società, a un team o si trova in un fuso orario diverso

La maggior parte degli indicatori nel campo Icone di stato sono collegamenti rapidi all’oggetto o all’area effettiva dell’oggetto che rappresentano.

Se nell’oggetto manca uno degli elementi rappresentati dalle icone, l’icona che rappresenta l’elemento mancante viene visualizzata come un contorno nella colonna Icone di stato anziché come immagine completa.\
![task_status_icone.png](assets/task-status-icons.png)\
Per ulteriori informazioni, consulta la sezione [Panoramica delle icone di stato e dei flag](#overview-of-status-icons-and-flags) in questo articolo.\
In alcune visualizzazioni, il **Icone di stato** campo denominato **Flag** o **Visualizza icone**.\
Non è possibile personalizzare l’aspetto delle icone incluse nel campo Icone di stato .

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Modificare l’accesso a Report, Dashboard e Calendari per aggiungere colonne a un report</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per una visualizzazione esistente</p> <p>Gestisci le autorizzazioni per un report per aggiungergli colonne</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Aggiungere il campo Icone di stato a una visualizzazione

Alcune viste e rapporti incorporati dispongono già del campo Icone di stato incluso.

Non è possibile aggiungere il campo Icone di stato a tutte le visualizzazioni.

Per aggiungere il campo Icone di stato a una visualizzazione personalizzata creata da zero:

1. Passare a un elenco di uno dei seguenti oggetti:

   * Attività
   * Problemi
   * Progetti
   * Attività modello
   * Modelli
   * Spese
   * Documenti
   * Utenti\
      Solo questi oggetti hanno **Icone di stato** campo disponibile.\
      Per informazioni sugli elenchi di oggetti, vedere [Guida introduttiva agli elenchi in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Da **Visualizza** menu a discesa, seleziona **Nuova vista**.

1. Fai clic su **Aggiungi colonna**.
1. In **Mostra in questa colonna** iniziare a digitare uno dei seguenti nomi di campo, quindi selezionarlo quando viene visualizzato nell&#39;elenco:

   * *Le icone di Stato*
   * *Flag*
   * *Visualizza icone *(solo nelle viste documento).

   Le icone incorporate sono elencate sotto uno qualsiasi di questi nomi.\
   Una visualizzazione Modello contiene sia la **Icone di stato** e **Flag** campi. In questo caso, le due colonne contengono icone identiche.\
   Le visualizzazioni documenti contengono un **Visualizza icone** campo .

1. Fai clic su **Salva visualizzazione**.
1. (Facoltativo) Specifica un nuovo nome per la visualizzazione, quindi fai clic su **Salva visualizzazione**.\
   Questo aggiunge il **Icone di stato** nella tua visualizzazione.
1. (Facoltativo) Passa il puntatore del mouse su un&#39;icona per capire cosa rappresenta.
1. (Facoltativo) Fai clic su un&#39;icona per passare all&#39;area dell&#39;oggetto da essa rappresentato.\
   Non tutte le icone sono collegamenti agli oggetti.\
   Per un elenco completo degli attributi per ciascuna icona, consulta [Panoramica delle icone di stato e dei flag](#overview-of-status-icons-and-flags) sezione .

## Panoramica delle icone di stato e dei flag {#overview-of-status-icons-and-flags}

Nella tabella seguente sono elencate tutte le icone di stato disponibili in Workfront, il tipo di oggetti che possono essere associati ad esse e ciò che accade quando si fanno clic su di esse.

Per poter fare clic su alcune delle icone seguenti e accedere a tali oggetti, è necessario disporre delle autorizzazioni per visualizzare almeno gli oggetti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Icona o contrassegno di stato</strong> </th> 
   <th><strong>Descrizione</strong> </th> 
   <th><strong>Oggetto</strong> </th> 
   <th>Al clic</th> 
   <th> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/condition-update-icon-on-target-29x34.png" alt="condition_update_icon_on_target.png" style="width: 29;height: 34;">o <img src="assets/screen-shot-2018-08-17-at-9.49.36-am-29x37.png" alt="Screen_Shot_2018-08-17_at_9.49.36_AM.png" style="width: 29;height: 37;"><br><img src="assets/condition-update-icon--in-trouble-29x26.png" alt="condition_update_icon__in_trou.png" style="width: 29;height: 26;"> o <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-29x26.png" style="width: 29;height: 26;"><br><img src="assets/condition-update-at-risk-27x28.png" alt="condition_update_at_risk.png" style="width: 27;height: 28;"> o <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-33x34.png" alt="Screen_Shot_2018-08-17_at_9.49.23_AM.png" style="width: 33;height: 34;"></td> 
   <td>Indica che la condizione del progetto è On Target (verde), In Trouble (rosso) o At Risk (giallo).<br>Per informazioni sulla condizione del progetto, consulta <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Panoramica del tipo di condizione e condizione del progetto</a>.</td> 
   <td>Progetti</td> 
   <td>Fai clic su per aprire l’elenco delle attività del progetto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>Indica che l’oggetto contiene note (aggiornamenti) nella scheda Aggiornamenti.</td> 
   <td> <p>Progetti<br>Attività<br>Problemi<br>Modelli<br>Attività dei modelli</p> </td> 
   <td> <p>Fare clic per aprire la scheda Aggiornamenti dell’oggetto. </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">oppure <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>Indica che all’oggetto sono associati documenti. </td> 
   <td> Progetti<br>Attività<br>Problemi<br>Modelli<br>Attività dei modelli </td> 
   <td>Fare clic per aprire la scheda Documenti dell'oggetto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issu_icon.png" style="width: 34;height: 36;">oppure <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>Indica che sono presenti problemi aperti nel progetto o nell’attività.</td> 
   <td> Progetti<br>Attività </td> 
   <td>Fare clic per aprire l’oggetto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="authorization_icon.png" style="width: 42;height: 38;"> oppure <img src="assets/new-approval-icon-33x35.png" alt="new_authorization_icon.png" style="width: 33;height: 35;"></td> 
   <td>Indica che sull'oggetto è presente un'approvazione.</td> 
   <td> Progetti<br>Attività<br>Problemi<br>Modelli<br>Attività dei modelli </td> 
   <td>Fare clic per aprire l’oggetto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="cost_icon.png" style="width: 52;height: 40;"> </td> 
   <td> <p>Puoi aggiungere una colonna Icona Spese nella visualizzazione per visualizzare questa icona. Ciò indica che il progetto o l'attività hanno le relative spese associate.</p> </td> 
   <td> <p>Progetti</p> <p>Attività</p> </td> 
   <td>Fai clic su per aprire la scheda Spese del progetto o dell’attività. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>Indica che lo stato di avanzamento di un'attività è uno dei seguenti:</p> 
    <ul> 
     <li>Ora di attivazione (quadrato verde)</li> 
     <li>Ritardo (cerchio rosso)</li> 
     <li>A rischio (diamante blu)</li> 
     <li>Dietro (triangolo giallo)</li> 
    </ul> <p>Per informazioni sullo stato di avanzamento delle attività, vedere <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Panoramica sullo stato dell'avanzamento dell'attività</a>.</p> </td> 
   <td>Attività</td> 
   <td>Fare clic per aprire l'attività. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="task_critical_path_icon.png" style="width: 36;height: 35;"> oppure <img src="assets/new-critical-path-icon-34x34.png" alt="new_critical_path_icon.png" style="width: 34;height: 34;"></td> 
   <td>Indica che l'attività è attualmente nel percorso critico. <br>Per informazioni sulle attività in un percorso critico del progetto, consulta <a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref">Panoramica del progetto Percorso critico</a>.</td> 
   <td>Attività</td> 
   <td>Fare clic per aprire l'attività.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="milestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>Indica che l'attività è associata a un'attività cardine. L’amministratore di sistema può personalizzare il colore del rombo nell’ambiente.<br>Per informazioni sulle milestone, vedi <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Creare un percorso cardine</a>.</td> 
   <td>Attività</td> 
   <td>Fare clic per aprire l'attività. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>Collega all'oggetto sorgente di un problema. L'oggetto di origine di un problema è l'oggetto in cui è stato registrato il problema. Un'attività o un progetto può essere oggetto di origine dei problemi. </td> 
   <td>Problemi</td> 
   <td>Fare clic per aprire l'oggetto di origine (attività o progetto) di un problema. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resolve_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>Indica che esiste un oggetto di risoluzione che risolve il problema. In questo caso, non è possibile completare il problema. Viene completato al completamento dell'oggetto di risoluzione. <br>Per informazioni sulla risoluzione degli oggetti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sulla risoluzione e risoluzione di oggetti </a>.</td> 
   <td>Problemi</td> 
   <td>Fare clic per aprire l'oggetto di risoluzione del problema. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>Visualizza un documento.</td> 
   <td>Documenti</td> 
   <td>Fai clic su per scaricare il documento.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/download-doc-icon.png"> </td> 
   <td>Scarica un documento.</td> 
   <td>Documenti</td> 
   <td>Fai clic su per scaricare il documento.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-type-icon.png"> </td> 
   <td>Indica il tipo di documento.</td> 
   <td>Documenti</td> 
   <td>Fai clic su per scaricare il documento.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_owned_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>Indica che l'utente è associato a un'azienda. </td> 
   <td>Utenti</td> 
   <td>Non disponibile</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>Indica che l'utente è associato a un team.</td> 
   <td>Utenti</td> 
   <td>Fai clic su per aprire il profilo utente.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>Collegamento alla scheda Allocazione dell’utente. </td> 
   <td>Utenti</td> 
   <td>Fai clic su per aprire la scheda Allocazione dell’utente e scopri gli elementi di lavoro assegnati all’utente.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/screen-shot-2018-07-26-at-2.31.40-pm-44x40.png" alt="Screen_Shot_2018-07-26_at_2.31.40_PM.png" style="width: 44;height: 40;"> </td> 
   <td>Indica che l'utente si trova in un fuso orario diverso da quello del sistema.</td> 
   <td>Utenti</td> 
   <td>Non disponibile</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="billable_cost_icon.png" style="width: 44;height: 45;"> </td> 
   <td>Indica che una spesa è fatturabile.<br>Per informazioni sulle spese, vedi <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gestione delle spese di progetto </a>.</td> 
   <td>Spese</td> 
   <td>Non disponibile</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expense-reimbursable-icon-44x45.png" alt="spesa_rimborsable_icon.png" style="width: 44;height: 45;"> </td> 
   <td> Indica che una spesa è rimborsabile.<br>Per informazioni sulle spese, vedi <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gestione delle spese di progetto </a>.</td> 
   <td>Spese</td> 
   <td>Non disponibile</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="purchased_cost_icon.png" style="width: 44;height: 43;"></td> 
   <td> Indica che una spesa è stata rimborsata.<br>Per informazioni sulle spese, vedi <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gestione delle spese di progetto </a>.</td> 
   <td>Spese</td> 
   <td>Non disponibile</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
