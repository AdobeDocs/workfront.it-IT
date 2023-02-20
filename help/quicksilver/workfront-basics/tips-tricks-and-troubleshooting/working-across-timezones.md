---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Utilizzo di fusi orari diversi
description: 'Può essere utile capire come [!DNL Adobe Workfront] utilizza i fusi orari per calcolare quanto segue: EDIT ME.'
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# Utilizzo di fusi orari diversi

Può essere utile capire come [!DNL Adobe Workfront] utilizza i fusi orari per calcolare quanto segue:

* Campi di tempo per gli oggetti
* Tempi in altri [!DNL Workfront] aree, ad esempio e-mail Workfront automatizzate

## Fusi orari in [!DNL Workfront]

Tempi di visualizzazione [!DNL Workfront] si basano sulle configurazioni del fuso orario per la tua organizzazione [!DNL Workfront] e per il profilo utente. Se questi due fusi orari sono diversi, è possibile che si verifichino discrepanze di tempo in diverse aree e caratteristiche utilizzate in [!DNL Workfront].

>[!NOTE]
>
><div class="preview">In un modulo personalizzato allegato a un oggetto, le istruzioni data e ora nei campi personalizzati calcolati vengono calcolate e salvate dall’Ora universale coordinata (UTC), non dalle configurazioni del fuso orario impostate per l’istanza dell’organizzazione e il profilo utente. I calcoli in un modulo personalizzato vengono generati e visualizzati in base ai singoli fusi orari di ciascun utente.</div>




* [La tua organizzazione [!DNL Workfront] istanza](#your-organization-s-workfront-instance)
* [Il tuo profilo utente](#your-user-profile)

### La tua organizzazione [!DNL Workfront] istanza {#your-organization-s-workfront-instance}

Il fuso orario della tua organizzazione [!DNL Workfront] L&#39;istanza è solitamente impostata per la posizione dell&#39;ufficio principale. Questo determina quanto segue:

* Il tempo visualizzato nelle e-mail generate da [!DNL Workfront]
* Il fuso orario per i nuovi utenti aggiunti (prima della [!DNL Workfront] l&#39;amministratore configura un fuso orario diverso per i singoli utenti in base al luogo in cui lavorano)

   Per ulteriori informazioni su questi due esempi, vedi [Configurare le informazioni di base per il sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Inizio o fine di un tasso di fatturazione ignorato per un progetto. Per ulteriori informazioni, consulta [Ignora tassi di fatturazione ruolo lavoro a livello di progetto](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Il tuo profilo utente {#your-user-profile}

Il fuso orario nel profilo utente deve essere configurato per la posizione in cui lavori. Questo determina quanto segue:

* Il tempo mostrato nella tua uscita [!DNL Workfront] messaggi e-mail
* Tempi di un oggetto su cui lavori, ad esempio l’ora di inizio e di fine

   Se gli utenti di più fusi orari sono assegnati a un oggetto, [!DNL Workfront] converte i tempi dell’oggetto per tutte le persone coinvolte, utilizzando il fuso orario configurato in ciascun profilo utente.

   **Esempio:** Nella zona Eastern Standard Time (EST) in cui si lavora, impostare un&#39;attività per l&#39;avvio alle 16:00 e assegnarla agli utenti che lavorano nella zona Pacific Standard Time (PST). Per questi utenti, l&#39;ora di inizio viene visualizzata alle 13:00. Se lo mostrassero alle 16:00, inizierebbero a lavorarci con tre ore di ritardo.

   Se il creatore dell&#39;oggetto non nota la differenza tra i fusi orari degli assegnatari e apporta le necessarie regolazioni durante l&#39;impostazione dei tempi dell&#39;oggetto, o se gli assegnatari non notano tale differenza, può essere difficile ottenere il momento giusto mentre tutti collaborano all&#39;oggetto.

   **Esempio:** Puoi configurare un’attività di un giorno per iniziare alle 09:00 EST, dimenticando che alcuni utenti dell’attività funzionano nella zona PST. Per loro, l&#39;ora di inizio 6:00 AM. Poiché non inizieranno a lavorarci fino alle 9:00 del loro tempo (mezzogiorno il tuo tempo), il compito inizia e termina con tre ore di ritardo.

Per informazioni sulla configurazione del fuso orario nel profilo utente, consulta [Configurare le impostazioni personali](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Per informazioni su come [!DNL Workfront] amministratore (o qualcuno con [!UICONTROL Modifica] accesso agli utenti) può configurare il fuso orario in un profilo utente, vedi [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Come semplificare il lavoro degli utenti tra diversi fusi orari

Puoi aiutare gli utenti a lavorare più facilmente in più fusi orari in diversi modi:

* [Usa pianificazioni](#use-schedules)
* [Utilizzare i campi tempo calcolati in un modulo personalizzato](#use-calculated-time-fields-in-a-custom-form)
* [Utilizzare campi di testo invece dei campi data in un modulo personalizzato](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Usa pianificazioni {#use-schedules}

[!DNL Workfront] gli amministratori creano pianificazioni separate per ogni fuso orario dell&#39;organizzazione per garantire che il lavoro sia pianificato in modo appropriato per tutti, ovunque si trovino. Una volta create le pianificazioni, l’amministratore può associarle a determinati progetti e utenti:

* **[!UICONTROL Progetti]**: Un creatore di progetti può selezionare una pianificazione per un singolo progetto. Questo determina la programmazione delle attività nel progetto, in base agli orari lavorativi impostati per i fusi orari degli assegnatari.
* **[!UICONTROL Utenti]**: A [!DNL Workfront] amministratore (o qualcuno con [!UICONTROL Modifica] accesso agli utenti) può selezionare una pianificazione per il singolo utente nel profilo dell’utente.

   Questa pianificazione potrebbe essere diversa da una pianificazione del progetto. Ad esempio, quando un utente crea un’attività nel progetto e non vi ha ancora assegnato nessuno, l’attività utilizza la pianificazione del progetto. Quando un utente viene assegnato all&#39;attività, l&#39;attività utilizza la pianificazione dell&#39;utente.

   Se a un&#39;attività sono assegnati più utenti, il sistema utilizza una delle seguenti opzioni, come configurato nelle preferenze di progetto a livello di sistema:

   * Fuso orario per la pianificazione del proprietario principale dell&#39;attività
   * Fuso orario per la pianificazione del progetto.

   Questo può causare la modifica delle date delle attività.

   **Esempio:** Un utente EST viene assegnato a un’attività di un giorno pianificata per l’inizio alle 9:00 PST, ovvero mezzogiorno EST. Poiché l’utente EST ha solo 2 ore lavorative rimanenti per il giorno, la data di completamento dell’attività si estende di circa 6 ore nel giorno lavorativo successivo.

   Per informazioni sulla [!UICONTROL Preferenze del progetto] area [!UICONTROL Configurazione], vedi [Configurare le preferenze del progetto a livello di sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   Per istruzioni su come assegnare una pianificazione a un progetto o a un utente, consulta [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   Per informazioni su come il fuso orario configurato nella pianificazione influisce sulla distribuzione di [!UICONTROL Orari pianificati] in [!DNL Workload Balancer], vedi [Gestisci le allocazioni degli utenti nel [!DNL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Utilizzare i campi tempo calcolati in un modulo personalizzato {#use-calculated-time-fields-in-a-custom-form}

È possibile utilizzare una serie di campi personalizzati calcolati in un modulo personalizzato per visualizzare l’ora corrente per gli utenti dell’organizzazione, ad esempio una riga di orologi aeroportuali che mostra l’ora in più città. È possibile creare un campo per ogni fuso orario in cui lavorano gli utenti, calcolando ad ogni fuso orario l’ora corrispondente.

Per ulteriori informazioni, consulta [Aggiungere dati calcolati a un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md), nonché la sezione [Campi personalizzati calcolati in base alla data e all’ora](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) nell&#39;articolo [Espressioni dati calcolate](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Utilizzare campi di testo invece dei campi data in un modulo personalizzato {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Se non vuoi [!DNL Workfront] per convertire i tempi di configurazione di un oggetto per gli utenti di fusi orari diversi, è possibile utilizzare un campo di testo in un modulo personalizzato allegato a un oggetto anziché un campo data. In questo modo, l’ora visualizza l’ora digitata per tutti gli utenti del progetto.

In questo caso, si consiglia agli utenti del modulo di calcolare la differenza tra il proprio fuso orario e il proprio, in modo che possano determinare quando iniziare e finire il lavoro. È possibile includere questa opzione nelle istruzioni digitate per il modulo personalizzato o in una descrizione comandi per tale campo. Per ulteriori informazioni, consulta [Aggiungere un campo personalizzato a un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
