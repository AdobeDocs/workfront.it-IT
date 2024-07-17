---
title: Concedere l’accesso agli utenti
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ad altri utenti in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: 3c5bcb85080a882a8b69bffcd01563a0479f98a5
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 1%

---


# Concedere l’accesso agli utenti

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l&#39;accesso di un utente ad altri utenti in Workfront, come spiegato in [Panoramica sui livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurazione dell’accesso agli utenti

È possibile gestire le informazioni che gli utenti possono visualizzare e modificare per altri utenti utilizzando un livello di accesso predefinito o personalizzato. Gli utenti con le licenze Pianificazione e Lavoro predefinite possono visualizzare le informazioni di contatto di altri utenti. Uno dei seguenti utenti può creare e modificare altri utenti:

* Un amministratore Workfront.

  Per ulteriori informazioni, vedere [Concedere a un utente l&#39;accesso amministrativo completo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* Utente con una licenza Pianificazione predefinita che ha anche accesso agli utenti, come spiegato in questo articolo.

  Gli utenti che non possono vedere solo gli utenti della propria società o della società principale hanno accesso alla modifica solo per gli utenti che possono vedere. Per ulteriori informazioni, vedere [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Utente con una licenza Pianificazione predefinita specificato anche come manager di un altro utente.

  Gli utenti che dispongono dell’accesso di modifica al loro livello di accesso possono gestire gli utenti che fanno riferimento a loro. Per informazioni sulla gestione di un utente, vedere [Visualizzare l&#39;organigramma](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* L&#39;utente con una licenza Pianificazione predefinita che ha creato un utente può disattivare, eliminare o modificare l&#39;utente creato. Per informazioni sulla creazione di nuovi utenti, vedere [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configurare l’accesso degli utenti per la modifica degli utenti utilizzando un livello di accesso personalizzato

1. Iniziare a creare o modificare il livello di accesso, come descritto in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Per modificare la capacità degli utenti con una licenza Pianificazione o Lavoro di visualizzare i profili di altri utenti:

   1. Fai clic sull&#39;icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante **Visualizza** a destra di **Utenti**.

   1. Disabilita **Visualizza info contatto**, quindi fai clic sulla X per chiudere la casella **Ottimizza le impostazioni**.

1. Per modificare la possibilità degli utenti con l&#39;accesso alla licenza Pianificazione di modificare altri utenti, fare clic sull&#39;icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante **Modifica** a destra di **Utenti**, quindi selezionare le funzionalità che si desidera concedere:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Crea</strong> </td> 
      <td> <p>Consente agli utenti di creare utenti.<br>Questa opzione è attivata per impostazione predefinita.</p> 
      &lt;!—
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Assicurati che questa modifica sia stata apportata prima di rimuovere queste 2 note. Il 29 marzo, il documento req afferma che ciò dipende dai risultati delle indagini.</p>

       &lt;p>&lt;b>NOTA&lt;/b>: questa opzione non è disponibile se l’organizzazione è stata integrata in Adobe Admin Console. Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.&lt;/p>
       —> &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Elimina</strong> </td> 
      <td> <p> Consente agli utenti di eliminare gli utenti che hanno creato personalmente.<br>Questa opzione è attivata per impostazione predefinita.</p> <p><b>NOTA</b>: questa opzione non è disponibile se l'organizzazione è stata integrata in Adobe Admin Console. Per ulteriori informazioni, rivolgersi all'amministratore di rete o IT.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Amministratore utenti (tutti gli utenti)</strong> </td> 
      <td> <p>Consente agli utenti di effettuare le seguenti operazioni per qualsiasi utente in Workfront:</p> 
       <ul> 
        <li>Modifica, elimina o disattiva l'utente</li> 
        <li>Accedi come utente</li> 
        <li>Reimposta password utente</li> 
       </ul> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Amministratore utenti (Utenti gruppi)</strong> </td> 
      <td> <p>Consente agli utenti di effettuare le seguenti operazioni per qualsiasi utente di un gruppo amministrato: 
        <ul>
         <li><p>Modifica, elimina o disattiva l'utente</p></li>
         <li>Accedi come utente</li>
         <li><p>Reimposta password utente</p><p><b>NOTA</b>: un amministratore di gruppo non può accedere come amministratore di Workfront né reimpostare la password di tale amministratore.</p></li>
        </ul><p>Questa opzione è disabilitata per impostazione predefinita.</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Se non si desidera concedere agli amministratori di gruppi l&#39;accesso a tutti i membri dei gruppi da essi amministrati, disattivare entrambe le opzioni Amministratore utenti descritte sopra. Gli amministratori di gruppi potranno comunque accedere ai membri del gruppo che aggiungono a Workfront o che fanno riferimento a loro in Workfront.

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configura l&#39;accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), ad esempio [Concedi l&#39;accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedi l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fare clic su **Salva**.

## Accesso agli utenti per tipo di licenza

Per informazioni sulle operazioni che gli utenti possono eseguire con gli utenti in ogni livello di accesso, vedere la sezione [Utenti](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) nell&#39;articolo [Funzionalità disponibile per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
