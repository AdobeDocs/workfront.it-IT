---
title: Creare gerarchie Workspace
description: In qualità di responsabile dell'area di lavoro, puoi creare più gerarchie di aree di lavoro tra i tipi di record in Adobe Workfront Planning. Dopo aver connesso i tipi di record in un'area di lavoro e aver creato una gerarchia, i tipi di record vengono connessi tra loro, con un tipo di record designato come padre e fino a 3 altri tipi di record configurati come figli.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 34921b12ad902ba7390e4ea34825331280e7a8d6
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 1%

---


# Creare gerarchie area di lavoro

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

In qualità di responsabile dell&#39;area di lavoro, in Adobe Workfront Planning è possibile creare più gerarchie di aree di lavoro tra tipi di record.

Dopo aver connesso i tipi di record all&#39;interno di un&#39;area di lavoro, è possibile creare una gerarchia che organizzi tali connessioni. Le gerarchie organizzano i tipi di record e di oggetti in relazioni padre-figlio e possono contenere fino a quattro livelli di tipi di oggetto.

Se non esiste già una connessione tra due tipi di record, è possibile crearla durante l&#39;impostazione della gerarchia. Una volta definita, la gerarchia stabilisce un percorso strutturato tra tipi di record correlati all’interno dell’area di lavoro.

Le gerarchie generano breadcrumb per i rispettivi record visualizzati nelle intestazioni. In questo modo, gli utenti sanno dove si trovano nella gerarchia in qualsiasi fase del flusso di lavoro.

Per informazioni generali sulle gerarchie e sulle breadcrumb, vedere [Panoramica sulle gerarchie e sulle breadcrumb](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Requisiti di accesso

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

Puoi creare fino a 5 gerarchie in un’unica area di lavoro.

{#step1-to-planning}

1. Fai clic su una scheda dell’area di lavoro.
1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome dell&#39;area di lavoro, quindi fai clic su **Impostazioni**.
Per impostazione predefinita, viene aperta la sezione **Gerarchie**.
1. Fai clic su **Nuova gerarchia** nell&#39;angolo superiore destro della pagina **Gerarchie**.
1. Fare clic su **Aggiungi oggetto** e selezionare un tipo di oggetto dal menu a discesa. Questo sarà il primo tipo di oggetto nella gerarchia. <!--logged bug to correct to "Add object type"-->

   Il primo tipo di oggetto può essere solo un tipo di record di Planning.

   I progetti Workfront non possono essere selezionati come padri di altri tipi di oggetto in una gerarchia.

1. Fai clic su **Aggiungi oggetto** per aggiungere un secondo tipo di oggetto, che è il primo figlio nella gerarchia, quindi seleziona un altro tipo di oggetto nel menu a discesa.
Ogni tipo di oggetto aggiuntivo diventa figlio dei tipi di oggetto precedenti.

   ![Nuova casella della gerarchia senza campo selezionato](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)

1. Fare clic su **Seleziona campo connesso** per indicare quale campo connette i due oggetti.
1. (Condizionale) Se sono presenti più campi di connessione, selezionane uno dall’elenco,

   Oppure

   Fare clic su **Aggiungi nuova connessione** per aggiungere un nuovo campo connessione.

   In questo modo viene creato un campo di connessione dal tipo di record utilizzato come padre e un campo di connessione corrispondente dal tipo di record utilizzato come figlio.

   Se stai creando una connessione a progetti Workfront, non viene creato alcun campo nel progetto.

1. (Condizionale) Se non sono disponibili campi connessi, fare clic su **Crea connessione** e aggiungere una nuova connessione, quindi fare clic su **Salva**.

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

1. (Condizionale) Se il campo **Crea campo corrispondente nel tipo di record collegato** non è stato selezionato al momento della creazione del campo connesso, viene visualizzato un errore e occorre prima effettuare le seguenti operazioni: <!--check back on these steps; this is supposed to be seamless, but now you have to abandon creating a hierarchy to do this-->

   1. Fare clic su **Annulla** nella casella **Nuova gerarchia**.
   1. Fare clic sulla freccia indietro a sinistra del nome dell&#39;area di lavoro, quindi fare clic sulla scheda del tipo di record che si desidera scegliere come padre.
   1. Apri la visualizzazione tabella del tipo di record selezionato nel passaggio precedente, quindi vai al campo connessione con il tipo di oggetto che desideri utilizzare come figlio, passa il puntatore sull&#39;intestazione della colonna, quindi fai clic sul campo **Modifica**.
   1. Attiva l&#39;impostazione **Crea campo corrispondente nel tipo di record collegato**, quindi fai clic su **Salva**.
   1. Torna all&#39;area **Impostazioni** dell&#39;area di lavoro e fai di nuovo clic su **Nuova gerarchia**, quindi segui i passaggi per creare una gerarchia.

1. (Facoltativo) Continua ad aggiungere fino a 4 tipi di oggetto alle gerarchie seguendo la procedura descritta sopra. È possibile aggiungere prima tutti i tipi di oggetto e quindi i campi di connessione tra di essi.
1. (Facoltativo) Fai clic sull&#39;icona **Rimuovi** ![Rimuovi icona](assets/minus-icon.png) per rimuovere una connessione.
1. Fai clic su **Salva** per salvare la gerarchia.

   >[!TIP]
   >
   >Il pulsante **Salva** è inattivo se non sono presenti tutti i campi connessi.

   Si verificano le seguenti situazioni:

   * La gerarchia viene aggiunta alla sezione **Gerarchie** dell&#39;area di lavoro.
   * I record che popolano i campi di connessione visualizzano tutte le connessioni nelle relative breadcrumb quando si passa alla pagina di un record.

   >[!NOTE]
   >
   >È possibile collegare un record da un tipo di record figlio a un massimo di 10 record da un tipo di record padre.
   >
   >Per ulteriori informazioni, vedere [Panoramica della gerarchia e delle breadcrumb](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

1. (Facoltativo) Passa il puntatore del mouse su una gerarchia, quindi fai clic sul menu **Altro**.

   ![Menu Altro gerarchia espanso](assets/hierarchy-more-menu-expanded.png)

1. Fare clic su una delle seguenti opzioni:

   * **Modifica**: apre la casella **Modifica gerarchia** in cui è possibile apportare modifiche.
   * **Elimina**: la gerarchia verrà eliminata definitivamente. Non è possibile recuperare le gerarchie eliminate. I campi di connessione non vengono eliminati.





