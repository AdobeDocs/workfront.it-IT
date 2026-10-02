---
product-area: documents
navigation-topic: approvals
title: Gestire le approvazioni raggruppate
description: Puoi aggiungere o rimuovere partecipanti e risorse in un’approvazione raggruppata senza interrompere il flusso di lavoro per il resto del gruppo.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 8250a95bec88df91e3422c8da7c05ac802b3cb22
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 4%
---

# Gestire le approvazioni raggruppate

{{highlighted-preview-article-level}}

Un’approvazione raggruppata raggruppa più risorse in un unico flusso di lavoro di approvazione, in modo che tutte le risorse passino attraverso le stesse fasi insieme invece di richiedere un’approvazione separata per ogni risorsa. Puoi aggiungere o rimuovere partecipanti e risorse in un’approvazione raggruppata attiva senza ricreare il flusso di lavoro.

Le approvazioni raggruppate supportano la modalità di base e avanzata, più fasi e percorsi paralleli allo stesso modo delle approvazioni con una singola risorsa. Per ulteriori informazioni, vedere [Creare un flusso di lavoro di approvazione documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>Il contenuto di questo articolo fa riferimento alla funzionalità di approvazione dei documenti aggiornata, disponibile solo per account specifici. Per informazioni sui processi di approvazione standard, vedere gli articoli elencati in [Approvazioni di lavoro](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

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

1. Fare clic su **Modifica flusso di lavoro**.

1. Individua il partecipante che desideri rimuovere dalla fase attiva, quindi fai clic sull&#39;icona **Rimuovi** accanto al nome.

1. Fai clic su **Salva**.

   Lo stato di approvazione degli altri partecipanti viene rivalutato per tenere conto della modifica.

## Aggiungere risorse a un’approvazione raggruppata

Puoi aggiungere risorse a un’approvazione raggruppata fino a quando la prima fase non viene bloccata. Una volta che la prima fase si blocca, non è più possibile aggiungere risorse, perché i partecipanti a quella fase non avrebbero avuto la possibilità di rivederle.

Per aggiungere una risorsa a un’approvazione raggruppata:

1. Vai al progetto, all&#39;attività o al problema che contiene l&#39;approvazione raggruppata, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fai clic su qualsiasi documento del gruppo, quindi fai clic sull&#39;icona **Approvazioni** sul lato destro della pagina.

1. Fai clic su **Modifica flusso di lavoro**, quindi sulla scheda **Documenti**.

1. Seleziona la risorsa o le risorse da aggiungere al gruppo.

1. Fai clic su **Salva**.

   A tutti i partecipanti al gruppo viene notificata l’aggiunta di una risorsa aggiuntiva da esaminare.

## Rimuovere risorse da un’approvazione raggruppata

È possibile rimuovere una risorsa da un’approvazione raggruppata in qualsiasi punto del flusso di lavoro. La risorsa rimossa diventa una propria approvazione indipendente e mantiene tutte le decisioni, i commenti e la cronologia esistenti senza riavviare. Poiché la risorsa contiene già una decisione di approvazione, non puoi aggiungerla nuovamente a un’approvazione raggruppata in seguito.

Per rimuovere una risorsa da un’approvazione raggruppata:

1. Vai al progetto, all&#39;attività o al problema che contiene l&#39;approvazione raggruppata, quindi seleziona **Documenti** nel pannello a sinistra.

1. Fai clic sul documento che desideri rimuovere, quindi fai clic sull&#39;icona **Approvazioni** sul lato destro della pagina.

1. Fai clic su **Modifica flusso di lavoro**, quindi sulla scheda **Documenti**. Il documento selezionato è bloccato in alto nell&#39;elenco ed è già selezionato.

1. Cancellare la selezione del documento che si desidera rimuovere dal gruppo.

1. Fai clic su **Salva**.

   Lo stato di approvazione della risorsa rimane visibile e invariato dal momento in cui è stata rimossa. La vista approvazione raggruppata si aggiorna per riflettere le risorse rimanenti nel gruppo.

## Risolvere una decisione di &quot;lavoro necessario&quot; in un&#39;approvazione raggruppata in più fasi

In un’approvazione raggruppata in più fasi, tutte le risorse di una fase devono pervenire a una decisione prima che il gruppo possa passare alla fase successiva. Se una risorsa è contrassegnata come **Da lavorare**, non può essere spostata in avanti con il resto del gruppo, pertanto deve essere rimossa dal gruppo per consentire l&#39;avanzamento della fase.

Per risolvere una decisione di tipo &quot;Necessità di lavoro&quot;:

1. Rimuovi dal gruppo la risorsa contrassegnata come **Da lavorare**. Per ulteriori informazioni, consulta [Rimuovere risorse da un&#39;approvazione raggruppata](#remove-assets-from-a-grouped-approval). La risorsa rimossa diventa la propria approvazione indipendente e mantiene le decisioni, i commenti e la cronologia esistenti.

1. Dopo l’aggiornamento della risorsa, richiedi di nuovo l’approvazione come singola risorsa o come parte di un nuovo gruppo. Poiché la risorsa contiene già una decisione di approvazione, non puoi aggiungerla nuovamente al gruppo originale.

   Per ulteriori informazioni, vedere [Creare un flusso di lavoro di approvazione documento](create-a-document-approval.md) e [Creare un&#39;approvazione raggruppata](create-a-grouped-approval.md).
