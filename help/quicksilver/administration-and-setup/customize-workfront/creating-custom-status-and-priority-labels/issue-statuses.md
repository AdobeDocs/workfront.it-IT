---
title: Accedere all’elenco degli stati dei problemi del sistema
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: È possibile utilizzare lo stato di un problema per mostrare agli utenti del sistema in quale fase di sviluppo si trova un problema in un determinato momento.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '1444'
ht-degree: 0%

---

# Accedere all’elenco degli stati dei problemi di sistema

È possibile utilizzare lo stato di un problema per mostrare agli utenti del sistema in quale fase di sviluppo si trova un problema in un determinato momento.

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
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>Oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Accedere agli stati dei problemi

Puoi accedere e modificare gli stati dei problemi a livello di sistema. È possibile modificare alcune informazioni sugli stati di sistema predefiniti oppure creare nuovi stati personalizzati. Per ulteriori informazioni sulla creazione di stati personalizzati o sulla modifica di stati di sistema, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Per accedere agli stati dei problemi a livello di sistema:

{{step-1-to-setup}}

1. Fai clic su **Preferenze progetto** > **Stati**.

1. Fai clic sulla scheda **Issues** per visualizzare gli stati dei problemi disponibili in Workfront.

   ![](assets/issue-status.png)

## Stati dei problemi di sistema

Workfront viene fornito con 10 stati di problema originali. Le prime 4 nella tabella seguente sono obbligatorie, pertanto è possibile sbloccarle, rinominarle e riordinarle, ma non è possibile nasconderle o eliminarle.

Puoi aggiungere stati di problema personalizzati in base alle esigenze della tua organizzazione. Per ulteriori informazioni, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Per gli utenti, la modifica dello stato di un problema è in genere un processo manuale. Tuttavia, in alcuni casi, descritti nell&#39;elenco seguente, lo stato di un problema cambia automaticamente a seconda di altri fattori che si verificano nel sistema.

Nell’istanza di Workfront vengono forniti i seguenti stati di problema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Stato problema di sistema</th> 
   <th>Come utilizzare lo stato</th> 
   <th>Cosa succede nello stato</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nuovo (stato obbligatorio)</td> 
   <td>Questo è lo stato predefinito per ogni problema appena creato.</td> 
   <td>Se il problema riguarda un progetto con lo stato Attuale, il problema viene visualizzato nella scheda Richieste di lavoro degli utenti assegnati al problema. Gli utenti possono ora iniziare a lavorare sul problema.</td> 
  </tr> 
  <tr> 
   <td>In corso (stato obbligatorio)</td> 
   <td> <p>È possibile inserire un problema in questo stato per indicare che il lavoro su tale problema è iniziato.</p> <p>Se la risoluzione del problema è connessa a un altro oggetto (un'attività, un progetto o un altro problema), lo stato del problema viene modificato automaticamente in In corso quando si modifica lo stato dell'oggetto di risoluzione in In corso. </p> <p>Per ulteriori informazioni sulla risoluzione degli oggetti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sugli oggetti risolvibili e risolvibili </a>.</p> </td> 
   <td> <p>Se il problema riguarda un progetto con lo stato Attuale, il problema viene visualizzato nella scheda Lavori in corso degli utenti assegnati al problema.</p> <p>Quando un problema è In corso, il problema mostra un valore per Data di inizio effettiva.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Chiuso (stato obbligatorio)</td> 
   <td> <p>Puoi contrassegnare manualmente un problema come Chiuso quando il lavoro su di esso viene completato. </p> <p>Se la risoluzione del problema è connessa a un altro oggetto (un'attività, un progetto o un altro problema), lo stato del problema viene modificato automaticamente in Chiuso, quando si modifica lo stato dell'oggetto di risoluzione in Chiuso.</p> <p>Per ulteriori informazioni sulla risoluzione degli oggetti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sugli oggetti risolvibili e risolvibili </a>.</p> </td> 
   <td> <p>Quando un problema viene chiuso, viene rimosso dall’elenco Lavori in corso dell’assegnatario. In questo caso, il problema mostra un valore per Data di completamento effettiva. </p> <p>Quando tutte le attività sono completate e i problemi sono chiusi in un progetto, il progetto può essere completato.</p> </td> 
  </tr> 
  <tr> 
   <td>In sospeso (stato obbligatorio)</td> 
   <td> <p>È possibile contrassegnare manualmente un problema come In sospeso, per indicare che si è verificato un ritardo nel completamento del problema. </p> </td> 
   <td> <p>Se il problema riguarda un progetto con lo stato Attuale, il problema viene visualizzato nella scheda Lavori in corso degli utenti assegnati al problema. </p> <p>Quando tutte le attività sono completate in un progetto, ma è presente almeno un problema In sospeso nel progetto, il progetto non può essere completato. </p> </td> 
  </tr> 
  <tr> 
   <td>Riaperto (equivale a In corso)</td> 
   <td> <p>È possibile inserire un problema in questo stato per indicare che il lavoro su tale problema non era ancora stato completato quando il problema era stato precedentemente chiuso e che era necessario riaprirlo per completare il lavoro.</p> </td> 
   <td> <p>Se il problema riguarda un progetto con lo stato Attuale, il problema viene visualizzato nella scheda Richieste di lavoro degli utenti assegnati al problema. Gli utenti possono ora iniziare a lavorare sul problema.</p> <p>Questo stato è importante nel reporting, per distinguere tra problemi aperti per la prima volta (di solito nello stato Nuovo) e problemi aperti dopo la chiusura precedente (di solito nello stato Riaperto). </p> </td> 
  </tr> 
  <tr> 
   <td>In attesa di feedback (equivale a In attesa)</td> 
   <td>È possibile inserire un problema in questo stato per indicare che si è in attesa di un feedback (in genere dal contatto principale) prima di poter continuare a lavorare sul problema. </td> 
   <td> <p>Se il problema riguarda un progetto con lo stato Attuale, il problema viene visualizzato nella scheda Lavori in corso degli utenti assegnati al problema.</p> <p>Se un problema è In attesa di feedback, non è possibile completare un progetto.</p> <p>Questo stato è importante nella generazione rapporti, per distinguere tra i problemi attualmente aperti ma su cui si sta lavorando (di solito nello stato In corso) e i problemi attualmente aperti ma non in fase di elaborazione, perché è necessario un feedback maggiore per completarli (di solito nello stato In attesa di feedback).</p> </td> 
  </tr> 
  <tr> 
   <td>Impossibile duplicare (equivale a Chiuso)</td> 
   <td>È possibile inserire un problema in questo stato per indicare che si sta chiudendo il problema, ma non è stato possibile visualizzare il problema che ha attivato l’apertura del problema. Il problema potrebbe ancora esistere, ma non può essere replicato in un determinato momento. </td> 
   <td> <p>Questo stato è importante nel reporting, per distinguere tra problemi completati e il cui problema è stato risolto (di solito nello stato Chiuso) e problemi il cui problema non è visibile in un dato momento (di solito nello stato Non può essere duplicato).</p> <p>Quando un problema è contrassegnato come non duplicabile, viene rimosso dall’elenco Working On dell’assegnatario. In questo caso, il problema mostra un valore per Actual CompletionDate.</p> <p>Se tutte le attività di un progetto sono completate e alcuni problemi si trovano in stato Impossibile duplicare, il progetto può essere completato.</p> </td> 
  </tr> 
  <tr> 
   <td>Risolto (equivale a Chiuso)</td> 
   <td>È possibile inserire un problema in questo stato per indicare che si sta chiudendo il problema e che il problema che lo ha creato è stato effettivamente risolto.</td> 
   <td> <p>Questo stato è importante nella generazione dei rapporti per distinguere tra i problemi chiusi con o senza risoluzione (di solito nello stato Chiuso) e i problemi chiusi con una risoluzione effettiva (di solito nello stato Risolto).</p> <p>Quando un problema è contrassegnato come Risolto, viene rimosso dall’elenco Lavori in corso dell’assegnatario. In questo caso, il problema mostra un valore per Data di completamento effettiva.</p> <p>Se tutte le attività di un progetto sono completate e almeno un problema si trova nello stato Risolto, il progetto può essere completato. </p> </td> 
  </tr> 
  <tr> 
   <td>Verifica completata (equivale a Chiusa)</td> 
   <td>È possibile inserire un problema in questo stato per indicare che si sta chiudendo il problema e che si è verificato che il problema che ha generato il problema è stato risolto.</td> 
   <td> <p>Quando un problema è contrassegnato come Completato verificato, viene rimosso dall’elenco Lavori in corso dell’assegnatario. In questo caso, il problema mostra un valore per Data di completamento effettiva.</p> <p>Se tutte le attività di un progetto sono completate e alcuni problemi si trovano in stato Completato verificato, il progetto può essere completato.</p> </td> 
  </tr> 
  <tr> 
   <td>Non risolvibile (equivale a Chiuso)</td> 
   <td>È possibile inserire un problema in questo stato per indicare che si sta chiudendo il problema, ma il problema che lo ha generato non può essere risolto.</td> 
   <td> <p>Questo stato è importante nella generazione dei rapporti per distinguere tra i problemi chiusi con o senza risoluzione (di solito nello stato Chiuso) e i problemi chiusi senza risoluzione effettiva (di solito nello stato Won't Resolve).</p> <p>Quando un problema è contrassegnato come Non risolvibile, viene rimosso dall’elenco Lavori in corso dell’assegnatario. In questo caso, il problema mostra un valore per Data di completamento effettiva.</p> <p>Se tutte le attività di un progetto sono completate e almeno un problema si trova nello stato Non risolvere, il progetto può essere completato.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzazione degli stati dei problemi

Un amministratore di Workfront può aggiungere a Workfront gli stati dei problemi a livello di sistema e di gruppo e modificare l’ordine in cui gli utenti li visualizzano. Per ulteriori informazioni, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Un amministratore di gruppo può aggiungere uno stato personalizzato specifico per un gruppo. Per ulteriori informazioni, vedere [Creare o modificare lo stato di un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
