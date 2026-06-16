---
product-area: projects
navigation-topic: manage-projects
title: Panoramica di Document Management per progetti e oggetti correlati
description: A seconda che l’amministratore di Workfront scelga per impostazione predefinita la preferenza di archiviazione, puoi archiviare i documenti sullo storage Workfront legacy o su quello cloud Adobe. Questo articolo descrive come gestire i documenti per progetti, portfolio, programmi, modelli, attività e problemi.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 397e5e36632872bb7be3f4e219b36e33b44136e9
workflow-type: tm+mt
source-wordcount: '2037'
ht-degree: 0%

---

# Panoramica sulla gestione dei documenti per progetti e oggetti correlati

L’amministratore di Adobe Workfront può definire l’impostazione predefinita per la preferenza di archiviazione della tua organizzazione in modo da indicare dove i documenti devono essere archiviati in Workfront.

L’amministratore di Workfront può scegliere una delle seguenti opzioni:

* Archiviazione Workfront
* Archiviazione cloud Adobe

Questa preferenza consente di memorizzare automaticamente i documenti allegati agli oggetti Workfront in una delle posizioni di archiviazione disponibili.

>[!IMPORTANT]
>
>La tua istanza di Workfront potrebbe non avere accesso allo storage Workfront e Adobe. Alcune istanze di Workfront hanno accesso solo a Workfront, mentre altre hanno accesso solo all’archiviazione cloud di Adobe per impostazione predefinita. Non è necessaria alcuna configurazione per i clienti con accesso a un solo tipo di storage.

L&#39;amministratore di Workfront può effettuare una delle seguenti operazioni:

* Scegliere una delle due opzioni di storage predefinite per l&#39;organizzazione
* Consente di scegliere il tipo di archiviazione da utilizzare quando si crea uno dei seguenti oggetti:

   * Progetti
   * Portfolio
   * Modelli

Per informazioni sull&#39;impostazione delle preferenze di archiviazione per Workfront, consulta [Abilitare l&#39;archiviazione cloud Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

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
* Solo archiviazione cloud Adobe. L&#39;area Preferenze di archiviazione in Preferenze di sistema non esiste.
* Archiviazione Workfront e archiviazione cloud Adobe. L’amministratore di Workfront può scegliere tra le seguenti opzioni:

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


I documenti memorizzati sugli oggetti nell’archiviazione Workfront vengono gestiti in modo diverso rispetto a quelli memorizzati nell’archiviazione cloud Adobe.

Per ulteriori informazioni, consulta [Panoramica sull&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Nelle sezioni seguenti viene illustrato il funzionamento dell’archiviazione dei documenti per gli oggetti Workfront quando nello stesso ambiente esistono opzioni di archiviazione cloud Workfront e Adobe.

### Gestione documenti per progetti

Quando si lavora con i progetti, considera quanto segue:

* Quando crei un progetto di archiviazione cloud Adobe, Workfront crea una cartella nella sezione Documenti del progetto in cui vengono salvati i documenti. Il nome della cartella corrisponde al nome del progetto. Impossibile eliminare o rinominare manualmente la cartella. La cartella viene rinominata se modificate il nome del progetto in modo che corrisponda al nuovo nome del progetto.
* Quando si crea o si sposta un progetto di archiviazione cloud Adobe in un portfolio o programma di archiviazione Workfront legacy, il portfolio o il programma viene automaticamente convertito in un oggetto di archiviazione cloud Adobe, se a tale portfolio o programma non sono allegati documenti prima che il progetto venga aggiunto.
* Non puoi creare un progetto di archiviazione Workfront legacy per un portfolio o programma di archiviazione cloud Adobe.
* Quando importi un progetto da MS Project, Workfront crea un progetto di archiviazione Workfront legacy, anche quando l’amministratore di Workfront ha impostato l’archiviazione cloud Adobe come predefinita per il sistema.
* Quando si creano progetti utilizzando un&#39;automazione di Workfront Planning, Workfront utilizza la preferenza di archiviazione predefinita del sistema per il progetto. È necessario acquistare il pacchetto Planning per accedere a Workfront Planning.

Per ulteriori informazioni, vedere anche la sezione [Gestione dei documenti per i modelli di progetto](#document-management-for-project-templates) in questo articolo.

### Gestione dei documenti per portfolio

Quando si lavora con i portfolio, considera quanto segue:

* Quando crei un portfolio di archiviazione cloud Adobe, Workfront crea una cartella nella sezione Documenti del portfolio in cui vengono salvati i documenti. Il nome della cartella corrisponde al nome del portfolio. Impossibile eliminare o rinominare manualmente la cartella. La cartella viene rinominata se modifichi il nome del portfolio in modo che corrisponda al nuovo nome del portfolio.

* Quando aggiungi un progetto di archiviazione cloud Adobe a un portfolio di archiviazione Workfront legacy e al portfolio non è allegato alcun documento, il portfolio viene convertito in un portfolio di archiviazione cloud Adobe.
* Quando aggiungi un progetto di archiviazione cloud Adobe a un portfolio di archiviazione Workfront legacy a cui sono allegati dei documenti, il portfolio di archiviazione dei documenti rimane nello storage Workfront. Tuttavia, l&#39;icona di archiviazione legacy di Workfront per il portfolio ![Icona di archiviazione legacy](assets/legacy-storage-project-icon.png) è stata rimossa dal portfolio.
* Non puoi aggiungere un progetto di archiviazione cloud Adobe a un portfolio di archiviazione legacy o un progetto di archiviazione legacy a un portfolio di archiviazione Adobe.
* L’amministratore può convertire un portfolio di archiviazione legacy in archiviazione cloud Adobe nell’area Preferenze di sistema di Configura. Tutti gli oggetti figlio (programmi, progetti e documenti) rimangono nell&#39;archiviazione legacy. I nuovi progetti utilizzeranno l’archiviazione cloud di Adobe. I nuovi documenti aggiunti al portfolio continueranno a essere memorizzati nello storage legacy.
Per informazioni, vedere [Configurare le preferenze di sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* Quando si creano i portfolio utilizzando un&#39;automazione di Workfront Planning, Workfront utilizza la preferenza di archiviazione predefinita del sistema per il portfolio. È necessario acquistare il pacchetto Planning per accedere a Workfront Planning.


### Gestione documenti per programmi

Quando si lavora con i programmi, considera quanto segue:

* Quando si crea un programma di archiviazione cloud Adobe, Workfront crea una cartella nella sezione Documenti del programma in cui vengono salvati i documenti. Il nome della cartella corrisponde al nome del programma. Impossibile eliminare o rinominare manualmente la cartella. Se si modifica il nome del programma, la cartella viene rinominata in base al nuovo nome del programma.

* Non puoi aggiungere un progetto di archiviazione Workfront legacy a un programma di archiviazione cloud Adobe.

* Non puoi aggiungere un programma di archiviazione cloud Adobe a un portfolio di archiviazione cloud legacy o un programma legacy a un portfolio di archiviazione cloud Adobe.
* Non puoi creare un progetto da un modello di archiviazione cloud Adobe in un programma di archiviazione legacy.
* Puoi creare un progetto da un modello di archiviazione legacy in un programma di archiviazione cloud Adobe, ma i documenti e le cartelle presenti nel modello non vengono aggiunti al nuovo progetto. Il progetto riceve l’archiviazione cloud di Adobe.
* Quando si creano programmi utilizzando un&#39;automazione di Workfront Planning, Workfront utilizza la preferenza di archiviazione predefinita del sistema per il programma. È necessario acquistare il pacchetto Planning per accedere a Workfront Planning.

### Gestione dei documenti per le attività

Quando si lavora con le attività, tenere presente quanto segue:

* Le attività ereditano il tipo di archiviazione dai progetti.
* Quando carichi un documento in un’attività su un progetto di archiviazione cloud Adobe, Workfront crea automaticamente una cartella nella sezione Documenti dell’attività. Il nome della cartella corrisponde a quello dell&#39;attività.
* È possibile rinominare ed eliminare la cartella documenti dall’attività di archiviazione cloud di Adobe, che elimina anche i documenti presenti nella cartella. Dopo aver aggiunto nuovi documenti all&#39;attività, la cartella viene ricreata automaticamente. I documenti eliminati non vengono inseriti nuovamente nella cartella.
* Per i progetti Adobe Cloud Storage, la cartella documenti di un’attività viene visualizzata come sottocartella nella cartella documenti creata automaticamente per il progetto.
* Non puoi copiare o spostare un’attività da un progetto di archiviazione Workfront legacy a un progetto di archiviazione cloud Adobe. Non è inoltre possibile fare l&#39;inverso.
* Durante la conversione di un&#39;attività in un progetto sono presenti i seguenti scenari: <!--this info also duplicated in Convert tasks to projects-->
   * Un&#39;attività di storage Workfront legacy crea un progetto di storage Workfront legacy.
   * Un’attività di archiviazione cloud Adobe crea un progetto di archiviazione cloud Adobe.
   * Quando si utilizza un modello di archiviazione Workfront legacy per convertire un’attività di archiviazione cloud di Adobe, viene creato un progetto di archiviazione cloud di Adobe.
   * L’utilizzo di un modello di archiviazione cloud Adobe per convertire un’attività di archiviazione Workfront legacy crea un progetto di archiviazione Workfront legacy.
* Non è possibile aggiungere documenti alle attività di archiviazione cloud di Adobe nel pannello Riepilogo.

### Gestione dei documenti per problemi

Quando si lavora con i problemi, tieni presente quanto segue:

* I problemi ereditano il tipo di archiviazione dai progetti.
* Quando carichi un documento su un problema relativo a un progetto di archiviazione cloud Adobe, Workfront crea automaticamente una cartella nella sezione Documenti del problema. Il nome della cartella corrisponde al problema.
* Puoi rinominare ed eliminare la cartella dei documenti dal problema di archiviazione cloud di Adobe, che comporta anche l’eliminazione dei documenti nella cartella. Dopo aver aggiunto nuovi documenti al problema, la cartella viene ricreata automaticamente. I documenti eliminati non vengono inseriti nuovamente nella cartella.
* Per i progetti Adobe Cloud Storage, la cartella dei documenti relativa a un problema viene visualizzata come sottocartella nella cartella dei documenti creata automaticamente per il progetto.
* Non puoi copiare o spostare un problema da un progetto di archiviazione legacy di Workfront a uno di archiviazione cloud Adobe. Non è inoltre possibile fare l&#39;inverso.
* Durante la conversione di un problema in un progetto sono presenti i seguenti scenari: <!--this info also duplicated in Convert an issue to a project-->
   * Un problema di storage Workfront legacy crea un progetto di storage Workfront legacy.
   * Un problema di archiviazione cloud Adobe crea un progetto di archiviazione cloud Adobe.
   * L’utilizzo di un modello di archiviazione Workfront legacy per convertire un problema di archiviazione cloud Adobe crea un progetto di archiviazione cloud Adobe.
   * L’utilizzo di un modello di archiviazione cloud Adobe per convertire un problema di archiviazione Workfront legacy crea un progetto di archiviazione Workfront legacy.
* Non è possibile aggiungere documenti a problemi di archiviazione cloud Adobe nel pannello Riepilogo.

### Gestione documenti per richieste

* Quando invii una richiesta Workfront con un documento allegato a un progetto di archiviazione Workfront legacy che funge da coda di richieste, l’area Documenti della richiesta visualizza il documento utilizzando il tipo di archiviazione del progetto, anche quando la preferenza predefinita per l’archiviazione del sistema è archiviazione cloud Adobe.
* Quando alleghi un documento a un problema inviato a una coda di richieste associata all’archiviazione di Adobe, viene creata una cartella per ogni problema inviato in cui sono memorizzati i documenti. La cartella viene aggiunta anche come sottocartella alla cartella di progetto creata automaticamente sul progetto della coda richieste.

### Gestione dei documenti per i modelli di progetto

Quando si lavora con i modelli, considera quanto segue:

* Quando si crea un modello di Adobe Cloud Storage, Workfront crea una cartella nella sezione Documenti del modello in cui vengono salvati i documenti. Il nome della cartella corrisponde al nome del programma. Impossibile eliminare o rinominare manualmente la cartella. Se si modifica il nome del modello, la cartella viene rinominata in base al nuovo nome del modello.
* Puoi utilizzare un modello di archiviazione Workfront legacy per creare progetti di archiviazione Workfront legacy; puoi utilizzare un modello di archiviazione cloud Adobe per creare un progetto di archiviazione cloud Adobe.

* Quando si creano progetti utilizzando modelli di un portfolio o di un programma, si verificano i seguenti scenari:
   * Non puoi utilizzare un modello di archiviazione cloud Adobe da un portfolio o programma di archiviazione Workfront legacy per creare un progetto.
   * Puoi creare un progetto di archiviazione cloud Adobe per un portfolio o un programma di archiviazione Adobe utilizzando un modello di archiviazione legacy. Tutti i documenti modello e le cartelle non sono allegati al nuovo progetto.

* È possibile allegare un modello di archiviazione Workfront legacy a un progetto di archiviazione cloud Adobe e questo non modifica il percorso di archiviazione dei documenti sul progetto.
* È possibile allegare un modello di archiviazione cloud Adobe a un progetto di archiviazione Workfront legacy senza modificare il percorso di archiviazione dei documenti nel progetto. I documenti contenuti nella cartella di archiviazione cloud di Adobe per il modello vengono aggiunti direttamente al progetto, senza la cartella, mentre i documenti contenuti nelle cartelle delle attività del modello vengono aggiunti alle cartelle associate alle attività del progetto nella sezione Documenti delle attività.
* Quando si salva un progetto come modello, il tipo di archiviazione del progetto viene trasferito al modello, indipendentemente da ciò che l&#39;amministratore di Workfront ha impostato per la preferenza di archiviazione del sistema.


### Gestione dei documenti per le attività modello

Quando si lavora con le attività modello, considera quanto segue:

* Le attività modello ereditano il tipo di archiviazione dai modelli.
* Quando carichi un documento in un’attività modello su un modello di Adobe Cloud Storage, Workfront crea automaticamente una cartella nella sezione Documenti dell’attività modello. Il nome della cartella corrisponde all&#39;attività modello.
* È possibile rinominare ed eliminare la cartella documenti dall’attività del modello di archiviazione cloud di Adobe, che elimina anche i documenti presenti nella cartella. Dopo aver aggiunto nuovi documenti all&#39;attività modello, la cartella viene ricreata automaticamente. I documenti eliminati non vengono inseriti nuovamente nella cartella.
* Per i modelli di archiviazione cloud Adobe, la cartella documenti di un’attività modello viene visualizzata come sottocartella nella cartella documenti creata automaticamente per il modello.
* Non puoi copiare o spostare un’attività modello da un modello di archiviazione Workfront legacy a un modello di archiviazione cloud Adobe. Non è inoltre possibile fare l&#39;inverso.

