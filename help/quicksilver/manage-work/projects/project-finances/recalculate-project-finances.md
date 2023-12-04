---
title: Ricalcolare i dati finanziari del progetto
product-area: projects
navigation-topic: financials
description: I dati finanziari vengono calcolati su un progetto in base alle modifiche apportate alle ore registrate per il progetto o ai tassi utilizzati per calcolare costi e ricavi.
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: bfe77796863bb2d7d324901721fda7fa045c2c0b
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 0%

---

# Ricalcolare i dati finanziari del progetto

I dati finanziari vengono calcolati su un progetto in base alle modifiche apportate alle ore registrate per il progetto o ai tassi utilizzati per calcolare costi e ricavi.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti e dati finanziari</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il progetto con le autorizzazioni per Gestire le finanze</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Considerazioni sul calcolo dei dati finanziari in Adobe Workfront

In Analisi avanzate, i dati finanziari vengono calcolati nei modi seguenti:

* È possibile ricalcolare manualmente costi e ricavi per un progetto utilizzando l&#39;opzione Ricalcola dati finanziari per un progetto.
* Inoltre, alcune azioni attivano un ricalcolo automatico.

Quando la frequenza di un utente o di un ruolo cambia durante la durata di un progetto, possono verificarsi le seguenti situazioni:

* Quando viene apportata la modifica, il tasso aggiornato viene utilizzato da quel momento in poi, man mano che vengono registrate le ore e vengono calcolate le informazioni finanziarie. La modifica della tariffa non influisce sul modo in cui le cose sono state calcolate prima della modifica. Per tutte le ore registrate esistenti, la tariffa precedente viene utilizzata per calcolare le informazioni finanziarie.
* Puoi forzare Adobe Workfront a utilizzare la nuova tariffa retroattivamente per tutte le ore registrate finora, utilizzando l’opzione Ricalcola contabilità. Questo costringe Workfront a ricalcolare retroattivamente tutte le ore inserite in precedenza, i costi pianificati e i ricavi in base alle nuove informazioni sui tassi.

>[!CAUTION]
>
>Prima di ricalcolare manualmente i dati finanziari per un determinato progetto, è possibile conservare i dati finanziari già calcolati a un tasso precedente. È consigliabile utilizzare l&#39;opzione Ricalcola dati finanziari solo se si è certi di non apportare modifiche alle informazioni esistenti o solo quando si desidera apportare tali modifiche.

## Mantieni dati finanziari per le attività con ore esistenti {#preserve-financial-data-for-tasks-with-existing-hours}

Quando i dati finanziari per un progetto vengono ricalcolati, Workfront ricalcola retroattivamente tutte le ore registrate in precedenza, i costi pianificati, effettivi e i ricavi pianificati ed effettivi, in base a qualsiasi informazione finanziaria nuova o aggiornata.

* [Mantieni ricavi progetto](#preserve-project-revenue)
* [Mantieni costo progetto](#preserve-project-cost)

### Mantieni ricavi progetto  {#preserve-project-revenue}

Le aliquote dei ricavi possono cambiare durante la durata di un progetto.

Per ulteriori informazioni sulle tariffe di fatturazione e sulle entrate, consulta l’articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

I tassi di ricavi possono variare ai seguenti livelli:

* Livello di sistema (per le mansioni)\
  Per ulteriori informazioni sulla creazione di mansioni con tariffe di fatturazione a livello di sistema, consulta l’articolo [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Livello utente\
  Per ulteriori informazioni sulla modifica delle informazioni sulle tariffe di fatturazione per gli utenti, consulta l’articolo [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Livello aziendale (per mansioni)\
  Per ulteriori informazioni, consulta [Sostituisci le tariffe di fatturazione dei ruoli a livello aziendale](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* Livello Progetto (per mansioni)\
  Per ulteriori informazioni sulla sostituzione delle percentuali di mansioni a livello di progetto, consulta l’articolo [Panoramica sulla sostituzione delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Ad esempio, la tariffa di fatturazione di un utente cambia durante il corso di un progetto da $ 50 a $ 75 all’ora e desideri che tutti i dati esistenti rimangano calcolati alla tariffa precedente ($ 50 e ora). Tuttavia, quando i dati finanziari del progetto vengono ricalcolati, per le attività che dispongono già di dati finanziari esistenti i ricavi vengono aggiornati in modo da riflettere la nuova tariffa di fatturazione (di $ 75 all&#39;ora).

* [Preservare i ricavi del progetto creando una fatturazione](#preserve-project-revenue-by-creating-a-billing-record)
* [Preservare i ricavi del progetto utilizzando più sostituzioni delle tariffe di fatturazione](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### Preservare i ricavi del progetto creando una fatturazione {#preserve-project-revenue-by-creating-a-billing-record}

Quando le tariffe di fatturazione cambiano a qualsiasi livello indicato sopra, è possibile mantenere i ricavi esistenti che sono già stati calcolati sul progetto evitando di utilizzare l&#39;opzione Ricalcola contabilità manuale o bloccando il tempo registrato sul progetto e calcolato utilizzando la tariffa precedente in un record di fatturazione con lo stato Fatturato.

Quando non si ricalcolano i dati finanziari sul progetto o quando si bloccano le ore registrate in un record di fatturazione fatturato, le ore registrate dopo le modifiche della tariffa verranno calcolate con la nuova tariffa e le ore registrate prima delle modifiche della tariffa rimarranno calcolate con la tariffa precedente.

Per ulteriori informazioni sulla creazione di record di fatturazione, consulta l’articolo [Crea record fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

#### Preservare i ricavi del progetto utilizzando più sostituzioni delle tariffe di fatturazione {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

Quando le tariffe di fatturazione cambiano per le mansioni a livello di progetto, puoi mantenere i ricavi esistenti che sono già stati calcolati sul progetto utilizzando più sostituzioni di tariffe di fatturazione che sono bloccate entro un intervallo di tempo specificato.

Per ulteriori informazioni sull’utilizzo di sostituzioni di più tariffe di fatturazione, consulta l’articolo [Panoramica sulla sostituzione delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>Questo si applica solo alle tariffe di fatturazione delle mansioni che vengono modificate a livello di progetto.

### Mantieni costo progetto {#preserve-project-cost}

I tassi di costo possono variare ai seguenti livelli:

* Livello di sistema (per mansioni)\
  Per ulteriori informazioni sulla creazione di mansioni con tassi di costo a livello di sistema, vedere l&#39;articolo [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Livello utente\
  Per ulteriori informazioni sulla modifica delle informazioni sulle tariffe per gli utenti, vedere l&#39;articolo [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Quando le tariffe di fatturazione cambiano a qualsiasi livello indicato sopra, puoi mantenere i costi esistenti che sono già stati calcolati sul progetto bloccando il tempo registrato sul progetto e calcolato utilizzando la tariffa precedente in una registrazione di fatturazione con lo stato Fatturato. Per ulteriori informazioni sulla creazione di record di fatturazione, consulta l’articolo [Crea record fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

È inoltre possibile evitare di utilizzare l&#39;opzione Ricalcola contabilità manuale se non si desidera creare un record di fatturazione, come descritto nella sezione [Ricalcolare manualmente i dati finanziari per un progetto](#manually-recalculate-finances-for-a-project) in questo articolo.

Quando non si ricalcolano i dati finanziari sul progetto o quando si bloccano le ore registrate in un record di fatturazione fatturato, le ore registrate dopo le modifiche della tariffa verranno calcolate con la nuova tariffa e le ore registrate prima delle modifiche della tariffa rimarranno calcolate con la tariffa precedente.

## Ricalcolare manualmente i dati finanziari per un progetto {#manually-recalculate-finances-for-a-project}

Se i tassi cambiano durante la durata di un progetto e si desidera che i calcoli dei costi e dei ricavi riflettano i nuovi tassi, è necessario ricalcolare manualmente i dati finanziari sul progetto.

>[!NOTE]
>
>È possibile impedire l&#39;aggiornamento dei valori dei ricavi per riflettere i nuovi tassi quando si ricalcola manualmente i dati finanziari seguendo i passaggi descritti nella sezione [Mantieni dati finanziari per le attività con ore esistenti](#preserve-financial-data-for-tasks-with-existing-hours) del presente articolo. I valori dei costi vengono sempre aggiornati per riflettere i nuovi tassi quando si ricalcolano manualmente i dati finanziari su un progetto.

È possibile ricalcolare i dati finanziari dei progetti in Workfront dalla pagina del progetto o da un elenco o report di progetti.

È possibile ricalcolare i dati finanziari durante la modifica in blocco. Per informazioni, vedere [Ricalcolare manualmente i dati finanziari in blocco](#manually-recalculate-finances-in-bulk) in questo articolo.

1. Passare al progetto in cui si desidera ricalcolare i dati finanziari e fare clic sul pulsante **Altro** icona ![](assets/qs-more-icon-on-an-object.png) a destra del nome del progetto.

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oppure

   Vai a un elenco o a un report di progetti e seleziona uno o più progetti, quindi fai clic su **Altro** icona ![](assets/qs-more-icon-on-an-object.png) nella parte superiore dell’elenco.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >A seconda della complessità dei progetti, si consiglia di non selezionare un numero elevato di progetti durante il ricalcolo in blocco delle finanze per garantire prestazioni ottimali. Alcuni elementi che potrebbero rendere un progetto troppo complesso potrebbero essere più dipendenze o assegnazioni o un numero elevato di campi personalizzati.

1. Clic **Ricalcola dati finanziari**.

   Tutti i costi e i ricavi pianificati per il progetto vengono ricalcolati con eventuali nuove informazioni.

   Nella parte superiore del browser dovresti ricevere una conferma che i dati finanziari del progetto sono stati ricalcolati correttamente.
I valori dei costi esistenti e alcuni valori dei ricavi che non sono stati bloccati vengono aggiornati per riflettere i nuovi tassi.

## Ricalcolare manualmente i dati finanziari in blocco{#manually-recalculate-finances-in-bulk}

È possibile ricalcolare manualmente i dati finanziari di diversi progetti modificandoli in blocco. In questo modo i ricavi sui progetti vengono ricalcolati retroattivamente.

>[!IMPORTANT]
>
>È possibile impedire l&#39;aggiornamento dei valori dei ricavi per riflettere i nuovi tassi quando si ricalcola manualmente i dati finanziari seguendo i passaggi descritti nella sezione [Mantieni dati finanziari per le attività con ore esistenti](#preserve-financial-data-for-tasks-with-existing-hours) del presente articolo. I valori dei costi vengono sempre aggiornati per riflettere i nuovi tassi quando si ricalcolano manualmente i dati finanziari sui progetti.

Per ricalcolare manualmente i dati finanziari di più progetti:

1. Consente di passare a un elenco di progetti.
1. Seleziona diversi progetti nell’elenco, quindi fai clic su **Altro** icona ![](assets/qs-more-icon-on-an-object.png) nella parte superiore dell’elenco.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >A seconda della complessità dei progetti, si consiglia di non selezionare un numero elevato di progetti quando li si modifica in blocco per garantire prestazioni ottimali. Alcuni elementi che potrebbero rendere un progetto troppo complesso potrebbero essere più dipendenze o assegnazioni o un numero elevato di campi personalizzati.

1. Clic **Ricalcola dati finanziari**.

   Tutti i costi e i ricavi pianificati per i progetti selezionati vengono ricalcolati con le nuove informazioni.

   Nella parte superiore del browser dovresti ricevere una conferma che i dati finanziari dei progetti sono stati ricalcolati correttamente.

## Azioni che attivano il ricalcolo automatico dei dati finanziari

Le azioni seguenti attivano il ricalcolo finanziario dei progetti in Workfront:

* Modifica dello stato dell&#39;attività
* Spostamento di un&#39;attività con ore in un altro progetto
* Modifica dello stato del progetto da Completo a Attivo

>[!NOTE]
>
>Quando si modifica lo stato del progetto, vengono ricalcolati solo i valori pianificati.

È inoltre possibile ricalcolare i dati finanziari manualmente in **Altro** menu ![](assets/qs-more-menu.png) a livello di progetto, facendo clic su **Ricalcola dati finanziari**.
