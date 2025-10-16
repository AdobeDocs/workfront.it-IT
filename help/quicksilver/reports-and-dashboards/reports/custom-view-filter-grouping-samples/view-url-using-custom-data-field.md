---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizza: URL esterno tramite campo dati personalizzato'
description: È possibile visualizzare un collegamento a un URL personalizzato interno utilizzando un campo personalizzato calcolato denominato "URL personalizzato" in una visualizzazione attività.
author: Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Visualizza: URL esterno tramite campo dati personalizzato

<!--Audited: 11/2024-->

È possibile visualizzare un collegamento a un URL personalizzato interno utilizzando un **campo personalizzato calcolato** denominato &quot;URL personalizzato&quot; in una **visualizzazione attività**.

Questo consente di collegare rapidamente alcuni oggetti in una visualizzazione a determinate aree dell’applicazione direttamente dai rapporti.

Quando crei un campo personalizzato calcolato, devi innanzitutto creare il campo, quindi creare la visualizzazione.

Le sezioni seguenti sono un esempio di campo personalizzato calcolato per le attività. Il campo personalizzato è denominato URL personalizzato. Nella visualizzazione personalizzata vengono visualizzati il valore del campo e il campo **URL** per le attività.

Utilizzando gli stessi passaggi, è possibile creare campi personalizzati calcolati e viste personalizzate simili per tutti gli oggetti del sistema che dispongono di un modulo personalizzato.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di una visualizzazione </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Creare il campo personalizzato calcolato &quot;URL personalizzato&quot;

Per informazioni sulla creazione di un campo personalizzato calcolato, vedere [Aggiungere campi calcolati a un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Se si dispone dell&#39;accesso per creare un modulo personalizzato, è possibile creare un campo personalizzato calcolato per le attività denominato &quot;URL personalizzato&quot;. Questo campo è collegato direttamente alla scheda secondaria **Panoramica** nella scheda **Dettagli attività**.

1. Crea un campo personalizzato calcolato.
1. Nel campo Calcolo immettere il codice seguente:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;)

1. Sostituisci &quot;`<domain>`&quot; con il nome di dominio effettivo, senza parentesi. La parte `/overview` di questo URL indirizza il collegamento alla sezione **Panoramica** nel pannello sinistro dell&#39;attività.

1. Dopo aver creato il **campo personalizzato calcolato**, allega il **modulo personalizzato** con questo campo a diverse attività in Adobe Workfront che desideri visualizzare nella nuova visualizzazione.

## Crea la visualizzazione che visualizza i campi &quot;URL personalizzato&quot; e &quot;URL&quot; dell’attività

L&#39;attività **Visualizza** nell&#39;esempio seguente visualizza il campo personalizzato **Calcolato** denominato &quot;URL personalizzato&quot; come collegamento diretto alla scheda secondaria **Panoramica** all&#39;interno della scheda attività&#x200B;**Dettagli** e al campo **URL** dell&#39;attività.

(assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Per personalizzare questa visualizzazione:

1. Consente di passare a un elenco di attività.
1. Espandi il menu a discesa **Visualizza** nella parte superiore dell&#39;elenco delle attività.
1. Fare clic su **Personalizza visualizzazione**.
1. Rimuove tutte le colonne all&#39;interno della vista, ad eccezione della prima colonna.
1. Fai clic sull’intestazione della prima colonna.
1. Fare clic su **Passa a modalità testo** > **Modifica modalità testo**.
1. Rimuovere il testo nella casella **Modifica modalità testo** e sostituirlo con il seguente codice:


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat= int
   column.0.link.lookup=link.view
   column.0.link.valuefield= objCode
   column.0.link.valueformat= val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.description=Custom URL
   column.1.link.isnewwindow=true
   column.1.link.url=customDataLabelsAsString(Custom URL)
   column.1.linkedname=direct
   column.1.listsort=customDataLabelsAsString(Custom URL)
   column.1.name=Custom URL
   column.1.querysort=URL
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=Custom URL
   column.1.valueformat=customDataLabelsAsString
   column.1.width=150
   column.2.descriptionkey=url
   column.2.linkedname=direct
   column.2.listsort=string(URL)
   column.2.namekey=url.abbr
   column.2.querysort=URL
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=URL
   column.2.valueformat=HTML
   column.2.width=150
   ```

   In questo esempio, la colonna &#39;column.1.&#39; Le righe visualizzano il valore nel campo &quot;URL personalizzato&quot; come collegamento nella sezione **Panoramica** dell&#39;attività; &quot;colonna.2.&quot; visualizza il valore archiviato nel **campo URL** dell&#39;attività.

1. Fai clic su **Fine** > **Salva visualizzazione**.
