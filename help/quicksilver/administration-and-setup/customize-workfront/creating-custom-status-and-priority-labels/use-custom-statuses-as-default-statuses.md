---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Usa stati personalizzati come stati predefiniti
description: Quando uno stato personalizzato viene impostato come predefinito, il nuovo stato predefinito viene utilizzato in tutto il sistema in vari modi. Il modo in cui viene utilizzato dipende dal fatto che sia impostato come stato predefinito a livello di sistema o di gruppo.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# Usa stati personalizzati come stati predefiniti

Quando uno stato personalizzato viene impostato come predefinito, il nuovo stato predefinito viene utilizzato in tutto il sistema in vari modi. Il modo in cui viene utilizzato dipende dal fatto che sia impostato come stato predefinito a livello di sistema o di gruppo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
     <p>Nuovo: Standard</p>
     <p>oppure</p>
     <p>Corrente: Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Stati personalizzati predefiniti a livello di sistema

Quando impostate uno stato personalizzato come stato predefinito del sistema, tutti i nuovi gruppi creati nel sistema ereditano tale stato.

I gruppi già esistenti quando si imposta il nuovo stato predefinito del sistema non lo ereditano automaticamente.

Ad esempio, supponiamo che nel tuo ambiente Adobe Workfront siano già presenti due gruppi (Marketing e Vendite). Crea un nuovo stato personalizzato che sia uguale a Corrente e richiama lo stato In elaborazione. Ora crei un nuovo gruppo denominato Engineering. In questo caso, il gruppo di progettazione eredita il nuovo stato predefinito, mentre i gruppi di marketing e vendite no.

## Stati predefiniti personalizzati a livello di gruppo

Lo stato personalizzato impostato come stato predefinito del gruppo viene utilizzato nelle seguenti circostanze:

* **Quando il sistema Workfront sceglie automaticamente uno stato, viene utilizzato lo stato predefinito del gruppo:** Lo stato personalizzato impostato come stato predefinito del gruppo viene utilizzato quando il sistema Workfront assegna automaticamente uno stato a un oggetto.

  Ad esempio, è possibile configurare un&#39;attività affinché passi automaticamente allo stato Completato quando la percentuale di completamento raggiunge il 100%. Se si crea uno stato personalizzato che equivale a Completo e lo si imposta come stato predefinito, Workfront modifica lo stato dell&#39;attività al nuovo stato predefinito.

  Gli stati personalizzati vengono utilizzati in questo modo solo con gli stati dei gruppi associati a un’attività o a un problema. Gli stati personalizzati non possono essere utilizzati in questo modo per gli stati associati a un progetto.

* Lo stato **di un progetto è determinato dal gruppo associato al progetto**: se il gruppo associato a un determinato progetto cambia, lo stato del progetto cambia a seconda degli stati predefiniti definiti per il gruppo. (Un gruppo può essere associato a un progetto tramite il campo Gruppi quando si modifica il progetto).

  Se tale gruppo cambia, lo stato del progetto cambia se per il nuovo gruppo è stato definito uno stato predefinito diverso che corrisponde allo stato corrente del progetto.

  Ad esempio, un progetto può essere associato al gruppo Marketing e lo stato del progetto è impostato su Planning. Il progetto viene modificato in modo che sia ora associato al gruppo Vendite. Il gruppo Vendite dispone di uno stato predefinito personalizzato denominato Pensiero (e questo stato equivale a Pianificazione). Poiché il Gruppo del progetto è stato modificato, lo stato del progetto ora cambia in Pensiero.

Se sei un amministratore di gruppo, vedi [Impostare uno stato come predefinito per un gruppo](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Stati problemi

Se lo stato personalizzato è uno stato Problema, tutti e quattro i tipi di problema devono essere abilitati (Rapporto bug, Ordine di modifica, Problema e Richiesta). Ad esempio, nello stato del problema mostrato di seguito, lo stato Riaperto non può essere utilizzato come stato predefinito perché il tipo di problema Ordine di modifica non è selezionato:

![](assets/all-4-issue-types-enabled.png)

## Impostare uno stato personalizzato come predefinito

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Preferenze progetto** > **Stati**.
1. (Condizionale) Se si imposta uno stato predefinito per un gruppo, iniziare a digitare il nome del gruppo nel menu nell&#39;angolo superiore destro, quindi selezionarlo quando viene visualizzato.
1. Apri la scheda **Progetto**, **Attività** o **Problemi**, a seconda del tipo di stato che desideri impostare come predefinito.
1. Fare clic sul menu a discesa **Imposta stati predefiniti**.
1. Selezionare lo stato predefinito desiderato nell&#39;area a discesa visualizzata accanto allo stato in cui si desidera impostare lo stato predefinito.
1. Fai clic su **Salva**.
1. Associa il progetto al gruppo in cui si trova lo stato.

   >[!NOTE]
   >
   >Se si imposta lo stato personalizzato di un gruppo e successivamente si assegna il progetto a un gruppo diverso, lo stato del progetto verrà ricaricato e potrebbe cambiare.

   1. Vai al progetto in cui desideri utilizzare lo stato personalizzato.
   1. Fai clic sul menu Altro ![](assets/more-icon.png), quindi fai clic su **Modifica**.
   1. Nella casella **Modifica progetto** visualizzata, nel campo **Gruppo** della **Associazione progetto**, selezionare il gruppo in cui si trova lo stato.
   1. Fai clic su **Salva modifiche**.
