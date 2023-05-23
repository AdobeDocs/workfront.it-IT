---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: URL esterno tramite campo dati personalizzato"
description: È possibile visualizzare un collegamento a un URL personalizzato interno utilizzando un campo personalizzato calcolato denominato "URL personalizzato" in una visualizzazione attività.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# Visualizza: URL esterno tramite campo dati personalizzato

Puoi visualizzare un collegamento a un URL personalizzato interno utilizzando una **Campo personalizzato calcolato** denominato &quot;URL personalizzato&quot; in un **Visualizzazione attività**.

Questo consente di collegare rapidamente alcuni oggetti in una visualizzazione a determinate aree dell’applicazione direttamente dai rapporti.

Quando crei un campo personalizzato calcolato, devi innanzitutto creare il campo, quindi creare la visualizzazione.

Le sezioni seguenti sono un esempio di campo personalizzato calcolato per le attività. Il campo personalizzato è denominato URL personalizzato. Nella visualizzazione personalizzata vengono visualizzati il valore del campo e il **URL** campo per le attività.

Utilizzando gli stessi passaggi, è possibile creare campi personalizzati calcolati e viste personalizzate simili per tutti gli oggetti del sistema che dispongono di un modulo personalizzato.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta di modifica di una vista </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Creare il campo personalizzato calcolato &quot;URL personalizzato&quot;

Per informazioni sulla creazione di un campo personalizzato calcolato, consulta l’articolo [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Se si dispone dell&#39;accesso per creare un modulo personalizzato, è possibile creare un campo personalizzato calcolato per le attività denominato &quot;URL personalizzato&quot;. Questo campo si collega direttamente al **Panoramica** scheda secondaria all’interno della **Dettagli Attività** scheda.

1. Crea un campo personalizzato calcolato.
1. Nel campo Calcolo immettere il codice seguente:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;&#39;)

1. Sostituisci &quot;`<domain>`&quot; con il nome di dominio effettivo, senza parentesi quadre.

   il

   ```
   /overview
   ```

   parte di questo URL indirizza il collegamento al **Panoramica** nel pannello sinistro dell’attività.

1. Dopo aver creato **Campo personalizzato calcolato**, allega **Modulo personalizzato** con questo campo a diverse attività in Adobe Workfront che desideri visualizzare nella nuova visualizzazione.

## Crea la visualizzazione che visualizza i campi &quot;URL personalizzato&quot; e &quot;URL&quot; dell’attività

L&#39;attività **Visualizza** nell’esempio seguente viene visualizzato il messaggio **Campo personalizzato calcolato** denominato &quot;URL personalizzato&quot; come collegamento diretto al **Panoramica** scheda secondaria all’interno dell’attività&#x200B;**Dettagli** , nonché **URL** dell&#39;attività.

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Per personalizzare questa visualizzazione:

1. Consente di passare a un elenco di attività.
1. Espandi **Visualizza** nella parte superiore dell’elenco attività.
1. Clic **Personalizza visualizzazione**.
1. Rimuove tutte le colonne all&#39;interno della vista, ad eccezione della prima colonna.
1. Fai clic sull’intestazione della prima colonna.
1. Clic **Passa alla modalità testo** nell’angolo superiore destro dell’interfaccia.
1. Clic **Fare clic per modificare il testo**.
1. Incolla la modalità testo seguente nella colonna uno.\
   In questo esempio, la colonna &#39;column.1.&#39; visualizza il valore nel campo &quot;URL personalizzato&quot; come collegamento nel campo dell’attività **Panoramica**. &#39;Colonna.2.&#39; visualizza il valore memorizzato in **Campo URL** dell&#39;attività.
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=URL personalizzato<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString(URL personalizzato)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(URL personalizzato)<br>column.1.name=URL personalizzato<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=URL personalizzato<br>column.1.valueformat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. Clic **Salva visualizzazione**.
