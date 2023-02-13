---
title: Reimpostare le preferenze di un utente
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: In qualità di amministratore di Adobe Workfront, puoi ripristinare o rimuovere le impostazioni delle preferenze utente per qualsiasi utente del sistema Workfront. I singoli utenti possono inoltre reimpostare le proprie preferenze utente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 2%

---

# Reimpostare le preferenze di un utente

In qualità di amministratore di Adobe Workfront, puoi ripristinare o rimuovere le impostazioni delle preferenze utente per qualsiasi utente del sistema Workfront.

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informazioni sulle impostazioni interessate

Quando reimpostate le preferenze utente, alcune preferenze vengono ripristinate sulle impostazioni predefinite del sistema e altre vengono eliminate o rimosse:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preferenza</strong> </th> 
   <th><strong>Stato dopo la reimpostazione</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Viste</td> 
   <td> <p> Ripristino dell'impostazione predefinita del sistema</p> <p>Le visualizzazioni esistenti non vengono eliminate. Puoi selezionarli di nuovo.</p> </td> 
  </tr> 
  <tr> 
   <td>Filtri</td> 
   <td> <p>Ripristino dell'impostazione predefinita del sistema</p> <p>I filtri esistenti non vengono eliminati. Puoi selezionarli di nuovo.</p> </td> 
  </tr> 
  <tr> 
   <td>Raggruppamenti</td> 
   <td> <p>Ripristino dell'impostazione predefinita del sistema</p> <p>I gruppi esistenti non vengono eliminati. Puoi selezionarli di nuovo.</p> </td> 
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
   <td> <p>Ripristino dell'impostazione predefinita del sistema</p> <p>Le notifiche e-mail vengono ripristinate ai valori predefiniti del sistema</p> </td> 
  </tr> 
  <tr> 
   <td>Schede personalizzate definite dall'utente</td> 
   <td>Rimosso</td> 
  </tr> 
  <tr> 
   <td>Opzioni di navigazione globale definite dall'utente</td> 
   <td>Imposta nuovamente la definizione del modello di layout o l'impostazione predefinita del sistema se non è assegnato alcun modello di layout.</td> 
  </tr> 
 </tbody> 
</table>

## Reimposta le preferenze utente

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Seleziona **Accedi come**.
1. Inizia a digitare il nome dell’utente di cui desideri reimpostare le preferenze, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.
1. Seleziona  **Accesso**.
1. Nel campo URL nella parte superiore del browser web, aggiungi `/resetUser` dopo `workfront.com`.

   >[!NOTE]
   >
   >Questo fa distinzione tra maiuscole e minuscole. L’U deve essere maiuscola e i caratteri rimanenti devono essere minuscoli. Ad esempio:
   >
   >
   ```
   >https://company_domain.my.workfront.com/resetUser
   >```

1. Press **Invio**.
1. Per ripristinare tutte le preferenze utente, seleziona **Reimposta**.

   Oppure

   Per ripristinare solo le schede personalizzate, seleziona **Ripristina schede**.
