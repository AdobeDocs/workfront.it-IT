---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Utilizzo dei fusi orari
description: Può essere utile capire come [!DNL Adobe Workfront] utilizza i fusi orari per calcolare i campi di tempo per gli oggetti e gli orari in altre aree, ad esempio le e-mail.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: tm+mt
source-wordcount: '1152'
ht-degree: 0%

---

# Utilizzo dei fusi orari

<!-- Audited: 2/2024 -->

Può essere utile capire come [!DNL Adobe Workfront] utilizza i fusi orari per calcolare quanto segue:

* Campi di tempo per gli oggetti
* Ore in altre [!DNL Workfront] aree, ad esempio e-mail Workfront automatizzate

>[!WARNING]
>
>Se non riesci a trovare il tuo fuso orario esatto nell’elenco che ti forniamo, individua quello più vicino e aggiornalo per la tua istanza.
>
>Inoltre, considera che un fuso orario simile potrebbe non corrispondere perfettamente al tuo.
>
>Ad esempio, alcuni paesi o territori potrebbero osservare l&#39;ora legale, ma il tuo paese potrebbe non farlo. Se necessario, potrebbe essere necessario regolare i fusi orari del sistema in base a queste modifiche.


## Fusi orari in [!DNL Workfront]

Ore visualizzate in [!DNL Workfront] si basano sulle configurazioni del fuso orario dell’organizzazione [!DNL Workfront] e per il tuo profilo utente. Se questi due fusi orari sono diversi, è possibile che si verifichino discrepanze di tempo in aree e caratteristiche diverse utilizzate in [!DNL Workfront].

>[!NOTE]
>
>In un modulo personalizzato allegato a un oggetto, le istruzioni di data e ora nei campi personalizzati calcolati vengono calcolate e salvate in base al tempo UTC (Coordinated Universal Time) e non in base alle configurazioni del fuso orario impostate per l’istanza della tua organizzazione e il tuo profilo utente. I calcoli in un modulo personalizzato vengono generati e visualizzati in base ai singoli fusi orari degli utenti.

* [Dell&#39;organizzazione [!DNL Workfront] istanza](#your-organization-s-workfront-instance)
* [Il tuo profilo utente](#your-user-profile)

### Dell&#39;organizzazione [!DNL Workfront] istanza {#your-organization-s-workfront-instance}

Il fuso orario dell’organizzazione [!DNL Workfront] L’istanza di è in genere impostata per l’ubicazione dell’ufficio principale. Questo determina quanto segue:

* L’ora visualizzata nelle e-mail generate da [!DNL Workfront]
* Il fuso orario per i nuovi utenti aggiunti (prima del [!DNL Workfront] l’amministratore configura per loro un fuso orario diverso in base al luogo in cui lavorano)

  Per ulteriori informazioni su questi due esempi, consulta [Configurare le informazioni di base per il sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* L’inizio o la fine di una tariffa di fatturazione sostituita per un progetto. Per ulteriori informazioni, consulta [Sostituisci tariffe di fatturazione mansione a livello di progetto](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Il tuo profilo utente {#your-user-profile}

Il fuso orario nel profilo utente deve essere configurato per la posizione in cui lavori. Questo determina quanto segue:

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Ore per un oggetto su cui si lavora, ad esempio ore di inizio e di fine

  Se a un oggetto vengono assegnati utenti in più fusi orari, [!DNL Workfront] converte gli orari dell’oggetto per tutti gli utenti coinvolti, utilizzando il fuso orario configurato in ciascun profilo utente.

  **Esempio:** Nella zona dell&#39;ora solare fuso orientale in cui si lavora, è possibile impostare l&#39;inizio di un&#39;attività alle 16.00 e assegnarla agli utenti che lavorano nella zona dell&#39;ora solare fuso orientale (PST). Per tali utenti, l’ora di inizio viene visualizzata come 1:00 PM. Se la visualizzasse alle 16:00, inizierebbe a lavorarci con tre ore di ritardo.

  Se il creatore dell&#39;oggetto non rileva la differenza tra i fusi orari degli assegnatari e apporta le modifiche necessarie durante l&#39;impostazione degli orari degli oggetti o se gli assegnatari non notano tale differenza, può essere difficile ottenere gli intervalli corretti mentre tutti collaborano all&#39;oggetto.

  **Esempio:** Si configura un&#39;attività di un giorno per iniziare alle 9:00 EST, dimenticando che alcuni utenti dell&#39;attività lavorano nella zona PST. Per loro, l&#39;ora di inizio 6:00 AM. Poiché non inizieranno a lavorarci fino alle 9:00 (mezzogiorno del tuo orario), l’attività inizia e termina con tre ore di ritardo.

Per informazioni sulla configurazione del fuso orario nel profilo utente, consulta [Configura le mie impostazioni](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Per informazioni su come [!DNL Workfront] amministratore (o un utente con [!UICONTROL Modifica] accesso agli utenti) può configurare il fuso orario in un profilo utente, vedi [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Come semplificare il lavoro degli utenti in più fusi orari

Puoi aiutare gli utenti a lavorare più facilmente in diversi fusi orari in diversi modi:

* [Usa pianificazioni](#use-schedules)
* [Utilizzare i campi tempo calcolati in un modulo personalizzato](#use-calculated-time-fields-in-a-custom-form)
* [Utilizzare campi di testo invece di campi data in un modulo personalizzato](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Usa pianificazioni {#use-schedules}

[!DNL Workfront] gli amministratori creano pianificazioni separate per ogni fuso orario all’interno dell’organizzazione per garantire che il lavoro sia pianificato in modo appropriato per tutti, ovunque si trovino. Dopo che l’amministratore ha creato le pianificazioni, queste possono essere associate a determinati progetti e utenti:

* **[!UICONTROL Progetti]**: un autore di progetto può selezionare una pianificazione per un singolo progetto. Determina la programmazione delle attività del progetto, in base alle ore lavorative impostate per i fusi orari degli assegnatari.
* **[!UICONTROL Utenti]**: A [!DNL Workfront] amministratore (o un utente con [!UICONTROL Modifica] accesso agli utenti) può selezionare una pianificazione per un singolo utente nel suo profilo.

  Questa pianificazione potrebbe essere diversa da quella di un progetto. Se ad esempio un utente crea un&#39;attività nel progetto e non ne ha ancora assegnata alcuna, l&#39;attività utilizzerà la pianificazione del progetto. Quando un utente viene assegnato all’attività, questa utilizza la pianificazione dell’utente.

  Se a un&#39;attività sono assegnati più utenti, il sistema utilizza uno dei seguenti, come configurato nelle preferenze di progetto a livello di sistema:

   * Fuso orario per la pianificazione del proprietario principale dell&#39;attività
   * Il fuso orario per la pianificazione del progetto.

  Questo può causare la modifica delle date delle attività.

  **Esempio:** Un utente EST è assegnato a un&#39;attività di un giorno pianificata per iniziare alle 09:00 PST, che è mezzogiorno EST. Poiché all&#39;utente EST rimangono solo 2 ore lavorative al giorno, la data di completamento dell&#39;attività viene estesa di circa 6 ore al giorno lavorativo successivo.

  Per informazioni su [!UICONTROL Preferenze progetto] area di [!UICONTROL Configurazione], vedi [Configurare le preferenze di progetto a livello di sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  Per istruzioni sull’assegnazione di una pianificazione a un progetto o a un utente, consulta [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  Per informazioni su come il fuso orario configurato nella pianificazione influisce sulla distribuzione di [!UICONTROL Ore pianificate] nel [!UICONTROL Bilanciatore dei carichi di lavoro], vedi [Gestire le allocazioni utente in [!UICONTROL Bilanciatore dei carichi di lavoro]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Utilizzare i campi tempo calcolati in un modulo personalizzato {#use-calculated-time-fields-in-a-custom-form}

È possibile utilizzare una serie di campi personalizzati calcolati in un modulo personalizzato per visualizzare l’ora corrente per gli utenti dell’organizzazione, ad esempio una riga di orologi aeroportuali che mostrano l’ora in più città. Puoi creare un campo per ciascuno dei fusi orari in cui lavorano gli utenti, ognuno dei quali calcola l’ora per il proprio fuso orario.

Per ulteriori informazioni, consulta [Aggiungere dati calcolati a un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md), nonché la sezione [Campi personalizzati calcolati per data e ora](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) nell’articolo [Panoramica delle espressioni di dati calcolati](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Utilizzare campi di testo invece di campi data in un modulo personalizzato {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Se non vuoi [!DNL Workfront] per convertire gli orari configurati per in un oggetto per utenti con fusi orari diversi, è possibile utilizzare un campo di testo in un modulo personalizzato da allegare a un oggetto, anziché un campo data. In questo modo, viene visualizzato il tempo digitato per tutti gli utenti del progetto.

In questo caso, si consiglia di ricordare agli utenti del modulo di calcolare la differenza tra il proprio fuso orario e quello dell&#39;utente, in modo che possano determinare quando iniziare e terminare il lavoro. È possibile includerlo nelle istruzioni digitate per il modulo personalizzato o in una descrizione comando per tale campo. Per ulteriori informazioni, consulta [Aggiungere un campo personalizzato a un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
