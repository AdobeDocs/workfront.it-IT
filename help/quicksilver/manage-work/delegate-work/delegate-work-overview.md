---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Panoramica sul lavoro delegato
description: Quando prevedi di uscire dall'ufficio per un breve periodo di tempo, puoi delegare temporaneamente il tuo lavoro ad altri utenti per assicurarti che la tua assenza non diventi un ostacolo al lavoro da completare.
author: Alina
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: f3ae487f53f7c4f8c389cf0d35323f21e76ece35
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 1%

---

# Panoramica sul lavoro delegato

Quando prevedi di uscire dall&#39;ufficio per un breve periodo di tempo, puoi delegare temporaneamente il tuo lavoro ad altri utenti per assicurarti che la tua assenza non diventi un ostacolo al lavoro da completare.

Ad esempio, se alcune attività sono dovute prima della restituzione ma non si dispone del tempo necessario per completarle prima di uscire, è possibile delegare le attività a un altro utente in modo che possano essere completate in tempo e non ritardare il completamento del progetto fino a quando non si ritorna.

Puoi delegare i seguenti oggetti in [!DNL Adobe Workfront]:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Attività assegnate
* Problemi assegnati
* Progetto, task, problema, approvazioni di documenti assegnati all&#39;utente.

Questo articolo contiene informazioni generali sulla delega di attività e problemi.

Per informazioni sulla delega delle approvazioni di progetti, task, problemi e documenti, vedere [Delega richiesta di approvazione](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Per informazioni su come delegare attività e problemi consulta [Delega di compiti e problemi](../../manage-work/delegate-work/how-to-delegate-work.md).

## Panoramica sul lavoro delegato

Quando deleghi attività e problemi, considera quanto segue:

* Le [!DNL Workfront] o l&#39;amministratore del gruppo deve abilitare le preferenze di delega nel [!UICONTROL Configurazione] prima di poter delegare il lavoro ad altri.

   Per informazioni, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Puoi delegare attività e problemi solo dal [!UICONTROL Pagina principale] area.
* Sono presenti eccezioni per i seguenti tipi di licenza:

   * Puoi delegare il lavoro a Revisori o Richiedenti, anche se [!DNL Workfront] non la consiglia.
   * I revisori possono delegare il lavoro ad altri. Non possono visualizzare gli elementi di lavoro [!UICONTROL Pagina principale] area. Possono visualizzare solo le approvazioni.
   * I richiedenti non possono delegare il lavoro ad altri. Non possono visualizzare gli elementi di lavoro [!UICONTROL Pagina principale] area
* Puoi delegare solo le attività e i problemi assegnati. Non è possibile delegare attività e problemi assegnati ad altri utenti, team o ruoli di lavoro.
* Puoi delegare solo le attività e i problemi che non vengono completati prima della data di inizio della delega.
* Se un elemento di lavoro viene completato durante l&#39;intervallo di tempo di delega, l&#39;elemento rimane nell&#39;area Home del delegato e del assegnatario per 2 settimane prima [!DNL Workfront] la rimuove automaticamente.
* Gli utenti selezionati come delegati ricevono le stesse autorizzazioni delle tue autorizzazioni sulle attività e sui problemi che deleghi loro. Le autorizzazioni devono funzionare entro i loro livelli di accesso e a volte i loro livelli di accesso potrebbero essere inferiori ai tuoi.

>[!NOTE]
>
>  Per gli elementi assegnati dopo l&#39;avvio della delega, può essere necessaria fino a un&#39;ora dopo l&#39;assegnazione dell&#39;elemento [!DNL Workfront] per condividere gli elementi appena assegnati con il delegato.

* Se durante il periodo di tempo selezionato per la delega del lavoro ad altri utenti vengono assegnate attività e problemi aggiuntivi, il nuovo lavoro assegnato viene automaticamente delegato alla stessa persona per l&#39;intervallo di tempo selezionato se le date del task o del problema si trovano entro tale intervallo di tempo.
* Lo stesso utente può essere selezionato come delegato da più utenti.
* Le attività e i problemi delegati non vengono visualizzati negli strumenti di gestione delle risorse, come [!UICONTROL Bilanciamento del carico di lavoro] o [!UICONTROL Planner risorse] per gli utenti delegati.
* Puoi visualizzare i nomi dei delegati e dei lavori delegati in diverse aree di [!DNL Workfront]. Per ulteriori informazioni, consulta la sezione &quot;Individuare informazioni sul lavoro delegato e delegare&quot; nell’articolo [Gestione dell&#39;attività e della delega dei problemi](../delegate-work/how-to-delegate-work.md).


   >[!IMPORTANT]
   >
   >  Se un utente dispone solo dell&#39;accesso Visualizza alle attività nel proprio livello di accesso e si dispone delle autorizzazioni Gestione per le attività che si delegano, riceverà le autorizzazioni Gestisci per le attività che si delegano a tali attività. Tuttavia, non saranno in grado di eseguire le stesse azioni eseguite dall’utente sulle attività delegate. Per poter aggiornare le attività in assenza, è necessario che l&#39;amministratore di sistema richieda l&#39;accesso a Modifica attività.

* L’arresto della delega non rimuove le autorizzazioni assegnate agli utenti delegati sulle attività e sui problemi per i quali sono stati delegati.
* Se un sistema o disabilita [!UICONTROL Consenti agli utenti di delegare le loro attività e i loro problemi] nella [!UICONTROL Configurazione] , gli utenti attualmente delegati vengono rimossi dalle attività e dai problemi a cui erano stati precedentemente delegati. Le loro autorizzazioni per le attività o i problemi non vengono rimosse.

## Differenze e somiglianze tra assegnazioni e delegazioni

| Azione | Assegnazioni | Deleghe |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Un utente assegnato o delegato può modificare o eliminare l’elemento di lavoro a cui è assegnato o delegato | In base a autorizzazioni e livello di accesso | In base a autorizzazioni e livello di accesso |
| Un utente assegnato o delegato viene visualizzato nell’intestazione dell’elemento di lavoro | Sì | Sì |
| Le attività o i problemi assegnati o delegati vengono visualizzati nell&#39;area Home del cessionario o del delegato | Sì, fino al completamento dell&#39;elemento | Sì, solo per l&#39;intervallo di tempo della delega |
| È possibile assegnare o delegare il lavoro agli utenti dall&#39;area Home | Sì | Sì |
| Puoi assegnare o delegare il lavoro agli utenti utilizzando | Sì | No |
| È possibile assegnare o delegare il lavoro agli utenti di un elenco o dall&#39;intestazione di un elemento di lavoro | Sì | No |
| Qualsiasi utente può assegnare o delegare altri utenti con elementi di lavoro a cui non è associato | In base a autorizzazioni e livello di accesso | No. Solo l&#39;assegnatario può delegare i propri elementi. |
| Ore pianificate, effettive o previste per il lavoro assegnato o delegato a un utente per tale utente in strumenti di gestione delle risorse | Sì | No |
