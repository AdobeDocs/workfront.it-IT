---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Raggruppamento: indica se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo"
description: "Raggruppamento: indica se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Raggruppamento: indica se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo

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
   <td> <p>Richiesta di modifica di un raggruppamento </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modifica l'accesso a Filtri, Viste, Raggruppamenti per modificare un raggruppamento</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Indica se i risultati di un raggruppamento devono essere compressi o espansi utilizzando la modalità testo

1. Consente di passare a un elenco di oggetti.
1. Dal menu a discesa **Raggruppamento** selezionare **Nuovo raggruppamento**.

1. Aggiungere un raggruppamento e fare clic su **Passa alla modalità testo**.

   Oppure

   Se il raggruppamento è già in modalità testo, aggiungere il codice seguente al livello di raggruppamento che si desidera visualizzare compresso:

   ```
   group.0.iscollapsed=true
   ```

1. (Facoltativo) Se vuoi che il raggruppamento venga visualizzato in modo espanso, aggiungi il seguente codice al livello di raggruppamento appropriato:

   ```
   group.0.iscollapsed=false
   ```

1. Fai clic su **Fine**, quindi su **Salva raggruppamento**.
