---
title: Concedere l’accesso agli utenti
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ad altri utenti in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: d1fe7165932fb6f2aff3c8488bdb8e1dfae3b6d3
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# Concedere l’accesso agli utenti

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ad altri utenti in Workfront, come spiegato in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurazione dell’accesso agli utenti

Puoi gestire le informazioni che gli utenti possono visualizzare e modificare per altri utenti utilizzando un livello di accesso predefinito o personalizzato creato. Gli utenti con le licenze di piano e lavoro predefinite possono visualizzare le informazioni di contatto di altri utenti. Uno dei seguenti utenti può creare e modificare altri utenti:

* Un amministratore Workfront.

   Per ulteriori informazioni, consulta [Concedere a un utente pieno accesso amministrativo](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* Un utente con una licenza di piano predefinita che ha accesso anche agli utenti, come spiegato in questo articolo.

   Gli utenti con restrizioni per visualizzare solo gli utenti della loro azienda o della società principale hanno accesso per modificare solo gli utenti che possono vedere. Per ulteriori informazioni, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Utente con una licenza di piano predefinita specificata anche come responsabile di un altro utente.

   Gli utenti a cui è concesso l’accesso Modifica agli utenti nel loro livello di accesso possono gestire gli utenti che inviano rapporti agli utenti. Per informazioni sulla gestione di un utente, consulta [Visualizza il grafico organizzativo](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* Un utente con una licenza di piano predefinita che ha creato un utente può disattivare, eliminare o modificare l&#39;utente creato. Per informazioni sulla creazione di nuovi utenti, consulta [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configurare l’accesso degli utenti per modificare gli utenti utilizzando un livello di accesso personalizzato

1. Inizia a creare o modificare il livello di accesso, come spiegato in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Per modificare la capacità degli utenti con una licenza Piano o Lavoro di visualizzare i profili di altri utenti:

   1. Fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sulla **Visualizza** a destra di **Utenti**.

   1. Disattiva **Visualizza informazioni contatto**, quindi fai clic sulla X per chiudere la **Ottimizzare le impostazioni** scatola.

1. Per modificare la capacità degli utenti con accesso a una licenza di piano di modificare altri utenti, fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sulla **Modifica** a destra di **Utenti**, quindi seleziona le capacità che desideri concedere:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Crea</strong> </td> 
      <td> <p>Consente agli utenti di creare utenti.<br>Questa opzione è attivata per impostazione predefinita.</p> 
      &lt;!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Assicurati che questa modifica venga apportata prima di annullare la stesura di queste 2 note. Il 29/3, il dottore del req dice che questo dipende dai risultati delle indagini.</p>

       &lt;p>&lt;b>NOTA&lt;/b>: Questa opzione non è disponibile se l’organizzazione è stata caricata in Adobe Admin Console. Per ulteriori informazioni, rivolgiti al tuo amministratore di rete o IT.&lt;/p>
       —>  &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Elimina</strong> </td> 
      <td> <p> Consente agli utenti di eliminare gli utenti che hanno creato da soli.<br>Questa opzione è attivata per impostazione predefinita.</p> <p><b>NOTA</b>: Questa opzione non è disponibile se l’organizzazione è stata caricata in Adobe Admin Console. Per ulteriori informazioni, rivolgiti al tuo amministratore di rete o IT.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Amministratore utenti (Tutti gli utenti)</strong> </td> 
      <td> <p>Consente agli utenti di effettuare le seguenti operazioni per qualsiasi utente in Workfront:</p> 
       <ul> 
        <li>Modificare, eliminare o disattivare l’utente</li> 
        <li>Accedi come utente</li> 
        <li>Reimpostare la password dell'utente</li> 
       </ul> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Amministratore utenti (Utenti gruppi)</strong> </td> 
      <td> <p>Consente agli utenti di effettuare le seguenti operazioni per qualsiasi utente di un gruppo che amministrano: 
        <ul>
         <li><p>Modificare, eliminare o disattivare l’utente</p></li>
         <li>Accedi come utente</li>
         <li><p>Reimpostare la password dell'utente</p><p><b>NOTA</b>: Un amministratore di gruppo non può accedere come o reimpostare la password di un amministratore di Workfront.</p></li>
        </ul><p>Questa opzione è disabilitata per impostazione predefinita.</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Se non desideri concedere agli amministratori dei gruppi l&#39;accesso a tutti i membri dei gruppi che amministrano, disattiva entrambe le opzioni Amministratore utenti riportate sopra. Gli amministratori di gruppo potranno comunque accedere ai membri del gruppo aggiunti a Workfront o che riferiscono a tali membri in Workfront.

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l’accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), quali [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fai clic su **Salva**.

## Accesso agli utenti per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ciascun livello di accesso possono eseguire con gli utenti, consulta la sezione . [Utenti](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) nell&#39;articolo [Funzionalità disponibile per ciascun tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
