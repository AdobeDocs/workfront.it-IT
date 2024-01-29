---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: utente,pianificazione
navigation-topic: configure-timesheets-and-schedules
title: Panoramica sugli Schedules
description: È possibile definire la settimana lavorativa utilizzando le programmazioni. È possibile associare una pianificazione a un utente o a un progetto. Ciò consente [!DNL Adobe Workfront] per calcolare le timeline e la disponibilità dell’utente. Per istruzioni, consulta Creare una pianificazione.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 32da139d7385e05436a669bdc6f36b71ad83c8d2
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Panoramica sugli Schedules

<!-- Audited: 1/2024 -->

È possibile definire la settimana lavorativa utilizzando le programmazioni e associare una programmazione a un utente o a un progetto. Ciò consente [!DNL Adobe Workfront] per calcolare le timeline e la disponibilità dell’utente. Per istruzioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Quando si lavora con le pianificazioni in Workfront, considera quanto segue:

* Il [!DNL Workfront] l’amministratore identifica le ore di funzionamento dell’organizzazione in una pianificazione.

  Analogamente, un amministratore di gruppo può identificare le ore di funzionamento di una pianificazione amministrata da un gruppo che gestisce. Per ulteriori informazioni sugli amministratori di gruppi, consulta [Amministratori di gruppi](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  Ad esempio, una pianificazione può essere definita come: dal lunedì al venerdì, dalle 8 alle 17, con una pausa pranzo.

* [!DNL Workfront] utilizza la pianificazione per determinare quando inizia e termina il giorno lavorativo.

  Ciò non impedisce a un utente di lavorare o completare un lavoro in [!DNL Workfront] al di fuori del normale orario di lavoro. In genere, non è necessario creare una nuova programmazione o un&#39;eccezione per concentrarsi sul lavoro pianificato la sera.

  Allo stesso modo, la tua organizzazione può avere orari di arrivo flessibili per la tua giornata lavorativa. Puoi avere un gruppo di dipendenti che arriva alle 8 del mattino e un altro gruppo che arriva alle 9 del mattino. Non è necessario creare programmi univoci per ciascun gruppo se i gruppi hanno programmi simili o identici. Tuttavia, se i gruppi hanno pianificazioni drasticamente diverse, i loro utenti devono essere associati a pianificazioni univoche. Un dipendente ha capito che il completamento di un&#39;assegnazione è previsto per le 17:00; ciò significa che il lavoro deve essere eseguito entro la fine della giornata lavorativa, indipendentemente dal momento in cui entra al lavoro.

* È consigliabile creare pianificazioni separate per ogni fuso orario associato all&#39;organizzazione.

  È possibile assegnare un fuso orario specifico per ogni pianificazione per garantire che il lavoro venga pianificato in modo appropriato per gli utenti che lavorano in fusi orari diversi.

* Il [!DNL Workfront] La pianificazione predefinita viene utilizzata nei calcoli della sequenza temporale quando utenti o progetti non sono associati a una pianificazione.

  La pianificazione predefinita viene fornita con [!DNL Workfront] e non possono essere eliminati a meno che non vengano sostituiti con una nuova pianificazione.

* Oltre al calcolo delle tempistiche, [!DNL Workfront] utilizza le pianificazioni per calcolare la disponibilità utente.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] utilizza l&#39;utente o la pianificazione del progetto per determinare la disponibilità delle risorse nella pianificazione risorse. Quale pianificazione viene utilizzata dipende da quale [!DNL Workfront] amministratore selezionato per il [!UICONTROL Calcola la disponibilità delle risorse tramite] impostazione. Per informazioni sulle impostazioni di Gestione risorse, vedi [Configurare le preferenze di Gestione risorse](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Gerarchia delle pianificazioni

Se un&#39;attività viene assegnata a un utente associato a una pianificazione e risiede in un progetto associato a una seconda pianificazione, sono disponibili almeno 2 pianificazioni che potrebbero essere potenzialmente applicate ai calcoli della sequenza temporale.

>[!IMPORTANT]
>
>[!DNL Workfront] utilizza la pianificazione di un utente solo quando [!UICONTROL Calcola la disponibilità delle risorse tramite] è impostato su [!UICONTROL La pianificazione dell&#39;utente] nel [!UICONTROL Gestione risorse] area di [!UICONTROL Configurazione]. Per informazioni su come [!UICONTROL Calcola la disponibilità delle risorse tramite] l&#39;impostazione influisce sulla pianificazione utilizzata per Gestione risorse, vedere [Configurare le preferenze di Gestione risorse](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

L&#39;ordine in cui le pianificazioni vengono utilizzate dal sistema quando ne esiste più di una è:

* Quando un utente viene assegnato a un’attività, [!DNL Workfront] utilizza la pianificazione dell&#39;utente per calcolare la sequenza temporale dell&#39;attività. Questo include anche il tempo personale dell’utente. La pianificazione del progetto viene ignorata.

  Per ulteriori informazioni sul tempo personale, consulta [Configurare l’indisponibilità personale](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Quando a un&#39;attività sono assegnati più utenti e gli utenti hanno pianificazioni diverse durante l&#39;intervallo di tempo dell&#39;attività, [!DNL Workfront] utilizza una delle pianificazioni seguenti, come definito nella [!UICONTROL Preferenze progetto] area di [!UICONTROL Configurazione]:

   * Pianificazione dell&#39;utente designato come assegnatario principale
   * La pianificazione associata al progetto.

     Per ulteriori informazioni sulle preferenze del progetto, consulta [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se l’utente assegnato all’attività non ha alcuna pianificazione o se l’attività è assegnata solo a una mansione, a un team o non è assegnata, [!DNL Workfront] utilizza la pianificazione del progetto per i calcoli della sequenza temporale.
* Se l&#39;utente assegnato all&#39;attività non dispone di alcuna pianificazione o se l&#39;attività è assegnata solo a una mansione, a un team o non è assegnata e il progetto non dispone di alcuna pianificazione, [!DNL Workfront] utilizza la pianificazione nel sistema designato come pianificazione predefinita per i calcoli della sequenza temporale.

  ![](assets/default-schedule.png)

## Collaborazione in [!DNL Workfront] tra fusi orari

Per informazioni sull&#39;utilizzo delle pianificazioni per consentire agli utenti di collaborare in [!DNL Workfront] tra fusi orari, vedi [Utilizzo dei fusi orari](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
