---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Creare o modificare uno stato di gruppo
description: In qualità di amministratore del gruppo, puoi creare stati personalizzati per un gruppo gestito. Questo aiuta a eliminare la necessità di dozzine di stati personalizzati a livello aziendale e consente una maggiore autonomia nelle gerarchie dei gruppi.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: 027d636e8256c6a12d552af736884f6f27886114
workflow-type: tm+mt
source-wordcount: '1313'
ht-degree: 1%

---

# Creare o modificare uno stato di gruppo

In qualità di amministratore del gruppo, puoi creare stati personalizzati per un gruppo gestito. Questo aiuta a eliminare la necessità di dozzine di stati personalizzati a livello aziendale e consente una maggiore autonomia nelle gerarchie dei gruppi.

È inoltre possibile modificare lo stato a livello di sistema di un gruppo gestito se lo stato è stato sbloccato da un amministratore Workfront. Per ulteriori informazioni, consulta [Stati bloccati e sbloccati a livello di sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

Se ci sono gruppi al di sopra del gruppo, i loro amministratori possono fare queste cose anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

>[!NOTE]
>
>Gli stati di gruppo personalizzati non possono essere visualizzati su un progetto quando il progetto viene visualizzato in una visualizzazione agile. Solo gli stati bloccati predefiniti e personalizzati sono visibili quando si visualizza un progetto in una visualizzazione agile. Per informazioni sulla personalizzazione di una visualizzazione agile per un progetto, consulta la sezione . [Creare o personalizzare una visualizzazione Agile](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) nell&#39;articolo [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Per informazioni generali sugli stati, consulta [Panoramica sugli stati](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

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

## Creare o modificare uno stato per un gruppo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fare clic sul nome del gruppo in cui si desidera creare o personalizzare gli stati.
1. Nel pannello a sinistra, fai clic su **Stati**.

   Se il gruppo che stai visualizzando è un gruppo di primo livello, l’elenco visualizzato include quanto segue:

   * Stati bloccati a livello di sistema.
   * Gli stati personalizzati sono già stati creati per il gruppo.

   Inoltre, se il gruppo visualizzato è un sottogruppo, l’elenco include anche:

   * Stati bloccati appartenenti ai gruppi sopra il sottogruppo.
   * Gli stati sbloccati che appartenevano ai gruppi sopra il sottogruppo al momento della creazione.

      Dopo la creazione di un sottogruppo, gli stati sbloccati creati nei gruppi sopra di esso non vengono inclusi nell’elenco di stato del sottogruppo. Tuttavia, se qualcuno blocca uno di questi successivamente, viene incluso nell’elenco di stato del sottogruppo. Per ulteriori informazioni, consulta [Come i gruppi ereditano gli stati](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).


1. Seleziona la scheda del tipo di oggetto (**Progetto**, **Attività** oppure **Problemi**) che si desidera associare allo stato.

1. (Condizionale) Se lo stato è un problema, assicurati che **Elenco principale** è selezionato.

   ![](assets/master-list.png)

   Per informazioni su come personalizzare gli altri tipi di problemi (rapporto bug, ordine di modifica, problema, richiesta), consulta [Personalizzare i tipi di problemi predefiniti](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. (Condizionale) Per creare un nuovo stato, fai clic su **Aggiungi un nuovo stato**.

   Oppure

   Per modificare uno stato esistente, passa il mouse sullo stato da modificare, quindi fai clic sul pulsante **Modifica** visualizzata all’estrema destra.

   ![](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >È possibile modificare uno stato per il gruppo solo se:
   >      
   >* Gestisci il gruppo per il quale è stato creato lo stato
   >* Un amministratore Workfront ha sbloccato lo stato a livello di sistema
   >* Lo stato è stato sbloccato da un amministratore di gruppo di un gruppo al di sopra del gruppo

   >      
   >      
   >Quando modifichi uno stato esistente, puoi modificarne solo il nome, la descrizione e il colore.
   >
   >Quando si modifica uno stato bloccato, le modifiche apportate vengono applicate a tutti i sottogruppi che hanno ereditato lo stato dal gruppo.
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
      <td> <p>Digitare un nome per lo stato. Questo è un campo obbligatorio.</p> <p>Quando crei un nome di stato, tieni presente che altri utenti del sistema possono creare uno stato con lo stesso nome. È consigliabile utilizzare un nome univoco per evitare confusione durante la selezione degli stati in Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>(Facoltativo) Immetti una descrizione dello stato. Questo comunica il suo scopo a coloro che lo utilizzano.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clr icn</td> 
      <td> <p>Per personalizzare il colore dello stato, fai clic sul campo del colore e seleziona un colore dal pannello Campione. È inoltre possibile immettere un numero esadecimale nel campo .</p> <p>Il colore di stato viene visualizzato nell’angolo superiore destro di Workfront quando un utente visualizza l’oggetto.</p> <p> <img src="assets/status-color.png"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Equivale a</td> 
      <td> <p>Selezionare dall’elenco una delle opzioni che meglio descrive la funzione dello stato. Ad esempio, se il nome dello stato è Fine, l’opzione con cui viene equiparato dovrebbe essere Completa.</p> <p>Ogni stato deve corrispondere a una di queste opzioni, in quanto determina il funzionamento dello stato.</p> <p>Questa opzione non può essere modificata dopo la creazione dello stato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chiave</td> 
      <td> <p>Se si sta creando un nuovo stato, digitare un codice o un'abbreviazione per lo stato o utilizzare quello generato per te. Questa chiave deve essere univoca in Workfront perché può essere utilizzata a scopo di reporting. Se si tenta di specificare una chiave già in uso nel sistema, il campo diventa rosso.</p> <p>Potrebbe essere utile utilizzare un’abbreviazione riconoscibile da chi la utilizzerà.</p> <p>Questa opzione non può essere modificata dopo la creazione dello stato.</p> <p>Non è possibile modificare il codice chiave per gli stati Planning, Current e Complete. Questo è importante se si crea un rapporto in modalità testo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nascondi stato</td> 
      <td> <p>(Solo stati progetto e attività)</p> <p>Abilita questa opzione se desideri che lo stato sia nascosto agli utenti. Quando è disattivato (impostazione predefinita), tutti i sottogruppi al di sotto del gruppo possono usare lo stato .</p> <p>Suggerimento: Puoi nascondere lo stato di un problema disattivando tutti e 4 i tipi di problema (Segnalazione bug, Modifica ordine, Problema, Richiesta).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca per tutti i gruppi</td> 
      <td> 
       <p>Se si lascia abilitata questa opzione, gli utenti del gruppo e dei relativi sottogruppi possono visualizzare e utilizzare lo stato e gli amministratori del gruppo non possono personalizzarlo per i sottogruppi minori.</p> 
       <p>Quando questa opzione è disabilitata, gli amministratori di gruppo possono personalizzare lo stato dei sottogruppi inferiori.</p> 
       <p><b>NOTA</b>: È possibile utilizzare sia lo stato bloccato che quello sbloccato in un processo di approvazione del gruppo. Se si crea un processo di approvazione del gruppo con uno stato di gruppo sbloccato, gli utenti possono allegare il processo di approvazione a qualsiasi progetto, attività o problema associato al gruppo.</p> 
       <p>Per ulteriori informazioni sul blocco degli stati, consulta <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">Stati del gruppo bloccati e sbloccati</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. Fai clic su **Salva**.

   Lo stato è ora disponibile per tutti i progetti associati al gruppo o al sottogruppo. Se l’hai bloccato, è disponibile per l’uso da parte di qualsiasi sottogruppo inferiore.

   È possibile configurare lo stato come stato predefinito per il gruppo. Per ulteriori informazioni, consulta [Utilizzare uno stato personalizzato come stato predefinito per un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Creare uno stato personalizzato per più gruppi

Se sei un amministratore di Workfront, puoi creare uno stato personalizzato per più gruppi creando uno stato a livello di sistema e quindi nascondendolo da qualsiasi gruppo che non ne abbia bisogno.

Se sei un amministratore di gruppo (o un amministratore Workfront), puoi creare uno stato personalizzato per più sottogruppi all’interno di una gerarchia di gruppi gestita creando uno stato per un gruppo di livello superiore e quindi nascondendolo da qualsiasi sottogruppo inferiore che non ne abbia bisogno.

1. Se sei un amministratore di Workfront, crea uno stato sbloccato a livello di sistema come descritto in [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
1. Nella casella nell&#39;angolo in alto a destra, elimina **Stati del sistema**, inizia a digitare il nome di un gruppo in cui desideri nascondere lo stato, quindi fai clic sul nome quando viene visualizzato.
1. Passa il puntatore del mouse sullo stato da nascondere al gruppo, quindi fai clic su **Modifica** quando appare.

   ![](assets/hover-click-edit.jpg)

1. Abilita la **Nascondi stato** che viene visualizzata.

   ![](assets/hide-group-status.png)

1. Fai clic su **Salva**.

   Lo stato è oscurato e non è più visibile a tutti gli utenti di quel gruppo.

1. Ripeti i passaggi da 3 a 5 per nascondere lo stato personalizzato a qualsiasi altro gruppo che non ne abbia bisogno.
