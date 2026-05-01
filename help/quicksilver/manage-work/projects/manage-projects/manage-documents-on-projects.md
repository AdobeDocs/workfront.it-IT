---
product-area: projects
navigation-topic: manage-projects
title: Panoramica di Document Management per progetti e oggetti correlati
description: A seconda che l'amministratore di Workfront scelga per impostazione predefinita la preferenza di archiviazione, è possibile archiviare i documenti sullo storage Workfront legacy o su quello aziendale Adobe. Questo articolo descrive come gestire i documenti per progetti, portfolio, programmi, modelli, attività e problemi.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 5c4ffeabf710374b14a2335b47342be4c393a7c8
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---

# Panoramica sulla gestione dei documenti per progetti e oggetti correlati

L’amministratore di Adobe Workfront può definire l’impostazione predefinita per la preferenza di archiviazione della tua organizzazione in modo da indicare dove i documenti devono essere archiviati in Workfront.

L’amministratore di Workfront può scegliere una delle seguenti opzioni:

* Archiviazione Workfront
* Storage aziendale Adobe

Questa preferenza consente di memorizzare automaticamente i documenti allegati agli oggetti Workfront in una delle posizioni di archiviazione disponibili.

>[!IMPORTANT]
>
>Non tutti i clienti hanno accesso sia allo storage Workfront che a quello Adobe. Alcuni clienti hanno accesso solo a Workfront, mentre altri hanno accesso solo allo storage Adobe Enterprise per impostazione predefinita. Per i clienti che non hanno accesso allo storage Workfront non è necessaria alcuna configurazione.

L&#39;amministratore di Workfront può effettuare una delle seguenti operazioni:

* Scegliere una delle due opzioni di storage predefinite per l&#39;organizzazione
* Consente di scegliere il tipo di archiviazione da utilizzare quando si crea uno dei seguenti oggetti:

   * Progetti
   * Portfolio
   * Modelli

Per informazioni sull&#39;impostazione delle preferenze di archiviazione per Workfront, consulta [Abilitare l&#39;archiviazione aziendale Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

Questo articolo descrive come gestire i documenti per progetti, portfolio, programmi, attività, problemi, modelli e attività modello.

<!--

Not sure we need these since this became an overview article: 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Light or higher</p>
   <p>Review or higher</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the objects you want to add documents to:</p>
   <ul><li>Projects</li>
   <li>Portfolios</li>
<li>Programs</li>
<li>Templates</li> 
<li>Tasks</li> 
<li>Issues</li> </ul>  
   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the objects you want to add documents to:</p>

<ul><li>A project</li>
   <li>A portfolio</li>
<li>A program</li>
<li>A template</li> 
<li>A task</li> 
<li>An issue</li> </ul>    
   
</td> 
  </tr> 
 </tbody> 
</table>

*For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

-->

## Panoramica sull’archiviazione dei documenti

I clienti possono avere accesso a una delle seguenti funzionalità di archiviazione dei documenti:

* Solo storage Workfront. L&#39;area Preferenze di archiviazione in Preferenze di sistema non esiste.
* Solo storage Adobe Enterprise. L&#39;area Preferenze di archiviazione in Preferenze di sistema non esiste.
* Storage Workfront e storage Adobe Enterprise. L’amministratore di Workfront può scegliere tra le seguenti opzioni:

   * Seleziona un ambiente di storage predefinito per la gestione dei documenti in futuro.
   * Consente agli utenti di scegliere la memoria di archiviazione da utilizzare per la creazione dei seguenti oggetti:

      * Progetti
      * Portfolio
      * Modelli

  >[!NOTE]
  >
  >* Le attività e i problemi ereditano il tipo di archiviazione dal progetto.
  >* Le attività modello ereditano il tipo di archiviazione dal modello
  >* I programmi ereditano il tipo di storage dal portfolio.


I documenti memorizzati sugli oggetti nell’archivio di Workfront vengono gestiti in modo diverso rispetto a quelli archiviati nell’archivio aziendale di Adobe.

Per ulteriori informazioni, consulta [Panoramica sull&#39;archiviazione aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Le sezioni seguenti documentano il funzionamento dell’archiviazione dei documenti per gli oggetti Workfront quando sono disponibili le opzioni di archiviazione aziendale Workfront e Adobe.

### Gestione documenti per progetti

Quando si lavora con i progetti, considera quanto segue:

* Quando si crea un progetto di archiviazione aziendale Adobe, Workfront crea una cartella nella sezione Documenti del progetto in cui vengono salvati i documenti. Il nome della cartella corrisponde al nome del progetto. Impossibile eliminare o rinominare manualmente la cartella. La cartella viene rinominata se modificate il nome del progetto in modo che corrisponda al nuovo nome del progetto.
* Quando si crea o si sposta un progetto di storage aziendale Adobe in un portfolio o programma di storage Workfront legacy, il portfolio o il programma viene automaticamente convertito in un oggetto di storage aziendale Adobe.
* Non è possibile creare un progetto di storage Workfront per un portfolio o un programma di storage aziendale Adobe.

### Gestione dei documenti per portfolio

Quando si lavora con i portfolio, considera quanto segue:

* Quando si crea un portfolio di storage aziendale Adobe, Workfront crea una cartella nella sezione Documenti del portfolio in cui vengono salvati i documenti. Il nome della cartella corrisponde al nome del portfolio. Impossibile eliminare o rinominare manualmente la cartella. La cartella viene rinominata se modifichi il nome del portfolio in modo che corrisponda al nuovo nome del portfolio.
* Quando si crea o si sposta un progetto di storage aziendale Adobe in un portfolio di storage Workfront legacy, il portfolio viene automaticamente convertito in un oggetto di storage aziendale Adobe.
* Se il portfolio convertito aveva già dei documenti allegati, questi rimangono memorizzati nello storage Workfront. I nuovi documenti vengono inoltre archiviati nell&#39;archivio Workfront.
* Se il portfolio convertito non aveva documenti allegati nello storage Workfront, i nuovi documenti vengono memorizzati nello storage aziendale Adobe.

### Gestione documenti per programmi

Quando si lavora con i programmi, considera quanto segue:

* Quando si crea un programma di archiviazione aziendale Adobe, Workfront crea una cartella nella sezione Documenti del programma in cui vengono salvati i documenti. Il nome della cartella corrisponde al nome del programma. Impossibile eliminare o rinominare manualmente la cartella. Se si modifica il nome del programma, la cartella viene rinominata in base al nuovo nome del programma.
* Quando si crea o si sposta un progetto di storage aziendale Adobe in un portfolio di storage Workfront legacy, il portfolio viene automaticamente convertito in un oggetto di storage aziendale Adobe.
* Se al programma convertito erano già allegati dei documenti, questi rimangono memorizzati nell&#39;archivio Workfront. I nuovi documenti vengono inoltre archiviati nell&#39;archivio Workfront.
* Se il programma convertito non aveva documenti allegati nello storage Workfront, i nuovi documenti vengono memorizzati nello storage aziendale Adobe.

### Gestione dei documenti per le attività

Quando si lavora con le attività, tenere presente quanto segue:

* Le attività ereditano il tipo di archiviazione dai progetti.
* Quando carichi un documento in un’attività su un progetto di archiviazione Adobe, Workfront crea automaticamente una cartella nella sezione Documenti dell’attività. Il nome della cartella corrisponde a quello dell&#39;attività.
* È possibile rinominare ed eliminare la cartella documenti dall&#39;attività di archiviazione aziendale di Adobe, che elimina anche i documenti contenuti nella cartella. Dopo aver aggiunto nuovi documenti all&#39;attività, la cartella viene ricreata automaticamente. I documenti eliminati non vengono inseriti nuovamente nella cartella.
* Per i progetti Adobe di archiviazione aziendale, la cartella documenti di un&#39;attività viene visualizzata come sottocartella nella cartella documenti creata automaticamente per il progetto.
* Non è possibile copiare o spostare un’attività da un progetto di archiviazione Workfront a uno di archiviazione Adobe. Non è inoltre possibile fare l&#39;inverso.

### Gestione dei documenti per problemi

Quando si lavora con i problemi, tieni presente quanto segue:

* I problemi ereditano il tipo di archiviazione dai progetti.
* Quando carichi un documento su un problema relativo a un progetto di archiviazione Adobe, Workfront crea automaticamente una cartella nella sezione Documenti del problema. Il nome della cartella corrisponde al problema.
* È possibile rinominare ed eliminare la cartella documenti dal problema di archiviazione aziendale di Adobe, che comporta anche l’eliminazione dei documenti nella cartella. Dopo aver aggiunto nuovi documenti al problema, la cartella viene ricreata automaticamente. I documenti eliminati non vengono inseriti nuovamente nella cartella.
* Per i progetti Adobe di archiviazione aziendale, la cartella documenti relativa a un problema viene visualizzata come sottocartella nella cartella documenti creata automaticamente per il progetto.
* Non è possibile copiare o spostare un problema da un progetto di archiviazione Workfront a uno di archiviazione Adobe. Non è inoltre possibile fare l&#39;inverso.

### Gestione dei documenti per i modelli di progetto

Quando si lavora con i modelli, considera quanto segue:

* Quando si crea un modello di archiviazione aziendale Adobe, Workfront crea una cartella nella sezione Documenti del modello in cui vengono salvati i documenti. Il nome della cartella corrisponde al nome del programma. Impossibile eliminare o rinominare manualmente la cartella. Se si modifica il nome del modello, la cartella viene rinominata in base al nuovo nome del modello.
* Puoi utilizzare un modello di archiviazione Workfront per creare progetti di archiviazione Workfront; puoi utilizzare un modello di archiviazione Adobe per creare un progetto di archiviazione Adobe.
* È possibile allegare un modello di archiviazione Workfront a un progetto di archiviazione Adobe senza che questo modifichi il percorso di archiviazione del progetto.
* È possibile allegare un modello di archiviazione Adobe a un progetto di archiviazione Workfront senza che questo modifichi il percorso di archiviazione del progetto.

### Gestione dei documenti per le attività modello

Quando si lavora con le attività modello, considera quanto segue:

* Le attività modello ereditano il tipo di archiviazione dai modelli.
* Quando carichi un documento in un&#39;attività modello su un modello di archiviazione Adobe, Workfront crea automaticamente una cartella nella sezione Documenti dell&#39;attività modello. Il nome della cartella corrisponde all&#39;attività modello.
* È possibile rinominare ed eliminare la cartella documenti dall&#39;attività Modello di archiviazione aziendale di Adobe, che elimina anche i documenti contenuti nella cartella. Dopo aver aggiunto nuovi documenti all&#39;attività modello, la cartella viene ricreata automaticamente. I documenti eliminati non vengono inseriti nuovamente nella cartella.
* Per i modelli di archiviazione aziendale Adobe, la cartella documenti di un&#39;attività modello viene visualizzata come sottocartella nella cartella documenti creata automaticamente per il modello.
* Non è possibile copiare o spostare un’attività modello da un modello di archiviazione Workfront a un modello di archiviazione Adobe. Non è inoltre possibile fare l&#39;inverso.
* Quando alleghi un documento a un problema inviato a una coda di richieste associata all’archiviazione di Adobe, viene creata una cartella per ogni problema inviato in cui sono memorizzati i documenti. La cartella viene aggiunta anche come sottocartella alla cartella di progetto creata automaticamente nella coda richieste.
