---
title: Concedere l’accesso ai documenti
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai documenti in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# Concedere l’accesso ai documenti

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai documenti, come spiegato in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Questo accesso si applica anche alle cartelle di documenti.

Per informazioni sull&#39;utilizzo dei livelli di accesso personalizzati per gestire l&#39;accesso degli utenti ad altri tipi di oggetto in Workfront, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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
   <td> <p>Devi essere un amministratore Workfront.&gt;</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare l’accesso utente ai documenti tramite un livello di accesso personalizzato

1. Inizia a creare o modificare il livello di accesso, come spiegato in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sulla **Visualizza** o **Modifica** a destra di Documenti, quindi selezionare le capacità che si desidera concedere in **Ottimizzare le impostazioni**.

   ![document_access.png](assets/document-access.png)

   Puoi consentire agli utenti di eseguire le seguenti operazioni su progetti, attività e problemi a cui hanno accesso:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Crea</td> 
      <td>Carica i documenti.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Elimina</td> 
      <td> <p>Rimuovi i documenti caricati.</p> <p>La <b>Crea</b> quando questa opzione è abilitata, l’opzione viene abilitata automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condividi</td> 
      <td>Condividere documenti con utenti specifici, ruoli e team.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condividi i documenti pubblicamente</td> 
      <td>Condividi documenti con utenti esterni (non disponi di una licenza Workfront).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condividi a livello di sistema</td> 
      <td> <p>Rendi i documenti disponibili a tutti nell’istanza di Workfront.</p> <p>Chiunque nel sistema può vedere un documento condiviso in questo modo se:</p> 
       <ul> 
        <li> <p>Puoi inviare loro un collegamento alla pagina Documenti in cui è stata caricata.</p> </li> 
        <li> <p>Lo cercano in Workfront</p> </li> 
       </ul> <p>La <b>Condividi</b> quando questa opzione è abilitata, l’opzione viene abilitata automaticamente.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Quando si configura un&#39;impostazione del livello di accesso per un determinato tipo di oggetto, tale configurazione non influisce sull&#39;accesso degli utenti agli oggetti con un livello inferiore. Ad esempio, è possibile impedire agli utenti di eliminare i progetti nel loro livello di accesso, ma ciò non impedisce loro di eliminare i documenti, che sono di livello inferiore rispetto ai progetti.Per ulteriori informazioni sulla gerarchia degli oggetti, vedere la sezione [Interdipendenza e gerarchia degli oggetti](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) nell&#39;articolo [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Facoltativo) Per limitare le autorizzazioni ereditate per i documenti da oggetti di classificazione superiore, fare clic su **Imposta restrizioni aggiuntive**, quindi seleziona **Non ereditare mai l’accesso ai documenti da progetti, attività, problemi e così via**.
1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l’accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), quali [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fai clic su **Salva**.

   Una volta creato il livello di accesso, puoi assegnarlo a un utente. Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accesso ai documenti per tipo di licenza

Per ulteriori informazioni sulle operazioni che gli utenti di ciascun livello di accesso possono eseguire con i documenti, consulta la sezione . [Documenti](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) nell&#39;articolo [Funzionalità disponibile per ciascun tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accesso ai documenti condivisi

Dopo aver caricato un documento in Workfront, puoi condividerlo con altri utenti concedendo loro autorizzazioni, come spiegato in [Condividere un documento](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

Quando condividi un oggetto con un altro utente, i diritti del destinatario sono determinati da una combinazione di due elementi:

* Autorizzazioni concesse al destinatario per l’oggetto
* Impostazioni del livello di accesso del destinatario per il tipo di oggetto
