---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Raggruppamento: indicare se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo'
description: 'Raggruppamento: indicare se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo'
author: Courtney
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 22%

---

# Raggruppamento: indicare se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo

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
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
