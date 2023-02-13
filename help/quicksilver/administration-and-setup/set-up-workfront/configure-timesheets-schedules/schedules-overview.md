---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: utente,pianificazione
navigation-topic: configure-timesheets-and-schedules
title: Panoramica sulle pianificazioni
description: È possibile definire la settimana lavorativa utilizzando le pianificazioni. Puoi associare una pianificazione a un utente o a un progetto. Ciò consente [!DNL Adobe Workfront] per calcolare le timeline e la disponibilità degli utenti. Per istruzioni, consulta Creare una pianificazione .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# Panoramica sulle pianificazioni

È possibile definire la settimana lavorativa utilizzando le pianificazioni e associare una pianificazione a un utente o a un progetto. Ciò consente [!DNL Adobe Workfront] per calcolare le timeline e la disponibilità degli utenti. Per istruzioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Quando si lavora con le pianificazioni in Workfront, considera quanto segue:

* La [!DNL Workfront] l’amministratore identifica gli orari di funzionamento dell’organizzazione in una pianificazione.

   Analogamente, un amministratore di gruppo può identificare le ore di funzionamento di una pianificazione gestita da un gruppo che gestisce.

   Per ulteriori informazioni sugli amministratori dei gruppi, consulta [Amministratori di gruppo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

   Ad esempio, una pianificazione può essere definita come: Da lunedì a venerdì, dalle 8 alle 17, con un&#39;ora di pausa per pranzo.

* [!DNL Workfront] utilizza la pianificazione per determinare quando inizia e termina il giorno lavorativo.

   Questo non impedisce a un utente di lavorare o completare il lavoro in [!DNL Workfront] al di fuori del normale orario di lavoro. Generalmente, non è necessario creare una nuova pianificazione o un&#39;eccezione di pianificazione per concentrarsi sul lavoro pianificato la sera.

   Allo stesso modo, la tua organizzazione può avere orari di arrivo flessibili per la tua giornata lavorativa. Puoi avere un set di dipendenti che arriva alle 8 del mattino e un altro set che arriva alle 9 del mattino. Non è necessario creare pianificazioni univoche per ciascun gruppo, se i gruppi hanno pianificazioni simili o identiche. Ma se i gruppi hanno pianificazioni drasticamente diverse, i loro utenti dovrebbero essere associati a pianificazioni univoche. Un dipendente capisce se un&#39;assegnazione deve essere completata alle 17.00 significa che il lavoro deve essere svolto entro la fine della giornata lavorativa, indipendentemente dal momento in cui entra a lavorare.

* È consigliabile creare pianificazioni separate per ogni fuso orario associato all’organizzazione.

   È possibile assegnare un fuso orario specifico per ogni pianificazione per garantire che il lavoro sia pianificato in modo appropriato per gli utenti che lavorano in fusi orari diversi.

* La [!DNL Workfront] La pianificazione predefinita viene utilizzata nei calcoli della timeline quando gli utenti o i progetti non sono associati a una pianificazione.

   La pianificazione predefinita viene fornita con [!DNL Workfront] e non può essere eliminato a meno che non venga sostituito con una nuova pianificazione creata.

* Oltre al calcolo delle scadenze, [!DNL Workfront] utilizza le pianificazioni per calcolare la disponibilità degli utenti.

   >[!IMPORTANT]
   >
   >[!DNL Workfront] utilizza la pianificazione dell&#39;utente o del progetto per determinare la disponibilità della risorsa nel planner risorse. Quale pianificazione viene utilizzata a seconda del tipo di [!DNL Workfront] amministratore selezionato per [!UICONTROL Calcolare la disponibilità delle risorse utilizzando] impostazione. Per informazioni sulle impostazioni di Gestione risorse, consulta [Configurare le preferenze di Gestione risorse](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Gerarchia delle pianificazioni

Se un&#39;attività viene assegnata a un utente associato a una pianificazione e risiede in un progetto associato a una seconda pianificazione, è possibile applicare almeno 2 pianificazioni ai calcoli della timeline.

>[!IMPORTANT]
>
>[!DNL Workfront] utilizza la pianificazione di un utente solo quando [!UICONTROL Calcolare la disponibilità delle risorse utilizzando] è impostato su [!UICONTROL Pianificazione dell&#39;utente] in [!UICONTROL Gestione risorse] area [!UICONTROL Configurazione]. Per informazioni su come [!UICONTROL Calcolare la disponibilità delle risorse utilizzando] l&#39;impostazione influisce sulla pianificazione utilizzata per la gestione delle risorse, vedere [Configurare le preferenze di Gestione risorse](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

L&#39;ordine in cui le pianificazioni vengono utilizzate dal sistema quando ne esistono più di una è il seguente:

* Quando un utente viene assegnato a un&#39;attività, [!DNL Workfront] utilizza la pianificazione dell&#39;utente per calcolare la timeline dell&#39;attività. Questo include anche l&#39;orario personale dell&#39;utente. La pianificazione del progetto viene ignorata.

   Per ulteriori informazioni sull&#39;orario personale, vedi [Configura il tempo di inattività personale in [!DNL Adobe Workfront]](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Quando più utenti vengono assegnati a un&#39;attività e gli utenti hanno pianificazioni diverse durante l&#39;intervallo di tempo dell&#39;attività, [!DNL Workfront] utilizza una delle seguenti pianificazioni, come definito nel [!UICONTROL Preferenze del progetto] area [!UICONTROL Configurazione]:

   * Pianificazione dell&#39;utente designato come assegnatario principale
   * La pianificazione associata al progetto.

      Per ulteriori informazioni sulle preferenze del progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se l&#39;utente assegnato all&#39;attività non dispone di una pianificazione o se l&#39;attività viene assegnata solo a un ruolo, a un team o se non viene assegnata, [!DNL Workfront] utilizza la pianificazione del progetto per i calcoli della timeline.
* Se l&#39;utente assegnato all&#39;attività non dispone di una pianificazione oppure l&#39;attività viene assegnata solo a un ruolo, a un team o a un ruolo non assegnato e il progetto non dispone di alcuna pianificazione, allora [!DNL Workfront] utilizza la pianificazione nel sistema designato come Pianificazione predefinita per i calcoli della timeline.

   ![](assets/default-schedule.png)

## Collaborazione in [!DNL Workfront] tra fusi orari diversi

Per informazioni sull&#39;utilizzo delle pianificazioni per aiutare gli utenti a collaborare in [!DNL Workfront] nei diversi fusi orari, vedi [Utilizzo di fusi orari diversi](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
