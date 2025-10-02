---
title: Creazione di oggetti Workfront da Workfront Planning durante la connessione ai record
description: È possibile creare tipi di oggetti di Workfront quando vengono collegati da altri record in Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 5b9b1f397c76afa2e2ae550e0ce62a6038b8bd86
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Creazione di oggetti Workfront da Workfront Planning durante la connessione ai record

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

È possibile creare oggetti Adobe Workfront da Workfront Planning nei modi seguenti:

* Quando si collegano oggetti Workfront da record di Planning

  In questo articolo viene descritto come creare oggetti Workfront da Workfront Planning quando vengono collegati da record di Planning.
* Quando si utilizzano le automazioni dalla pagina di un record.

  Per informazioni sulla creazione di oggetti Workfront tramite automazioni, vedere [Creare oggetti tramite automazioni record di Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

>[!IMPORTANT]
>
>È possibile creare i seguenti oggetti di Workfront da Workfront Planning quando vengono collegati ai record di Planning:
>
>* Progetti
>* Portfolio
>* Programmi
>
>È possibile connettere i seguenti oggetti Workfront con i record di Planning, ma non è possibile crearli nel processo di connessione:
>
>* Gruppi
>* Aziende
>

Durante la connessione e la creazione di oggetti Workfront ai record di Workfront Planning, tenere presente quanto segue:

* È possibile collegare progetti, portfolio, programmi, gruppi e società Workfront da un campo di connessione dalle seguenti aree di Workfront Planning:

   * Visualizzazione tabella di un tipo di record
   * Pagina Dettagli o casella di anteprima di un record
   * Scheda Connessioni di un record

* È possibile creare progetti dalle seguenti aree di Workfront Planning:

   * Visualizzazione tabella di un tipo di record
   * Area Dettagli di un record nel campo connessione
   * <span class="preview">Pagina Record connesso di un record nell&#39;area Dettagli</span>

* È possibile creare portfolio e programmi dalle seguenti aree di Workfront Planning:

   * Visualizzazione tabella di un tipo di record
   * Area Dettagli di un record nel campo connessione

Per informazioni sulla connessione dei record di Planning con gli oggetti di Workfront, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td> Standard
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p> 
   <p>Accesso di modifica con accesso a Crea oggetti in Workfront per i tipi di oggetto che si desidera creare (progetti, portfolio, programmi). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td> <p>Consente di gestire le autorizzazioni per l'area di lavoro e il tipo di record in cui si desidera aggiungere record. </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
   <p>Gestisci le autorizzazioni per gli oggetti Workfront (portfolio) per aggiungere oggetti figlio (progetti).</p>
   </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti per la creazione di oggetti Workfront quando vengono collegati ai record di Workfront Planning

Prima di poter aggiungere nuovi progetti o portfolio collegandoli da record esistenti, è necessario disporre dei seguenti elementi:

* Tipi di record connessi a progetti, portfolio o programmi Workfront. Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).
* Record per i tipi di record connessi a oggetti Workfront. Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
* L&#39;accesso e le autorizzazioni corretti in Workfront Planning e Workfront, come descritto nella sezione [Requisiti di accesso](#access-requirements) in questo articolo.

## Creazione di progetti durante la connessione con i record di Workfront Planning

È possibile creare progetti quando si collegano a record in Workfront Planning nelle seguenti aree di Workfront Planning:

* Visualizzazione tabella di un tipo di record o area Dettagli di un record nel campo connessione
* <span class="preview">Pagina Record connesso di un record nell&#39;area Dettagli di un record </span>

### Creare progetti dall&#39;area Dettagli di un record o dalla vista tabella di un tipo di record

Per creare progetti mentre li si connette da altri record:

1. Passare alla pagina dei dettagli di un record o alla tabella del tipo di record e iniziare a collegare i record di Workfront Planning ai progetti Workfront, come descritto nell&#39;articolo [Connetti record](/help/quicksilver/planning/records/connect-records.md).

1. (Condizionale) Fai clic su **Aggiungi progetto**
Oppure
Inizia a digitare il nome di un progetto, quindi fai clic su **Aggiungi progetto** se non riesci a trovarlo. Il pulsante Aggiungi è seguito dal nome del progetto digitato.

   ![Aggiungi progetto quando lo connetti da un campo di connessione](assets/add-project-when-connecting-it-from-connection-field.png)

   Viene visualizzata la casella **Crea progetto**.

1. (Facoltativo) Aggiorna il **nome progetto**. Per impostazione predefinita, il progetto prende il nome da quello che hai aggiunto come elemento di ricerca quando lo connetti dal record.
1. (Facoltativo) Seleziona un **modello di progetto**. Se non si seleziona un modello, Workfront crea un progetto vuoto, senza attività.
1. Fai clic su **Crea**.
1. (Condizionale) Se hai selezionato di creare un progetto da un modello, segui i passaggi descritti nell&#39;articolo [Creare un progetto utilizzando un modello](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) per completare l&#39;aggiunta del progetto.

   Il nuovo progetto viene creato e aggiunto al campo connesso del record selezionato.

1. (Facoltativo) Fare clic sul nome del nuovo progetto da Workfront Planning per aprire la pagina del progetto in Workfront e apportare ulteriori aggiornamenti al progetto.

<div class="preview">

### Creare progetti dalla pagina Record connessi di un record

1. Connettere il tipo di oggetto Project a un tipo di record di Workfront Planning nella vista tabella.

   Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Fare clic sul nome di un record in qualsiasi visualizzazione. Viene visualizzata la casella di anteprima Dettagli (Details).

1. Aggiungi **Pagina record connessi** per i progetti.

   Per informazioni, vedere la sezione &quot;Aggiungere una pagina di record connessi a un record&quot; nell&#39;articolo [Gestire il layout della pagina di record](/help/quicksilver/planning/records/manage-the-record-page.md).

   La pagina Record collegati viene visualizzata nella vista Tabella. I progetti connessi vengono visualizzati nella tabella.

   ![Visualizzazione tabella progetti nella pagina dei record connessi](assets/projects-connected-records-page-table.png)

1. Fare clic su **Nuova riga** nella tabella dei progetti per aggiungere un progetto.

   In quest’area è possibile aggiungere solo un progetto vuoto. Non è possibile aggiungere un progetto utilizzando un modello.
1. (Facoltativo) Fai clic sul nome del progetto nella vista a tabella per aprirlo in Workfront e aggiungere ulteriori informazioni.

</div>

## Creazione di portfolio durante la connessione con i record di Workfront Planning

È possibile creare i portfolio dalla vista tabella di un tipo di record o dalla pagina Dettagli di un record.

Per creare i portfolio durante la connessione dai record di Planning:

1. Andare alla pagina dei dettagli di un record o alla tabella del tipo di record e iniziare a collegare i record di Workfront Planning ai portfolio Workfront, come descritto nell&#39;articolo [Connetti record](/help/quicksilver/planning/records/connect-records.md).

1. (Condizionale) Fai clic su **Aggiungi portfolio**

   Oppure

   Inizia a digitare il nome di un portfolio, quindi fai clic su **Aggiungi portfolio** se non riesci a trovarlo. Il pulsante Aggiungi è seguito dal nome del portfolio digitato.

   ![Aggiungi portfolio quando lo connetti da un campo di connessione](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Il portfolio viene creato e aggiunto al campo di connessione del record selezionato.

1. (Facoltativo) Fare clic sul nome del nuovo portfolio da Workfront Planning per aprire la pagina del portfolio in Workfront e apportare ulteriori aggiornamenti al portfolio.

## Creazione di programmi durante la connessione con i record di Workfront Planning

È possibile creare programmi dalla vista tabella di un tipo di record o dalla pagina Dettagli di un record.

Per creare i programmi mentre li si connette dai record di Planning, procedere come segue.

1. Andare alla pagina dei dettagli di un record o alla tabella del tipo di record e iniziare a collegare i record di Workfront Planning ai portfolio Workfront, come descritto nell&#39;articolo [Connetti record](/help/quicksilver/planning/records/connect-records.md).

1. Fai clic su **Aggiungi programma**

   Oppure

   Inizia a digitare il nome di un programma, quindi fai clic su **Aggiungi programma** se non riesci a trovarlo. Il pulsante Aggiungi è seguito dal nome del programma digitato.

   ![Aggiungi programma Workfront durante la connessione dal campo di connessione](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   Viene visualizzata la casella **Crea programma**.

1. Aggiorna il **nome programma**. Questo è un campo obbligatorio.
1. Scegli un **Portfolio** dall&#39;elenco a discesa oppure inizia a digitare il nome di un portfolio, quindi selezionalo quando viene visualizzato nell&#39;elenco. Questo è un campo obbligatorio.
1. Fai clic su **Crea**.

   Il programma viene creato e aggiunto al campo di connessione del record selezionato.

1. (Facoltativo) Fare clic sul nome del nuovo programma da Workfront Planning per aprire la pagina del programma in Workfront e apportare ulteriori aggiornamenti.

