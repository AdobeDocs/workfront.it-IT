---
title: Creare gerarchie Workspace
description: In qualità di responsabile dell'area di lavoro, puoi creare più gerarchie di aree di lavoro tra i tipi di record in Adobe Workfront Planning. Dopo aver connesso i tipi di record in un'area di lavoro e aver creato una gerarchia, i tipi di record vengono connessi tra loro, con un tipo di record designato come padre e fino a 6 altri tipi di record configurati come figli.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# Creare gerarchie area di lavoro

In qualità di responsabile dell&#39;area di lavoro, puoi creare più gerarchie di aree di lavoro tra i tipi di record in Adobe Workfront Planning.

Dopo aver connesso i tipi di record in un&#39;area di lavoro e aver creato una gerarchia, i tipi di record vengono connessi tra loro, con un tipo di record designato come padre e fino a 6 altri tipi di record configurati come figli. <!--asking Robert how many we can have in one hierarchy; I think 7 total but not sure-->

Le gerarchie genereranno breadcrumb per i tipi di record e i record <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> visualizzati nelle relative intestazioni. In questo modo, gli utenti sanno dove si trovano nella gerarchia in qualsiasi fase del flusso di lavoro.

Per informazioni generali sulle gerarchie e sulle breadcrumb, vedere [Panoramica sulle gerarchie e sulle breadcrumb](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Requisiti di accesso

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

+++ Espandere per visualizzare i requisiti di accesso per eseguire i passaggi descritti in questo articolo:  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Qualsiasi pacchetto Workfront e Planning</p></li>
Oppure
<li><p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p></li></ul>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestire le autorizzazioni per un’area di lavoro</p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una gerarchia di workspace

{#step1-to-planning}

1. Fai clic su una scheda dell’area di lavoro.
1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome dell&#39;area di lavoro, quindi fai clic su **Impostazioni**.
Per impostazione predefinita, viene aperta la sezione **Gerarchie**.
1. Fai clic su **Nuova gerarchia** nell&#39;angolo superiore destro della pagina **Gerarchie**.
1. Fare clic su **Aggiungi oggetto** e selezionare un oggetto dal menu a discesa. Questo sarà l&#39;oggetto principale nella gerarchia.
È possibile selezionare un tipo di record dall&#39;area di lavoro corrente o un progetto da Workfront.
1. Fai clic su **Aggiungi oggetto** per aggiungere un secondo oggetto, che è il primo figlio nella gerarchia, quindi seleziona un altro oggetto nel menu a discesa.
   ![Nuova casella della gerarchia senza campo selezionato](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)
1. Fare clic su **Seleziona campo connesso** per indicare quale campo connette i due oggetti.
1. (Condizionale) Se esiste un campo connesso tra i due tipi di oggetto, selezionarlo dall&#39;elenco. In caso contrario, fare clic su **Aggiungi nuova connessione**.

   >[!WARNING]
   >
   >Se il campo **Crea campo corrispondente nel tipo di record collegato** non è stato selezionato al momento della creazione del campo connesso, è necessario modificare il campo prima di continuare.

1. (Condizionale) Se stai aggiungendo una nuova connessione, effettua le seguenti operazioni:

   1. Aggiungi un nome per il campo connesso nella casella **Nome**.
   1. Selezionare uno dei tipi di connessione seguenti:

      * **Molti a molti**
      * **Uno a molti**
      * **Molti a uno**
      * **Uno a uno**
   1. Selezionare uno dei tipi di aspetto dei record riportati di seguito.

      * **Nome e immagine**
      * **Nome**
      * **Immagine**
Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).
   1. Fai clic su **Salva**.
1. (Facoltativo) Continua ad aggiungere fino a 4 tipi di oggetto alle gerarchie seguendo la procedura descritta sopra. È possibile aggiungere prima tutti i tipi di oggetto e quindi i campi di connessione tra di essi.
1. (Facoltativo) Fai clic sull&#39;icona **Rimuovi** ![Rimuovi icona](assets/minus-icon.png) per rimuovere una connessione.
1. Fai clic su **Salva** per salvare la gerarchia.

   >[!TIP]
   >
   >Il pulsante **Salva** è inattivo se non sono presenti tutti i campi connessi.

   Si verificano le seguenti situazioni:

   * La gerarchia viene aggiunta alla sezione **Gerarchie** dell&#39;area di lavoro.
   * I record che popolano i campi di connessione visualizzano tutte le connessioni nelle relative breadcrumb quando si passa alla pagina di un record.
1. (Facoltativo) Passa il puntatore del mouse su una gerarchia, quindi fai clic sul menu **Altro**, quindi fai clic su una delle seguenti opzioni:

   * **Modifica**: apre la casella **Modifica gerarchia** in cui è possibile apportare modifiche.
   * **Elimina**: la gerarchia verrà eliminata definitivamente. Non è possibile recuperare le gerarchie eliminate. I campi di connessione non vengono eliminati.





