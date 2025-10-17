---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Ereditarietà degli stati dei gruppi
description: Quando si elencano gli stati disponibili per un gruppo, vengono visualizzati i seguenti elementi
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# Ereditarietà degli stati da parte dei gruppi

Quando si elencano gli stati disponibili per un gruppo, vengono visualizzati i seguenti elementi

* Stati personalizzati creati per il gruppo, come spiegato in [Creare o modificare lo stato di un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Gli stati ereditati dal sistema e dall’alto nella gerarchia dei gruppi, come spiegato in questo articolo.

## Ereditarietà degli stati

Il gruppo eredita gli stati quando si verifica una delle seguenti situazioni:

* Create il gruppo.
* Un amministratore blocca uno stato in un gruppo di livello superiore.
* Un amministratore elimina un altro gruppo e sceglie il tuo gruppo per sostituirlo.

La tabella seguente illustra ciascuna di queste circostanze.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Quando si crea un gruppo</td> 
   <td> <p>Quando si crea un nuovo gruppo, questo eredita automaticamente:</p> 
    <ul> 
     <li>Gli stati sbloccati nel gruppo di livello superiore, se il nuovo gruppo è un sottogruppo.</li> 
    </ul> 
    <ul> 
     <li>Stati bloccati a livello di sistema.</li> 
    </ul> 
     <b>ESEMPIO:</b></span></span> 
     <p>Supponiamo che un gruppo denominato Marketing abbia 2 sottogruppi denominati Marketing Communications and Branding.</p> 
     <p>Un amministratore di gruppo del gruppo Marketing crea un nuovo stato personalizzato denominato Individuazione.</p> 
     <p>In seguito, crei un nuovo sottogruppo sotto il gruppo Marketing e lo chiami Advertising.</p> 
     <p>Il sottogruppo eredita lo stato di individuazione perché il gruppo è stato creato dopo che l'altro amministratore ha creato lo stato di individuazione sbloccato.</p> 
     <p>Poiché i sottogruppi Marketing Communications and Branding esistevano già al di sotto del gruppo Marketing, non ereditano lo stato Discovery sbloccato.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando un amministratore blocca uno stato a un livello superiore</td> 
   <td> <p>Quando un amministratore di Workfront blocca uno stato a livello di sistema, il gruppo lo eredita insieme a tutti gli altri gruppi del sistema.</p> <p>Analogamente, quando un amministratore blocca uno stato per un gruppo al di sopra del gruppo, il gruppo lo eredita insieme a tutti gli altri sottogruppi al di sotto del gruppo più alto.</p> <p><b>NOTA</b>: in seguito, se un amministratore sblocca uno di questi stati a livello di sistema o in un gruppo al di sopra del gruppo, il gruppo mantiene lo stato ereditato in precedenza. Ora si tratta di una versione separata dello stato e puoi personalizzarlo solo per il tuo gruppo.</p> 
    <p><b>ESEMPIO:</b></p>
    <p>L’amministratore del gruppo di marketing blocca lo stato di individuazione menzionato sopra per accertarsi che sia presente in tutti e 3 i sottogruppi.</p> 
    <p>Oltre al gruppo Advertising, ora anche i gruppi Marketing Communications e Branding hanno lo stato Discovery. L’hanno ereditata quando era bloccata nel gruppo Marketing al di sopra di loro.</p> 
    <p>L’amministratore del gruppo di marketing sblocca quindi lo stato di individuazione in modo che tutti e 3 i sottogruppi dispongano di una propria versione dello stato di individuazione. Ora tu e gli amministratori degli altri 2 gruppi potete personalizzare lo stato di individuazione in base alle esigenze dei vostri gruppi.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando un amministratore elimina un gruppo</td> 
   <td> <p>Quando un amministratore elimina un gruppo e sceglie il tuo per sostituirlo nel sistema, il tuo gruppo eredita gli stati personalizzati del gruppo eliminato, se non esistono già nel tuo gruppo.</p> 
   <p><b>ESEMPIO: </b></p>
     <p>Un gruppo denominato Messaggistica deve essere unito al gruppo Advertising, pertanto un amministratore Workfront elimina il gruppo Messaggistica e sceglie il gruppo in sostituzione.</p> 
     <p>Il gruppo Messaggistica aveva uno stato univoco denominato In elaborazione. Il tuo gruppo Advertising ora dispone di tale stato per l’utilizzo.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Ereditarietà delle configurazioni di stato

Quando crei un gruppo di primo livello, questo eredita le seguenti configurazioni dal livello di sistema. Quando crei un sottogruppo, questo eredita le seguenti configurazioni dal gruppo immediatamente superiore.

* Configurazioni di stato predefinite

  Per informazioni su questi stati, vedere [Utilizzare stati personalizzati come stati predefiniti](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Stato: configurazioni ordine di visualizzazione

  Per informazioni su queste, vedere [Riordinare gli stati a livello di sistema e di gruppo](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Se qualcuno modifica queste configurazioni dopo la creazione del gruppo, il suo stato non viene modificato.
