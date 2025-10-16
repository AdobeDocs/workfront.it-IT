---
product-area: projects
navigation-topic: task-duration
title: Aggiornare le ore e la durata pianificate di un'attività con un tipo di durata semplice
description: Per impostazione predefinita, Adobe Workfront calcola la durata di un'attività con un tipo di durata semplice in base alla quantità di ore pianificate. Tuttavia, in alcune aree di Workfront è anche possibile modificare manualmente la quantità di ore pianificate e la durata di un'attività di durata semplice.
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 1%

---

# Aggiornare le ore e la durata pianificate di un&#39;attività con un tipo di durata semplice

Per impostazione predefinita, Adobe Workfront calcola la durata di un&#39;attività con un tipo di durata semplice in base alla quantità di ore pianificate. Tuttavia, in alcune aree di Workfront è anche possibile modificare manualmente la quantità di ore pianificate e la durata di un&#39;attività di durata semplice.

È possibile modificare le ore pianificate e la durata di un&#39;attività con un tipo di durata semplice in linea o a livello di attività nell&#39;area Assegnazioni.

Per ulteriori informazioni sulla modifica delle informazioni in linea, vedere [Elementi di modifica in linea in un elenco in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

Questo articolo descrive come aggiornare le ore e la durata pianificate per un&#39;attività con un tipo di durata semplice a livello di attività, nell&#39;area Assegnazioni.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard o superiore</p> 
   <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso ai progetti di visualizzazione o superiore</p> <p>Modifica l'accesso alle Attività</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire l’accesso all’attività </p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Aggiornare le ore e la durata pianificate di un&#39;attività con un tipo di durata semplice

>[!IMPORTANT]
>
>Dopo aver aggiornato manualmente la durata in un&#39;attività di durata semplice, Workfront non la calcola più in base alle ore pianificate.

Per modificare le ore e la durata pianificate di un&#39;attività con un tipo di durata semplice nella casella Assegnazioni avanzate:

1. In un elenco di attività fare clic sul nome dell&#39;attività per la quale si desidera modificare il tipo di durata.
1. Esegui una delle operazioni seguenti:

   * Fai clic sull&#39;icona **Altro** ![](assets/qs-more-icon-on-an-object.png) accanto al nome dell&#39;attività, fai clic su **Modifica**, quindi su **Assegnazioni**.
   * Fai clic su **Assegnato a** o sul nome delle assegnazioni nell&#39;area Assegnazioni dell&#39;intestazione dell&#39;attività, quindi fai clic su **Avanzate**.

1. Immetti un valore totale per **Ore pianificate** per tutte le assegnazioni, ad esempio 10 ore. Il numero totale di ore pianificate viene distribuito equamente tra tutte le risorse assegnate all&#39;attività.
1. (Facoltativo) Modifica manualmente le ore pianificate di ciascuna risorsa assegnata all&#39;attività. Il numero totale di ore pianificate per l&#39;attività viene aggiornato in modo da riflettere le nuove ore assegnate individualmente alle risorse.
1. Immetti un valore per l&#39;attività **Durata**, ad esempio 2 Giorni.

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Fai clic su **Salva**.
