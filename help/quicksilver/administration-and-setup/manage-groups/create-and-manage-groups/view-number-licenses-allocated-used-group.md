---
title: Visualizza il numero di licenze allocate e utilizzate in un gruppo
description: In qualità di amministratore di Adobe Workfront, puoi visualizzare i conteggi dei singoli tipi di licenze attualmente utilizzati nel tuo gruppo e nei suoi sottogruppi. Questa opzione è utile quando è necessario valutare se ridistribuire le licenze.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: 0e8f8973ad4c1310b973bae4e6fe3578c05db204
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---

# Visualizza il numero di licenze allocate e utilizzate in un gruppo

In qualità di amministratore di Adobe Workfront, puoi visualizzare i conteggi dei singoli tipi di licenze attualmente utilizzati nel tuo gruppo e nei suoi sottogruppi. Questa opzione è utile quando è necessario valutare se ridistribuire le licenze.

Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

>[!IMPORTANT]
>
>La licenza di un utente viene conteggiata in un determinato gruppo solo se il gruppo è il Gruppo Predefinito dell&#39;utente.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza disponibile, contattare l&#39;amministratore di Workfront.

## Visualizza il numero di licenze utilizzate in un gruppo

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fare clic sul nome del gruppo.
1. Nella pagina visualizzata, nell&#39;area dell&#39;intestazione nell&#39;angolo superiore destro, visualizzare **Licenze in uso** per visualizzare il numero di **Piano** e **Lavoro** licenze attualmente in uso.

   Se si visualizza un gruppo di primo livello e l&#39;amministratore di Workfront ha definito un numero massimo di ogni tipo di licenza per il gruppo, vengono visualizzati anche questi numeri. Ad esempio, nel gruppo seguente, un massimo di 10 utenti può disporre di una licenza Pianificazione e un massimo di 15 può disporre di una licenza Lavoro:

   ![](assets/licenses-used-allocated.png)

   Per informazioni su come un amministratore di Workfront definisce un numero massimo di licenze allocate per un gruppo, vedere la sezione [Impostare il numero massimo di licenze per un gruppo predefinito](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) nell’articolo [Gestire le licenze disponibili nel sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Se il gruppo che si sta esaminando è un sottogruppo, è possibile visualizzare solo il numero di licenze utilizzate e non il numero massimo di licenze allocate per il gruppo. Questo perché gli amministratori di Workfront non definiscono un numero massimo di licenze per un sottogruppo.
   >
   >![](assets/subgroup-used-licenses-only.png)

1. Per conteggi separati di ciascun tipo di licenza attualmente utilizzato nel gruppo (inclusi Revisione e Richiesta), fare clic sull&#39;area di testo direttamente sottostante **Licenze in uso:**

   ![](assets/click-text-to-see-more.png)

   La casella visualizzata fornisce le stesse informazioni per tutti e quattro i tipi di licenza di Workfront: Pianificazione, Lavoro, Revisione e Richiesta. Nella parte inferiore della casella è visualizzato il numero totale di licenze utilizzate dai membri di questo gruppo o di uno dei suoi sottogruppi:

   ![](assets/more-license-info.png)

   Per le licenze Revisione e Richiesta, la colonna Max visualizza sempre Unlimited.
