---
title: Configurare una colonna di tabella in Reporting Canvas
description: Configurare una colonna di tabella in Reporting Canvas
author: Nolan
feature: Reports and Dashboards
exl-id: ce33888f-344d-4f69-b527-9679340d134b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 2%

---


# Configurare una colonna di tabella in Reporting Canvas

Le colonne di una tabella possono essere configurate per la visualizzazione. È possibile modificare i seguenti aspetti di una colonna:

* Nome
* Ordinamento
* Modifica autorizzazione
* Testo al passaggio del mouse
* Aggregazione
* Formattazione condizionale

## Prerequisiti

Prima di iniziare, è necessario iscriversi alla versione beta di Reporting Canvas. Per ulteriori informazioni, consulta [Reporting Canvas beta: panoramica](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Modificare le colonne in una tabella

1. Passa a un rapporto esistente e fai clic sul pulsante **Menu Altro** icona ![](assets/more-icon.png) nell’intestazione del rapporto, seleziona **Modifica**.
1. Nell’intestazione della tabella del rapporto, fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Se la tabella è stata creata e non sono stati ancora aggiunti campi, fare clic sul pulsante Modifica al centro della tabella.

1. (Facoltativo) Aggiungi, riposiziona o elimina colonne nella tabella. Per ulteriori informazioni sulla modifica dei campi in una tabella, consulta [Aggiungere o modificare un blocco di tabella in Reporting Canvas](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | Aggiungi una nuova colonna | Per aggiungere una colonna a una tabella, fai clic su e trascina un campo dal menu **Campi** a destra della pagina nella tabella in cui si desidera posizionarla oppure fare doppio clic su un campo per aggiungerlo come colonna più a destra. |
   |---|---|
   | Spostare una colonna | Per ridisporre l’ordine delle colonne di una tabella, fare clic sul nome di una colonna e trascinarla in una nuova posizione. |
   | Eliminare una colonna | Per eliminare una colonna da una tabella, fai clic sulla colonna da eliminare, quindi fai clic sulla x a destra del nome della colonna. |

   {style=&quot;table-layout:auto&quot;}

1. Per configurare una colonna, fai clic sul nome della colonna da modificare nella riga di intestazione della tabella, quindi seleziona una delle seguenti schede nel pannello di destra:

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-step-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">Scheda Dati</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Aggregato basato su</td>
      <td><p> Per aggregare (riepilogare nell’intestazione) le informazioni in una colonna, seleziona il tipo di aggregazione desiderato dalla <strong>Aggregato basato su</strong> menu a discesa. Le opzioni disponibili dipendono dal tipo di dati contenuto nella colonna .</p><p>Se utilizzi gruppi nella tabella, il valore aggregato viene visualizzato nella riga del gruppo sopra il nome della colonna anziché accanto al nome della colonna.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Formato campo</td>
      <td><p>Disponibile solo se la colonna contiene dati relativi a data, percentuale, valuta o ora, non testo. Seleziona il formato desiderato per i dati nella <b>Formato campo</b> a discesa. Ad esempio, è possibile visualizzare i segni di percentuale dopo i numeri in una colonna o modificare la modalità di visualizzazione delle date.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Il campo è modificabile</td>
      <td><span>Abilita la <strong>Campo modificabile</strong> per consentire agli utenti che visualizzano la tabella di modificare il nome della colonna.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Ordina</strong></td>
      <td><p>Per impostazione predefinita, la tabella ordina in base ai dati presenti nella colonna più a sinistra, in ordine crescente. Per ordinare in base alla colonna selezionata, fai clic sulla freccia rivolta verso il basso accanto a <strong>Ordinare</strong>, quindi fai clic sulla casella di controllo <b>Ordina per colonna</b>. È quindi possibile selezionare una <strong>Ordinamento</strong> direzione (valori ascendenti o discendenti) e <strong>Ordinamento</strong> (la priorità di ordinamento relativa di questa colonna rispetto ad altre colonne di ordinamento della tabella).</p><p>È possibile ripetere questo processo per ordinare la tabella in base a 5 colonne diverse. Assicurati che ogni colonna abbia il corretto <strong>Ordinamento</strong> rispetto a qualsiasi nuova colonna selezionata per l’ordinamento.</p><p>Nota: Se si elimina una colonna selezionata per ordinare una tabella e se è selezionata per l’ordinamento un’altra colonna, questa viene utilizzata per ordinare la tabella in ordine decrescente. Se non sono state selezionate altre colonne per l’ordinamento, la tabella torna all’impostazione predefinita: ordinamento in base alla prima colonna.</p><p>Quando si designa una colonna per ordinare la tabella, accanto al nome della colonna viene visualizzata una piccola casella con un numero che indica la priorità relativa di tale colonna nell’ordinamento della tabella (la tabella viene ordinata prima per 1, quindi 2 e così via) e una freccia per indicare se la direzione di ordinamento è crescente o decrescente. </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
     </tr>
    </tbody>
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <th role="rowheader" colspan="2">Scheda Stile</th> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Etichetta colonna personalizzata</strong> </td> 
      <td>Immettere un nuovo nome visualizzato per la colonna (limite di 100 caratteri).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostra testo al passaggio del mouse</td> 
      <td> <p>Determinare se si desidera visualizzare il testo esplicativo quando si passa il mouse su un nome di colonna.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Testo al passaggio del mouse</td> 
      <td>(Disponibile solo quando <strong>Mostra testo al passaggio del mouse</strong> è abilitato). Personalizza il testo esplicativo visualizzato quando si passa il mouse sul nome di una colonna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formattazione condizionale</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>Aggiungi <img src="assets/add-rule.png">, modifica <img src="assets/edit-icon.png">o eliminare <img src="assets/delete.png"> una regola che formatta le celle della colonna quando i relativi valori soddisfano i criteri specificati.</p> <p>Ad esempio, puoi creare una regola che modifica il font nel campo "Stato progetto" in grassetto viola quando il valore di quel campo è uguale a "Creazione".</p> <p>Oppure puoi utilizzare <b>Mostra un’icona</b> per aggiungere un’icona di flag verde a ogni elemento della colonna con lo stato "Corrente".</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>Nota: Se utilizzi <strong>Mostra un’icona</strong>, le altre opzioni di formattazione non sono disponibili.</p> <p>È possibile selezionare <strong>Applica a tutta la riga</strong> se si desidera che la formattazione influisca sull'intera riga di una cella che soddisfa le condizioni della regola. Ad esempio, puoi evidenziare i progetti che devono essere completati dopo una determinata data applicando un colore di sfondo giallo non solo alle celle della data nella colonna "Due su", ma all’intera riga in cui si verificano tali date.</p> <p>Suggerimento: Quando si aggiungono opzioni di formattazione a una regola, il formato della cella risultante viene visualizzato in <strong>Anteprima</strong> nella parte inferiore del pannello.</p> </li> 
        <li value="2">Al termine dell’aggiunta di una regola, fai clic su <strong>Salva</strong>.</li> 
        <li value="3"> <p>(Facoltativo) Fai clic su <b>+ Aggiungi regola</b> per aggiungere ulteriori regole alla stessa colonna.</p> <p>Più regole di formattazione condizionale in una tabella vengono applicate nell’ordine seguente:</p> 
         <ul> 
          <li> <p>Le regole che si applicano alle righe intere vengono valutate prima, da sinistra a destra per ogni colonna e poi dall’alto verso il basso all’interno di una colonna.</p> <p>Nota: La formattazione delle righe sostituisce la formattazione condizionale per le celle della riga, anche se in caso contrario soddisfano la condizione della regola di un’altra colonna.</p> </li> 
          <li> <p>Altre regole vengono valutate successivamente, dall’alto verso il basso in quanto sono elencate nel pannello di destra per una colonna. Puoi trascinare <img src="assets/drag-object-icon.png"> regole salvate in quel pannello per modificarne l’ordine.</p> <p>Nota: Le celle vengono formattate in base alla prima condizione che soddisfano e non verranno formattate ulteriormente anche se soddisfano altre condizioni.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic sul pulsante **Torna indietro** nell’angolo in alto a sinistra dello schermo per tornare al rapporto.
