---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Raggruppamento: indicare se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo"
description: "Raggruppamento: indica se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo"
author: Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Raggruppamento: indica se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

È possibile indicare se i risultati di un raggruppamento devono essere compressi o espansi in un elenco o in un report utilizzando il generatore di report standard. Per impostazione predefinita, i risultati in un raggruppamento vengono visualizzati in modalità espansa. Per informazioni sulla creazione di un raggruppamento, vedere [Creare raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* Quando modifichi manualmente i raggruppamenti durante la visualizzazione di un elenco, Adobe Workfront ricorda la preferenza manuale fino alla disconnessione. Quando effettui di nuovo l’accesso, l’elenco viene visualizzato in base a questa impostazione.
>* I risultati di un raggruppamento vengono sempre visualizzati in modalità espansa dopo essere stati accessibili da un elemento del grafico.
>

È inoltre possibile indicare se un raggruppamento deve essere espanso o compresso utilizzando la modalità testo.

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
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
    <p>Nuovo:</p>
   <ul><li><p>Collaboratore per modificare un filtro </p></li>
   <li><p>Standard per modificare un rapporto</p></li> </ul>

<p>Corrente:</p>
   <ul><li><p>Richiesta di modifica di un filtro </p></li>
   <li><p>Pianificare la modifica di un rapporto</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Indica se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo

1. Consente di passare a un elenco di oggetti.
1. Dal menu a discesa **Raggruppamento** selezionare **Nuovo raggruppamento**.

1. Aggiungi un raggruppamento, quindi fai clic su **Passa alla modalità testo**.

   Oppure

   Se il raggruppamento è già in modalità testo, aggiungere il codice seguente al livello di raggruppamento che si desidera visualizzare compresso:

   `group.0.iscollapsed=true`

1. (Facoltativo) Se vuoi che il raggruppamento venga visualizzato in modo espanso, aggiungi il seguente codice al livello di raggruppamento appropriato:

   `group.0.iscollapsed=false`

1. Fai clic su **Fine**, quindi su **Salva raggruppamento**.
1. (facoltativo) Aggiornare il nome del raggruppamento, quindi fare clic su **Salva raggruppamento**.
