---
product-area: projects
navigation-topic: convert-issues
title: Scollega i problemi dai relativi oggetti risolutivi
description: Quando si crea un progetto o un’attività convertendo un problema in progetto o in un’attività, è possibile mantenere il problema originale. L’amministratore di Adobe Workfront deve abilitare questa preferenza affinché tu possa disporre di questa opzione durante la conversione del problema. Per ulteriori informazioni sulla conversione dei problemi in progetti e attività, consulta Panoramica sulla conversione dei problemi in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Scollega i problemi dai relativi oggetti risolutivi

Quando si crea un progetto o un’attività convertendo un problema in progetto o in un’attività, è possibile mantenere il problema originale. L’amministratore di Adobe Workfront deve abilitare questa preferenza affinché tu possa disporre di questa opzione durante la conversione del problema.\
Per ulteriori informazioni sulla conversione dei problemi in progetti e attività, vedere [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Quando decidi di mantenere il problema convertito nel progetto o nell’attività, la sua risoluzione è associata al progetto o all’attività. Il problema diventa l’oggetto risolvibile del progetto o dell’attività. Il progetto o l&#39;attività sono gli oggetti risolutivi del problema.

Puoi anche collegare manualmente un problema a un altro. Il secondo problema diventa l’oggetto risolutivo per il primo problema, in questo caso.\
Per ulteriori informazioni sulla risoluzione di oggetti, vedere [Panoramica sulla risoluzione e la risoluzione di oggetti](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>Non è possibile modificare lo stato del problema, poiché cambia automaticamente con lo stato dell&#39;oggetto risolutivo.

È possibile scollegare la risoluzione di un problema da quella di un progetto, attività o problema rimuovendo il progetto, l’attività o il problema dal problema.

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
   <td> <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p>Visualizza accesso ad attività e progetti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni sul problema</p> <p>Visualizza autorizzazioni per l'attività o il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Scollegare un problema da un progetto, un’attività o un problema

1. Passa al problema collegato a un progetto, un’attività o un problema.
1. Fai clic sulla sezione **Dettagli problema**.
1. Vai all&#39;area **Panoramica** della sezione **Dettagli problema**.
1. Nel campo **Risolto da**, rimuovere il tipo di oggetto risolvibile.\
   Un problema può essere risolto da un progetto, un’attività o un problema.

   Questo rimuove l’oggetto di risoluzione dal problema.

1. Fai clic su **Salva** **Modifiche**.\
   Il problema non è più collegato a un progetto, un’attività o un problema e ora puoi risolverlo in modo indipendente.
