---
title: Reimpostare le preferenze di un utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: In qualità di amministratore di Adobe Workfront, puoi reimpostare o rimuovere le impostazioni delle preferenze utente per qualsiasi utente del sistema Workfront. I singoli utenti possono inoltre reimpostare le proprie preferenze utente.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: 5706ebd11985b9e67c93686918f8f0327adabdf1
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 3%

---

# Reimpostare le preferenze di un utente

<!-- Audited: 12/2023 -->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambiente Sandbox di anteprima ed è in fase di rilascio in un rollout graduale in produzione.</span>

In qualità di amministratore di Adobe Workfront, puoi reimpostare o rimuovere le impostazioni delle preferenze utente per qualsiasi utente del sistema Workfront.

I singoli utenti possono inoltre reimpostare le proprie preferenze utente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Amministratore di Sistema</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informazioni sulle impostazioni interessate

Quando si reimpostano le preferenze utente, alcune vengono ripristinate ai valori predefiniti di sistema e altre vengono cancellate o rimosse:

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
   <th><strong>Status after the reset</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Views</td> 
   <td> <p> Reverted to the system default</p> <p>Existing views are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing groupings are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Recent Items list</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Favorites list</td> 
   <td>Unaffected</td> 
  </tr> 
  <tr> 
   <td>User Preferences</td> 
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults. The default notifications are listed in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Event notifications available in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition, or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>
-->

<!--Display this table and hide the HTML table above, when the unshim is released.-->

<div class="preview">

| Preferenza | Stato dopo il ripristino |
| --- | --- |
| Viste | Ripristino dei valori predefiniti di sistema <p>Le viste esistenti non vengono eliminate. Puoi selezionarli di nuovo.</p> |
| Filtri | Ripristino dei valori predefiniti di sistema <p>I filtri esistenti non vengono eliminati. Puoi selezionarli di nuovo.</p> |
| Raggruppamenti | Ripristino dei valori predefiniti di sistema <p>I raggruppamenti esistenti non vengono eliminati. Puoi selezionarli di nuovo.</p> |
| Elenco elementi recenti | Cancellato |
| Elenco Preferiti | Non interessato |
| Preferenze utente | Ripristino dei valori predefiniti di sistema <p>Le notifiche e-mail vengono ripristinate ai valori predefiniti del sistema. Le notifiche predefinite sono elencate in [Notifiche evento disponibili in Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).</p> |

</div>

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

1. Se la tua organizzazione è stata integrata in Adobe Unified Experience, segui questo passaggio:

   * Nel campo URL nella parte superiore del browser Web, aggiungi `/resetUser` dopo `workfront`.

     >[!NOTE]
     >
     >È sensibile a maiuscole e minuscole. La U deve essere in maiuscolo e i caratteri rimanenti devono essere minuscoli. Ad esempio:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Premere **Invio**.

1. <span class="preview">Per reimpostare tutte le preferenze utente, fare clic su **Reimposta**.</span>

   <span class="preview">O</span>

   <span class="preview">Per ripristinare la navigazione a sinistra dell&#39;utente alla configurazione originale del modello di layout, fare clic su **Ripristina navigazione a sinistra**.</span>
