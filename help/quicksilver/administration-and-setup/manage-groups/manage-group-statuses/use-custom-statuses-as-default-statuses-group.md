---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Utilizzare uno stato personalizzato come stato predefinito per un gruppo
description: In qualità di amministratore del gruppo, puoi configurare uno stato personalizzato come stato predefinito per un gruppo o sottogruppo gestito. Questa funzione è utile quando il sistema deve assegnare automaticamente uno stato Workfront a un progetto, un'attività o un problema. Un progetto, un'attività o un problema visualizza sempre lo stato personalizzato impostato come stato predefinito, anziché visualizzare lo stato Workfront a cui corrisponde.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Utilizzare uno stato personalizzato come stato predefinito per un gruppo

In qualità di amministratore del gruppo, puoi configurare uno stato personalizzato come stato predefinito per un gruppo o sottogruppo gestito. Questa funzione è utile quando il sistema deve assegnare automaticamente uno stato Workfront a un progetto, un&#39;attività o un problema. Un progetto, un&#39;attività o un problema visualizza sempre lo stato personalizzato impostato come stato predefinito, anziché visualizzare lo stato Workfront a cui corrisponde.

Lo stato configurato può essere qualsiasi stato personalizzato creato per il gruppo, ereditato da un gruppo al di sopra del gruppo o ereditato dal livello di sistema.

Se ci sono gruppi al di sopra del gruppo che gestisci, i loro amministratori possono farlo anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

>[!INFO]
>
>**Esempio:** È possibile creare uno stato personalizzato denominato Finished e impostarlo come stato predefinito, con lo stato Workfront Complete.
>
>Quindi, per le attività impostate per passare allo stato Completato quando raggiungono il 100%, lo stato viene visualizzato come Completato anziché Completo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>È necessario essere un amministratore del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Stato del problema

Se lo stato personalizzato è uno stato di problema, tutti e quattro i tipi di problema devono essere attivati (rapporto bug, ordine di modifica, problema e richiesta). Ad esempio, nello stato del problema mostrato di seguito, lo stato Riaperto non può essere utilizzato come stato predefinito perché il tipo di problema Cambia ordine non è selezionato:

![](assets/all-4-issue-types-enabled.png)

## Impostare uno stato personalizzato come stato predefinito per un gruppo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).
1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png), quindi fai clic sul nome del gruppo in cui desideri creare o personalizzare gli stati.
1. Nel pannello a sinistra, fai clic su **Stati** ![](assets/gear-icon-settings.png).
1. Apri **Progetto**, **Attività** oppure **Problemi** a seconda del tipo di stato che si desidera impostare come stato predefinito.
1. Fai clic su **Imposta stati predefiniti** nell&#39;angolo in alto a destra.
1. Nell’area a discesa visualizzata, accanto allo stato in cui si desidera impostare lo stato predefinito, selezionare lo stato predefinito da impostare.
1. Fai clic su **Salva**.

   Lo stato è ora disponibile come stato predefinito da utilizzare con i progetti associati al gruppo.

1. Associa lo stato personalizzato al progetto in cui desideri utilizzarlo.

   È possibile associare lo stato al progetto associando il gruppo in cui lo stato risiede al progetto. Gli utenti possono utilizzare lo stato personalizzato solo se il gruppo in cui risiede lo stato è associato al progetto.

   >[!NOTE]
   >
   >Se assegni il progetto a un gruppo diverso, lo stato del progetto verrà ricaricato e potrebbe cambiare.

   1. Passa al progetto in cui desideri usare lo stato personalizzato.
   1. Fai clic sul menu Altro ![](assets/more-icon.png), quindi fai clic su **Modifica**.
   1. In **Modifica progetto** nella casella visualizzata **Gruppo** campo sotto **Associazione dei progetti**, seleziona il gruppo a cui è associato lo stato personalizzato.

   1. Fai clic su **Salva modifiche**.

## I gruppi ereditano le configurazioni di stato predefinite

Dopo che un amministratore di Workfront configura uno stato personalizzato come stato predefinito, i nuovi gruppi creati ereditano tale configurazione.

Allo stesso modo, dopo che un amministratore di gruppo imposta uno stato personalizzato come stato predefinito, i nuovi sottogruppi creati direttamente sotto il gruppo ereditano tale configurazione.

Per ulteriori informazioni, consulta [Come i gruppi ereditano gli stati](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## Quando uno stato predefinito è nascosto

Se nascondi uno stato predefinito (abilitando l&#39;opzione Nascondi stato), il sistema cerca invece di impostare come predefinito un altro stato del tipo equivalente.

Se non è disponibile uno stato del tipo equivalente, il tipo di stato viene visualizzato come **Nascosto** e non è disponibile per gli elementi di lavoro.

![](assets/when-hide-default-status-no-equivalent.png)
