---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Panoramica sul lavoro dei delegati
description: Quando prevedi di uscire dall'ufficio per un breve periodo di tempo, puoi delegare temporaneamente il tuo lavoro ad altri utenti per evitare che la tua assenza diventi un ostacolo al completamento del lavoro.
author: Becky
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/O-G3HS2JWZB36Y-kSloHo6u4--Z3q40fwAgfcEuELi4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: c33d85a1-be85-4290-854c-87408c10aa80
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 906
ht-degree: 2%

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

## Panoramica su come delegare attività e problemi

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
| Puoi assegnare o delegare il lavoro agli utenti utilizzando il Bilanciatore dei carichi di lavoro | Sì | No |
| È possibile assegnare o delegare il lavoro agli utenti di un elenco o dall&#39;intestazione di un elemento di lavoro | Sì | No |
| Qualsiasi utente può assegnare o delegare altri utenti con elementi di lavoro a cui non è associato | In base alle autorizzazioni e al livello di accesso | No. Solo l’assegnatario può delegare i propri elementi. |
| Le ore pianificate, effettive o preventivate per il lavoro assegnato o delegato a un utente vengono visualizzate per tale utente negli strumenti di gestione delle risorse | Sì | No |
