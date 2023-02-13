---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Visualizzare tutti gli aggiornamenti in un rapporto Nota
description: Visualizzare tutti gli aggiornamenti in un rapporto Nota
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Visualizzare tutti gli aggiornamenti in un rapporto Nota

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

L’area Aggiornamenti di un oggetto visualizza per impostazione predefinita un numero massimo di 200 aggiornamenti. Per visualizzare tutti gli aggiornamenti immessi da uno degli utenti per un oggetto, è possibile creare un rapporto Nota che visualizzi tutti gli aggiornamenti.

>[!NOTE]
>
>È possibile creare un rapporto per visualizzare gli aggiornamenti sugli oggetti in Anteprima con il rapporto di immissione sul giornale. Per ulteriori informazioni, consulta [Rapporto sull’area Aggiornamenti](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Modifica accesso a:</p> 
    <ul> 
     <li> <p>Creare rapporti, dashboard e calendari</p> </li> 
     <li> <p>Creare filtri, visualizzazioni e gruppi</p> </li> 
    </ul> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso.<br>Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Visualizza</p> <p>Nota: Se non si dispone dell'autorizzazione Visualizza o superiore per un oggetto, le informazioni relative a tale oggetto non vengono visualizzate nel rapporto.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare un rapporto sulle note

La creazione di un rapporto per Note per qualsiasi oggetto è identica, indipendentemente dall&#39;oggetto.

Ad esempio, per creare un rapporto Nota per tutte le note di un progetto:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**, quindi scegli **Nota**.

1. (Facoltativo) Fai clic su **Viste**, quindi **Aggiungi colonna** per aggiungere **Nome** del **Progetto** nella vista del rapporto. 

1. (Facoltativo) Fai clic su **Raggruppamenti**, quindi **Aggiungi raggruppamento** per raggruppare **Nome progetto**, se esegui il reporting per più progetti contemporaneamente.\
   In questo modo le note vengono raggruppate in base ai rispettivi progetti, facilitando la lettura del rapporto. 

1. (Facoltativo) Fai clic su **Filtri,** then **Aggiungere una regola filtro** per filtrare un solo progetto o progetti specifici.

1. (Condizionale e opzionale) Imposta il **Nome progetto** come **Uguale** al nome del progetto per il quale desideri visualizzare gli aggiornamenti.  

1. Fai clic su **Salva e chiudi**.\
   Tutti gli aggiornamenti immessi sul progetto da tutti gli utenti con autorizzazioni per almeno visualizzare il progetto vengono visualizzati nel rapporto.
