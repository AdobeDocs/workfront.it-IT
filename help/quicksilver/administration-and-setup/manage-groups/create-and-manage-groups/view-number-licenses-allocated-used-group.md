---
title: Visualizza il numero di licenze assegnate e utilizzate in un gruppo
description: In qualità di amministratore di Adobe Workfront, puoi visualizzare il numero dei singoli tipi di licenze attualmente utilizzati nel gruppo e nei relativi sottogruppi. Questo è utile quando devi valutare se ridistribuire le licenze.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Visualizza il numero di licenze assegnate e utilizzate in un gruppo

In qualità di amministratore di Adobe Workfront, puoi visualizzare il numero dei singoli tipi di licenze attualmente utilizzati nel gruppo e nei relativi sottogruppi. Questo è utile quando devi valutare se ridistribuire le licenze.

Se ci sono gruppi al di sopra del gruppo che gestisci, i loro amministratori possono farlo anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

>[!IMPORTANT]
>
>La licenza di un utente viene conteggiata in un determinato gruppo solo se il gruppo è il gruppo home dell&#39;utente.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">piano Workfront</a>*</td> 
   <td> <p>Team o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Licenza Adobe Workfront</a>*</td> 
   <td> <p>Piano </p> <p>È necessario essere un amministratore del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Visualizza il numero di licenze utilizzate in un gruppo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fare clic sul nome del gruppo.
1. Nella pagina visualizzata, nell’area dell’intestazione posta in prossimità dell’angolo superiore destro, viene visualizzata la **Licenze in uso** area per visualizzare il numero di **Pianificare** e **Lavoro** licenze attualmente in uso.

   Se visualizzi un gruppo di livello principale e l’amministratore di Workfront ha definito un numero massimo di ogni tipo di licenza per il gruppo, vengono visualizzati anche questi numeri. Ad esempio, nel gruppo seguente, un massimo di 10 utenti può avere una licenza Plan e un 15 può avere una licenza Work:

   ![](assets/licenses-used-allocated.png)

   Per informazioni su come un amministratore di Workfront definisce un numero massimo di licenze allocate per un gruppo, consulta la sezione . [Imposta il numero massimo di licenze per un gruppo home](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) nell&#39;articolo [Gestione delle licenze disponibili nel sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Se il gruppo che si sta esaminando è un sottogruppo, è possibile visualizzare solo il numero di licenze utilizzate e non il numero massimo di licenze assegnate per il gruppo. Questo perché gli amministratori di Workfront non definiscono un numero massimo di licenze per un sottogruppo.
   >
   >![](assets/subgroup-used-licenses-only.png)

1. Per i conteggi separati di ciascun tipo di licenza attualmente utilizzata nel gruppo (tra cui Revisione e Richiesta), fai clic sull&#39;area di testo direttamente qui sotto **Licenze in uso:**

   ![](assets/click-text-to-see-more.png)

   La casella visualizzata fornisce le stesse informazioni per tutti e quattro i tipi di licenza Workfront: Pianificare, lavorare, esaminare e richiedere. Nella parte inferiore della casella è possibile vedere il numero totale di licenze utilizzate dai membri di questo gruppo o di uno dei suoi sottogruppi:

   ![](assets/more-license-info.png)

   Per le licenze di revisione e richiesta, la colonna Max visualizza sempre Senza limiti.
