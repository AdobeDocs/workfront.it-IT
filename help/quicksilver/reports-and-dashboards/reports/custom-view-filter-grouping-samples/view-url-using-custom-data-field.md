---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: URL esterno tramite campo dati personalizzato"'
description: Puoi visualizzare un collegamento a un URL personalizzato interno utilizzando un campo personalizzato calcolato denominato "URL personalizzato" in una visualizzazione attività.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# Visualizza: URL esterno tramite campo dati personalizzato

Puoi visualizzare un collegamento a un URL personalizzato interno utilizzando un **Campo personalizzato calcolato** denominato &quot;URL personalizzato&quot; in un **Visualizzazione attività**.

Questo consente di collegare rapidamente da alcuni oggetti in una vista a determinate aree dell&#39;applicazione direttamente dai rapporti.

Quando crei un campo personalizzato calcolato, devi prima creare il campo, quindi creare la visualizzazione.

Le sezioni seguenti sono un esempio di un campo personalizzato calcolato per le attività. Il campo personalizzato è denominato URL personalizzato. Nella visualizzazione personalizzata vengono visualizzati il valore del campo e la **URL** campo per le attività.

Utilizzando gli stessi passaggi, è possibile creare campi personalizzati calcolati e viste personalizzate simili per tutti gli oggetti del sistema che dispongono di un modulo personalizzato.

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

## Crea il campo personalizzato calcolato &quot;URL personalizzato&quot;

Per informazioni sulla creazione di un campo personalizzato calcolato, consulta l’articolo [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Se si dispone dell’accesso per creare un modulo personalizzato, è possibile creare un campo personalizzato calcolato per le attività denominate &quot;URL personalizzato&quot;. Questo campo si collega direttamente al **Panoramica** sottoscheda all’interno di **Dettagli attività** scheda .

1. Crea un campo personalizzato calcolato.
1. Nel campo Calcolo , immetti il codice seguente:

   CONCAT(&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;, ID,&quot;/overview&#39;)

1. Sostituisci &quot;`<domain>`&quot; con il nome di dominio effettivo, senza parentesi.

   il

   ```
   /overview
   ```

   parte di questo URL indirizza il collegamento al **Panoramica** nel pannello a sinistra dell’attività.

1. Dopo aver creato il **Campo personalizzato calcolato**, allega **Modulo personalizzato** con questo campo a diverse attività in Adobe Workfront che desideri visualizzare nella nuova visualizzazione.

## Crea la visualizzazione che visualizza i campi &quot;URL personalizzato&quot; e &quot;URL&quot; dell’attività

Attività **Visualizza** nell’esempio seguente viene visualizzata la variabile **Campo personalizzato calcolato** denominato &quot;URL personalizzato&quot; come collegamento diretto al **Panoramica** sottoscheda all’interno dell’attività&#x200B;**Dettagli** , nonché **URL** campo dell&#39;attività.

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Per personalizzare la visualizzazione:

1. Passare a un elenco di attività.
1. Espandi la **Visualizza** nella parte superiore dell’elenco delle attività.
1. Fai clic su **Personalizza visualizzazione**.
1. Rimuovere tutte le colonne all’interno della visualizzazione, ad eccezione della prima colonna.
1. Fai clic sull’intestazione della prima colonna.
1. Fai clic su **Passa alla modalità testo** nell’angolo superiore destro dell’interfaccia.
1. Fai clic su **Fare clic per modificare il testo**.
1. Incolla la modalità di testo sottostante in una colonna.\
   In questo esempio il valore &#39;column.1&#39;. visualizza il valore nel campo &quot;URL personalizzato&quot; come collegamento nel campo dell&#39;attività **Panoramica**. &#39;Colonna.2.&#39; visualizza il valore memorizzato in **Campo URL** del compito.
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.value.field= objCode<br>column.0.link.valueformat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.short=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=URL personalizzato<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString(URL personalizzato)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(URL personalizzato)<br>column.1.name=URL personalizzato<br>column.1.querysort=URL<br>column.1.short=false<br>column.1.stretch=0<br>column.1.valuefield=URL personalizzato<br>column.1.value.format=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.short=false<br>column.2.stretch=0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. Fai clic su **Salva visualizzazione**.
