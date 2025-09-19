---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Configurare se il tempo è registrato in ore o giorni
description: In qualità di utente con una licenza Pianificazione, puoi configurare se effettuare l’accesso ad Adobe Workfront in ore o giorni. Gli amministratori di sistema possono configurare questa impostazione per singoli utenti o per più utenti dell’organizzazione. Per impostazione predefinita, gli utenti accedono in ore.
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: 106ef838bfee5e496cae864eca5c19fd12fdd18e
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 1%

---

# Configurare se il tempo è registrato in ore o giorni

In qualità di utente con una licenza Planner, puoi configurare se effettuare l’accesso ad Adobe Workfront in ore o giorni. Gli amministratori di sistema possono configurare questa impostazione per singoli utenti o per più utenti dell’organizzazione. Per impostazione predefinita, gli utenti accedono in ore. Per informazioni su come registrare l&#39;ora in Workfront, vedere [Registra ora](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>È consigliabile registrare il tempo nello stesso modo, ovvero ore o giorni, in tutta l’organizzazione per garantire l’accuratezza del reporting.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>I responsabili della pianificazione possono configurare autonomamente il tempo. Solo un amministratore di Workfront può configurare il tempo per altri utenti.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

1. Effettua una delle seguenti operazioni, a seconda dell’obiettivo e del livello di accesso nel sistema:

   * **Utente Planner che configura autonomamente la registrazione dell&#39;ora:** Fai clic sull&#39;icona **del** menu principale![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic sul nome utente accanto all&#39;immagine del tuo profilo. Fai clic sull&#39;icona **Altro** accanto al tuo nome e seleziona **Modifica**.

   * **L&#39;amministratore di sistema configura la registrazione ore per altri utenti:** Inizia a modificare uno o più account utente, come descritto in [Modifica il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Nella finestra di dialogo risultante, nella sezione **Pianificazione risorse**, individuare l&#39;opzione **Registra tempo in**.

   ![Tempo di connessione nelle opzioni](assets/user-profile-log-time-options.png)

1. (Condizionale) Se sei un amministratore di sistema che modifica più utenti contemporaneamente, seleziona **Registra ora in**.
1. Selezionare una delle seguenti opzioni per la registrazione dell&#39;ora:

   | Opzione | Descrizione |
   |---|---|
   | **Ore** | Gli utenti specificano le ore quando si registrano in Workfront. |
   | **Giorni** | Gli utenti specificano i giorni per la registrazione in Workfront. |

1. (Condizionale) Se hai selezionato di registrare il tempo in giorni, nel campo **Ore equivalenti per Full Workday**, digita il numero di ore che equivalgono a un giorno intero. Un giorno sulla scheda orario di un utente equivale al numero di ore immesse qui.

   Quando configuri questa impostazione, tieni presente quanto segue:

   * Questa opzione non è disponibile quando si configura per registrare il tempo in ore.
   * Questa opzione è utilizzata solo per registrare il tempo. Questa opzione non è correlata all&#39;opzione **Pianifica** disponibile anche quando si modifica un utente. L&#39;opzione **Pianifica** viene utilizzata per il calcolo delle sequenze temporali e in altre aree di Workfront. Per ulteriori informazioni sull&#39;utilizzo dell&#39;opzione **Pianifica**, vedere [Crea una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md). 

1. Fai clic su **Salva modifiche**.
