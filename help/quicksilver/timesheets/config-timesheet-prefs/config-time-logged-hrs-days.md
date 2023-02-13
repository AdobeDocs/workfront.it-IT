---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Configura se l'ora è registrata in ore o giorni
description: In qualità di utente con una licenza di piano, puoi configurare se registrare l’ora in Adobe Workfront in ore o giorni. Gli amministratori di sistema possono configurare questa impostazione per singoli utenti o per più utenti della propria organizzazione. Per impostazione predefinita, gli utenti registrano il tempo in ore.
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b4ab350af22afa44774f06d82daf1c3fb266d2b9
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# Configura se l&#39;ora è registrata in ore o giorni

In qualità di utente con una licenza Planner, puoi configurare se registrare l’ora in Adobe Workfront in ore o giorni. Gli amministratori di sistema possono configurare questa impostazione per singoli utenti o per più utenti della propria organizzazione. Per impostazione predefinita, gli utenti registrano il tempo in ore. Per informazioni su come registrare l’ora in Workfront, vedi [Tempo di log](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>Consigliamo di registrare il tempo nello stesso modo, ore o giorni, in tutta l’organizzazione per garantire l’accuratezza dei rapporti.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>I pianificatori possono configurare il tempo per se stessi. Solo un amministratore Workfront può configurare il tempo per altri utenti.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

1. Effettua una delle seguenti operazioni, a seconda dell’obiettivo e del livello di accesso nel sistema:

   * **L&#39;utente del planner sta configurando autonomamente la registrazione dei tempi:** Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic sul nome utente accanto all’immagine del tuo profilo. Quindi, fai clic sul pulsante **Altro** accanto al nome e seleziona **Modifica**.

   * **Amministratore di sistema: configurazione della registrazione dei tempi per altri utenti:** Inizia a modificare uno o più account utente, come descritto in [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Nella finestra di dialogo risultante, nella **Pianificazione delle risorse** , individua la sezione **Accesso** opzione .

   ![](assets/new-timesheet-log-hours-350x249.png)

1. (Condizionale) Se sei un amministratore di sistema che modifica contemporaneamente più utenti, seleziona **Accesso**.
1. Selezionare tra le seguenti opzioni per il tempo di registrazione:

   | Opzione | Descrizione |
   |---|---|
   | **Ore** | Gli utenti specificano le ore di accesso in Workfront. |
   | **Giorni** | Gli utenti specificano i giorni durante l’accesso in Workfront. |

1. (Condizionale) Se hai selezionato di registrare il tempo in giorni, nella **Ore equivalenti per Workday completo** campo , digitare il numero di ore che equivalgono a un giorno intero. Un giorno nella scheda attività di un utente corrisponde al numero di ore immesse qui.

   Quando configuri questa impostazione, tieni presente quanto segue:

   * Questa opzione non è disponibile per la configurazione dell’ora di accesso in ore.
   * Questa opzione viene utilizzata solo per il tempo di registrazione. Questa opzione non è correlata al **Pianificazione** opzione disponibile anche durante la modifica di un utente. La **Pianificazione** viene utilizzata per calcolare le timeline e in altre aree di Workfront. (Per ulteriori informazioni sull&#39;utilizzo di **Pianificazione** opzione , vedi [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).) 

1. Fai clic su **Salva modifiche**.
