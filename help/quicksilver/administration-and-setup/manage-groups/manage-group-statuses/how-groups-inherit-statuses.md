---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Come i gruppi ereditano gli stati
description: Quando elenchi gli stati disponibili per un gruppo, vengono visualizzati i seguenti
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Come i gruppi ereditano gli stati

Quando elenchi gli stati disponibili per un gruppo, vengono visualizzati i seguenti

* Stati personalizzati creati per il gruppo, come spiegato in [Creare o modificare uno stato di gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Gli stati ereditati dal sistema e da superiore nella gerarchia dei gruppi, come spiegato in questo articolo.

## Eredità degli stati

Il gruppo eredita gli stati quando si verifica uno dei seguenti eventi:

* Il gruppo viene creato.
* Un amministratore blocca lo stato in un gruppo di livello superiore.
* Un amministratore elimina un altro gruppo e sceglie il gruppo per sostituirlo.

La tabella seguente illustra ciascuna di queste circostanze.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Quando crei un gruppo</td> 
   <td> <p>Quando crei un nuovo gruppo, questo eredita automaticamente:</p> 
    <ul> 
     <li>Stato sbloccato nel gruppo un livello verso l’alto, se il nuovo gruppo è un sottogruppo.</li> 
    </ul> 
    <ul> 
     <li>Stati bloccati a livello di sistema .</li> 
    </ul> 
     <b>ESEMPIO:</b></span></span> 
     <p>Supponiamo che un gruppo chiamato Marketing abbia 2 sottogruppi denominati Marketing Communications e Branding .</p> 
     <p>Un amministratore di gruppo del gruppo Marketing crea un nuovo stato personalizzato denominato Discovery.</p> 
     <p>Successivamente, crei un nuovo sottogruppo sotto il gruppo Marketing e lo chiami Advertising.</p> 
     <p>Il sottogruppo eredita lo stato Discovery perché il gruppo è stato creato dopo che l'altro amministratore ha creato lo stato Discovery sbloccato.</p> 
     <p>Poiché i sottogruppi Marketing Communications e Branding esistevano già sotto il gruppo Marketing in questo caso, non ereditano lo stato di Discovery sbloccato.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando un amministratore blocca uno stato a un livello superiore</td> 
   <td> <p>Quando un amministratore di Workfront blocca uno stato a livello di sistema, il gruppo lo eredita insieme a tutti gli altri gruppi del sistema.</p> <p>Allo stesso modo, quando un amministratore blocca lo stato di un gruppo al di sopra del gruppo, il gruppo lo eredita insieme a qualsiasi altro sottogruppo al di sotto del gruppo superiore.</p> <p><b>NOTA</b>: Successivamente, se un amministratore sblocca uno di questi stati a livello di sistema o in un gruppo al di sopra del gruppo, il gruppo mantiene lo stato ereditato in precedenza. Ora si tratta di una versione separata dello stato e puoi personalizzarla solo per il tuo gruppo.</p> 
    <p><b>ESEMPIO:</b></p>
    <p>L’amministratore del gruppo di marketing blocca lo stato Discovery indicato sopra per assicurarti che sia presente in tutti e 3 i sottogruppi.</p> 
    <p>Insieme al gruppo Advertising, i gruppi Marketing Communications e Branding hanno lo stato Discovery. L'hanno ereditato quando era bloccato nel gruppo Marketing sopra di loro.</p> 
    <p>L'amministratore del gruppo di marketing sblocca quindi lo stato Discovery in modo che tutti e 3 i sottogruppi abbiano la propria versione dello stato Discovery. Ora tu e gli amministratori degli altri 2 gruppi potete personalizzare lo stato di individuazione in base alle esigenze dei gruppi.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando un amministratore elimina un gruppo</td> 
   <td> <p>Quando un amministratore elimina un gruppo e sceglie di sostituirlo nel sistema, il gruppo eredita gli stati personalizzati del gruppo eliminato se non esistono già nel gruppo.</p> 
   <p><b>ESEMPIO: </b></p>
     <p>Un gruppo denominato Messaging deve unirsi al gruppo Advertising, in modo che un amministratore Workfront elimini il gruppo Messaging e scelga il gruppo per sostituirlo.</p> 
     <p>Il gruppo di messaggistica aveva uno stato univoco denominato In processo. Questo stato è ora disponibile per l’uso nel gruppo Advertising.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Eredita delle configurazioni di stato

Quando crei un gruppo di livello principale, eredita le seguenti configurazioni dal livello di sistema. Quando crei un sottogruppo, eredita le seguenti configurazioni dal gruppo superiore successivo.

* Configurazioni di stato predefinite

   Per informazioni, consulta [Usa stati personalizzati come stati predefiniti](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Configurazioni dell&#39;ordine di visualizzazione dello stato

   Per informazioni, consulta [Riordinare gli stati a livello di sistema e di gruppo](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Se qualcuno modifica queste configurazioni dopo la creazione del gruppo, i relativi stati non vengono interessati.
