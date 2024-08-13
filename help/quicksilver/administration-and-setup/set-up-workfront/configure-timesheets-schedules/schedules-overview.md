---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: utente,pianificazione
navigation-topic: configure-timesheets-and-schedules
title: Panoramica degli Schedules
description: È possibile definire la settimana lavorativa utilizzando le programmazioni. È possibile associare una pianificazione a un utente o a un progetto. Questo consente a  [!DNL Adobe Workfront]  di calcolare le tempistiche e la disponibilità dell'utente. Per istruzioni, consulta Creare una pianificazione.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Panoramica sugli Schedules

<!-- Audited: 1/2024 -->

È possibile definire la settimana lavorativa utilizzando le programmazioni e associare una programmazione a un utente o a un progetto. Questo consente a [!DNL Adobe Workfront] di calcolare le timeline e la disponibilità dell&#39;utente. Per istruzioni, vedere [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Quando si lavora con le pianificazioni in Workfront, considera quanto segue:

* L&#39;amministratore [!DNL Workfront] identifica le ore di funzionamento dell&#39;organizzazione in una pianificazione.

  Analogamente, un amministratore di gruppo può identificare le ore di funzionamento di una pianificazione amministrata da un gruppo che gestisce. Per ulteriori informazioni sugli amministratori di gruppi, vedere [Amministratori di gruppi](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  Ad esempio, una pianificazione può essere definita come: dal lunedì al venerdì, dalle 8 alle 17, con una pausa pranzo.

* [!DNL Workfront] utilizza la pianificazione per determinare quando inizia e termina il giorno lavorativo.

  Ciò non impedisce a un utente di lavorare o completare il lavoro in [!DNL Workfront] al di fuori del normale orario di lavoro. In genere, non è necessario creare una nuova programmazione o un&#39;eccezione per concentrarsi sul lavoro pianificato la sera.

  Allo stesso modo, la tua organizzazione può avere orari di arrivo flessibili per la tua giornata lavorativa. Puoi avere un gruppo di dipendenti che arriva alle 8 del mattino e un altro gruppo che arriva alle 9 del mattino. Non è necessario creare programmi univoci per ciascun gruppo se i gruppi hanno programmi simili o identici. Tuttavia, se i gruppi hanno pianificazioni drasticamente diverse, i loro utenti devono essere associati a pianificazioni univoche. Un dipendente ha capito che il completamento di un&#39;assegnazione è previsto per le 17:00; ciò significa che il lavoro deve essere eseguito entro la fine della giornata lavorativa, indipendentemente dal momento in cui entra al lavoro.

* È consigliabile creare pianificazioni separate per ogni fuso orario associato all&#39;organizzazione.

  È possibile assegnare un fuso orario specifico per ogni pianificazione per garantire che il lavoro venga pianificato in modo appropriato per gli utenti che lavorano in fusi orari diversi.

* La pianificazione predefinita [!DNL Workfront] viene utilizzata nei calcoli della sequenza temporale quando gli utenti o i progetti non sono associati a una pianificazione.

  La pianificazione predefinita viene fornita con il sistema [!DNL Workfront] e non può essere eliminata a meno che non venga sostituita con una nuova pianificazione creata.

* Oltre a calcolare le sequenze temporali, [!DNL Workfront] utilizza le pianificazioni per calcolare la disponibilità dell&#39;utente.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] utilizza l&#39;utente o la pianificazione del progetto per determinare la disponibilità delle risorse nella Programmazione risorse. La pianificazione utilizzata dipende da cosa ha selezionato l&#39;amministratore [!DNL Workfront] per l&#39;impostazione [!UICONTROL Calcola la disponibilità delle risorse utilizzando]. Per informazioni sulle impostazioni di Gestione risorse, vedere [Configurare le preferenze di Gestione risorse](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Gerarchia delle pianificazioni

Se un&#39;attività viene assegnata a un utente associato a una pianificazione e risiede in un progetto associato a una seconda pianificazione, sono disponibili almeno 2 pianificazioni che potrebbero essere potenzialmente applicate ai calcoli della sequenza temporale.

>[!IMPORTANT]
>
>[!DNL Workfront] utilizza la pianificazione di un utente solo quando l&#39;impostazione [!UICONTROL Calcola disponibilità risorse utilizzando] è impostata su [!UICONTROL La pianificazione dell&#39;utente] nell&#39;area [!UICONTROL Gestione risorse] di [!UICONTROL Configurazione]. Per informazioni sul modo in cui l&#39;impostazione [!UICONTROL Calcola la disponibilità delle risorse utilizzando] influisce sulla pianificazione utilizzata per la gestione delle risorse, vedere [Configurare le preferenze di gestione delle risorse](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

L&#39;ordine in cui le pianificazioni vengono utilizzate dal sistema quando ne esiste più di una è:

* Quando un utente viene assegnato a un&#39;attività, [!DNL Workfront] utilizza la pianificazione dell&#39;utente per calcolare la sequenza temporale dell&#39;attività. Questo include anche il tempo personale dell’utente. La pianificazione del progetto viene ignorata.

  Per ulteriori informazioni sull&#39;orario personale, vedere [Configurare l&#39;orario di riposo personale](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Quando più utenti vengono assegnati a un&#39;attività e gli utenti hanno pianificazioni diverse durante l&#39;intervallo di tempo dell&#39;attività, [!DNL Workfront] utilizza una delle pianificazioni seguenti, come definito nell&#39;area [!UICONTROL Preferenze progetto] di [!UICONTROL Configurazione]:

   * Pianificazione dell&#39;utente designato come assegnatario principale
   * La pianificazione associata al progetto.

     Per ulteriori informazioni sulle preferenze del progetto, vedere [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se l&#39;utente assegnato all&#39;attività non ha alcuna pianificazione o l&#39;attività è assegnata solo a una mansione, a un team o non è assegnata, [!DNL Workfront] utilizza la pianificazione del progetto per i calcoli della sequenza temporale.
* Se l&#39;utente assegnato all&#39;attività non dispone di una pianificazione o l&#39;attività è assegnata solo a una mansione, a un team o non è assegnata e il progetto non dispone di una pianificazione, [!DNL Workfront] utilizza la pianificazione nel sistema designato come pianificazione predefinita per i calcoli della sequenza temporale.

  ![](assets/default-schedule.png)

## Collaboration in [!DNL Workfront] tra fusi orari

Per informazioni sull&#39;utilizzo delle pianificazioni per consentire agli utenti di collaborare in [!DNL Workfront] tra fusi orari, vedere [Utilizzo tra fusi orari diversi](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
