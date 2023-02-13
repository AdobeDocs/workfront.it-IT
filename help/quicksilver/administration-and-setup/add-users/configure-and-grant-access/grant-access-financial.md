---
title: Concedere l’accesso ai dati finanziari
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi definire l’accesso di un utente ai dati finanziari in Workfront attraverso il suo livello di accesso.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Concedere l’accesso ai dati finanziari

In qualità di amministratore di Adobe Workfront, puoi definire l’accesso di un utente ai seguenti elementi attraverso il livello di accesso dell’utente, come spiegato in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md):

* Informazioni finanziarie sui progetti in Workfront
* Informazioni sull&#39;allocazione delle risorse negli strumenti di pianificazione delle risorse

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

## Considerazioni per la concessione dell&#39;accesso ai dati finanziari

Quando concedi agli utenti l&#39;accesso ai dati finanziari in Workfront, considera quanto segue:

* Un utente il cui livello di accesso non consente l’accesso ai dati finanziari non può creare un rischio per un progetto. Per ulteriori informazioni, consulta [Creare e modificare i rischi relativi ai progetti](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
* È inoltre possibile utilizzare un livello di accesso per determinare quali attività di gestione delle risorse possono essere utilizzate da un utente per eseguire il budget o visualizzare l&#39;allocazione delle risorse. Per informazioni, consulta [Concedere l’accesso a Gestione risorse](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Configurare l’accesso dell’utente ai dati finanziari tramite un livello di accesso personalizzato

1. Inizia a creare o modificare il livello di accesso, come spiegato in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sulla **Visualizza** o **Modifica** pulsante a destra di Dati finanziari, quindi selezionare le capacità che si desidera concedere in **Ottimizzare le impostazioni**.

   ![](assets/financial-data-fine-tune-nwe.png)

1. (Facoltativo) In **Consenti accesso amministrativo per** selezionare le seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tassi di cambio</td> 
      <td> <p>Aggiungi nuova valuta in Workfront.</p> <p>Senza questo accesso, l’utente può solo aggiungere una valuta esistente a un progetto creato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td> <p>Visualizza tutte le spese relative agli oggetti in Workfront.</p> <p>Ciò non consente all'utente di creare nuovi tipi di spesa.</p> <p>Senza questo accesso, l'utente può solo visualizzare quanto segue:</p> 
       <ul> 
        <li>Spese relative a progetti, attività o problemi che gestiscono</li> 
        <li>Le proprie spese</li> 
        <li>Le spese dei loro subordinati</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l’accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) quali [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Al termine, fai clic su **Salva**.

   Una volta creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accesso alle informazioni finanziarie condivise

È possibile condividere informazioni finanziarie su un progetto, un&#39;attività o un problema con altri utenti concedendo loro autorizzazioni, come spiegato in [Condividere le autorizzazioni finanziarie su un oggetto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Quando condividi un oggetto con un altro utente, i diritti del destinatario sono determinati da una combinazione di due elementi:

* Autorizzazioni concesse al destinatario per l’oggetto
* Impostazioni del livello di accesso del destinatario per il tipo di oggetto

## Accesso alle informazioni finanziarie per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ciascun livello di accesso possono eseguire con le informazioni finanziarie, consulta la sezione . [Dati finanziari](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) nell&#39;articolo [Funzionalità disponibile per ciascun tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso alle informazioni finanziarie tramite l&#39;impostazione

Le informazioni seguenti sono utili per comprendere come utilizzare le impostazioni del livello di accesso per controllare l&#39;accesso degli utenti ai dati finanziari.

### Nessun accesso

Un utente senza accesso ai dati finanziari non ha accesso ai seguenti elementi:

* Sezione Finanza sotto gli oggetti Progetto e Task
* Business case
* Registri di fatturazione e di fatturazione
* Costo per ora e fatturazione per ora sulle preferenze utente

   Puoi configurarlo utilizzando l’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante Visualizza al punto 4.

* Costo per ora e fatturazione per ora in Ruoli lavoro

   Puoi configurarlo utilizzando l’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante Visualizza al punto 4.

### Visualizza accesso

Un utente con accesso Visualizza ai dati finanziari può visualizzare (non modificare) quanto segue:

* Sezione Finanza sotto gli oggetti Progetto e Task
* Business case
* Registri di fatturazione e di fatturazione
* Costo per ora e fatturazione per ora sulle preferenze utente

   Puoi configurarlo utilizzando l’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante Visualizza al punto 4.

* Costo per ora e fatturazione per ora in Ruoli lavoro

   Puoi configurarlo utilizzando l’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante Visualizza al punto 4.

### Modifica accesso

Un utente con accesso Modifica ai dati finanziari può visualizzare e modificare quanto segue:

* Sezione Finanza sotto gli oggetti Progetto e Task
* Business case
* Registri di fatturazione e di fatturazione
* Costo per ora e fatturazione per ora sulle preferenze utente

   Puoi configurarlo utilizzando l’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante Modifica nel passaggio 4 precedente.

* Costo per ora e fatturazione per ora in Ruoli lavoro

   Puoi configurarlo utilizzando l’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sul pulsante Modifica nel passaggio 4 precedente.
