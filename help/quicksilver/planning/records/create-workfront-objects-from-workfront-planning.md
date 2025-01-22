---
title: Creazione di oggetti Workfront da Workfront Planning
description: È possibile creare tipi di oggetti di Workfront quando vengono collegati da altri record in Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: eb68357ed4fd8f323707aa4a54a0f946253bf4e0
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Creazione di oggetti Workfront da Workfront Planning

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

È possibile creare i seguenti tipi di oggetti Workfront da Workfront Planning:

* Progetti
* Portfolio

È possibile creare progetti e portafogli Workfront da Workfront Planning quando si collega un record di Workfront Planning a un progetto o a un portfolio.

>[!IMPORTANT]
>
>* Puoi creare solo progetti e portfolio in Workfront quando li connetti da un record.
>
>* Non è possibile creare programmi, gruppi o società quando si collegano da un record in Workfront Planning.
>
<!--* You cannot create a project from a template when when you create projects by connecting them from a record. You must manually add tasks and project information or a template to the new project after you add it to the record.-->

Per informazioni sulla connessione dei record di Planning con gli oggetti di Workfront, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
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
   <p>Modificare l'accesso in Workfront per i tipi di oggetto che si desidera creare (progetti e portafogli) quando si collegano i record. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td> <p>Consente di gestire le autorizzazioni per l'area di lavoro a cui si desidera aggiungere record. </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
   <p>Gestisci le autorizzazioni per gli oggetti Workfront (portfolio) per aggiungere oggetti figlio (progetti).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti per la creazione di oggetti Workfront quando vengono collegati ai record di Workfront Planning

Prima di poter aggiungere nuovi progetti o portfolio collegandoli da record esistenti, è necessario disporre dei seguenti elementi:

* Tipi di record connessi a progetti o portfolio Workfront. Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).
* Record. Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
* L&#39;accesso e le autorizzazioni corretti in Workfront Planning e Workfront, come descritto nella sezione [Requisiti di accesso](#access-requirements) in questo articolo.

## Creazione di progetti durante la connessione con i record di Workfront Planning

Per creare progetti mentre li si connette da altri record:

1. Passare alla pagina dei dettagli di un record o alla tabella del tipo di record e iniziare a collegare i record di Workfront Planning ai progetti Workfront, come descritto nell&#39;articolo [Connetti record](/help/quicksilver/planning/records/connect-records.md).

   È possibile connettere progetti da un campo di connessione nelle seguenti aree di Workfront Planning:

   * Visualizzazione tabella di un tipo di record
   * Pagina dei dettagli o casella di anteprima di un record

1. (Condizionale) Se non riesci a trovare un progetto quando tenti di aggiungerlo dal campo record connesso di un altro record, aggiungi un nome e fai clic su **+ Aggiungi**. Il pulsante **+ Aggiungi** è seguito dal nome del tipo di oggetto a cui ci si connette. Ad esempio, &quot;Aggiungi progetto&quot;, quando si aggiunge un nuovo progetto a una campagna esistente. Il pulsante Aggiungi è seguito anche dal nome del progetto digitato.

   ![](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview">Viene aperta la casella **Crea progetto**.</span>

1. <span class="preview">(Facoltativo) Aggiornare **Nome progetto**. Per impostazione predefinita, il progetto prende il nome da quello che hai aggiunto come elemento di ricerca quando lo connetti dal record. </span>
1. <span class="preview">(Facoltativo) Selezionare un **modello di progetto**. Se non si seleziona un modello, Workfront crea un progetto vuoto, senza attività. </span>
1. <span class="preview">Fai clic su **Crea**. </span>
1. <span class="preview">(Condizionale) Se hai selezionato di creare un progetto da un modello, segui i passaggi descritti nell&#39;articolo [Creare un progetto utilizzando un articolo modello](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) per completare l&#39;aggiunta del progetto.</span>

   Il nuovo progetto viene creato e aggiunto al campo connesso del record selezionato.

1. (Facoltativo) Fare clic sul nome del nuovo progetto da Workfront Planning per aprire la pagina del progetto in Workfront e apportare ulteriori aggiornamenti al progetto.

## Creazione di portfolio durante la connessione con i record di Workfront Planning

Per creare i portfolio durante la connessione da altri record:

1. Andare alla pagina dei dettagli di un record o alla tabella del tipo di record e iniziare a collegare i record di Workfront Planning ai portfolio Workfront, come descritto nell&#39;articolo [Connetti record](/help/quicksilver/planning/records/connect-records.md).

   È possibile connettere i portfolio da un campo di connessione nelle seguenti aree di Workfront Planning:

   * Visualizzazione tabella di un tipo di record
   * Pagina dei dettagli o casella di anteprima di un record

1. (Condizionale) Se non riesci a trovare un portfolio quando tenti di aggiungerlo dal campo record connesso di un altro record, aggiungi un nome e fai clic su **+ Aggiungi**. Il pulsante **+ Aggiungi** è seguito dal nome del tipo di oggetto a cui ci si connette. Ad esempio, &quot;Aggiungi portfolio&quot;, quando si aggiunge un nuovo portfolio a una campagna esistente. Il pulsante Aggiungi è seguito anche dal nome del portfolio digitato.

   ![](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Il portfolio viene creato e aggiunto al campo di connessione del record selezionato.

1. (Facoltativo) Fare clic sul nome del nuovo portfolio da Workfront Planning per aprire la pagina del portfolio in Workfront e apportare ulteriori aggiornamenti al portfolio.
