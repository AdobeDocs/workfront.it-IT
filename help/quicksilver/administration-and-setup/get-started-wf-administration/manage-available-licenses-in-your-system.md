---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Gestire le licenze disponibili nel sistema
description: In qualità di amministratore di Adobe Workfront, puoi accedere a informazioni sul tuo account Workfront, compreso il numero di licenze acquistate per la tua organizzazione e il numero di tali licenze attualmente in uso.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '1111'
ht-degree: 0%

---

# Gestire le licenze disponibili nel sistema

In qualità di amministratore di Adobe Workfront, puoi accedere a informazioni sul tuo account Workfront, compreso il numero di licenze acquistate per la tua organizzazione e il numero di tali licenze attualmente in uso.

## Requisiti di accesso

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visualizzare le licenze della tua organizzazione

Il numero di licenze utilizzate viene aggiornato automaticamente quando si assegnano i livelli di accesso agli utenti aggiunti a Workfront. Per ulteriori informazioni, consulta [Aggiungi utenti](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Per visualizzare le informazioni sulle licenze nel sistema:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nella parte inferiore del pannello sinistro, fai clic su **Sistema** > **Licenze**.

   Per ulteriori informazioni sulle licenze elencate in questa pagina, consulta [Panoramica sulle licenze](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >Le licenze Proof sono disponibili solo per i clienti che hanno acquistato a pagamento il componente aggiuntivo Workfront Proof, oltre alla licenza Workfront. Per informazioni su questo componente aggiuntivo, vedere [Workfront Proof: indice articolo](../../workfront-proof/workfront-proof.md).

1. (Condizionale) Se viene visualizzato il messaggio **Per impostare un massimo, è necessario aggiungere un Gruppo Predefinito**, aggiungi un gruppo predefinito nel sistema come descritto nella sezione [Aggiungere o rimuovere un gruppo predefinito nella pagina Licenze](#add-or-remove-a-home-group-to-the-licenses-page) in questo articolo.

## Visualizzare informazioni sulle licenze per i componenti aggiuntivi di Workfront

Nella schermata seguente, **5 di 10 Licenze Verifica** indica che questa organizzazione dispone del componente aggiuntivo a pagamento Workfront Proof e attualmente utilizza 5 delle 10 licenze Workfront Proof acquistate.

![](assets/updated-licenses-page.png)

Se la tua organizzazione ha acquistato Workfront Goals, qui vengono visualizzate anche le informazioni sulla licenza per questo prodotto. In questo caso, puoi visualizzare le seguenti informazioni:

* Numero totale di licenze Workfront Goals acquistate dalla società
* Il numero di licenze Workfront Goals associate agli utenti. Questo è il numero di utenti a cui è stato concesso almeno l’accesso di visualizzazione agli obiettivi nel rispettivo livello di accesso.

Per informazioni sugli obiettivi di Workfront, consulta [Panoramica sugli obiettivi di Adobe Workfront](../../workfront-goals/goal-management/wf-goals-overview.md). Per informazioni sull’accesso agli obiettivi di Workfront, consulta [Concedere l’accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

>[!NOTE]
>
>Workfront consente di assegnare più licenze Workfront Goals acquistate. Tuttavia, quando si assegnano più licenze di quelle consentite dal contratto Workfront Goals, un account manager Workfront contatterà l&#39;utente per informarlo del superamento del numero di contratto.
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>Gli utenti senza accesso amministrativo possono utilizzare un rapporto di gruppo per visualizzare il numero di licenze. Nella scheda Report, crea un nuovo report di gruppo e aggiungi le seguenti colonne:>
>* Limite tipo di licenza: limite lavoratore
>* Limite tipo di licenza: Limite planner
>
>Per ulteriori informazioni sulla creazione di un rapporto, consulta [Creare un rapporto personalizzato](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
>

## Visualizza informazioni sulle assegnazioni di bozze e documenti decisionali mensili

>[!IMPORTANT]
>
>I limiti di decisione per bozze e documenti si applicano solo agli utenti delle nuove licenze. Per ulteriori informazioni, consulta [Panoramica sulle nuove licenze](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

Le decisioni su bozze e documenti sono limitate per tutte le licenze Workfront non a pagamento. Limiti reimpostati per ogni utente ogni mese.

I limiti di decisione per ogni licenza variano a seconda del piano su cui stai lavorando. Puoi visualizzare l’assegnazione mensile in Configurazione > Licenze.

Per ulteriori informazioni sui limiti di decisione per bozze e documenti, consulta [Documento limitato e decisione sulla bozza per utenti non pagati - Panoramica](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

![](assets/monthly-decision-allotment.png)

## Aggiungere o rimuovere un gruppo predefinito nella pagina Licenze {#add-or-remove-a-home-group-to-the-licenses-page}

Per utilizzare questa funzione è necessario un piano Workfront aziendale o aziendale. Per ulteriori informazioni sui vari piani disponibili, vedere [Piani Workfront.](https://www.workfront.com/plans)

Ogni utente può essere assegnato a un solo Gruppo Predefinito. Workfront fornisce un conteggio delle licenze orientato al gruppo calcolando il numero di licenze allocate e attualmente utilizzate in ciascun Gruppo predefinito.

Se viene visualizzato il messaggio **Per impostare un massimo, è necessario aggiungere un Gruppo Predefinito** nella pagina Licenze è necessario aggiungere almeno un gruppo predefinito alla pagina Licenze.

>[!IMPORTANT]
>
>* Per gestire in modo efficace le licenze con i gruppi home, si consiglia di impostare gruppi home specifici per le unità aziendali prima di aggiornare il numero massimo di licenze. Per ulteriori informazioni, consulta [Panoramica sui gruppi predefiniti](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* È possibile aggiungere solo i gruppi di primo livello come gruppi principali, non i sottogruppi. Se a un utente è assegnato un sottogruppo come Gruppo predefinito, la licenza viene aggiunta al numero di licenze per il gruppo di livello superiore al di sopra di tale sottogruppo.
>

Per aggiungere o rimuovere un gruppo predefinito nella pagina Licenze:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nella parte inferiore del pannello sinistro, fai clic su **Sistema** > **Licenze**.

1. Clic **Gestisci elenco gruppi**.
1. Inizia a digitare il nome del gruppo di primo livello nel **Gruppi predefiniti** casella.
1. Per aggiungere il gruppo, fare clic sul nome quando viene visualizzato.

   Oppure

   Per rimuovere il gruppo, fare clic sull&#39;icona X a destra del nome.

1. Fai clic su **Salva**.

In qualità di amministratore di Workfront, puoi impostare il numero massimo di licenze per i gruppi Home per impedire a una business unit di utilizzare le licenze Workfront acquistate per altre business unit. Per istruzioni, consulta [Impostare il numero massimo di licenze per un gruppo predefinito](#set-the-maximum-license-count-for-a-home-group) in questo articolo.

## Impostare il numero massimo di licenze per un gruppo predefinito {#set-the-maximum-license-count-for-a-home-group}

In qualità di amministratore di Workfront, puoi impostare il numero massimo di licenze per i gruppi principali del tuo sistema. Ciò consente di impedire a una business unit di utilizzare le licenze Workfront acquistate per altre business unit all&#39;interno dell&#39;organizzazione.

Per impostazione predefinita, il numero massimo di licenze è impostato su N/D, il che significa che non esiste alcun limite.

Gli amministratori di gruppi possono visualizzare il numero di licenze allocate e utilizzate in un Gruppo predefinito che gestiscono. Per ulteriori informazioni, consulta [Visualizzare il numero di licenze allocate e utilizzate in un gruppo nella nuova esperienza Adobe Workfront](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

Per impostare il numero massimo di licenze per un gruppo predefinito:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nella parte inferiore del pannello sinistro, fai clic su **Sistema** > **Licenze**.

1. Individuare il Gruppo Predefinito nell&#39;elenco.
1. In **Max** del gruppo, fare clic sul valore per il quale si desidera impostare un valore massimo.
1. Digitare il numero massimo, quindi premere Invio.

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >Per ripristinare il valore predefinito della licenza massima di un gruppo, non digitare 0. Eliminare invece il numero nella casella. L&#39;impostazione del valore di licenza massimo su 0 indica che non sono state allocate licenze a tale gruppo.
