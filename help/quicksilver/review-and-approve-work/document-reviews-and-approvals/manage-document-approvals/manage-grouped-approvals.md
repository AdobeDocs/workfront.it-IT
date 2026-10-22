---
product-area: documents
navigation-topic: approvals
title: Gestire le approvazioni raggruppate
description: È possibile aggiungere o rimuovere partecipanti e documenti in un'approvazione raggruppata senza interrompere il flusso di lavoro per il resto del gruppo.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: e62ae215bcc7ea42701d6eb92cf43f531a6afc0d
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 5%
---

# Gestire le approvazioni raggruppate

Un’approvazione raggruppata raggruppa più documenti in un unico flusso di lavoro di approvazione, in modo che tutti i documenti passino attraverso le stesse fasi insieme invece di richiedere un’approvazione separata per documento. È possibile aggiungere o rimuovere partecipanti e documenti in un&#39;approvazione raggruppata attiva senza ricreare il flusso di lavoro.

Le approvazioni raggruppate supportano la modalità di base e avanzata, più fasi e percorsi paralleli allo stesso modo delle approvazioni con una singola risorsa. Per ulteriori informazioni, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>Se la tua organizzazione utilizza l’archiviazione cloud Adobe, quando accedi ai documenti in Workfront visualizzerai la nuova area Documenti. Le approvazioni raggruppate sono disponibili solo nella nuova area Documenti. Per ulteriori informazioni sull&#39;archiviazione cloud Adobe, consulta [Panoramica sull&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Pacchetto Adobe Workfront</td>
   <td> <p>Qualsiasi pacchetto di flusso di lavoro per gestire le approvazioni tramite l’archiviazione cloud Adobe</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Licenza di Adobe Workfront</td>
   <td>
   <p>Collaboratore o successiva</p>
   <p>Revisione o successiva</p>
   <p>Se utilizzi l’integrazione Frame.io, devi disporre di una licenza Standard per creare flussi di lavoro di approvazione.</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Configurazioni del livello di accesso</td>
   <td> <p>Accesso di visualizzazione o superiore a progetti, attività, problemi, modelli, portafogli, programmi, report, dashboard, calendari e documenti</p></td>
  </tr>
  <tr>
   <td role="rowheader">Autorizzazioni sugli oggetti</td>
   <td> <p>Gestire l’accesso all’oggetto associato alla richiesta o all’approvazione</p></td>
  </tr>
 </tbody>
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungere partecipanti a un&#39;approvazione raggruppata attiva

È possibile aggiungere approvatori o revisori a un&#39;approvazione raggruppata mentre una fase è attiva, senza interrompere le approvazioni già in corso.

Per aggiungere partecipanti a un&#39;approvazione raggruppata attiva:

1. Vai al progetto, all&#39;attività o al problema che contiene l&#39;approvazione raggruppata, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fai clic su qualsiasi documento del gruppo, quindi fai clic sull&#39;icona **Approvazioni** sul lato destro della pagina.

   ![Aggiungi approvatori nel riepilogo documenti](assets/approvals-icon-new.png)

1. Fare clic su **Modifica flusso di lavoro**.

1. Digita l&#39;utente, il team o l&#39;e-mail nel campo **Aggiungi nomi o e-mail** della fase attiva.

1. Per ogni persona aggiunta, scegliere se si tratta di un approvatore o revisore.

1. Fai clic su **Salva**.

   I nuovi partecipanti vedono ogni approvazione aperta nel gruppo nella loro coda. Non vedono le decisioni prese prima di essere aggiunte, quindi devono ancora completare da soli tutte le approvazioni attualmente aperte.

## Rimuovere i partecipanti da un&#39;approvazione raggruppata attiva

È possibile rimuovere approvatori o revisori da un&#39;approvazione raggruppata mentre una fase è attiva. I partecipanti rimossi smettono immediatamente di vedere le approvazioni del gruppo nella loro coda, ma le decisioni già prese vengono mantenute e non vengono reimpostate.

Per rimuovere partecipanti da un&#39;approvazione raggruppata attiva:

1. Vai al progetto, all&#39;attività o al problema che contiene l&#39;approvazione raggruppata, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fai clic su qualsiasi documento del gruppo, quindi fai clic sull&#39;icona **Approvazioni** sul lato destro della pagina.

   ![Rimuovi approvatori nel riepilogo documenti](assets/approvals-icon-new.png)

1. Fare clic su **Modifica flusso di lavoro**.

1. Individua il partecipante che desideri rimuovere dalla fase attiva, quindi fai clic sull&#39;icona **Rimuovi** accanto al nome.

1. Fai clic su **Salva**.

## Aggiungere documenti a un’approvazione raggruppata

È possibile aggiungere documenti a un’approvazione raggruppata fino a quando la prima fase non viene bloccata. Una volta che la prima fase si blocca, non è più possibile aggiungere documenti.

Per aggiungere un documento a un’approvazione raggruppata:

1. Vai al progetto, all&#39;attività o al problema che contiene l&#39;approvazione raggruppata, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fai clic su qualsiasi documento del gruppo, quindi fai clic sull&#39;icona **Approvazioni** sul lato destro della pagina.

1. Fai clic su **Modifica flusso di lavoro**, quindi sulla scheda **Documenti**.

1. Selezionare il documento o i documenti da aggiungere al gruppo.

1. Fai clic su **Salva**.

   A tutti i partecipanti al gruppo viene notificato che è stato aggiunto un documento aggiuntivo da esaminare.

## Rimuovere documenti da un&#39;approvazione raggruppata

È possibile rimuovere un documento da un&#39;approvazione raggruppata in qualsiasi punto del flusso di lavoro. Il documento rimosso diventa una propria approvazione autonoma e mantiene tutte le decisioni, i commenti e la cronologia esistenti senza riavviare. Poiché il documento contiene già una decisione di approvazione, non è possibile aggiungerlo nuovamente a un’approvazione raggruppata in seguito.

Per rimuovere un documento da un&#39;approvazione raggruppata:

1. Vai al progetto, all&#39;attività o al problema che contiene l&#39;approvazione raggruppata, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fai clic sul documento che desideri rimuovere, quindi fai clic sull&#39;icona **Approvazioni** sul lato destro della pagina.

1. Fai clic su **Modifica flusso di lavoro**, quindi sulla scheda **Documenti**. Il documento selezionato è bloccato in alto nell&#39;elenco ed è già selezionato.

1. Cancellare la selezione del documento che si desidera rimuovere dal gruppo.

1. Fai clic su **Salva**.

   >[!NOTE]
   >
   >Lo stato di approvazione del documento rimane visibile e invariato dal momento in cui è stato rimosso. La vista approvazione raggruppata si aggiorna per riflettere i documenti rimanenti nel gruppo.


## Risolvere una decisione di &quot;lavoro necessario&quot; su un singolo documento in un&#39;approvazione raggruppata in più fasi

In un’approvazione raggruppata in più fasi, tutti i documenti di una fase devono pervenire a una decisione prima che il gruppo possa passare alla fase successiva. Se un documento è contrassegnato come **Richiede lavoro**, non può essere spostato in avanti con il resto del gruppo, pertanto deve essere rimosso manualmente dal gruppo per consentire l&#39;avanzamento della fase.

Quando rimuovi il documento dal gruppo, questo diventa la propria approvazione autonoma e mantiene tutte le decisioni, i commenti e la cronologia esistenti senza riavviarlo. È possibile aggiungere il documento revisionato come nuova versione all&#39;approvazione autonoma o crearne una nuova approvazione raggruppata.

Per risolvere una decisione di tipo &quot;Necessità di lavoro&quot;:

1. Rimuovi dal gruppo il documento contrassegnato come **Da lavorare**. Per ulteriori informazioni, vedere [Rimuovere documenti da un&#39;approvazione raggruppata](#remove-documents-from-a-grouped-approval). Il documento rimosso diventa una propria approvazione autonoma e mantiene le decisioni, i commenti e la cronologia esistenti.

1. Dopo aver aggiornato il documento, caricalo come nuova versione e richiedi nuovamente l’approvazione oppure aggiungilo come parte di un nuovo gruppo.

   Per ulteriori informazioni, consulta

   * [Caricare una nuova versione del documento e richiedere un’approvazione](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md)
   * [Creare un flusso di lavoro di approvazione documento](create-a-document-approval.md)
   * [Creare un’approvazione raggruppata](create-a-grouped-approval.md)


## Limitazioni note

Si è verificato un problema temporaneo di sincronizzazione con Frame.io quando si aggiungono o si rimuovono documenti in un&#39;approvazione raggruppata. Le modifiche verranno applicate a Frame.io solo alla successiva sincronizzazione del documento.