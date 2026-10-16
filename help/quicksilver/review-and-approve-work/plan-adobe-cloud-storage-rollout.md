---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Pianifica il rollout dell’archiviazione cloud Adobe
description: Scegli in che modo l’archiviazione cloud di Adobe viene visualizzata agli utenti, eseguendo un test con un singolo gruppo e sequenziando il lavoro in modo da evitare sorprese per revisori, approvatori e proprietari dei progetti.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
exl-id: b4413742-c250-4110-9097-6d38842355a4
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 0%

---
# Pianifica il rollout dell’archiviazione cloud Adobe

Decidi come e quando l’archiviazione cloud di Adobe raggiunge i tuoi utenti. Nulla cambia finché un amministratore di Workfront non imposta Adobe Cloud Storage come opzione di archiviazione predefinita nell’area di configurazione, in modo da avere il tempo di testare l’esperienza e preparare i team prima che chiunque vi lavori.

Questo articolo descrive le configurazioni di rollout che puoi scegliere, come eseguire il test pilota con un singolo gruppo e un ordine di lavoro suggerito.

## Scegli come viene eseguito il rollout dell’archiviazione cloud di Adobe

Esistono due configurazioni e puoi applicarne una all’intera organizzazione o a gruppi Workfront specifici. Per impostazione predefinita, ogni progetto creato nell’archiviazione cloud di Adobe utilizza le approvazioni unificate e il visualizzatore Frame.io.

Per istruzioni dettagliate, consulta [Abilitare l&#39;archiviazione cloud Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

### Opzioni di configurazione

* **Solo archiviazione cloud Adobe**: per impostazione predefinita, i nuovi progetti utilizzano l&#39;archiviazione cloud Adobe. Gli utenti non possono creare progetti legacy.
* **Archiviazione cloud Adobe e archiviazione Workfront legacy**: quando gli utenti creano un progetto, scelgono tra l&#39;archiviazione cloud Adobe (con etichetta &quot;Nuovo progetto&quot;) e l&#39;archiviazione Workfront legacy (con etichetta &quot;Archiviazione legacy&quot;). Questa opzione è abilitata selezionando la casella di controllo **Consenti all&#39;utente di selezionare il provider di archiviazione** nell&#39;area di installazione.

>[!TIP]
>
>Per mettere l’archiviazione cloud di Adobe prima di un team più piccolo, applica una delle due configurazioni a un singolo gruppo Workfront. Questo consente di eseguire un programma pilota mirato prima di implementarlo in modo più ampio. Per una valutazione controllata, consigliamo di iniziare con un rollout a livello di gruppo, quindi di espanderlo all’intera organizzazione una volta che il gruppo pilota avrà convalidato l’esperienza.

Gli oggetti esistenti mantengono il modello di archiviazione con cui sono stati creati. La modifica della preferenza di archiviazione predefinita non comporta la modifica di alcun oggetto esistente.

![preferenze di archiviazione in configurazione](assets/storage-preference-groups.png)

## Pianificare il rollout

Ogni ambiente Workfront è diverso. Prima di impostare l’archiviazione cloud di Adobe come predefinita per gli utenti, pianifica l’aspetto di un rollout di successo per la tua organizzazione. I suggerimenti riportati di seguito non sono una lista di controllo esatta, ma un punto di partenza per il tuo piano.

### Scegli un gruppo pilota

Un rollout con ambito di gruppo consente di mettere l’archiviazione cloud Adobe prima di un team più piccolo, raccogliere feedback e apportare le modifiche necessarie prima di un rollout più ampio. Scegli un gruppo i cui modelli di lavoro siano sufficientemente rappresentativi da far emergere i problemi che desideri conoscere in anticipo.

### Esegui il test prima della pubblicazione

L’archiviazione cloud di Adobe è disponibile in ambienti sandbox Workfront, per cui puoi convalidare gran parte dell’esperienza prima della produzione. Il visualizzatore Frame.io non è disponibile in sandbox, pertanto puoi convalidare l’esperienza di revisione e approvazione completa in produzione con il gruppo pilota. Per ulteriori informazioni, consulta [Abilitare l&#39;archiviazione cloud Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

### Comunicare la modifica agli utenti finali

La più grande modifica visibile per revisori, approvatori e proprietari di progetti è la nuova area Documenti e il visualizzatore Frame.io che consente la revisione e l’approvazione sui progetti di archiviazione cloud Adobe. Pianifica come presentarli in modo che gli utenti sappiano cosa aspettarsi quando incontrano il loro primo progetto di archiviazione cloud Adobe. L&#39;articolo [Introduzione a revisione e approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) è un utile punto di partenza per il materiale rivolto all&#39;utente finale.

### Rivedere le autorizzazioni e la governance

Nei progetti Adobe di archiviazione cloud, sia Manage che Contribute mappano a Edit &amp; Share in Frame.io, che include la condivisione esterna. Rivedi i pattern di condivisione e decidi se si adattano al modello di governance prima di portare i team nell’archiviazione cloud di Adobe. Per ulteriori informazioni, consulta [Differenze nell&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-permissions-mapping).

### Modelli di controllo e denominazione

L’archiviazione cloud di Adobe applica regole di denominazione severe e Workfront rinomina automaticamente gli oggetti in conflitto con essi. Se crei progetti a partire da modelli, rivedi tali modelli in modo che i nomi e la struttura da essi generati siano conformi alle regole. Per ulteriori informazioni, consulta [Differenze nell&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-naming-rules).

### Pianificare Workfront Fusion

Gli scenari di Fusion basati su bozze esistenti continuano a funzionare sui progetti legacy, ma non sui progetti di archiviazione cloud Adobe. Prima di trasferire i team che dipendono da tali scenari nell’archiviazione cloud di Adobe, classifica ogni scenario come Modifica, Ricostruisci o Ritira. Per ulteriori informazioni, vedere [Aggiornare gli scenari di Workfront Fusion per la revisione e l&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).

### Piano per la generazione di rapporti sulle modifiche

I dati del flusso di lavoro di approvazione e reporting unificati vengono visualizzati nei dashboard di Canvas. I rapporti di approvazione legacy non vengono trasferiti automaticamente, pertanto imposta un dashboard di sostituzione prima che il team pilota ne abbia bisogno. Per ulteriori informazioni, vedere [Creare un dashboard report per la revisione e le approvazioni](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

## Sequenza suggerita

Utilizza questo ordine come modello, adattandolo al tuo ambiente:

1. Prova l’esperienza in una sandbox e con un gruppo pilota in produzione.
2. Classifica e aggiorna gli scenari di Fusion e crea i rapporti delle dashboard di Canvas.
3. Controlla i modelli e rivedi le autorizzazioni e il modello di condivisione.
4. Comunica la modifica ai revisori, agli approvatori e ai proprietari dei progetti che la utilizzeranno.
5. Imposta l’archiviazione cloud di Adobe come predefinita per il gruppo pilota, quindi espandi a più gruppi o all’intera organizzazione una volta che il pilota convalida l’esperienza.
