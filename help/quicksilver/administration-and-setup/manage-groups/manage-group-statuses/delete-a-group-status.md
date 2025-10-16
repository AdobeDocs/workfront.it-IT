---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Eliminare uno stato gruppo
description: In qualità di amministratore di gruppo, puoi eliminare uno stato per un gruppo che gestisci se non è configurato come obbligatorio o bloccato a livello di sistema o per un gruppo più alto nella gerarchia.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: 1554c067afcc548c7f7abd03dbc3a49404e3c89c
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Eliminare lo stato di un gruppo

In qualità di amministratore di gruppo, puoi eliminare uno stato per un gruppo che gestisci se non è configurato come obbligatorio o bloccato a livello di sistema o per un gruppo più alto nella gerarchia.

Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

>[!NOTE]
>
>Non è possibile eliminare i seguenti elementi:
>
>* Gli stati incorporati Planning, Current e Complete. Puoi aggiornarne i nomi, modificarne i colori e bloccarli o sbloccarli, ma non è possibile eliminarli.
>* Stati in attesa di approvazione per almeno un oggetto associato al gruppo o a uno dei suoi sottogruppi.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr>
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminare lo stato di un gruppo

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi**.
1. Fare clic sul nome del gruppo di primo livello.
1. Nel pannello sinistro fai clic su **Stati**.
1. Nell&#39;elenco degli stati visualizzati, passa il cursore sullo stato che desideri eliminare, quindi fai clic su **Elimina** quando viene visualizzato all&#39;estrema destra.

   ![Elimina](assets/hover-click-delete.jpg)

1. Nella casella visualizzata, selezionare uno stato per designare uno stato sostitutivo per gli oggetti (progetti, attività, problemi e processi di approvazione) che utilizzavano lo stato che si sta eliminando.

   Sono disponibili solo gli stati che corrispondono allo stato che si sta eliminando. Ad esempio, se si elimina uno stato che equivale a Corrente, è possibile visualizzare solo gli stati che equivalgono a Corrente.

   Inoltre, gli stati visualizzati dipendono dal fatto che lo stato che si sta eliminando sia sbloccato o bloccato:

   * **Se è sbloccato**: sono disponibili stati non nascosti bloccato e bloccato.

     Oltre agli stati creati per il sottogruppo, sono inclusi gli stati ereditati dai gruppi di livello superiore e di sistema.

   * **Se è bloccato**: si verifica una delle seguenti condizioni:

      * Se sono presenti altri stati bloccati e non nascosti, sono disponibili solo quelli.
      * Se non è presente uno stato bloccato non nascosto, lo stato predefinito di Workfront è disponibile, anche se è nascosto o sbloccato.

        Per informazioni sugli stati predefiniti di Workfront, vedere [Accedere all&#39;elenco degli stati dei progetti di sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [Accedere all&#39;elenco degli stati delle attività di sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md) e le informazioni sui 4 stati dei problemi richiesti in [Accedere all&#39;elenco degli stati dei problemi di sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Fare clic su **Elimina stato**.

   Se lo stato eliminato era lo stato predefinito per quel tipo nel gruppo, lo stato di sostituzione prende il suo posto.

   Se lo stato di eliminazione è stato impostato come stato predefinito del progetto nelle preferenze del progetto, la preferenza viene impostata sullo stato di sostituzione.

## Quando un gruppo viene eliminato

Quando un gruppo viene eliminato e sostituito da un altro gruppo, tutti gli stati univoci del gruppo eliminato vengono aggiunti agli stati del gruppo sostitutivo. Per ulteriori informazioni, vedere [Stati personalizzati in un gruppo spostato o eliminato](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
