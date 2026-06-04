---
product-area: documents
navigation-topic: approvals
title: Autorizzazioni di oggetto e panoramica del livello di accesso per il modello di archiviazione cloud Adobe
description: Autorizzazioni di Adobe per l’archiviazione cloud e panoramica degli accessi
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 758d17e6-f31f-42b7-a9e6-6bd1821f5c15
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ckHEVC5iDp8A8xidvA16L0csKu0ey8LZHVlA2-QlCgQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 944
ht-degree: 1%

---

# Autorizzazioni di oggetto e panoramica del livello di accesso per il modello di archiviazione cloud Adobe

<!--linked in UI -->

Adobe Cloud Storage è una soluzione di archiviazione basata su cloud che funge da archivio di archiviazione centrale per le risorse tra i prodotti aziendali Adobe. Gli ambienti Workfront che utilizzano Adobe Cloud Storage hanno autorizzazioni degli oggetti e comportamenti del livello di accesso leggermente diversi rispetto a quelli che utilizzano lo storage dei documenti Workfront legacy.

## Livelli di accesso

I livelli di accesso a Workfront si applicano solo all&#39;interno di Workfront. Le restrizioni per progetti e documenti in Workfront non si applicano sempre ad altre applicazioni Adobe.

### Ambienti che utilizzano sia l’archiviazione cloud Adobe che l’archiviazione Workfront legacy

L’accesso ai documenti funziona in modo diverso a seconda che il progetto si trovi nell’archiviazione cloud Adobe o nell’archiviazione Workfront legacy:

* **Archiviazione Workfront legacy**: i progetti, i programmi, i portfolio e i modelli che utilizzano l&#39;archiviazione Workfront legacy seguono la logica standard del livello di accesso Workfront per l&#39;accesso ai documenti. Quando un livello di accesso ha **Nessun accesso** selezionato per i documenti, non è possibile visualizzare i documenti in Workfront o in altri prodotti Adobe come Frame.io o Creative Cloud.
* **Archiviazione cloud Adobe**: i progetti, i programmi, i portfolio e i modelli che utilizzano l&#39;archiviazione cloud Adobe seguono la logica del livello di accesso all&#39;archiviazione cloud Adobe per altri prodotti Adobe.


   * **Autorizzazioni per oggetti Progetti, programmi, portfolio e modelli**: se per progetti, programmi, portfolio e modelli è selezionato **Nessun accesso** a un livello di accesso, ma l&#39;oggetto è condiviso con gli utenti, questi non possono visualizzare l&#39;oggetto in Workfront, ma possono comunque visualizzare il nome dell&#39;oggetto e qualsiasi documento associato in altri strumenti di Adobe, come Frame.io e Adobe Creative Cloud.
   * **Autorizzazioni documenti**: quando per un livello di accesso è selezionato **Nessun accesso** per i documenti, gli utenti non sono in grado di visualizzare i documenti nei progetti in Workfront, ma possono comunque visualizzare e gestire i documenti per i progetti condivisi con loro in altri strumenti di Adobe, come Frame.io e Adobe Creative Cloud. Questo perché l’accesso ai documenti è determinato dalle autorizzazioni a livello di progetto nell’archiviazione cloud di Adobe, anziché dai soli livelli di accesso di Workfront.

Se nel tuo ambiente Workfront è abilitata l’archiviazione cloud Adobe, puoi creare sia progetti di archiviazione cloud Adobe che progetti di archiviazione Workfront legacy. I progetti di storage Workfront precedenti presentano un&#39;icona accanto al nome del progetto in qualsiasi punto di Workfront. I progetti Adobe cloud storage non mostrano un’icona.

![icona legacy workfront storage accanto al nome del progetto](assets/legacy-project-icon.png)


### Ambienti che utilizzano solo l’archiviazione cloud Adobe

Non è possibile modificare le autorizzazioni dei documenti a livello di accesso per progetti, programmi e portfolio che utilizzano l’archiviazione cloud di Adobe.

Tutti i livelli di accesso dispongono dell&#39;accesso in modifica ai documenti. Le autorizzazioni a livello di progetto determinano l’accesso ai documenti in altri strumenti di Adobe.

Non è possibile limitare l&#39;accesso all&#39;ereditarietà dei documenti.


### Ambienti che utilizzano solo storage Workfront legacy

Nessuna modifica ai livelli o al comportamento di accesso ai documenti.

## Autorizzazioni sugli oggetti

Le autorizzazioni per gli oggetti determinano ciò che è possibile visualizzare e fare con progetti, attività, problemi e documenti in Workfront. Le autorizzazioni vengono assegnate quando qualcuno condivide un oggetto con te.

>[!IMPORTANT]
>
>Nell’archiviazione cloud Adobe, le autorizzazioni per i documenti funzionano in modo diverso rispetto all’archiviazione Workfront legacy. I documenti ereditano le autorizzazioni dal progetto, dall’attività o dal problema a cui sono collegati.


### Funzionamento delle autorizzazioni per i documenti

Le autorizzazioni del documento dipendono dall&#39;oggetto a cui è collegato il documento. Non è possibile impostare autorizzazioni per singoli documenti.

Quando carichi un documento in un’attività o in un problema, viene creata una cartella generata dal sistema utilizzando il nome dell’attività o del problema. Questa cartella è collegata all’attività o al problema ed eredita le relative autorizzazioni.

È possibile creare sottocartelle nella cartella generata dal sistema per organizzare ulteriormente i documenti. Tutte le sottocartelle ereditano le autorizzazioni dalla cartella principale. A livello di progetto, è possibile caricare documenti all’esterno di una cartella, ma solo gli utenti con accesso a livello di progetto possono visualizzarli.

A livello di progetto, le cartelle generate dal sistema visualizzano un oggetto collegato. In genere si tratta del nome dell’attività o del problema ed è così che il sistema sa su quale attività o problema visualizzare la cartella.

### Autorizzazioni progetto

Se disponi di autorizzazioni a livello di progetto, puoi visualizzare e gestire i documenti per quel progetto in Workfront e altri prodotti Adobe come Frame.io e Adobe Creative Cloud. In questi strumenti è visibile anche il nome del progetto. Gli altri dati del progetto non sono visibili all’esterno di Workfront.

### Autorizzazioni per attività e problemi

Attività e problemi ereditano le autorizzazioni dal progetto. Se disponi di autorizzazioni a livello di attività o problema, puoi visualizzare e gestire i documenti collegati a tale attività o problema in Workfront e altri prodotti Adobe come Frame.io e Adobe Creative Cloud.

**Cartelle generate dal sistema**

* La rimozione degli utenti da un’attività o da un problema non rimuove automaticamente l’accesso alle cartelle. Possono ancora avere accesso tramite autorizzazioni a livello di progetto.
* Le sottoattività non ereditano le autorizzazioni della cartella generata dal sistema dalle attività padre. Per accedere alla cartella generata dal sistema, è necessario essere aggiunti direttamente a una sottoattività.
* L’aggiunta di utenti a un’attività o a un problema condivide con loro la cartella generata dal sistema dell’oggetto.

**Spostamento e ridenominazione delle cartelle generate dal sistema:**

* Le cartelle generate dal sistema possono essere rinominate e spostate.
* Se una cartella generata dal sistema viene spostata in un&#39;altra posizione, l&#39;oggetto collegato viene aggiornato al nuovo oggetto. Le autorizzazioni vengono quindi ereditate dal nuovo oggetto padre.

Le richieste seguono lo stesso comportamento delle attività e dei problemi.

### Approvazioni

Quando si viene aggiunti a un flusso di lavoro di approvazione di un documento, è possibile visualizzare quanto segue indipendentemente dalle autorizzazioni del progetto:

* Nome progetto
* Nome documento
* Miniatura documento


## Mappatura delle autorizzazioni su Frame.io

Come parte dell&#39;integrazione, le autorizzazioni utente sono controllate in Workfront e si estendono fino a Frame.io. Ciò significa che non è possibile invitare un utente a un progetto in Frame.io o modificare le autorizzazioni utente in Frame.io. Queste azioni devono essere eseguite tramite la finestra modale Condivisione progetto in Workfront.

Nella tabella seguente viene illustrato il mapping delle autorizzazioni di Workfront alle autorizzazioni Frame.io:

<table>
<tr>
<th>Autorizzazione utente di Workfront</th>
<th>Autorizzazione utente Frame.io</th>
</tr>
<tr>
<td>Gestione</td>
<td>Modifica e condividi</td>
</tr>
<tr>
<td>Contribuisci</td>
<td>Modifica e condividi</td>
</tr>
<tr>
<td>Visualizzazione</td>
<td>Solo commento</td>
</tr>
</table>






