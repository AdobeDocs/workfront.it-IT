---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Riordina stati gruppo
description: In qualità di amministratore di gruppo, puoi modificare l’ordine degli stati di progetto, attività e problema per un gruppo che gestisci.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 6%

---

# Riordina stati gruppo

In qualità di amministratore di gruppo, puoi modificare l’ordine degli stati di progetto, attività e problema per un gruppo che gestisci.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

>[!NOTE]
>
>* Un amministratore Workfront può riordinare gli stati a livello di sistema. Ciò non influisce sull’ordine degli stati all’interno dei gruppi.
>
>  Tuttavia, gli stati all’interno di un gruppo di primo livello appena creato ereditano l’ordine degli stati a livello di sistema. (Un nuovo sottogruppo eredita l’ordine degli stati nel gruppo di un livello superiore).
>
>* È possibile riordinare gli stati bloccati. Per informazioni sugli stati bloccati, vedere [Creare o modificare lo stato di un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront* </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Ordine predefinito degli stati

Per impostazione predefinita, gli stati vengono visualizzati nell&#39;ordine seguente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">Progetto</th> 
   <th width="33.33%">Attività</th> 
   <th width="33.33%">Problema</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
     <p>Attuali</p> 
     <p>Morto</p> 
     <p> In sospeso </p> 
     <p> In Pianificazione </p> 
     <p> Completato </p> 
     <p> Richiesto il </p> 
     <p> Approvato </p> 
     <p> Rifiutato </p> 
     <p> Idea </p> 
   </td> 
   <td> 
     <p>Nuovo</p> 
     <p>In corso</p> 
     <p>Completato</p> 
   </td> 
   <td> 
     <p>Nuovo</p> 
     <p>In corso</p> 
     <p>Ri-Aperto</p> 
     <p>In attesa di Riscontro</p> 
     <p>In sospeso</p> 
     <p>Non Duplicabile</p> 
     <p>Chiuso</p> 
     <p>Risolto</p> 
     <p>Verifica Completata</p> 
     <p>Non Risolvibile</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## Riordina gli stati per le attività e i progetti in un gruppo che gestisci

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi**, quindi sul nome del gruppo.
1. Nel pannello a sinistra, fai clic su **Stati**.
1. Sopra l&#39;elenco Stati visualizzato, fare clic sulla scheda **Progetti** o **Attività**.

1. Trascina e rilascia gli stati nell’ordine desiderato.

   Il nuovo ordine di stato viene salvato automaticamente.

1. Per verificare il nuovo ordine di stato, accedi a un&#39;attività o a un progetto associato al gruppo, fai clic sullo stato nell&#39;angolo in alto a destra e accertati che gli stati visualizzati siano nell&#39;ordine configurato.

## Riordina gli stati per i problemi

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi**, quindi sul nome del gruppo.
1. Nel pannello a sinistra, fai clic su **Stati**.
1. Fai clic sulla scheda **Issues**.
1. (Facoltativo) Seleziona un tipo di problema (**Segnalazione bug**, **Ordine di modifica**, **Problema** o **Richiesta**).

   >[!NOTE]
   >
   >* Non è possibile personalizzare l&#39;ordine degli stati per l&#39;elenco principale.
   >* È consigliabile ordinare allo stesso modo gli stati per ogni tipo di problema. Per ulteriori informazioni sui tipi di problema, vedere [Configurare i tipi di richiesta](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Trascina e rilascia gli stati nell’ordine desiderato.

   Il nuovo ordine di stato viene salvato automaticamente.

1. Per verificare il nuovo ordine di stato, accedi a un problema associato al gruppo, fai clic sullo stato nell’angolo in alto a destra e assicurati che gli stati visualizzati siano nell’ordine configurato.
