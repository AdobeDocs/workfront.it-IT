---
product-area: projects
navigation-topic: convert-issues
title: Collegare manualmente la risoluzione di un problema ad altri problemi, attività o progetti
description: È possibile collegare manualmente la risoluzione di un problema alla risoluzione di un progetto, un’attività o un problema senza convertire il problema. Il problema diventa uno degli oggetti risolvibili del progetto, dell'attività o del problema selezionato. In questo caso, una modifica dello stato del progetto, dell’attività o del problema determina una modifica dello stato del problema originale.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# Collegare manualmente la risoluzione di un problema ad altri problemi, attività o progetti

È possibile collegare manualmente la risoluzione di un problema alla risoluzione di un progetto, un’attività o un problema senza convertire il problema. Il problema diventa uno degli oggetti risolvibili del progetto, dell&#39;attività o del problema selezionato. In questo caso, una modifica dello stato del progetto, dell’attività o del problema determina una modifica dello stato del problema originale.

>[!TIP]
>
>Quando si associa la risoluzione di un problema alla risoluzione di un altro oggetto, non è più possibile modificare manualmente lo stato del problema originale.

Per ulteriori informazioni sulla risoluzione e la risoluzione degli oggetti, vedere [Panoramica sugli oggetti risolvibili e risolvibili](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso a Issues, Tasks, Projects</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il problema collegato a un altro problema, attività o progetto</p> <p>Visualizza o consente di accedere ad altre autorizzazioni per il problema, l'attività o il progetto aggiunto al problema esistente</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Prerequisiti

Prima di iniziare, è necessario:

* Si è verificato un problema la cui risoluzione si desidera collegare alla risoluzione di un altro problema, attività o progetto

* Hai un problema, un&#39;attività o un progetto aggiuntivo

## Associare la risoluzione di un problema alla risoluzione di un altro problema, attività o progetto

1. Passare a un problema la cui risoluzione si desidera associare alla risoluzione di un altro problema o alla risoluzione di un&#39;attività o di un progetto.
1. Fai clic su **Dettagli problema** nel pannello a sinistra, quindi espandi l&#39;area **Panoramica**.

   ![](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Fai clic sul campo **Risolto da** e seleziona uno dei seguenti tipi di oggetti di risoluzione:

   * **Progetto**
   * **Attività**
   * **Problema**

   A seconda dell’oggetto selezionato, vengono visualizzati i campi seguenti:

   * **Progetto risolutivo**
   * **Attività risolutiva**
   * **Problema risolutivo**

1. Inizia a digitare il nome di un progetto, attività o problema specifico nel campo **Progetto risolutivo**, **Attività** o **Problema**, quindi fai clic su di esso quando viene visualizzato nell&#39;elenco.

   >[!NOTE]
   >
   >Non è possibile collegare la risoluzione di un problema all&#39;attività o al progetto in cui si trova il problema. L&#39;attività o il progetto del problema non viene visualizzato nei campi Attività risolutiva o Attività risolutiva.


1. Fai clic su **Salva modifiche**.

   Il problema originale diventa l&#39;oggetto risolvibile per il progetto, l&#39;attività o il problema selezionato nei passaggi 4 e 5. Ciò significa che il problema originale viene completato quando viene completato l’oggetto di risoluzione (il progetto, l’attività o il problema a cui l’hai collegato).

   >[!NOTE]
   >
   >Un progetto, un&#39;attività o un problema può presentare più problemi come oggetti risolvibili.
