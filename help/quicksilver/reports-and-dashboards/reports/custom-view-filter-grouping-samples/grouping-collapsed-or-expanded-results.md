---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Raggruppamento: indica se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo"
description: "Raggruppamento: indica se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Raggruppamento: indica se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

È possibile indicare se i risultati di un raggruppamento devono essere visualizzati compressi o espansi in un elenco o in un report utilizzando il generatore di report standard. Per impostazione predefinita, la visualizzazione di un raggruppamento viene espansa. Per informazioni sulla creazione di un raggruppamento, consulta [Creare raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* Quando regoli manualmente i raggruppamenti quando visualizzi un elenco, Adobe Workfront ricorda le preferenze manuali finché non disconnetti. Quando si effettua di nuovo l’accesso, l’elenco viene visualizzato in base a questa impostazione.
>* I risultati di un raggruppamento vengono sempre espansi dopo l’accesso da un elemento grafico.
>


È inoltre possibile indicare se un raggruppamento deve essere visualizzato espanso o compresso utilizzando la modalità testo.

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

## Indica se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo

1. Passare a un elenco di oggetti.
1. Da **Raggruppamento** menu a discesa, seleziona **Nuovo raggruppamento**.

1. Aggiungi un raggruppamento e fai clic su **Passa alla modalità testo**.

   Oppure

   Se il raggruppamento è già in modalità testo, aggiungi il seguente codice al livello di raggruppamento che desideri visualizzare compresso:

   ```
   group.0.iscollapsed=true
   ```

1. (Facoltativo) Se desideri visualizzare il raggruppamento espanso, aggiungi il seguente codice al livello di raggruppamento appropriato:

   ```
   group.0.iscollapsed=false
   ```

1. Fai clic su **Fine**, quindi **Salva raggruppamento**.
