---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Creazione o modifica dello stato di un gruppo
description: In qualità di amministratore di gruppo, puoi creare stati personalizzati per un gruppo che gestisci. Questo consente di eliminare la necessità di decine di stati personalizzati a livello di azienda e consente una maggiore autonomia nelle gerarchie di gruppo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1335'
ht-degree: 1%

---

# Creare o modificare lo stato di un gruppo

In qualità di amministratore di gruppo, puoi creare stati personalizzati per un gruppo che gestisci. Questo consente di eliminare la necessità di decine di stati personalizzati a livello di azienda e consente una maggiore autonomia nelle gerarchie di gruppo.

È inoltre possibile modificare lo stato a livello di sistema di un gruppo gestito da un amministratore di Workfront. Per ulteriori informazioni, vedere [Stati bloccati e sbloccati a livello di sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

Se ci sono gruppi al di sopra del gruppo, gli amministratori possono eseguire queste operazioni anche per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

>[!NOTE]
>
>Non è possibile visualizzare gli stati di gruppo personalizzati in un progetto quando si visualizza il progetto in una visualizzazione agile. Quando si visualizza un progetto in una visualizzazione agile, sono visibili solo gli stati bloccati predefiniti e personalizzati. Per informazioni sulla personalizzazione di una visualizzazione Agile per un progetto, vedere la sezione [Creare o personalizzare una visualizzazione Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) nell&#39;articolo [Creare o modificare le visualizzazioni in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

Per informazioni generali sugli stati, vedere [Panoramica sugli stati](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

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
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>Oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare o modificare uno stato per un gruppo

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fare clic sul nome del gruppo in cui si desidera creare o personalizzare gli stati.
1. Nel pannello a sinistra, fai clic su **Stati**.

   Se il gruppo visualizzato è un gruppo di primo livello, l&#39;elenco visualizzato include quanto segue:

   * Stati bloccati a livello di sistema.
   * Stati personalizzati già creati per il gruppo.

   Inoltre, se il gruppo visualizzato è un sottogruppo, l’elenco include anche:

   * Stati bloccati appartenenti ai gruppi sopra il sottogruppo.
   * Stati sbloccati che appartenevano ai gruppi al di sopra del sottogruppo al momento della creazione.

     Dopo la creazione di un sottogruppo, gli stati sbloccati creati nei gruppi superiori non vengono inclusi nell&#39;elenco degli stati del sottogruppo. Tuttavia, se qualcuno ne blocca uno in un secondo momento, viene incluso nell’elenco di stato del sottogruppo. Per ulteriori informazioni, vedere [Modalità di ereditarietà degli stati dei gruppi](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

1. Selezionare la scheda del tipo di oggetto (**Progetto**, **Attività** o **Problemi**) che si desidera associare allo stato.

1. (Condizionale) Se lo stato è un problema, assicurati che sia selezionato **Elenco principale**.

   ![](assets/master-list.png)

   Per informazioni sulla personalizzazione degli altri tipi di problemi (rapporto bug, ordine di modifica, problema, richiesta), vedere [Personalizzare i tipi di problemi predefiniti](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. (Condizionale) Per creare un nuovo stato, fare clic su **Aggiungi nuovo stato**.

   Oppure

   Per modificare uno stato esistente, passa il puntatore del mouse sullo stato da modificare, quindi fai clic sull&#39;opzione **Modifica** visualizzata all&#39;estrema destra.

   ![](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >Puoi modificare uno stato per il gruppo solo se:
   >      
   >* È possibile gestire il gruppo per il quale è stato creato lo stato
   >* Un amministratore di Workfront ha sbloccato lo stato a livello di sistema
   >* Lo stato è stato sbloccato da un amministratore di gruppo di un gruppo al di sopra del gruppo
   >      
   >      
   >Quando si modifica uno stato esistente, è possibile modificarne solo il nome, la descrizione e il colore.
   >
   >Quando si modifica uno stato bloccato, le modifiche hanno effetto su tutti i sottogruppi che hanno ereditato lo stato dal gruppo.
   >   
   >Al contrario, la modifica di uno stato sbloccato non influisce sui sottogruppi che hanno ereditato lo stato dal gruppo.

1. Specifica le seguenti informazioni.

   Se si modifica uno stato, è possibile modificare solo le prime 3 impostazioni.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome stato</td> 
      <td> <p>Digita un nome per lo stato. Questo è un campo obbligatorio.</p> <p>Quando crei un nome di stato, tieni presente che altri utenti nel sistema possono creare uno stato con lo stesso nome. È consigliabile utilizzare un nome univoco per evitare confusione durante la selezione degli stati in Workfront.</p><p>Se esistono stati duplicati, l’amministratore del gruppo deve aggiornare i nomi per differenziarli. L’unico indicatore di univocità nel sistema è la Chiave di stato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>(Facoltativo) Digita una descrizione dello stato. Questo comunica il suo scopo a coloro che lo usano.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Colore</td> 
      <td> <p>Personalizzate il colore dello stato facendo clic sul campo del colore e selezionando un colore dal pannello Campione. Puoi anche immettere un numero esadecimale nel campo.</p> <p>Il colore dello stato viene visualizzato nell’angolo superiore destro di Workfront quando un utente visualizza l’oggetto.</p> <p> <img src="assets/status-color.png"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Equivale a</td> 
      <td> <p>Seleziona una delle opzioni dall’elenco che descrive meglio la funzione dello stato. Ad esempio, se il nome dello stato è Fatto (Done), l'opzione corrispondente deve essere Completa.</p> <p>Ogni stato deve corrispondere a una di queste opzioni, in quanto determina il funzionamento dello stato.</p> <p>Questa opzione non può essere modificata dopo la creazione dello stato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chiave</td> 
      <td> <p>Se si sta creando un nuovo stato, digitare un codice o un'abbreviazione per lo stato oppure utilizzare quello generato automaticamente. Questa chiave deve essere univoca in Workfront perché può essere utilizzata a scopo di reporting. Se si tenta di specificare una chiave già in uso nel sistema, il campo diventa rosso.</p> <p>Potrebbe essere utile utilizzare un’abbreviazione riconoscibile da coloro che la utilizzeranno.</p> <p>Questa opzione non può essere modificata dopo la creazione dello stato.</p> <p>Non è possibile modificare il codice chiave per gli stati Pianificazione, Corrente e Completo. Questo è importante se stai creando un rapporto in modalità testo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nascondi stato</td> 
      <td> <p>(Solo stati Progetto e Attività)</p> <p>Abilita questa opzione se desideri che lo stato sia nascosto agli utenti. Quando è disattivato (impostazione predefinita), tutti i sottogruppi del gruppo possono utilizzare lo stato.</p> <p>Suggerimento: è possibile nascondere lo stato di un problema disabilitando tutti e 4 i tipi di problemi (Rapporto bug, Ordine di modifica, Problema, Richiesta).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca per tutti i gruppi</td> 
      <td> 
       <p>Se questa opzione viene lasciata attivata, gli utenti del gruppo e dei relativi sottogruppi potranno visualizzare e utilizzare lo stato e gli amministratori del gruppo non potranno personalizzarlo per i sottogruppi inferiori.</p> 
       <p>Se questa opzione è disattivata, gli amministratori dei gruppi possono personalizzare lo stato dei sottogruppi inferiori.</p> 
       <p><b>NOTA</b>: in un processo di approvazione di gruppo è possibile utilizzare sia lo stato bloccato che quello sbloccato. Se si crea un processo di approvazione di gruppo con uno stato di gruppo sbloccato, gli utenti possono allegare il processo di approvazione a qualsiasi progetto, attività o problema associato al gruppo.</p> 
       <p>Per ulteriori informazioni sugli stati di blocco, vedere <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">Stati di gruppo bloccati e sbloccati</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. Fai clic su **Salva**.

   Lo stato è ora disponibile per tutti i progetti associati al gruppo o al sottogruppo. Se l’hai bloccato, è disponibile per l’uso da parte di qualsiasi sottogruppo inferiore.

   È possibile configurare lo stato come stato predefinito per il gruppo. Per ulteriori informazioni, vedere [Utilizzare uno stato personalizzato come stato predefinito per un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Creare uno stato personalizzato per più gruppi

Se si è un amministratore di Workfront, è possibile creare uno stato personalizzato per più gruppi creando uno stato a livello di sistema, quindi nascondendolo da tutti i gruppi che non ne hanno bisogno.

Gli amministratori di gruppi o gli amministratori di Workfront possono creare uno stato personalizzato per più sottogruppi all’interno di una gerarchia di gruppi gestita creando uno stato per un gruppo di livello superiore e nascondendo tale stato da qualsiasi sottogruppo inferiore che non ne abbia bisogno.

1. Se sei un amministratore di Workfront, crea uno stato sbloccato a livello di sistema come descritto in [Crea o modifica uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
1. Nella casella in alto a destra, elimina **Stati di sistema**, inizia a digitare il nome di un gruppo in cui vuoi nascondere lo stato, quindi fai clic sul nome quando viene visualizzato.
1. Passa il puntatore del mouse sullo stato che desideri nascondere al gruppo, quindi fai clic su **Modifica** quando viene visualizzato.

   ![](assets/hover-click-edit.jpg)

1. Abilita l&#39;opzione **Nascondi stato** visualizzata.

   ![](assets/hide-group-status.png)

1. Fai clic su **Salva**.

   Lo stato è inattivo e non è più visibile a tutti gli utenti del gruppo.

1. Ripeti i passaggi da 3 a 5 per nascondere lo stato personalizzato a tutti gli altri gruppi che non ne hanno bisogno.

