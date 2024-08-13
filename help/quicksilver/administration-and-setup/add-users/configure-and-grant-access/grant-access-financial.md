---
title: Concedere l’accesso ai dati finanziari
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi definire l’accesso di un utente ai dati finanziari in Workfront tramite il suo livello di accesso.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 0%

---

# Concedere l’accesso ai dati finanziari

{{highlighted-preview}}

In qualità di amministratore di Adobe Workfront, puoi definire l&#39;accesso di un utente ai seguenti elementi tramite il suo livello di accesso, come spiegato in [Panoramica sui livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md):

* Informazioni finanziarie sui progetti in Workfront
* Informazioni sul budget delle risorse negli strumenti di pianificazione delle risorse

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Considerazioni per la concessione dell’accesso ai dati finanziari

Quando consenti agli utenti di accedere ai dati finanziari in Workfront, considera quanto segue:

* Un utente il cui livello di accesso non consente l’accesso ai dati finanziari non può creare un rischio per un progetto. Per ulteriori informazioni, vedere [Creare e modificare i rischi nei progetti](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
* È inoltre possibile utilizzare un livello di accesso per determinare quali attività di gestione delle risorse un utente può utilizzare per preventivare o visualizzare l&#39;allocazione delle risorse. Per informazioni, vedere [Concedere l&#39;accesso a Gestione risorse](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Configurare l’accesso degli utenti ai dati finanziari utilizzando un livello di accesso personalizzato

1. Iniziare a creare o modificare il livello di accesso, come descritto in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull&#39;icona ingranaggio ![](assets/gear-icon-settings.png) sul pulsante **Visualizza** o **Modifica** a destra di Dati finanziari, quindi seleziona le abilità che desideri concedere in **Ottimizza le impostazioni**.

   ![](assets/financial-data-fine-tune-nwe.png)

1. (Facoltativo) Nell&#39;area **Consenti accesso amministrativo per**, selezionare le opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tassi di cambio</td> 
      <td> <p>Aggiungi nuova valuta in Workfront.</p> <p>Senza questo accesso, l’utente può solo aggiungere una valuta esistente a un progetto che ha creato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td> <p>Visualizza tutte le spese sugli oggetti in Workfront.</p> <p>Ciò non consente all’utente di creare nuovi Tipi di Spesa.</p> <p>Senza questo accesso, l’utente può visualizzare solo quanto segue:</p> 
       <ul> 
        <li>Spese per progetti, attività o problemi da loro gestiti</li> 
        <li>Le proprie spese</li> 
        <li>Le spese dei loro subordinati</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l&#39;accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), ad esempio [Concedere l&#39;accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Al termine, fare clic su **Salva**.

   Dopo aver creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accesso alle informazioni finanziarie condivise

È possibile condividere informazioni finanziarie su un progetto, un&#39;attività o un problema con altri utenti concedendo loro le autorizzazioni necessarie, come spiegato in [Condividere le autorizzazioni finanziarie su un oggetto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Quando si condivide un oggetto con un altro utente, i diritti del destinatario su di esso sono determinati da una combinazione di due fattori:

* Autorizzazioni concesse al destinatario per l&#39;oggetto
* Impostazioni del livello di accesso del destinatario per il tipo di oggetto

## Accesso alle informazioni finanziarie per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ogni livello di accesso possono eseguire con le informazioni finanziarie, vedere la sezione [Dati finanziari](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) nell&#39;articolo [Funzionalità disponibile per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso alle informazioni finanziarie mediante impostazione

Le informazioni seguenti consentono di comprendere come utilizzare le impostazioni del livello di accesso per controllare l&#39;accesso degli utenti ai dati finanziari.

### Nessun accesso

Un utente che non ha accesso ai dati finanziari non ha accesso ai seguenti elementi:

* Sezione Finanza in Oggetti progetto e attività
* Business case
* Tariffe di fatturazione e record di fatturazione
* <span class="preview">Classifica schede</span>
* Costo orario e fatturazione all&#39;ora in base alle preferenze utente

  È possibile configurarlo utilizzando l&#39;icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante Visualizza nel passaggio 4 precedente.

* Costo orario e fatturazione all&#39;ora per le mansioni

  È possibile configurarlo utilizzando l&#39;icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante Visualizza nel passaggio 4 precedente.

### Visualizza accesso

Un utente con accesso di visualizzazione ai dati finanziari può visualizzare (non modificare) quanto segue:

* Sezione Finanza in Oggetti progetto e attività
* Business case
* Tariffe di fatturazione e record di fatturazione
* Costo orario e fatturazione all&#39;ora in base alle preferenze utente

  È possibile configurarlo utilizzando l&#39;icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante Visualizza nel passaggio 4 precedente.

* Costo orario e fatturazione all&#39;ora per le mansioni

  È possibile configurarlo utilizzando l&#39;icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante Visualizza nel passaggio 4 precedente.

### Modifica accesso

L’utente con accesso in modifica ai dati finanziari può visualizzare e modificare quanto segue:

* Sezione Finanza in Oggetti progetto e attività
* Business case
* Tariffe di fatturazione e record di fatturazione
* <span class="preview">Classifica schede</span>
* Costo orario e fatturazione all&#39;ora in base alle preferenze utente

  È possibile configurarlo utilizzando l&#39;icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante Modifica nel passaggio 4 precedente.

* Costo orario e fatturazione all&#39;ora per le mansioni

  È possibile configurarlo utilizzando l&#39;icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante Modifica nel passaggio 4 precedente.
