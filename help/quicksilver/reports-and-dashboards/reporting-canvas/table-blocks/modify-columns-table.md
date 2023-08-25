---
title: Configurare una colonna di tabella nell’area di lavoro Reporting
description: Configurare una colonna di tabella nell’area di lavoro Reporting
hidefromtoc: true
hide: true
source-git-commit: 350d64577bac677bb0cc9bcb804c32b0301bc5d4
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 2%

---


# Configurare una colonna di tabella nell’area di lavoro Reporting

Le colonne di una tabella possono essere configurate per la visualizzazione. È possibile modificare i seguenti aspetti di una colonna:

* Nome
* Ordinamento
* Modifica autorizzazione
* Testo al passaggio del mouse
* Aaggregazione
* Formattazione condizionale

## Prerequisiti

Prima di iniziare, devi iscriverti alla versione beta di Reporting Canvas. Per ulteriori informazioni, consulta [Reporting Canvas beta: panoramica](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Modificare le colonne in una tabella

1. Vai a un rapporto esistente, fai clic su **Menu Altro** icona ![](assets/more-icon.png) nell’intestazione del rapporto, seleziona quindi **Modifica**.
1. Nell’intestazione della tabella del rapporto, fai clic su **Modifica** icona ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Se la tabella è stata appena creata e non sono ancora stati aggiunti campi, fare clic sul pulsante Modifica al centro della tabella.

1. (Facoltativo) Aggiungi, riposiziona o elimina colonne nella tabella. Per ulteriori informazioni sulla modifica dei campi di una tabella, vedere [Aggiungere o modificare un blocco di tabella nell’area di lavoro rapporti](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | Aggiungi una nuova colonna | Per aggiungere una colonna a una tabella, fare clic su un campo e trascinarlo dalla **Campi** sulla destra della pagina nella tabella in cui si desidera inserirlo oppure fare doppio clic su un campo per aggiungerlo come colonna all&#39;estrema destra. |
   |---|---|
   | Spostare una colonna | Per modificare l&#39;ordine delle colonne in una tabella, fare clic sul nome di una colonna e trascinarlo in una nuova posizione. |
   | Eliminare una colonna | Per eliminare una colonna da una tabella, fai clic sulla colonna da eliminare, quindi fai clic sulla x a destra del nome della colonna. |

   {style="table-layout:auto"}

1. Per configurare una colonna, fai clic sul nome della colonna da modificare nella riga di intestazione della tabella, quindi su una delle seguenti schede nel pannello di destra:

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">Scheda Dati</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Aggregato basato su</td>
      <td><p> Per aggregare (riepilogare nell'intestazione) le informazioni in una colonna, selezionare il tipo di aggregazione desiderato dall' <strong>Aggregato basato su</strong> menu a discesa. Le opzioni disponibili dipendono dal tipo di dati contenuti nella colonna.</p><p>Se si utilizzano i gruppi nella tabella, il valore aggregato viene visualizzato nella riga del gruppo sopra il nome della colonna anziché accanto al nome della colonna.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Formato campo</td>
      <td><p>Disponibile solo se la colonna contiene dati relativi a data, percentuale, valuta o ora, non testo. Selezionare il formato desiderato per i dati in <b>Formato campo</b> a discesa. Ad esempio, è possibile visualizzare simboli di percentuale dopo i numeri di una colonna o modificare la modalità di visualizzazione delle date.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Il campo è modificabile</td>
      <td><span>Abilita <strong>Il campo è modificabile</strong> se si desidera consentire agli utenti che visualizzano la tabella di modificare il nome della colonna.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Ordina</strong></td>
      <td><p>Per impostazione predefinita, la tabella viene ordinata in base ai dati nella colonna più a sinistra, in ordine crescente. Per ordinare in base alla colonna selezionata, fare clic sulla freccia in giù accanto a <strong>Ordina</strong>, quindi fare clic sulla casella di controllo <b>Ordina per questa colonna</b>. È quindi possibile selezionare una <strong>Ordinamento</strong> direzione (valori crescenti o decrescenti) e un <strong>Ordinamento</strong> (priorità di ordinamento relativa di questa colonna rispetto ad altre colonne della tabella).</p><p>È possibile ripetere questo processo per ordinare la tabella in base a un massimo di 5 colonne diverse. Assicurati che ogni colonna abbia il <strong>Ordinamento</strong> rispetto alle nuove colonne selezionate per l'ordinamento.</p><p>Nota: se si elimina una colonna selezionata per l'ordinamento di una tabella e viene selezionata anche un'altra colonna per l'ordinamento, tale colonna verrà utilizzata per l'ordinamento decrescente della tabella. Se non sono selezionate altre colonne per l'ordinamento, la tabella torna all'impostazione predefinita: ordinamento per prima colonna.</p><p>Quando si designa una colonna per l'ordinamento della tabella, accanto al nome della colonna viene visualizzata una piccola casella con un numero che indica la priorità relativa della colonna nell'ordinamento della tabella (la tabella viene ordinata prima per 1, quindi per 2 e così via) e una freccia per indicare se la direzione dell'ordinamento è crescente o decrescente. </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
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
      <td>Immettere un nuovo nome visualizzato per la colonna (al massimo 100 caratteri).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostra testo al passaggio del mouse</td> 
      <td> <p>Determina se visualizzare il testo esplicativo quando qualcuno passa il mouse sul nome di una colonna.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Testo al passaggio del mouse</td> 
      <td>(Disponibile solo quando <strong>Mostra testo al passaggio del mouse</strong> è attivato.) Personalizza il testo esplicativo visualizzato quando qualcuno passa il mouse sul nome di una colonna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formattazione condizionale</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>Aggiungi <img src="assets/add-rule.png">, modifica <img src="assets/edit-icon.png">, o elimina <img src="assets/delete.png"> regola che formatta le celle della colonna quando i valori soddisfano i criteri specificati.</p> <p>Ad esempio, puoi creare una regola che modifichi in viola grassetto il font nel campo "Stato progetto" quando il valore del campo è uguale a "Costruzione".</p> <p>Oppure puoi utilizzare <b>Mostra un'icona</b> per aggiungere un'icona di flag verde a ogni elemento della colonna con lo stato "Corrente".</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>Nota: se utilizzi <strong>Mostra un'icona</strong>, le altre opzioni di formattazione non sono disponibili.</p> <p>Puoi selezionare <strong>Applica all'intera riga</strong> se si desidera che la formattazione abbia effetto sull'intera riga di una cella che soddisfa la condizione della regola. Ad esempio, puoi evidenziare i progetti in scadenza dopo una certa data applicando un colore di sfondo giallo non solo alle celle della colonna "Data di scadenza", ma all’intera riga in cui tali date si verificano.</p> <p>Suggerimento: quando si aggiungono opzioni di formattazione a una regola, il formato di cella risultante viene visualizzato in <strong>Anteprima</strong> nella parte inferiore del pannello.</p> </li> 
        <li value="2">Dopo aver aggiunto una regola, fai clic su <strong>Salva</strong>.</li> 
        <li value="3"> <p>(Facoltativo) Fai clic su <b>+ Aggiungi regola</b> per aggiungere altre regole alla stessa colonna.</p> <p>In una tabella vengono applicate più regole di formattazione condizionale nell'ordine seguente:</p> 
         <ul> 
          <li> <p>Le regole che si applicano a righe intere vengono valutate per prime, da sinistra a destra per ogni colonna e quindi dall'alto verso il basso all'interno di una colonna.</p> <p>Nota: la formattazione delle righe sovrascriverà la formattazione condizionale delle celle della riga, anche se soddisferebbe altrimenti la condizione della regola di un'altra colonna.</p> </li> 
          <li> <p>Altre regole vengono valutate successivamente, dall’alto verso il basso, in quanto sono elencate nel pannello di destra per una colonna. Puoi trascinare <img src="assets/drag-object-icon.png"> ha salvato le regole in quel pannello per modificarne l’ordine.</p> <p>Nota: le celle vengono formattate in base alla prima condizione che soddisfano e non verranno formattate ulteriormente anche se soddisfano altre condizioni.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Torna indietro** nell’angolo in alto a sinistra dello schermo per tornare al rapporto.
