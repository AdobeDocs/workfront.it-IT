---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Panoramica sul lavoro dei delegati
description: Quando prevedi di uscire dall'ufficio per un breve periodo di tempo, puoi delegare temporaneamente il tuo lavoro ad altri utenti per evitare che la tua assenza diventi un ostacolo al completamento del lavoro.
author: Becky
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: 9cdf3d78e1d19f3d581f8d527919a608c5cc0ddc
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 1%

---

# Panoramica sul lavoro dei delegati

Quando prevedi di uscire dall&#39;ufficio per un breve periodo di tempo, puoi delegare temporaneamente il tuo lavoro ad altri utenti per evitare che la tua assenza diventi un ostacolo al completamento del lavoro.

Ad esempio, se alcune attività sono in scadenza prima della restituzione ma non si dispone del tempo necessario per completarle prima di uscire, è possibile delegare le attività a un altro utente in modo che possano essere completate in tempo e non ritardare il completamento del progetto fino a dopo la restituzione.

È possibile delegare i seguenti oggetti in [!DNL Adobe Workfront]:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Attività assegnate a te
* Problemi assegnati a te
* Le approvazioni di progetti, attività o problemi che ti sono state assegnate.

  >[!TIP]
  >
  >   Non puoi delegare le approvazioni di schede orario, documenti o bozze.


Questo articolo contiene informazioni generali sulla delega di attività e problemi assegnati all&#39;utente.

Per informazioni sulla delega delle approvazioni di progetti, attività e problemi, vedere [Delegare la richiesta di approvazione](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Per informazioni su come delegare attività e problemi, vedere [Delegare attività e problemi](../../manage-work/delegate-work/how-to-delegate-work.md).

## Panoramica su delega attività e problemi

Quando deleghi attività e problemi, tieni presente quanto segue:

* L&#39;amministratore di [!DNL Workfront] o del gruppo deve abilitare le preferenze di delega nell&#39;area [!UICONTROL Configurazione] prima di poter delegare il lavoro ad altri.

  Per informazioni, consulta [Configurare le preferenze per attività e problemi a livello di sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Puoi delegare attività e problemi solo dall&#39;area [!UICONTROL Home].
* Quando si delega un lavoro, sono presenti eccezioni per i seguenti tipi di licenza:

   * Puoi delegare il lavoro a revisori o richiedenti, anche se [!DNL Workfront] non lo consiglia.
   * I revisori possono delegare il lavoro ad altri. Non possono visualizzare gli elementi di lavoro nella loro area [!UICONTROL Home]. Possono visualizzare solo le approvazioni.
   * I richiedenti non possono delegare il lavoro ad altri. Non possono visualizzare gli elementi di lavoro nella loro area [!UICONTROL Home]
* Puoi delegare solo le attività e i problemi assegnati a te. Non puoi delegare attività e problemi assegnati ad altri utenti, team o mansioni.
* Puoi delegare solo attività e problemi non completati prima della data di inizio della delega.
* Se un elemento di lavoro viene completato durante il periodo di delega, l&#39;elemento rimane nell&#39;area Home del delegato e dell&#39;assegnatario per 2 settimane prima che [!DNL Workfront] lo rimuova automaticamente.
* Gli utenti che selezioni come delegati ricevono le stesse autorizzazioni delle tue autorizzazioni per le attività e i problemi che deleghi loro. Le autorizzazioni devono funzionare all’interno dei loro livelli di accesso e a volte i loro livelli di accesso potrebbero essere inferiori ai tuoi.

>[!NOTE]
>
>  Per gli elementi che vengono assegnati dopo l&#39;avvio della delega, può essere necessaria un&#39;ora dopo l&#39;assegnazione dell&#39;elemento per [!DNL Workfront] per condividere gli elementi appena assegnati con il delegato.

* Se durante il periodo di tempo selezionato per la delega del lavoro ad altri utenti vengono assegnate attività e problemi aggiuntivi, il nuovo lavoro assegnato viene delegato automaticamente alla stessa persona per l&#39;intervallo di tempo selezionato, se le date dell&#39;attività o del problema sono comprese in tale intervallo di tempo.
* Più utenti possono selezionare come delegato lo stesso utente.
* Le attività e i problemi delegati non vengono visualizzati negli strumenti di gestione delle risorse, come il [!UICONTROL Bilanciatore dei carichi di lavoro] o il [!UICONTROL Pianificazione risorse] per gli utenti delegati.
* È possibile visualizzare i nomi dei delegati e dei lavori delegati in diverse aree di [!DNL Workfront]. Per ulteriori informazioni, vedere la sezione &quot;Individuare le informazioni sul lavoro delegato e sui delegati&quot; nell&#39;articolo [Delegare attività e problemi](../delegate-work/how-to-delegate-work.md).


  >[!IMPORTANT]
  >
  >  Se un utente dispone solo dell&#39;accesso di visualizzazione alle attività nel proprio livello di accesso e si dispone delle autorizzazioni di gestione per le attività delegate, riceverà le autorizzazioni di gestione per le attività delegate. Tuttavia, non potranno eseguire le stesse azioni che esegui sulle attività delegate. Devono richiedere all&#39;amministratore di sistema l&#39;accesso di modifica alle attività per poter aggiornare le attività in assenza dell&#39;utente.

* L&#39;arresto della delega non rimuove le autorizzazioni concesse agli utenti delegati sulle attività e sui problemi per i quali sono stati delegati.
* Se un sistema o disabilita l&#39;impostazione [!UICONTROL Consenti agli utenti di delegare le attività e i problemi] nell&#39;area [!UICONTROL Configurazione], gli utenti attualmente delegati vengono rimossi dalle attività e dai problemi a cui erano stati delegati in precedenza. Le autorizzazioni per le attività o i problemi non vengono rimosse.

## Differenze e analogie tra assegnazioni e deleghe

| Azione | Assegnazioni | Deleghe |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Un utente assegnato o delegato può modificare o eliminare l&#39;elemento di lavoro a cui è assegnato o delegato | In base alle autorizzazioni e al livello di accesso | In base alle autorizzazioni e al livello di accesso |
| Un utente assegnato o delegato viene visualizzato nell&#39;intestazione dell&#39;elemento di lavoro | Sì | Sì |
| Le attività o i problemi assegnati o delegati vengono visualizzati nell&#39;area Home dell&#39;assegnatario o del delegato | Sì, fino al completamento dell&#39;elemento | Sì, solo per l’intervallo di tempo della delega |
| È possibile assegnare o delegare il lavoro agli utenti dall&#39;area Home | Sì | Sì |
| Puoi assegnare o delegare il lavoro agli utenti utilizzando | Sì | No |
| È possibile assegnare o delegare il lavoro agli utenti di un elenco o dall&#39;intestazione di un elemento di lavoro | Sì | No |
| Qualsiasi utente può assegnare o delegare altri utenti con elementi di lavoro a cui non è associato | In base alle autorizzazioni e al livello di accesso | No. Solo l’assegnatario può delegare i propri elementi. |
| Le ore pianificate, effettive o preventivate per il lavoro assegnato o delegato a un utente vengono visualizzate per tale utente negli strumenti di gestione delle risorse | Sì | No |
