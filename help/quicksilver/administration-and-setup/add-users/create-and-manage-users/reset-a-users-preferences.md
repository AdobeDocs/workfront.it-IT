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
source-git-commit: ae063189eebb17a3341aabb978ee0f0e03d1e299
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 2%

---

# Reimpostare le preferenze di un utente

<!-- Audited: 12/2023 -->

In qualità di amministratore di Adobe Workfront, puoi reimpostare o rimuovere le impostazioni delle preferenze utente per qualsiasi utente del sistema Workfront.

I singoli utenti possono inoltre reimpostare le proprie preferenze utente.

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
   <td><p>Nuovo: Standard</p>
       <p>oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>Ripristino dei valori predefiniti di sistema</p> <p>Le notifiche e-mail vengono ripristinate ai valori predefiniti del sistema.</p> </td> 
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

1. Seleziona **Accedi come**.
1. Inizia a digitare il nome dell’utente di cui desideri reimpostare le preferenze, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.
1. Seleziona  **Accedi**.
1. Nel campo URL nella parte superiore del browser web, aggiungi `/resetUser` dopo `workfront.com`.

   >[!NOTE]
   >
   >È sensibile a maiuscole e minuscole. La U deve essere in maiuscolo e i caratteri rimanenti devono essere minuscoli. Ad esempio:
   >
   >`https://company_domain.my.workfront.com/resetUser`

1. Premi **Invio**.
1. Per reimpostare tutte le preferenze utente, seleziona **Reimposta**.

   Oppure

   Per ripristinare solo le schede personalizzate, seleziona **Reimposta schede**.
