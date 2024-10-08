---
title: Reimpostare le preferenze di un utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: In qualità di amministratore di Adobe Workfront, puoi reimpostare o rimuovere le impostazioni delle preferenze utente per qualsiasi utente del sistema Workfront. I singoli utenti possono inoltre reimpostare le proprie preferenze utente.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 2%

---

# Reimpostare le preferenze di un utente

<!-- Audited: 12/2023 -->

In qualità di amministratore di Adobe Workfront, puoi reimpostare o rimuovere le impostazioni delle preferenze utente per qualsiasi utente del sistema Workfront.

I singoli utenti possono inoltre reimpostare le proprie preferenze utente.

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
   <td><p>Nuovo: Standard</p>
       <p>Oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informazioni sulle impostazioni interessate

Quando si reimpostano le preferenze utente, alcune vengono ripristinate ai valori predefiniti di sistema e altre vengono cancellate o rimosse:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preferenza</strong> </th> 
   <th><strong>Stato dopo il ripristino</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Viste</td> 
   <td> <p> Ripristino dei valori predefiniti di sistema</p> <p>Le viste esistenti non vengono eliminate. Puoi selezionarli di nuovo.</p> </td> 
  </tr> 
  <tr> 
   <td>Filtri</td> 
   <td> <p>Ripristino dei valori predefiniti di sistema</p> <p>I filtri esistenti non vengono eliminati. Puoi selezionarli di nuovo.</p> </td> 
  </tr> 
  <tr> 
   <td>Raggruppamenti</td> 
   <td> <p>Ripristino dei valori predefiniti di sistema</p> <p>I raggruppamenti esistenti non vengono eliminati. Puoi selezionarli di nuovo.</p> </td> 
  </tr> 
  <tr> 
   <td>Elenco elementi recenti</td> 
   <td>Cancellato</td> 
  </tr> 
  <tr> 
   <td>Elenco Preferiti</td> 
   <td>Non interessato</td> 
  </tr> 
  <tr> 
   <td>Preferenze utente</td> 
   <td> <p>Ripristino dei valori predefiniti di sistema</p> <p>Le notifiche e-mail vengono ripristinate ai valori predefiniti del sistema. Le notifiche predefinite sono elencate in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Notifiche evento disponibili in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Linguette Customizzate Definite Dall'Utente</td> 
   <td>Rimosso</td> 
  </tr> 
  <tr> 
   <td>Opzioni di navigazione globale definite dall'utente</td> 
   <td>Tornare alla definizione del modello di layout o all'impostazione predefinita del sistema se non è stato assegnato alcun modello di layout.</td> 
  </tr> 
 </tbody> 
</table>

## Reimposta preferenze utente

{{step-1-to-setup}}

1. Selezionare **Accedi Come**.
1. Inizia a digitare il nome dell’utente di cui desideri reimpostare le preferenze, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.
1. Seleziona **Accedi**.
1. Se per la tua organizzazione non è stato eseguito l’onboarding in Adobe Unified Experience, segui questo passaggio:

   * Nel campo URL nella parte superiore del browser Web, aggiungi `/resetUser` dopo `workfront.com`.

     >[!NOTE]
     >
     >È sensibile a maiuscole e minuscole. La U deve essere in maiuscolo e i caratteri rimanenti devono essere minuscoli. Ad esempio:
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. Se la tua organizzazione è stata integrata nell’esperienza unificata di Adobe, segui questo passaggio:

   * Nel campo URL nella parte superiore del browser Web, aggiungi `/resetUser` dopo `workfront`.

     >[!NOTE]
     >
     >È sensibile a maiuscole e minuscole. La U deve essere in maiuscolo e i caratteri rimanenti devono essere minuscoli. Ad esempio:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Premere **Invio**.
1. Per reimpostare tutte le preferenze utente, selezionare **Reimposta**.

   Oppure

   Per reimpostare solo le schede personalizzate, selezionare **Reimposta schede**.
