---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Gestire le licenze disponibili nel sistema
description: In qualità di amministratore di Adobe Workfront, puoi accedere a informazioni sul tuo account Workfront, compreso il numero di licenze acquistate per la tua organizzazione e il numero di tali licenze attualmente in uso.
author: Lisa, Becky
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1216'
ht-degree: 0%

---

# Gestire le licenze disponibili nel sistema

<!-- Audited: 12/2023 -->

In qualità di amministratore di Adobe Workfront, puoi accedere a informazioni sul tuo account Workfront, compreso il numero di licenze acquistate per la tua organizzazione e il numero di tali licenze attualmente in uso.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
    <p>Nuovo: Standard</p>
    <p>oppure</p>
    <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di sistema o un amministratore di gruppo. L'amministratore del gruppo ha una visualizzazione limitata delle informazioni sulla licenza.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

>[!NOTE]
>
>Le seguenti istruzioni sono valide solo per i nuovi piani.
>
>Per il piano Select:
>
>1. Gli amministratori di sistema non possono impostare limiti per i gruppi home.
>2. Gli amministratori di sistema possono visualizzare solo il numero totale di licenze utilizzate in tutti i gruppi home.
>3. Gli amministratori di gruppi non possono accedere alla pagina Licenze.
>
>Per i piani di Prime e Ultimate:
>
>1. Gli amministratori di sistema possono aggiungere gruppi predefiniti alla pagina Licenze per visualizzare l&#39;utilizzo delle licenze in tali gruppi e impostare i limiti di licenza.
>2. Gli amministratori di gruppi possono accedere alla pagina Licenze e visualizzare l&#39;utilizzo delle licenze dei gruppi da loro gestiti che sono state aggiunte alla pagina Licenze dagli amministratori di sistema.
>3. Gli amministratori di gruppi non possono visualizzare informazioni per altri gruppi Home o aggiungere valori massimi.

+++

## Visualizzare le licenze della tua organizzazione

Il numero di licenze in uso viene aggiornato automaticamente quando si assegnano i livelli di accesso agli utenti aggiunti a Workfront. Per ulteriori informazioni, vedere [Aggiungere utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Per visualizzare le informazioni sulle licenze nel sistema:

{{step-1-to-setup}}

1. Nella parte inferiore del pannello a sinistra, fai clic su **Sistema** > **Licenze**.

   Per ulteriori informazioni sulle licenze elencate in questa pagina, vedere [Panoramica sulle licenze](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >Le licenze Verifica sono disponibili solo per i clienti che hanno acquistato a pagamento il componente aggiuntivo Workfront Proof oltre alla licenza Workfront. Per informazioni su questo componente aggiuntivo, vedere [Workfront Proof: article index](../../workfront-proof/workfront-proof.md).

1. (Condizionale) Se viene visualizzato il messaggio **Per impostare un massimo, è necessario aggiungere un gruppo predefinito**, aggiungere un gruppo predefinito nel sistema come descritto nella sezione [Aggiungere o rimuovere un gruppo predefinito nella pagina Licenze](#add-or-remove-a-home-group-to-the-licenses-page) di questo articolo.

   >[!NOTE]
   >
   >Per i nuovi piani, il piano Select non consente agli amministratori di visualizzare le licenze per gruppo predefinito. È possibile visualizzare solo il numero complessivo di licenze utilizzate. I piani di Prime e Ultimate consentono di impostare il numero massimo di licenze per gruppo predefinito.

## Visualizzare informazioni sulle licenze per i componenti aggiuntivi di Workfront

Se l&#39;organizzazione dispone del componente aggiuntivo a pagamento Workfront Proof, vengono visualizzati il numero di licenze utilizzate e il numero di licenze disponibili. Ad esempio, **5 delle 10 licenze di verifica** indica che l&#39;organizzazione sta attualmente utilizzando 5 delle 10 licenze di Workfront Proof acquistate.

![Licenza per i componenti aggiuntivi di Workfront](assets/updated-licenses-page.png)

Se la tua organizzazione ha acquistato Workfront Goals, qui vengono visualizzate anche le informazioni sulla licenza per questo prodotto. In questo caso, puoi visualizzare le seguenti informazioni:

* Numero totale di licenze Workfront Goals acquistate dalla società
* Il numero di licenze Workfront Goals associate agli utenti. Questo è il numero di utenti a cui è stato concesso almeno l’accesso di visualizzazione agli obiettivi nel rispettivo livello di accesso.

Per informazioni sugli obiettivi di Workfront, consulta [Panoramica sugli obiettivi di Adobe Workfront](../../workfront-goals/goal-management/wf-goals-overview.md). Per informazioni sull&#39;accesso agli obiettivi di Workfront, vedere [Concedere l&#39;accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

>[!NOTE]
>
>Workfront consente di assegnare più licenze Workfront Goals acquistate. Tuttavia, quando si assegnano più licenze di quelle consentite dal contratto Workfront Goals, un account manager Workfront contatterà l&#39;utente per informarlo del superamento del numero di contratto.
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>Gli utenti senza accesso amministrativo possono utilizzare un rapporto di gruppo per visualizzare il numero di licenze. Nella scheda Rapporto, crea un nuovo rapporto di gruppo e aggiungi le colonne seguenti:
>
>* Limite tipo di licenza: limite lavoratore
>* Limite tipo di licenza: Limite planner
>
>Per ulteriori informazioni sulla creazione di un report, vedere [Creare un report personalizzato](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Visualizza informazioni sulle assegnazioni di bozze e documenti decisionali mensili

>[!IMPORTANT]
>
>I limiti di decisione per bozze e documenti si applicano solo agli utenti delle nuove licenze. Per ulteriori informazioni, vedere [Panoramica delle nuove licenze](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

Le decisioni su bozze e documenti sono limitate per tutte le licenze Workfront non a pagamento. Limiti reimpostati per ogni utente ogni mese.

I limiti di decisione per ogni licenza variano a seconda del piano su cui stai lavorando. Puoi visualizzare l’assegnazione mensile in Configurazione > Licenze.

Per ulteriori informazioni sui limiti di decisione per bozze e documenti, consulta [Panoramica su documenti e bozze con limitazioni per utenti non pagati](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

![Ripartizione mensile delle decisioni](assets/monthly-decision-allotment.png)

## Aggiungere o rimuovere un gruppo predefinito nella pagina Licenze {#add-or-remove-a-home-group-to-the-licenses-page}

<!--A Business or Enterprise Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)-->

Ogni utente può essere assegnato a un solo Gruppo Predefinito. Workfront fornisce un conteggio delle licenze orientato al gruppo calcolando il numero di licenze allocate e attualmente utilizzate in ciascun Gruppo predefinito.

Se viene visualizzato il messaggio **Per impostare un massimo, è necessario aggiungere un gruppo predefinito** nella pagina Licenze, è necessario aggiungere almeno un gruppo predefinito alla pagina Licenze.

>[!IMPORTANT]
>
>* Per gestire in modo efficace le licenze con i gruppi home, si consiglia di impostare gruppi home specifici per le unità aziendali prima di aggiornare il numero massimo di licenze. Per ulteriori informazioni, vedere [Panoramica sui gruppi principali](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* È possibile aggiungere solo i gruppi di primo livello come gruppi principali, non i sottogruppi. Se a un utente è assegnato un sottogruppo come Gruppo predefinito, la licenza viene aggiunta al numero di licenze per il gruppo di livello superiore al di sopra di tale sottogruppo.
>

Per aggiungere o rimuovere un gruppo predefinito nella pagina Licenze:

{{step-1-to-setup}}

1. Nella parte inferiore del pannello a sinistra, fai clic su **Sistema** > **Licenze**.

1. Fare clic su **Gestione elenco gruppi**.
1. Inizia a digitare il nome del gruppo di primo livello nella casella **Gruppi principali**.
1. Per aggiungere il gruppo, fare clic sul nome quando viene visualizzato.

   Oppure

   Per rimuovere il gruppo, fare clic sull&#39;icona X a destra del nome.

1. Fai clic su **Salva**.

In qualità di amministratore di Workfront, puoi impostare il numero massimo di licenze per i gruppi Home per impedire a una business unit di utilizzare le licenze Workfront acquistate per altre business unit. Per istruzioni, vedere [Impostare il numero massimo di licenze per un gruppo predefinito](#set-the-maximum-license-count-for-a-home-group) in questo articolo.

## Impostare il numero massimo di licenze per un gruppo predefinito {#set-the-maximum-license-count-for-a-home-group}

In qualità di amministratore di Workfront, puoi impostare il numero massimo di licenze per i gruppi principali del tuo sistema. Ciò consente di impedire a una business unit di utilizzare le licenze Workfront acquistate per altre business unit all&#39;interno dell&#39;organizzazione.

Per impostazione predefinita, il numero massimo di licenze è impostato su N/D, il che significa che non esiste alcun limite.

Gli amministratori di gruppi possono visualizzare il numero di licenze allocate e utilizzate in un Gruppo predefinito che gestiscono. Per ulteriori informazioni, vedere [Visualizzare il numero di licenze allocate e utilizzate in un gruppo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

Per impostare il numero massimo di licenze per un gruppo predefinito:

{{step-1-to-setup}}

1. Nella parte inferiore del pannello a sinistra, fai clic su **Sistema** > **Licenze**.

1. Individuare il Gruppo Predefinito nell&#39;elenco.
1. Nella colonna **Max** del gruppo fare clic sul valore per il quale si desidera impostare un valore massimo.
1. Digitare il numero massimo, quindi premere Invio.

   ![Numero massimo di licenze per il gruppo](assets/updated-max.png)

   >[!NOTE]
   >
   >Per ripristinare il valore predefinito della licenza massima di un gruppo, non digitare 0. Eliminare invece il numero nella casella. L&#39;impostazione del valore di licenza massimo su 0 indica che non sono state allocate licenze a tale gruppo.
