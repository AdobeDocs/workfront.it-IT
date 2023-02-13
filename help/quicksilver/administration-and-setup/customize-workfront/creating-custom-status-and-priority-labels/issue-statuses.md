---
title: Accedere all’elenco degli stati dei problemi del sistema
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Puoi utilizzare lo stato di un problema per mostrare agli utenti del sistema in quale fase di sviluppo un problema si trova in un dato momento.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# Accedere all’elenco degli stati dei problemi del sistema

Puoi utilizzare lo stato di un problema per mostrare agli utenti del sistema in quale fase di sviluppo un problema si trova in un dato momento.

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Stato dei problemi di accesso

Puoi accedere e modificare gli stati dei problemi a livello di sistema. È possibile modificare alcune informazioni sugli stati di sistema predefiniti oppure creare nuovi stati personalizzati. Per ulteriori informazioni sulla creazione di stati personalizzati o sulla modifica degli stati del sistema, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Per accedere agli stati dei problemi a livello di sistema:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Preferenze del progetto** > **Stati**.

1. Fai clic sul pulsante **Problemi** per visualizzare gli stati del problema disponibili in Workfront.

   ![](assets/issue-status.png)

## Stato dei problemi del sistema

Workfront viene fornito con 10 stati di problemi originali. I primi 4 della tabella seguente sono obbligatori, il che significa che è possibile sbloccare, rinominare e riordinare i file, ma non è possibile nasconderli o eliminarli.

Puoi aggiungere stati di problema personalizzati per soddisfare le esigenze della tua organizzazione. Per ulteriori informazioni, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Per gli utenti, cambiare lo stato di un problema è in genere un processo manuale. Tuttavia, in alcune situazioni, descritte nell’elenco seguente, lo stato di un problema cambia automaticamente in base ad altri fattori che si verificano nel sistema.

Con l’istanza Workfront vengono forniti i seguenti stati del problema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Stato del problema del sistema</th> 
   <th>Come utilizzare lo stato</th> 
   <th>Cosa succede nello stato</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nuovo (stato obbligatorio)</td> 
   <td>Questo è lo stato predefinito per ogni nuovo problema creato.</td> 
   <td>Se il problema si trova in un progetto con stato Corrente, il problema viene visualizzato nella scheda Richieste di lavoro degli utenti assegnati al problema. Gli utenti possono ora iniziare a lavorare sul problema.</td> 
  </tr> 
  <tr> 
   <td>In corso (stato richiesto)</td> 
   <td> <p>È possibile inserire un problema in questo stato per indicare che il lavoro su tale problema è iniziato.</p> <p>Se la risoluzione del problema è collegata a un altro oggetto (un'attività, un progetto o un altro problema), lo stato del problema viene automaticamente modificato in In corso quando si cambia lo stato dell'oggetto di risoluzione in In corso. </p> <p>Per ulteriori informazioni sulla risoluzione degli oggetti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sulla risoluzione e risoluzione di oggetti </a>.</p> </td> 
   <td> <p>Se il problema si trova in un progetto con stato Current, il problema viene visualizzato nella scheda Working on degli utenti che sono stati assegnati al problema.</p> <p>Quando un problema è in corso, il problema mostra un valore per la Data di inizio effettiva.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Chiuso (stato richiesto)</td> 
   <td> <p>Puoi contrassegnare manualmente un problema come Chiuso al termine del lavoro. </p> <p>Se la risoluzione del problema è collegata a un altro oggetto (un'attività, un progetto o un altro problema), lo stato del problema viene modificato automaticamente in Chiuso quando si cambia lo stato dell'oggetto di risoluzione in Chiuso.</p> <p>Per ulteriori informazioni sulla risoluzione degli oggetti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sulla risoluzione e risoluzione di oggetti </a>.</p> </td> 
   <td> <p>Quando un problema viene chiuso, il problema viene rimosso dall'elenco di lavoro degli assegnatari. In questo caso, il problema mostra un valore per la Data di completamento effettiva. </p> <p>Quando tutte le attività vengono completate e i problemi vengono chiusi in un progetto, il progetto può essere completato.</p> </td> 
  </tr> 
  <tr> 
   <td>Bloccato (stato richiesto)</td> 
   <td> <p>Puoi contrassegnare manualmente un problema come Bloccato, per indicare che si è verificato un ritardo nel completamento del problema. </p> </td> 
   <td> <p>Se il problema si trova in un progetto con stato Current, il problema viene visualizzato nella scheda Working on degli utenti che sono stati assegnati al problema. </p> <p>Quando tutte le attività vengono completate su un progetto, ma il progetto è problematico per almeno un problema in blocco, il progetto non può essere completato. </p> </td> 
  </tr> 
  <tr> 
   <td>Riaperto (Equivale a in corso)</td> 
   <td> <p>È possibile inserire un problema in questo stato per indicare che il lavoro su quel problema non è stato completato quando il problema era stato precedentemente chiuso e che era necessario riaprirlo per completare il lavoro.</p> </td> 
   <td> <p>Se il problema si trova in un progetto con stato Corrente, il problema viene visualizzato nella scheda Richieste di lavoro degli utenti assegnati al problema. Gli utenti possono ora iniziare a lavorare sul problema.</p> <p>Questo stato è importante nei rapporti, per distinguere tra i problemi aperti per la prima volta (di solito nello stato Nuovo) e quelli aperti dopo la chiusura in precedenza (di solito nello stato Riaperto). </p> </td> 
  </tr> 
  <tr> 
   <td>In attesa di un feedback (Equates with On Hold)</td> 
   <td>È possibile inserire un problema in questo stato per indicare che si sta aspettando un feedback (tipicamente dal contatto principale) prima di continuare a lavorare sul problema. </td> 
   <td> <p>Se il problema si trova in un progetto con stato Current, il problema viene visualizzato nella scheda Working on degli utenti che sono stati assegnati al problema.</p> <p>Se un problema è In attesa di un feedback, non è possibile completare un progetto.</p> <p>Questo stato è importante nel reporting, per distinguere tra i problemi attualmente aperti ma su cui si sta lavorando (in genere nello stato In corso) e i problemi attualmente aperti ma sui quali non si sta lavorando, perché è necessario un maggiore feedback per completarli (in genere nello stato Feedback in attesa).</p> </td> 
  </tr> 
  <tr> 
   <td>Impossibile duplicare (equivale a chiuso)</td> 
   <td>È possibile inserire un problema in questo stato per indicare che si sta chiudendo il problema, ma non è stato possibile vedere il problema che ha attivato l'apertura del problema. Il problema potrebbe ancora esistere, ma non può essere replicato in un dato momento. </td> 
   <td> <p>Questo stato è importante nel reporting, per distinguere tra i problemi completati e i cui problemi sono stati risolti (in genere nello stato Chiuso) e i problemi il cui problema non è visibile in un dato momento (in genere nello stato Non duplicare).</p> <p>Quando un problema è contrassegnato come Non duplicare, il problema viene rimosso dall'elenco Lavorare con dell'assegnatario. In questo caso, il problema mostra un valore per la Data completamento effettiva.</p> <p>Se tutte le attività di un progetto sono completate e lo stato di alcuni problemi è Impossibile duplicare, il progetto può essere completato.</p> </td> 
  </tr> 
  <tr> 
   <td>Risolto (Equazioni con chiuse)</td> 
   <td>Puoi inserire un problema in questo stato per indicare che stai chiudendo il problema e che il problema che lo ha creato è stato risolto.</td> 
   <td> <p>Questo stato è importante nel reporting, per distinguere tra i problemi chiusi con o senza una risoluzione (di solito nello stato Chiuso) e i problemi chiusi con una risoluzione effettiva (di solito nello stato Risolto).</p> <p>Quando un problema viene contrassegnato come Risolto, viene rimosso dall'elenco Lavorare con l'assegnatario. In questo caso, il problema mostra un valore per la Data di completamento effettiva.</p> <p>Se tutte le attività di un progetto sono completate e almeno un problema è in stato Risolto, il progetto può essere completato. </p> </td> 
  </tr> 
  <tr> 
   <td>Verificato completo (Equazioni con chiuse)</td> 
   <td>Puoi inserire un problema in questo stato per indicare che stai chiudendo il problema e che hai verificato che il problema generato sia stato risolto.</td> 
   <td> <p>Quando un problema viene contrassegnato come Verified Complete, il problema viene rimosso dall'elenco Working On dell'assegnatario. In questo caso, il problema mostra un valore per la Data di completamento effettiva.</p> <p>Se tutte le attività di un progetto sono state completate e alcuni problemi si trovano in uno stato di completamento verificato, il progetto può essere completato.</p> </td> 
  </tr> 
  <tr> 
   <td>Non risolvere (Equazioni con chiuse)</td> 
   <td>Puoi inserire un problema in questo stato per indicare che stai chiudendo il problema, ma il problema che lo ha generato non può essere risolto.</td> 
   <td> <p>Questo stato è importante nel reporting, per distinguere tra i problemi chiusi con o senza una risoluzione (di solito nello stato Chiuso) e i problemi chiusi senza una risoluzione effettiva (di solito nello stato Non risolvere).</p> <p>Quando un problema è contrassegnato come Non risolvere, il problema viene rimosso dall'elenco di lavoro dell'assegnatario. In questo caso, il problema mostra un valore per la Data di completamento effettiva.</p> <p>Se tutte le attività di un progetto sono state completate e almeno un problema si trova nello stato Non risolvere , il progetto può essere completato.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzazione degli stati dei problemi

Un amministratore Workfront può aggiungere a Workfront gli stati dei problemi a livello di sistema e di gruppo e modificare l’ordine in cui gli utenti li visualizzano. Per ulteriori informazioni, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Un amministratore di gruppo può aggiungere uno stato personalizzato specifico per un gruppo. Per ulteriori informazioni, consulta [Creare o modificare uno stato di gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
