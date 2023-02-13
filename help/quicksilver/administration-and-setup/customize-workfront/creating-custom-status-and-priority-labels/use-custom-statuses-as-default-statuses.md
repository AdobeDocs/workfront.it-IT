---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Usa stati personalizzati come stati predefiniti
description: Quando uno stato personalizzato viene impostato come stato predefinito, il nuovo stato predefinito viene utilizzato in tutto il sistema in vari modi. Il modo in cui viene utilizzato dipende dal fatto che sia impostato come stato predefinito a livello di sistema o come stato predefinito a livello di gruppo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# Usa stati personalizzati come stati predefiniti

Quando uno stato personalizzato viene impostato come stato predefinito, il nuovo stato predefinito viene utilizzato in tutto il sistema in vari modi. Il modo in cui viene utilizzato dipende dal fatto che sia impostato come stato predefinito a livello di sistema o come stato predefinito a livello di gruppo.

## Requisiti di accesso

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Stati personalizzati predefiniti a livello di sistema

Quando si imposta uno stato personalizzato come stato predefinito del sistema, qualsiasi nuovo gruppo creato nel sistema eredita tale stato.

I gruppi già esistenti quando si imposta il nuovo stato predefinito del sistema non lo ereditano automaticamente.

Ad esempio, supponiamo che nell’ambiente Adobe Workfront siano già stati creati due gruppi (Marketing e Vendite). È possibile creare un nuovo stato personalizzato che corrisponda a Corrente e chiamare lo stato In corso. Ora crei un nuovo gruppo chiamato Engineering. In questo scenario, il gruppo Engineering eredita il nuovo stato predefinito; i gruppi Marketing e Vendite non lo fanno.

## Stati predefiniti a livello di gruppo personalizzati

Lo stato personalizzato impostato come stato predefinito del gruppo viene utilizzato nelle seguenti circostanze:

* **Quando il sistema Workfront sceglie automaticamente uno stato, viene utilizzato lo stato predefinito del gruppo:** Lo stato personalizzato impostato come stato predefinito del gruppo viene utilizzato quando il sistema Workfront assegna automaticamente uno stato a un oggetto.

   Ad esempio, è possibile configurare un&#39;attività per passare automaticamente allo stato Completa quando la percentuale di completamento raggiunge il 100%. Se si crea uno stato personalizzato che equivale a Completa e si imposta lo stato personalizzato come stato predefinito, Workfront modifica lo stato dell&#39;attività nel nuovo stato predefinito.

   Gli stati personalizzati vengono utilizzati in questo modo solo con gli stati del gruppo associati a un&#39;attività o a un problema. Gli stati personalizzati non possono essere utilizzati in questo modo per gli stati associati a un progetto.

* La **lo stato di un progetto è determinato dal gruppo associato al progetto**: Se il gruppo associato a un determinato progetto cambia, lo stato del progetto cambia a seconda degli stati predefiniti definiti per il gruppo. Durante la modifica di un progetto, è possibile associare un gruppo a un progetto tramite il campo Gruppi .

   Se il gruppo viene modificato, lo stato del progetto cambia se per il nuovo gruppo è stato definito uno stato predefinito diverso che corrisponde allo stato corrente del progetto.

   Ad esempio, un progetto può essere associato al gruppo Marketing e lo stato del progetto è impostato su Planning. Il progetto viene modificato in modo che sia ora associato al gruppo Vendite. Il gruppo Vendite dispone di uno stato di gruppo predefinito personalizzato denominato Pensiero (e questo stato corrisponde a Planning). Poiché il gruppo sul progetto è stato modificato, lo stato del progetto ora diventa Pensiero.

Se sei un amministratore di gruppo, consulta [Impostare uno stato come stato predefinito per un gruppo](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Stato del problema

Se lo stato personalizzato è uno stato di problema, tutti e quattro i tipi di problema devono essere attivati (rapporto bug, ordine di modifica, problema e richiesta). Ad esempio, nello stato del problema mostrato di seguito, lo stato Riaperto non può essere utilizzato come stato predefinito perché il tipo di problema Cambia ordine non è selezionato:

![](assets/all-4-issue-types-enabled.png)

## Impostare uno stato personalizzato come stato predefinito

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).
1. Nel pannello a sinistra, fai clic su **Preferenze del progetto** > **Stati**.
1. (Condizionale) Se si imposta uno stato predefinito per un gruppo, inizia a digitare il nome del gruppo nel menu nell’angolo in alto a destra, quindi selezionalo quando viene visualizzato.
1. Apri **Progetto**, **Attività** oppure **Problemi** a seconda del tipo di stato che si desidera impostare come stato predefinito.
1. Fai clic sul pulsante **Imposta stati predefiniti** menu a discesa.
1. Nell’area a discesa visualizzata, accanto allo stato in cui si desidera impostare lo stato predefinito, selezionare lo stato predefinito desiderato.
1. Fai clic su **Salva**.
1. Associa il progetto al gruppo in cui si trova lo stato .

   >[!NOTE]
   >
   >Se si imposta lo stato personalizzato per un gruppo e successivamente si assegna il progetto a un gruppo diverso, lo stato del progetto verrà ricaricato e potrebbe cambiare.

   1. Passa al progetto in cui desideri usare lo stato personalizzato.
   1. Fai clic sul menu Altro ![](assets/more-icon.png), quindi fai clic su **Modifica**.
   1. In **Modifica progetto** nella casella visualizzata **Gruppo** campo sotto **Associazione dei progetti**, seleziona il gruppo in cui si trova lo stato.
   1. Fai clic su **Salva modifiche**.
