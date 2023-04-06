---
title: Modificare i raggruppamenti esistenti
description: Modificare i raggruppamenti esistenti
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Modificare i raggruppamenti esistenti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is the third part of a former artcle split in 3: two how-tos and one refernece article about creating and customizing groupings)</p>
-->

Puoi personalizzare un raggruppamento esistente creato originariamente o condiviso con te. Quindi puoi salvarlo come nuovo raggruppamento.

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
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Modificare l’accesso a Report, Dashboard e Calendari per modificare un raggruppamento in un report</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Gestire le autorizzazioni per un rapporto per modificare un raggruppamento in un rapporto</p> <p>Gestire le autorizzazioni per un raggruppamento </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario creare un raggruppamento prima di modificarlo.

Per informazioni sulla creazione di un raggruppamento, consulta [Creare raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## Procedura dettagliata

1. Passare a un elenco di oggetti contenente il raggruppamento che si desidera personalizzare.
1. Fai clic sul pulsante **Raggruppamento** icona.
1. Seleziona il raggruppamento da personalizzare, quindi fai clic sul pulsante **Modifica** icona.

   ![Seleziona l’icona di modifica.](assets/customizegrouping-nwe-standard-350x291.png)

   Viene aperto il generatore di interfacce per personalizzare il raggruppamento.

1. In **Anteprima raggruppamento** sezione, fai clic su **Aggiungi raggruppamento** per definire come organizzare le informazioni nel rapporto. Di seguito viene mostrata un’anteprima dell’aspetto del raggruppamento nel rapporto.

1. Inizia a digitare il nome del campo che rappresenta la modalità di organizzazione delle informazioni nel rapporto, quindi fai clic su di esso quando viene visualizzato nell’elenco a discesa.
1. (Facoltativo e condizionale) Quando visualizzi un elenco aggiornato, seleziona **Comprimi questo raggruppamento per impostazione predefinita** se desideri che i risultati nel raggruppamento vengano visualizzati compressi anziché espansi. Questa impostazione è disabilitata per impostazione predefinita e i risultati del raggruppamento vengono sempre visualizzati nell’elenco espanso.

   Per informazioni sugli elenchi aggiornati e legacy, consulta la sezione &quot;La differenza tra elenchi aggiornati e precedenti&quot; nell’articolo [Guida introduttiva agli elenchi in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* Quando si regolano manualmente i raggruppamenti quando si visualizza un elenco, Workfront ricorda le preferenze manuali fino a quando non si disconnette. Quando si effettua di nuovo l’accesso, l’elenco viene visualizzato in base a questa impostazione.
   >* I risultati di un raggruppamento vengono sempre espansi dopo l’accesso da un elemento grafico o da un elenco legacy. In questi casi, questa impostazione viene ignorata.


1. Ripetere i passaggi 4, 5 e 6 per definire raggruppamenti aggiuntivi.\
   Puoi definire fino a tre raggruppamenti per l’organizzazione delle informazioni. Puoi organizzare ulteriormente le informazioni con un massimo di quattro raggruppamenti creando un rapporto sulla matrice. Per ulteriori informazioni sui rapporti sulle matrici, vedi [Creare un rapporto sulla matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Fai clic su **Salva come nuovo raggruppamento** per sostituire il raggruppamento corrente con le modifiche apportate.
