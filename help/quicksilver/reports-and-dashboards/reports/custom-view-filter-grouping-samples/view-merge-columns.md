---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizzazione: unire le informazioni provenienti da più colonne in una colonna condivisa"
description: È possibile unire le informazioni visualizzate in più colonne separate e visualizzarle in una colonna condivisa.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 0%

---

# Vista: unire le informazioni provenienti da più colonne in una colonna condivisa

<!-- Audited: 1/2024 -->

È possibile unire le informazioni visualizzate in più colonne separate e visualizzarle in una colonna condivisa.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p> Corrente: 
   <ul>
   <li>Richiesta di modifica di una vista</li> 
   <li>Pianificare la modifica di un rapporto</li>
   </ul>
     </p>
     <p> Nuovo: 
   <ul>
   <li>Collaboratore per modificare una visualizzazione</li> 
   <li>Standard per modificare un rapporto</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni durante la condivisione o l’unione di colonne

* È possibile unire due colonne adiacenti e visualizzare le informazioni di ciascuna colonna separate da un&#39;interruzione di riga oppure unire le informazioni in due colonne adiacenti senza separatori tra le informazioni di ciascuna colonna.
* È possibile unire le informazioni di più colonne applicando la stessa sintassi descritta in questo articolo a una colonna già condivisa e a una adiacente.
* Il `valueformat=HTML` riga obbligatoria in una colonna condivisa. In caso contrario, le colonne non contengono informazioni (saranno vuote) quando il rapporto viene esportato da Adobe Workfront.
* La formattazione condizionale potrebbe non essere supportata nelle colonne unite.

  Esistono le seguenti eccezioni:

   * Quando si visualizzano le informazioni in Workfront, la formattazione della prima colonna viene mantenuta e la formattazione di tutte le altre colonne viene ignorata se le colonne che compongono una colonna unita hanno una formattazione diversa,.
   * Quando si esporta la visualizzazione in un file PDF, la formattazione condizionale viene applicata alla prima colonna di una colonna unita.
   * Quando si esporta la visualizzazione in un file Excel, le colonne unite vengono visualizzate come colonne separate. Le singole colonne visualizzano anche le rispettive regole di formattazione condizionale.

* Colonne con **viewalias** L&#39;attributo può limitare la quantità di colonne che è possibile unire. Per evitare questi limiti, evita di utilizzare **viewalias** attributo. Se è necessario includere **viewalias** in una colonna, assicurarsi che sia l&#39;ultimo elemento elencato nella colonna.

* Se si esporta un elenco con colonne condivise in un formato Excel o delimitato da tabulazioni, queste colonne vengono separate nel file esportato.

* Quando una o entrambe le colonne visualizzano `tile` tipo, nella colonna unita viene automaticamente introdotta un’interruzione di riga forzata. Ad esempio, i campi di testo con formattazione sono `tile` digita i campi. In questo caso, è presente un codice di riga `type=tile` quando si visualizzano le colonne in modalità testo.

## Unisci dati da due colonne senza interruzione di riga

È possibile unire i dati di più colonne separate per visualizzarli in una colonna senza interruzioni o spazi tra i valori di ciascuna colonna.

>[!TIP]
>
>Questo approccio è consigliato quando si uniscono due colonne che non possono mai mostrare un valore per lo stesso record contemporaneamente. Ad esempio, in un rapporto Elemento di lavoro, è possibile unire le colonne Nome problema e Nome attività senza un&#39;interruzione di riga tra di esse perché un elemento di lavoro non può mai avere contemporaneamente un nome problema e un nome attività. Un elemento di lavoro può essere un problema o un’attività in Workfront.

Per unire i dati di due colonne senza interruzioni di riga:

1. Utilizzando la modalità testo per una visualizzazione, aggiungere il testo seguente alla prima colonna che si desidera unire:

   `sharecol=true`

   Quando si uniscono le prime due colonne di un elenco o di un report, Workfront precede ogni riga di testo contenente informazioni sull&#39;oggetto nella prima colonna con `column.0.` e le righe di testo che contengono informazioni sulla seconda colonna con `column.1.` .

   È necessario anteporre al numero di colonna della prima colonna il numero di tale colonna. Il conteggio delle colonne inizia sempre con la colonna più a sinistra dell’elenco o del rapporto etichettata come `column.0.`.

   Se condividi più colonne, assicurati di aggiungere il numero di colonna nelle righe di codice che contengono le informazioni di condivisione per ciascuna colonna.

   **Esempio:** Di seguito è riportato il codice in modalità testo per una colonna unita che contiene tre colonne separate, a partire dalla seconda colonna dell&#39;elenco. I valori uniti sono Nome progetto, Data inizio pianificata e Nome del proprietario del progetto e non vi è alcuna interruzione tra i tre valori:

   `column.1.valuefield=name`

   `column.1.valueformat=HTML`

   `column.1.sharecol=true`

   `column.2.valuefield=plannedStartDate`

   `column.2.valueformat=atDate`

   `column.2.sharecol=true`

   `column.3.valuefield=owner:name`

   `column.3.valueformat=HTML`

![](assets/shared-column-no-line-breaks-350x142.png)

1. Clic **Salva**, quindi **Salva visualizzazione**.

## Unisci dati da due colonne con un’interruzione di riga

Per unire i dati di più colonne in modo da visualizzarli in una colonna comune con un&#39;interruzione di riga tra i valori di ciascuna colonna, eseguire le operazioni seguenti:

1. Aggiungere una terza colonna tra le due colonne che si desidera unire.

   >[!TIP]
   >
   >* Le colonne che si desidera unire devono essere adiacenti.
   >* Fare clic sulla prima colonna che si desidera unire.

1. Clic **Passa alla modalità testo** e aggiungi il seguente codice nella colonna centrale aggiunta al passaggio 1:

   `value=<br>`

   `valueformat=HTML`

   `width=1`

   `sharecol=true`


1. Fai clic sulla prima colonna e fai clic su **Passa alla modalità testo**, quindi aggiungi il seguente testo alla colonna:

   `sharecol=true`

   Quando si uniscono le prime due colonne di un elenco o di un report, Workfront precede ogni riga di testo contenente informazioni sull&#39;oggetto nella prima colonna con `column.0.`, la colonna con le informazioni di condivisione `column.1.`e le righe di testo che contengono informazioni sulla seconda colonna con `column.2.`.

   Se la colonna combinata si trova al centro della vista, le colonne vengono numerate in base alla loro posizione nella vista. Il conteggio delle colonne inizia sempre con la colonna più a sinistra dell’elenco o del rapporto etichettata come `column.0.`.

   Se condividi più di una colonna, assicurati di aggiungere il numero della colonna nelle righe di codice che contengono le informazioni di condivisione.

   **Esempio:** Di seguito è riportato il codice in modalità testo per una colonna condivisa che contiene Nome progetto, Data inizio pianificata e Nome del proprietario del progetto con un&#39;interruzione di riga. La colonna condivisa è la seconda colonna di una visualizzazione di progetto.


   `column.1.displayname=Project_StartDate_Owner`

   `column.1.sharecol=true`

   `column.1.textmode=true`

   `column.1.valuefield=name`

   `column.1.valueformat=HTML`

   `column.2.value=<br>`

   `column.2.width=1`

   `column.2.valueformat=HTML`

   `column.2.sharecol=true`

   `column.3.valuefield=plannedStartDate`

   `column.3.valueformat=atDate`

   `column.3.sharecol=true`

   `column.4.value=<br>`

   `column.4.width=1`

   `column.4.valueformat=HTML`

   `column.4.sharecol=true`

   `column.5.textmode=true`

   `column.5.valuefield=owner:name`

   `column.5.valueformat=HTML`


   ![](assets/shared-column-with-line-breaks-350x199.png)


1. Clic **Salva**, quindi **Salva visualizzazione**.
