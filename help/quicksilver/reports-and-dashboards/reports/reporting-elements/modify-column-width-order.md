---
product-area: reporting
navigation-topic: reporting-elements
title: Modificare la larghezza e l’ordine delle colonne
description: Leggi questo articolo per scoprire le linee guida per la larghezza delle colonne e come modificare la larghezza e l’ordine delle colonne in Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# Modificare la larghezza e l’ordine delle colonne

Di seguito sono riportate le linee guida relative al funzionamento delle larghezze di colonna in Adobe Workfront:

* Per impostazione predefinita, Workfront definisce la larghezza delle colonne negli elenchi e nei rapporti.
* Workfront regola automaticamente la larghezza delle colonne in base alla `valueformat`informazioni in tutti gli elenchi e i rapporti, salvo diversa indicazione nella modalità testo della colonna.

   >[!NOTE]
   >
   >Workfront non regola la larghezza delle colonne in base al `valueformat` negli elenchi disponibili nelle aree Configurazione e Rapporti.

   La `valueformat` definisce il tipo di informazioni da visualizzare nella colonna. Ad esempio, le colonne che visualizzano un numero sono più strette rispetto alle colonne che visualizzano il campo Descrizione .

* Puoi personalizzare la larghezza delle colonne negli elenchi e nei rapporti di Workfront in base alle tue esigenze, a seconda del tipo di informazioni che desideri visualizzare nelle colonne.

   È possibile modificare temporaneamente la larghezza delle colonne, durante la visualizzazione di un elenco o di un rapporto o in modo permanente, regolando la larghezza della colonna nel generatore di viste. Per informazioni su come modificare temporaneamente la larghezza delle colonne, consulta la sezione [Considerazioni sulla modifica temporanea della larghezza e dell’ordine delle colonne](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) in questo articolo.

* Le colonne visualizzate nelle viste incorporate hanno larghezze precedentemente definite da Workfront e codificate a livello hardware. Per modificare queste larghezze, è necessario aggiornare manualmente la larghezza di queste colonne utilizzando la modalità testo nel generatore di viste.

   Per informazioni sulla modifica della colonna in modalità testo, consulta [Visualizza: modificare in modo permanente la larghezza di una colonna](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Modificare l’accesso a Report, Dashboard e Calendari per modificare la visualizzazione in un report</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Gestire le autorizzazioni per un rapporto per modificare una visualizzazione in un rapporto</p> <p>Gestire le autorizzazioni per una visualizzazione per modificarla</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Modificare la larghezza e l’ordine delle colonne

Puoi modificare la larghezza e l’ordine delle colonne nei rapporti nei modi seguenti:

* [Modificare temporaneamente la larghezza e l&#39;ordine delle colonne](#modify-width-and-order-of-columns-temporarily)
* [Modificare in modo permanente la larghezza e l&#39;ordine delle colonne](#modify-width-and-order-of-columns-permanently)

### Modificare temporaneamente la larghezza e l&#39;ordine delle colonne {#modify-width-and-order-of-columns-temporarily}

È possibile trascinare i bordi di colonna per ridimensionare le colonne e trascinarle e rilasciarle temporaneamente per riordinarle nella maggior parte degli elenchi in tutto il sito Workfront. Sono inclusi rapporti, visualizzazioni, rapporti sulle dashboard e la visualizzazione Gantt.

Per ulteriori informazioni sugli elenchi di Workfront, consulta l’articolo [Guida introduttiva agli elenchi in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [Considerazioni sulla modifica temporanea della larghezza e dell’ordine delle colonne](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [Ridimensiona temporaneamente le colonne](#resize-columns-temporarily)
* [Riordina temporaneamente le colonne](#reorder-columns-temporarily)

#### Considerazioni sulla modifica temporanea della larghezza e dell’ordine delle colonne {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

È possibile modificare temporaneamente la larghezza e l’ordine delle colonne di un elenco senza modificarne la visualizzazione.

Quando si ridimensionano e ordinano temporaneamente le colonne, tenere presente quanto segue:

* Quando si ridimensionano le colonne, le nuove dimensioni delle colonne vengono memorizzate nell’archivio locale del browser e vengono salvate per impostazione predefinita. Se utilizzi un browser diverso o cancelli la cache o i dati di navigazione, le dimensioni delle colonne vengono ripristinate rispetto a quelle predefinite. Durante l’aggiornamento della pagina vengono mantenute le modifiche apportate alla larghezza delle colonne.
* Quando riordinate le colonne, l’ordine scelto viene mantenuto solo fino a quando non vi allontanate dall’elenco o non aggiornate la pagina del browser. Dopo aver abbandonato l’elenco o aver aggiornato la pagina del browser, le colonne vengono ripristinate nell’ordine predefinito.
* Per ottenere prestazioni ottimali, le colonne da riordinare non devono contenere più di 100 elementi nell’elenco.
* Quando si ridimensionano le colonne, le modifiche vengono applicate solo alla visualizzazione in uso e sono visibili solo all’utente. La condivisione di una visualizzazione con un altro utente non condivide le dimensioni delle colonne definite.
* Dopo aver ridimensionato una colonna trascinandone il bordo verso destra, la larghezza della colonna adiacente viene mantenuta tranne nei seguenti casi:

   * Area Configurazione
   * Area Rapporti
   * Elenchi di documenti e rapporti

   >[!NOTE]
   >
   >Non è possibile spostare il bordo sinistro di una colonna oltre il bordo sinistro della colonna adiacente in alcun elenco.

* Se si esporta un elenco in un file, l’ordine temporaneo delle colonne non viene trasferito al file esportato. Il file esportato visualizza l’ordine delle colonne nell’elenco originale, prima che le colonne siano state riordinate.

Per ulteriori informazioni sull’esportazione di dati da elenchi e rapporti, consulta l’articolo [Esportare i dati](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Ridimensiona temporaneamente le colonne {#resize-columns-temporarily}

1. Passa all’elenco da modificare.
1. Trascinare il bordo di una colonna fino a raggiungere la dimensione desiderata.\
   ![](assets/column-resize-350x124.png)

#### Riordina temporaneamente le colonne {#reorder-columns-temporarily}

1. Passa all’elenco da modificare.
1. Fare clic su una colonna da spostare in un&#39;altra posizione per scegliere la colonna.
1. Trascina la colonna nella posizione corretta.
1. Rilascia la colonna nella posizione, per spostarla.

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>Questa funzione è particolarmente utile quando si visualizzano contemporaneamente il diagramma di Gantt e la vista a elenco. Quando si visualizza il diagramma di Gantt, le colonne possono risultare nascoste. Per visualizzare una colonna mentre è visualizzato il diagramma di Gantt, è sufficiente trascinare la colonna che si desidera visualizzare in modo che venga visualizzata sul lato sinistro della pagina.

### Modificare in modo permanente la larghezza e l&#39;ordine delle colonne {#modify-width-and-order-of-columns-permanently}

Per riordinare in modo permanente le colonne, consulta la sezione [Creare o personalizzare una visualizzazione standard](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) nell&#39;articolo [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

È possibile modificare in modo permanente la larghezza di una colonna solo utilizzando la modalità testo.

Per ulteriori informazioni sull’utilizzo della modalità testo e sulla modifica permanente della larghezza di una colonna, consulta l’articolo [Panoramica degli usi comuni della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
