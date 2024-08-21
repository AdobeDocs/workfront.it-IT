---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Utilizzare uno stato personalizzato come stato predefinito per un gruppo
description: In qualità di amministratore di gruppo, puoi configurare uno stato personalizzato come stato predefinito per un gruppo o un sottogruppo che gestisci.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Utilizzare uno stato personalizzato come stato predefinito per un gruppo

In qualità di amministratore di gruppo, puoi configurare uno stato personalizzato come stato predefinito per un gruppo o un sottogruppo che gestisci. Questa funzione è utile quando il sistema deve assegnare automaticamente uno stato Workfront a un progetto, attività o problema. Un progetto, un&#39;attività o un problema visualizza sempre lo stato personalizzato impostato come predefinito invece dello stato Workfront a cui corrisponde.

Lo stato configurato può essere qualsiasi stato personalizzato creato per il gruppo, ereditato da un gruppo sopra il gruppo o ereditato dal livello di sistema.

Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

>[!INFO]
>
>**Esempio:** è possibile creare uno stato personalizzato denominato Finished e impostarlo come stato predefinito con lo stato Workfront Complete.
>
>Quindi, per le attività impostate per passare allo stato Completato quando raggiungono il 100%, lo stato viene visualizzato come Completato invece di Completato.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Stati problemi

Se lo stato personalizzato è uno stato Problema, tutti e quattro i tipi di problema devono essere abilitati (Rapporto bug, Ordine di modifica, Problema e Richiesta). Ad esempio, nello stato del problema mostrato di seguito, lo stato Riaperto non può essere utilizzato come stato predefinito perché il tipo di problema Ordine di modifica non è selezionato:

![](assets/all-4-issue-types-enabled.png)

## Impostazione di uno stato personalizzato come stato predefinito per un gruppo

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png), quindi fai clic sul nome del gruppo in cui desideri creare o personalizzare gli stati.
1. Nel pannello a sinistra, fai clic su **Stati** ![](assets/gear-icon-settings.png).
1. Apri la scheda **Progetto**, **Attività** o **Problemi**, a seconda del tipo di stato che desideri impostare come predefinito.
1. Fai clic su **Imposta stati predefiniti** nell&#39;angolo superiore destro.
1. Nell&#39;area a discesa visualizzata, accanto allo stato in cui si desidera impostare lo stato predefinito, selezionare lo stato predefinito che si desidera impostare.
1. Fai clic su **Salva**.

   Lo stato è ora disponibile come stato predefinito da utilizzare con i progetti associati al gruppo.

1. Associa lo stato personalizzato al progetto in cui desideri utilizzarlo.

   Associate lo stato al progetto associando al progetto il gruppo in cui si trova lo stato. Gli utenti possono utilizzare lo stato personalizzato solo se al progetto è associato il gruppo in cui si trova lo stato.

   >[!NOTE]
   >
   >Se si assegna il progetto a un gruppo diverso, lo stato del progetto verrà ricaricato e potrebbe cambiare.

   1. Vai al progetto in cui desideri utilizzare lo stato personalizzato.
   1. Fai clic sul menu Altro ![](assets/more-icon.png), quindi fai clic su **Modifica**.
   1. Nella casella **Modifica progetto** visualizzata, nel campo **Gruppo** della **Associazione progetto**, selezionare il gruppo a cui è associato lo stato personalizzato.

   1. Fai clic su **Salva modifiche**.

## I gruppi ereditano le configurazioni di stato predefinite

Dopo che un amministratore di Workfront configura uno stato personalizzato come stato predefinito, i nuovi gruppi creati ereditano tale configurazione.

Analogamente, dopo che l’amministratore di un gruppo imposta uno stato personalizzato come predefinito, i nuovi sottogruppi creati direttamente sotto il gruppo ereditano tale configurazione.

Per ulteriori informazioni, vedere [Modalità di ereditarietà degli stati dei gruppi](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## Quando uno stato predefinito è nascosto

Se si nasconde uno stato predefinito (attivando l&#39;opzione Nascondi stato), il sistema tenta di impostare un altro stato del tipo equivalente come predefinito.

Se non è disponibile alcuno stato del tipo equivalente, il tipo di stato viene visualizzato come **Nascosto** e non è disponibile per gli elementi di lavoro.

![](assets/when-hide-default-status-no-equivalent.png)
