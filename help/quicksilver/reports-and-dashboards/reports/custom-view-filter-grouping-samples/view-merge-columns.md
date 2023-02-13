---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: unire informazioni da più colonne in una colonna condivisa"'
description: È possibile unire le informazioni visualizzate in più colonne separate e visualizzarle in una colonna condivisa.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# Visualizza: unire informazioni da più colonne in una colonna condivisa

È possibile unire le informazioni visualizzate in più colonne separate e visualizzarle in una colonna condivisa.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni durante la condivisione o l’unione di colonne

* È possibile unire due colonne adiacenti e visualizzare le informazioni di ciascuna colonna separata da un’interruzione di riga oppure unire le informazioni in due colonne adiacenti senza separatore tra le informazioni di ciascuna colonna.
* È possibile unire le informazioni provenienti da più di due colonne applicando la stessa sintassi descritta in questo articolo a una colonna già condivisa e a una adiacente.
* il

   ```
   valueformat=HTML
   ```

   La riga è obbligatoria in una colonna condivisa. In caso contrario, quando il rapporto viene esportato da Adobe Workfront, le colonne non contengono alcuna informazione (saranno vuote).
* La formattazione condizionale potrebbe non essere supportata nelle colonne unite.

   Esistono le seguenti eccezioni:

   * Quando si visualizzano le informazioni in Workfront, viene mantenuta la formattazione della prima colonna e la formattazione di tutte le altre colonne viene ignorata se le colonne che compongono una colonna unita hanno una formattazione diversa l’una dall’altra,
   * Quando si esporta la visualizzazione in un file PDF, la formattazione condizionale si applica alla prima colonna di una colonna unita.
   * Quando si esporta la visualizzazione in un file Excel, le colonne unite vengono visualizzate come colonne separate. Le singole colonne presentano anche le rispettive regole di formattazione condizionale.

* Colonne con **viewalias** L&#39;attributo può limitare la quantità di colonne che è possibile unire. Per evitare questi limiti, evita di utilizzare il **viewalias** attributo. Se devi includere **viewalias** in una colonna, accertati che sia l’ultimo elemento elencato nella colonna.

* Se si esporta un elenco con colonne condivise in un formato Excel o Tab Delimited, tali colonne sono separate nel file esportato.

## Unisci dati da due colonne senza interruzione di riga

È possibile unire i dati di più colonne separate per visualizzarli in una colonna senza interruzioni o spazi tra i valori di ciascuna colonna.

>[!TIP]
>
>Questo approccio è consigliato quando si uniscono due colonne che non possono mai mostrare un valore per lo stesso record contemporaneamente. Ad esempio, in un rapporto Elemento di lavoro è possibile unire le colonne Nome problema e Nome attività senza interruzioni di riga, perché un elemento di lavoro non può avere un nome problema e un nome attività contemporaneamente. Un elemento di lavoro può essere un problema o un&#39;attività in Workfront.

Per eseguire questa operazione:

1. Utilizzando la modalità testo per una visualizzazione, aggiungere il testo seguente alla prima colonna da unire:

   ```
   sharecol=true
   ```

   Quando si uniscono le prime due colonne di un elenco o di un rapporto, Workfront precede ogni riga di testo che contiene informazioni sull’oggetto nella prima colonna con

   ```
   column.0.
   ```

   e le righe di testo che contengono informazioni sulla seconda colonna con

   ```
   column.1.
   ```

   .\
   È necessario precedere il numero di colonna della prima colonna con il numero di tale colonna. Il conteggio delle colonne inizia sempre con la colonna più a sinistra dell’elenco o del rapporto etichettato come

   ```
   column.0.
   ```

   .

   Se condividi più colonne, accertati di aggiungere il numero di colonna nelle righe di codice che contengono le informazioni di condivisione per ciascuna colonna.

   **Esempio:** Di seguito è riportato il codice della modalità testo per una colonna unita che contiene tre colonne separate, a partire dalla seconda colonna dell’elenco. I valori uniti sono Nome progetto, Data inizio pianificata e Nome del proprietario del progetto e non esiste alcuna interruzione tra i tre valori:

   ```
   column.1.valuefield=name
   ```

   ```
   column.1.valueformat=HTML
   ```

   ```
   column.1.sharecol=true
   ```

   ```
   column.2.valuefield=plannedStartDate
   ```

   ```
   column.2.valueformat=atDate
   ```

   ```
   column.2.sharecol=true
   ```

   ```
   column.3.valuefield=owner:name
   ```

   ```
   column.3.valueformat=HTML
   ```

   <pre><img src="assets/shared-column-no-line-breaks-350x142.png" style="width: 350;height: 142;"></pre>

1. Fai clic su **Salva**, quindi **Salva visualizzazione**.

## Unione di dati da due colonne con interruzione di riga

Effettua le seguenti operazioni per unire i dati di più colonne in modo da visualizzarli in una colonna comune con un’interruzione di riga tra i valori di ciascuna colonna:

1. Aggiungi una terza colonna tra le due colonne da unire.

   >[!TIP]
   * Le colonne che si desidera unire devono essere adiacenti.
   * Fare clic sulla prima colonna che si desidera unire.


1. Fai clic su **Passa alla modalità testo** e aggiungi il seguente codice nella colonna centrale aggiunto al passaggio 1:

   ```
   value=<br>
   ```

   ```
   valueformat=HTML
   ```

   ```
   width=1
   ```

   ```
   sharecol=true
   ```

1. Aggiungi il testo seguente alla prima colonna:

   ```
   sharecol=true
   ```

   Quando si uniscono le prime due colonne di un elenco o di un rapporto, Workfront precede ogni riga di testo che contiene informazioni sull’oggetto nella prima colonna con

   ```
   column.0.
   ```

   , la colonna con le informazioni di condivisione con

   ```
   column.1.
   ```

   e le righe di testo che contengono informazioni sulla seconda colonna con

   ```
   column.2.
   ```

   . Se la colonna combinata si trova al centro della vista, le colonne vengono numerate in base alla loro posizione nella vista. Il conteggio delle colonne inizia sempre con la colonna più a sinistra dell’elenco o del rapporto etichettato come

   ```
   column.0.
   ```

   .

   Se condividi più colonne, accertati di aggiungere il numero di colonna nelle righe di codice che contengono le informazioni di condivisione.

   **Esempio:** Di seguito è riportato il codice della modalità di testo per una colonna condivisa contenente Nome progetto, Data inizio pianificata e Nome del proprietario del progetto con un&#39;interruzione di riga. La colonna condivisa è la seconda colonna di una visualizzazione del progetto.

   ```
   column.1.displayname=Project_StartDate_Owner
   ```

   ```
   column.1.sharecol=true
   ```

   ```
   column.1.textmode=true
   ```

   ```
   column.1.valuefield=name
   ```

   ```
   column.1.valueformat=HTML
   ```

   ```
   column.2.value=<br>
   ```

   ```
   column.2.width=1
   ```

   ```
   column.2.valueformat=HTML
   ```

   ```
   column.2.sharecol=true
   ```

   ```
   column.3.valuefield=plannedStartDate
   ```

   ```
   column.3.valueformat=atDate
   ```

   ```
   column.3.sharecol=true
   ```

   ```
   column.4.value=<br>
   ```

   ```
   column.4.width=1
   ```

   ```
   column.4.valueformat=HTML
   ```

   ```
   column.4.sharecol=true
   ```

   ```
   column.5.textmode=true
   ```

   ```
   column.5.valuefield=owner:name
   ```

   ```
   column.5.valueformat=HTML
   ```

   <pre><img src="assets/shared-column-with-line-breaks-350x199.png" style="width: 350;height: 199;"></pre>

1. Fai clic su **Salva**, quindi **Salva visualizzazione**.
