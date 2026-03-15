---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare la formattazione condizionale nelle viste
description: Quando condividi i tuoi report con altri utenti in Adobe Workfront, valuta la possibilità di personalizzare la visualizzazione dei report, per facilitare la lettura di determinate informazioni o semplicemente per metterti in risalto.
author: Courtney
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 8%

---

# Utilizzare la formattazione condizionale nelle viste

<!-- Audited: 11/2024 -->

Quando condividi i tuoi report con altri utenti in Adobe Workfront, valuta la possibilità di personalizzare la visualizzazione dei report, per facilitare la lettura di determinate informazioni o semplicemente per metterti in risalto.

È possibile personalizzare la scheda Dettagli dei report aggiungendo formattazione speciale o condizionale alla visualizzazione dei report.

Per ulteriori informazioni sulla creazione di report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

La formattazione condizionale delle colonne nella visualizzazione del report consente di impostare regole che influiscono sulla visualizzazione del report. Quando tali condizioni o regole sono soddisfatte, viene applicata la formattazione speciale.

Se, ad esempio, la percentuale di completamento di un&#39;attività è inferiore al 20%, è possibile evidenziare il campo visualizzando il numero di percentuale in grassetto, testo rosso e un colore di sfondo giallo.

Con una visualizzazione con formattazione condizionale è possibile:

* Modificare l&#39;intestazione di una colonna.
* Change the value of a column to customized text or an image.
* Format the display of a field by changing the font type, color, alignment, or the color of the background.

The changes you make in the view of the report take effect only in the Details tab of the report. These changes do not affect the Summary, Matrix, or Chart tabs of the report.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</strong></td> 
   <td> 
    <p>Visualizzazione standard o piano per report</p>
    <p>Contributor or Request for list views</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l'accesso a filtri, viste, raggruppamenti</p> <p>Modificare l’accesso a report, dashboard, calendari per modificare una visualizzazione in un report</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
    <td> <p>Gestire le autorizzazioni per un report per creare o modificare una visualizzazione in un report</p> <p>Gestire le autorizzazioni per una visualizzazione</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

È necessario creare un report prima di aggiungere la formattazione condizionale alla relativa visualizzazione.

Per informazioni sulla creazione di un report, vedere [Creare un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Creare una vista con formattazione condizionale

{{step1-to-reports}}

1. Click the name of a report where you want to create a conditionally-formatted view

   Oppure

   Click **New Report**, then select an object type to build a new report.

1. (Conditional) If you edit an existing report, click **Report Actions**, then click **Edit**.

1. In the **Columns (View)** tab, click to select an existing column, or click **Add Column** to create a column.
1. In the **Show in this column** field in the upper-left corner of the report builder, select the field you want to display in the new column.
1. Fare clic su **Opzioni avanzate**.

1. Specificate le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Etichetta colonna personalizzata</strong></td> 
      <td> <p>Specify a name for the column.</p> <p>If you are editing an existing column, specifying a name here changes the existing column name.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato campo</strong></td> 
      <td>Scegliete il formato in cui viene visualizzato il valore nella colonna. A seconda del campo colonna, è possibile impostare la modalità di visualizzazione di date, numeri o valuta. Questa opzione non è visualizzata in tutte le colonne.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra questa colonna quando in un dashboard</strong></td> 
      <td>Selezionare questo campo se si desidera che la colonna venga visualizzata quando il report viene inserito in un dashboard. La colonna viene sempre visualizzata quando si esamina il report all'esterno di un dashboard.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Aggiungi una regola per la colonna**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. In the **When the:** section, set a condition statement for the column.

   For example: &quot;when the Task Percent Complete Equals (Case Sensitive) 50.&quot;
1. In the **Show the field like this:** section specify what this field looks like when the condition defined above is met.

   Specificate le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Colore testo</strong></td> 
      <td> <p>Selezionate il colore in cui il testo viene visualizzato mediante il selettore colore.</p> <p><b>NOTA</b></p> <p> Se il campo contiene un collegamento ipertestuale, le selezioni del colore del testo non vengono applicate a questo campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formato testo</strong></td> 
      <td>Scegliere se visualizzare il testo in grassetto o in corsivo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Allineamento testo</strong></td> 
      <td>Seleziona se allineare il testo a destra, al centro o a sinistra all’interno della colonna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Informazioni di base</strong></td> 
      <td>Seleziona il colore dello sfondo per il testo utilizzando il selettore colore.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra icona</strong></td> 
      <td>Selezionate una delle 16 icone disponibili per visualizzare un'icona anziché il valore effettivo della colonna.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mostra testo</strong></td> 
      <td> <p>Selezionare questa opzione per visualizzare un'etichetta personalizzata per la colonna anziché il valore effettivo. Specificate il testo da visualizzare anziché il valore nel campo fornito.</p> <p><b>IMPORTANTE</b></p> <p>La selezione di <strong>Mostra testo</strong> disabilita la possibilità di modificare il testo in linea in questa colonna.<br>Inoltre, non è possibile modificare il valore di una colonna Predecessore perché contiene logica incorporata.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Applica a tutta la riga</strong></td> 
      <td>Select this option to apply settings to the entire row rather than applying settings to just the selected column.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Add Rule**.\
   You can add additional rules to the same column, or add rules to other columns.

   Rules are applied in the order that they were created. They are combined but they do not overwrite each other, though a column rule takes precedence over a row rule on the same cell.

   **ESEMPIO 1**

   Puoi innanzitutto creare una regola in base alla quale, quando un progetto è impostato sullo stato Edificio, il colore del testo è viola e grassetto. Viene quindi creata una seconda regola che indica che quando il nome di un&#39;attività non è vuoto, il colore del testo è rosso e corsivo e il colore di sfondo è verde. In questo esempio si verifica quanto segue:

   * Le attività il cui Stato progetto è Generato vengono visualizzate in viola e grassetto. If the task name is not blank, tasks also have a green background.
   * Tasks whose Project Status is anything other than Building (and the Task Name is not blank) are displayed in a red and italicized text with a green background.

   **ESEMPIO 2**

   Creare una regola nella colonna Data completamento pianificato progetto che influisca sull&#39;intera riga, rendendo lo sfondo grigio se il progetto viene annullato, ad esempio quando lo stato del progetto è Morto. Quindi crea una regola di colonna che renda lo sfondo rosso quando la Data di completamento pianificata del progetto è precedente alla data odierna (ovvero il progetto è in ritardo). In questo esempio, se a un progetto annullato è associata una data di completamento in ritardo, la cella verrà visualizzata in rosso anche se le altre celle nella riga sono grigie. Per correggere questa formattazione:

   * Modifica la formattazione per la data di completamento pianificata ed elimina la regola di colonna per lo sfondo rosso nei progetti in ritardo.
   * Aggiungi una regola di colonna con la stessa formattazione della regola di riga (sfondo grigio quando Stato progetto = Morto).
   * Aggiungi nuovamente la regola di colonna per lo sfondo rosso nei progetti in ritardo.
   * Quando salvi le regole e la vista, lo sfondo rosso non viene applicato a un progetto annullato.

1. Fai clic su **Salva**.
1. Fai clic su **Salva e Chiudi**.\
   Nel report, gli utenti visualizzano le modifiche apportate al formato se sono state soddisfatte le condizioni specificate.
