---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Utilizzo dei fusi orari
description: Può essere utile capire come [!DNL Adobe Workfront] utilizza i fusi orari per calcolare i campi di tempo per gli oggetti e gli orari in altre aree, ad esempio le e-mail.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: ef7f5d00bd74feee5e06b935c4bb8a18ee8b08a8
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 0%

---

# Utilizzo dei fusi orari

<!-- Audited: 2/2024 -->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Può essere utile capire in che modo [!DNL Adobe Workfront] utilizza i fusi orari per calcolare quanto segue:

* Campi di tempo per gli oggetti
* Ore in altre aree [!DNL Workfront], ad esempio e-mail Workfront automatizzate

>[!WARNING]
>
>Se non riesci a trovare il tuo fuso orario esatto nell’elenco che ti forniamo, individua quello più vicino e aggiornalo per la tua istanza.
>
>Inoltre, considera che un fuso orario simile potrebbe non corrispondere perfettamente al tuo.
>
>Ad esempio, alcuni paesi o territori potrebbero osservare l&#39;ora legale, ma il tuo paese potrebbe non farlo. Se necessario, potrebbe essere necessario regolare i fusi orari del sistema in base a queste modifiche.


## Fusi orari in [!DNL Workfront]

Gli orari visualizzati in [!DNL Workfront] si basano sulle configurazioni del fuso orario per l&#39;istanza [!DNL Workfront] dell&#39;organizzazione e per il profilo utente. Se questi due fusi orari sono diversi, è possibile che si verifichino discrepanze di orario in aree e funzionalità diverse utilizzate in [!DNL Workfront].

>[!NOTE]
>
>In un modulo personalizzato allegato a un oggetto, le istruzioni di data e ora nei campi personalizzati calcolati vengono calcolate e salvate in base al tempo UTC (Coordinated Universal Time) e non in base alle configurazioni del fuso orario impostate per l’istanza della tua organizzazione e il tuo profilo utente. I calcoli in un modulo personalizzato vengono generati e visualizzati in base ai singoli fusi orari degli utenti.

* [Istanza  [!DNL Workfront]  della tua organizzazione](#your-organization-s-workfront-instance)
* [Il tuo profilo utente](#your-user-profile)

### Istanza [!DNL Workfront] della tua organizzazione {#your-organization-s-workfront-instance}

Il fuso orario per l&#39;istanza [!DNL Workfront] dell&#39;organizzazione è in genere impostato per l&#39;ubicazione dell&#39;ufficio principale. Questo determina quanto segue:

* Ora visualizzata nelle e-mail generate da [!DNL Workfront]
* Il fuso orario per gli utenti appena aggiunti (prima che l&#39;amministratore [!DNL Workfront] configuri un fuso orario diverso per gli utenti in base alla loro posizione di lavoro)

  Per ulteriori informazioni su questi due esempi, vedere [Configurare le informazioni di base per il sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* L’inizio o la fine di una tariffa di fatturazione sostituita per un progetto. Per ulteriori informazioni, vedere [Sostituire le tariffe di fatturazione dei ruoli a livello di progetto](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Il tuo profilo utente {#your-user-profile}

Il fuso orario nel profilo utente deve essere configurato per la posizione in cui lavori. Questo determina quanto segue:

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Ore per un oggetto su cui si lavora, ad esempio ore di inizio e di fine

  Se a un oggetto vengono assegnati utenti con più fusi orari, [!DNL Workfront] converte gli orari dell&#39;oggetto per tutti gli utenti coinvolti, utilizzando il fuso orario configurato in ciascun profilo utente.

  **Esempio:** Nella zona dell&#39;ora solare orientale (EST) in cui si lavora, impostare un&#39;attività affinché inizi alle 16:00 e assegnarla agli utenti che lavorano nella zona dell&#39;ora solare del Pacifico (PST). Per tali utenti, l’ora di inizio viene visualizzata come 1:00 PM. Se la visualizzasse alle 16:00, inizierebbe a lavorarci con tre ore di ritardo.

  Se il creatore dell&#39;oggetto non rileva la differenza tra i fusi orari degli assegnatari e apporta le modifiche necessarie durante l&#39;impostazione degli orari degli oggetti o se gli assegnatari non notano tale differenza, può essere difficile ottenere gli intervalli corretti mentre tutti collaborano all&#39;oggetto.

  **Esempio:** è possibile configurare un&#39;attività di un giorno affinché inizi alle 9.00 EST, dimenticando che alcuni utenti dell&#39;attività lavorano nella zona PST. Per loro, l&#39;ora di inizio 6:00 AM. Poiché non inizieranno a lavorarci fino alle 9:00 (mezzogiorno del tuo orario), l’attività inizia e termina con tre ore di ritardo.

Per informazioni sulla configurazione del fuso orario nel profilo utente, vedere [Configurare le impostazioni personali](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Per informazioni su come un amministratore [!DNL Workfront] (o un utente con accesso [!UICONTROL Modifica] agli utenti) può configurare il fuso orario in un profilo utente, vedi [Modifica del profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Come semplificare il lavoro degli utenti in più fusi orari

Puoi aiutare gli utenti a lavorare più facilmente in diversi fusi orari in diversi modi:

* [Usa pianificazioni](#use-schedules)
* [Utilizzare i campi tempo calcolati in un modulo personalizzato](#use-calculated-time-fields-in-a-custom-form)
* [Utilizzare campi di testo invece di campi data in un modulo personalizzato](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Usa pianificazioni {#use-schedules}

Gli amministratori di [!DNL Workfront] creano pianificazioni separate per ogni fuso orario all&#39;interno dell&#39;organizzazione per garantire che il lavoro sia pianificato in modo appropriato per tutti, ovunque si trovino. Dopo che l’amministratore ha creato le pianificazioni, queste possono essere associate a determinati progetti e utenti:

* **[!UICONTROL Progetti]**: il creatore di un progetto può selezionare una pianificazione per un singolo progetto. Determina la programmazione delle attività del progetto, in base alle ore lavorative impostate per i fusi orari degli assegnatari.
* **[!UICONTROL Utenti]**: un amministratore [!DNL Workfront] (o un utente con accesso [!UICONTROL Modifica] agli utenti) può selezionare una pianificazione per il singolo utente nel profilo dell&#39;utente.

  Questa pianificazione potrebbe essere diversa da quella di un progetto. Se ad esempio un utente crea un&#39;attività nel progetto e non ne ha ancora assegnata alcuna, l&#39;attività utilizzerà la pianificazione del progetto. Quando un utente viene assegnato all’attività, questa utilizza la pianificazione dell’utente.

  Se a un&#39;attività sono assegnati più utenti, il sistema utilizza uno dei seguenti elementi, come configurato nelle preferenze di progetto a livello di sistema o di gruppo:

   * Fuso orario per la pianificazione del proprietario principale dell&#39;attività
   * Il fuso orario per la pianificazione del progetto.

  <div class="preview">

  Se a un&#39;attività è assegnato un utente, il sistema utilizza uno dei seguenti elementi, come configurato nelle preferenze di progetto a livello di sistema o di gruppo:

   * Fuso orario per la pianificazione dell&#39;assegnatario dell&#39;attività
   * Il fuso orario per la pianificazione del progetto.

  </div>

  Questo può causare la modifica delle date delle attività.

>[!BEGINSHADEBOX]

**ESEMPIO:**
Un utente EST è assegnato a un&#39;attività di un giorno pianificata per iniziare alle 09:00 PST, che è mezzogiorno EST. Poiché all&#39;utente EST rimangono solo 2 ore lavorative al giorno, la data di completamento dell&#39;attività viene estesa di circa 6 ore al giorno lavorativo successivo.


>[!ENDSHADEBOX]

Per informazioni sull&#39;area [!UICONTROL Preferenze progetto] di [!UICONTROL Configurazione], vedere [Configurare le preferenze di progetto a livello di sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Per istruzioni sull&#39;assegnazione di una pianificazione a un progetto o a un utente, vedere [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Per informazioni su come il fuso orario configurato nella pianificazione influisce sulla distribuzione di [!UICONTROL Ore pianificate] nel [!UICONTROL Bilanciatore dei carichi di lavoro], vedi [Gestione delle allocazioni utente nel [!UICONTROL Bilanciatore dei carichi di lavoro]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Utilizzare i campi tempo calcolati in un modulo personalizzato {#use-calculated-time-fields-in-a-custom-form}

È possibile utilizzare una serie di campi personalizzati calcolati in un modulo personalizzato per visualizzare l’ora corrente per gli utenti dell’organizzazione, ad esempio una riga di orologi aeroportuali che mostrano l’ora in più città. Puoi creare un campo per ciascuno dei fusi orari in cui lavorano gli utenti, ognuno dei quali calcola l’ora per il proprio fuso orario.

Per ulteriori informazioni, vedere [Aggiungere campi calcolati a un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md), nonché la sezione [Campi personalizzati calcolati per data e ora](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) nell&#39;articolo [Panoramica delle espressioni di dati calcolati](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Utilizzare campi di testo invece di campi data in un modulo personalizzato {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Se non si desidera che [!DNL Workfront] converta gli orari configurati per in un oggetto per utenti con fusi orari diversi, è possibile utilizzare un campo di testo in un modulo personalizzato allegato a un oggetto, anziché un campo data. In questo modo, viene visualizzato il tempo digitato per tutti gli utenti del progetto.

In questo caso, si consiglia di ricordare agli utenti del modulo di calcolare la differenza tra il proprio fuso orario e quello dell&#39;utente, in modo che possano determinare quando iniziare e terminare il lavoro. È possibile includerlo nelle istruzioni digitate per il modulo personalizzato o in una descrizione comando per tale campo. Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
