---
title: Ricalcolare le finanze del progetto
product-area: projects
navigation-topic: financials
description: I finanziamenti vengono calcolati su un progetto quando si verificano modifiche nelle ore registrate per il progetto o nei tassi utilizzati per calcolare i costi e i ricavi.
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1590'
ht-degree: 0%

---

# Ricalcolare le finanze del progetto

I finanziamenti vengono calcolati su un progetto quando si verificano modifiche nelle ore registrate per il progetto o nei tassi utilizzati per calcolare i costi e i ricavi.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso a progetti e dati finanziari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il progetto con autorizzazioni per Manage Finance</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sul calcolo delle finanze in Adobe Workfront

Le finanze vengono calcolate in Analisi avanzata nei seguenti modi:

* È possibile ricalcolare manualmente i costi e i ricavi di un progetto utilizzando l&#39;opzione Ricalcola finanziamenti su un progetto.
* Inoltre, alcune azioni attivano un ricalcolo automatico.

Quando il tasso di un utente o di un ruolo cambia durante la durata di un progetto, si può verificare quanto segue:

* Quando la modifica viene apportata, il tasso aggiornato viene utilizzato da quel momento in poi durante la registrazione delle ore e le informazioni finanziarie vengono calcolate. La modifica del tasso non influisce sul modo in cui sono stati calcolati gli elementi prima della modifica. Per tutte le ore esistenti registrate, il vecchio tasso viene utilizzato per calcolare le informazioni finanziarie.
* È possibile forzare Adobe Workfront a utilizzare il nuovo tasso retroattivamente per tutte le ore registrate finora, utilizzando l&#39;opzione Ricalcola contabilità. Questo costringe Workfront a ricalcolare retroattivamente tutte le ore immesse in precedenza, i costi pianificati e le entrate in conformità con le nuove informazioni sulle tariffe.

>[!CAUTION]
>
>Prima di ricalcolare manualmente le finanze di un determinato progetto, è possibile conservare tutti i dati finanziari già calcolati a un tasso precedente. Si consiglia di utilizzare l&#39;opzione Ricalcola contabilità solo quando si è certi di non apportare modifiche alle informazioni esistenti o solo quando tali modifiche sono desiderate.

## Conserva i dati finanziari per le attività con ore esistenti {#preserve-financial-data-for-tasks-with-existing-hours}

Quando i dati finanziari di un progetto vengono ricalcolati, Workfront ricalcola retroattivamente tutte le ore registrate in precedenza, le spese pianificate, i costi effettivi e i ricavi pianificati ed effettivi, in base a eventuali informazioni finanziarie nuove o aggiornate.

* [Mantenere i ricavi del progetto](#preserve-project-revenue)
* [Mantieni costo progetto](#preserve-project-cost)

### Mantenere i ricavi del progetto  {#preserve-project-revenue}

Le percentuali di ricavi possono variare durante la durata di un progetto.

Per ulteriori informazioni su tariffe e ricavi di fatturazione, consulta l’articolo [Panoramica di fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

I tassi di ricavi possono variare ai seguenti livelli:

* Livello di sistema (per i ruoli di lavoro)\
   Per ulteriori informazioni sulla creazione di ruoli di lavoro con tassi di fatturazione a livello di sistema, consulta l’articolo [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Livello utente\
   Per ulteriori informazioni sulla modifica delle informazioni sulla tariffa di fatturazione per gli utenti, consulta l’articolo [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Livello dell&#39;azienda (per i ruoli di lavoro)\
   Per ulteriori informazioni, consulta [Escludere i tassi di fatturazione dei ruoli di lavoro a livello aziendale](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* Livello di progetto (per i ruoli di lavoro)\
   Per ulteriori informazioni sull’override dei tassi di ruolo del lavoro a livello di progetto, consulta l’articolo [Panoramica sulla priorità dei tassi di fatturazione dei ruoli di lavoro e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Ad esempio, il tasso di fatturazione di un utente cambia nel corso di un progetto da $ 50 a $ 75 all’ora e si desidera che tutti i dati esistenti rimangano calcolati al vecchio tasso ($50 e ora). Tuttavia, quando le finanze del progetto vengono ricalcolate, le attività che dispongono già di dati finanziari esistenti avranno il ricavo aggiornato per riflettere il nuovo tasso di fatturazione (di $75 all&#39;ora).

* [Mantenere i ricavi di progetto creando un record di fatturazione](#preserve-project-revenue-by-creating-a-billing-record)
* [Mantenere i ricavi del progetto utilizzando più sostituzioni del tasso di fatturazione](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### Mantenere i ricavi di progetto creando un record di fatturazione {#preserve-project-revenue-by-creating-a-billing-record}

Quando i tassi di fatturazione cambiano a qualsiasi livello menzionato sopra, è possibile conservare i ricavi esistenti che sono già stati calcolati sul progetto evitando di utilizzare l&#39;opzione Ricalcola contabilità manuale o bloccando il tempo registrato sul progetto e calcolato utilizzando il vecchio tasso in un record di fatturazione con lo stato Fatturato.

Quando non si ricalcolano le finanze del progetto o si bloccano le ore registrate in un record di fatturazione fatturata, le ore registrate dopo le modifiche del tasso vengono calcolate con il nuovo tasso e le ore registrate prima che le modifiche del tasso di costo rimangano calcolate al vecchio tasso.

Per ulteriori informazioni sulla creazione di record di fatturazione, consulta l’articolo [Creazione di record di fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

#### Mantenere i ricavi del progetto utilizzando più sostituzioni del tasso di fatturazione {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

Quando i tassi di fatturazione cambiano per i ruoli di lavoro a livello di progetto, puoi conservare i ricavi esistenti già calcolati sul progetto utilizzando più sostituzioni dei tassi di fatturazione che sono bloccate entro un intervallo di tempo specificato.

Per ulteriori informazioni sull&#39;utilizzo di più sostituzioni dei tassi di fatturazione, consulta l&#39;articolo [Panoramica sulla priorità dei tassi di fatturazione dei ruoli di lavoro e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>Questo vale solo per le tariffe di fatturazione dei ruoli di lavoro modificate a livello di progetto.

### Mantieni costo progetto {#preserve-project-cost}

I tassi di costo possono variare ai seguenti livelli:

* Livello di sistema (per i ruoli di lavoro)\
   Per ulteriori informazioni sulla creazione di ruoli di lavoro con tassi di costo a livello di sistema, consulta l’articolo [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Livello utente\
   Per ulteriori informazioni sulla modifica delle informazioni sul tasso di costo per gli utenti, consulta l’articolo [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Quando i tassi di fatturazione cambiano a qualsiasi livello menzionato sopra, è possibile conservare i costi esistenti che sono già stati calcolati sul progetto bloccando il tempo registrato sul progetto e calcolato utilizzando il vecchio tasso in un record di fatturazione con lo stato Billing. Per ulteriori informazioni sulla creazione di record di fatturazione, consulta l’articolo [Creazione di record di fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

È inoltre possibile evitare di utilizzare l&#39;opzione Ricalcola contabilità manuale, se non si desidera creare un record di fatturazione, come descritto nella sezione [Ricalcolare manualmente le finanze di un progetto](#manually-recalculate-finances-for-a-project) in questo articolo.

Quando non si ricalcolano le finanze del progetto o si bloccano le ore registrate in un record di fatturazione fatturata, le ore registrate dopo le modifiche del tasso vengono calcolate con il nuovo tasso e le ore registrate prima che le modifiche del tasso di costo rimangano calcolate al vecchio tasso.

## Ricalcolare manualmente le finanze di un progetto {#manually-recalculate-finances-for-a-project}

Se i tassi cambiano durante la durata di un progetto e si desidera che i calcoli dei costi e dei ricavi riflettano i nuovi tassi, è necessario ricalcolare manualmente i costi relativi al progetto.

>[!NOTE]
>
>È possibile impedire l&#39;aggiornamento dei valori dei ricavi per riflettere i nuovi tassi quando si ricalcola manualmente il finanziamento seguendo i passaggi descritti nella sezione [Conserva i dati finanziari per le attività con ore esistenti](#preserve-financial-data-for-tasks-with-existing-hours) del presente articolo. I valori di costo vengono sempre aggiornati per riflettere i nuovi tassi quando si ricalcola manualmente le finanze di un progetto.

È possibile ricalcolare le finanze dei progetti in Workfront dalla pagina del progetto o da un elenco o da un rapporto di progetto.

È possibile ricalcolare le finanze durante la modifica in serie. Per informazioni, consulta la sezione [Ricalcolare manualmente le finanze in blocco nella casella Modifica progetti](#manually-recalculate-finances-in-bulk-in-the-edit-projects-box) in questo articolo.

1. Passa al progetto in cui desideri ricalcolare le finanze e fai clic sul pulsante **Altro** icona ![](assets/qs-more-icon-on-an-object.png) a destra del nome del progetto

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oppure

   Vai a un elenco o a un rapporto di progetti e seleziona uno o più progetti, quindi fai clic su **Altro** icona ![](assets/qs-more-icon-on-an-object.png) in cima all&#39;elenco.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >A seconda della complessità dei progetti, si consiglia di non selezionare un gran numero di progetti quando si ricalcolano le finanze in massa per garantire prestazioni ottimali. Alcuni elementi che potrebbero rendere un progetto troppo complesso potrebbero essere più dipendenze o assegnazioni o un numero elevato di campi personalizzati.

1. Fai clic su **Ricalcola finanza**.

   Tutti i costi e i ricavi previsti del progetto vengono ricalcolati con eventuali nuove informazioni.

   Riceverai una conferma nella parte superiore del browser che le finanze del progetto sono state ricalcolate correttamente.\
   I valori di costo esistenti e alcuni valori di ricavo che non sono stati bloccati vengono aggiornati per riflettere i nuovi tassi.

## Ricalcolare manualmente le finanze in blocco nella casella Modifica progetti {#manually-recalculate-finances-in-bulk-in-the-edit-projects-box}

È possibile ricalcolare manualmente le finanze di diversi progetti modificandoli in blocco. Questo fa sì che i ricavi dei progetti vengano ricalcolati retroattivamente.

>[!IMPORTANT]
>
>È possibile impedire l&#39;aggiornamento dei valori dei ricavi per riflettere i nuovi tassi quando si ricalcola manualmente il finanziamento seguendo i passaggi descritti nella sezione [Conserva i dati finanziari per le attività con ore esistenti](#preserve-financial-data-for-tasks-with-existing-hours) del presente articolo. I valori di costo vengono sempre aggiornati per riflettere i nuovi tassi quando si ricalcola manualmente le finanze sui progetti.

Per ricalcolare manualmente le finanze di diversi progetti:

1. Vai a un elenco di progetti.
1. Seleziona diversi progetti nell’elenco, quindi fai clic su **Modifica**.

   >[!TIP]
   >
   >A seconda della complessità dei progetti, si consiglia di non selezionare un gran numero di progetti quando li si modifica in serie per garantire prestazioni ottimali. Alcuni elementi che potrebbero rendere un progetto troppo complesso potrebbero essere più dipendenze o assegnazioni o un numero elevato di campi personalizzati.

1. Fai clic su **Impostazioni**, quindi seleziona **Ricalcolare Costi E Entrate**.

1. Fai clic su **Salva modifiche**.

## Azioni che attivano un ricalcolo automatico delle finanze

Le seguenti azioni attivano il ricalcolo finanziario dei progetti in Workfront:

* Modifica dello stato dell&#39;attività
* Spostamento di un&#39;attività con ore in un altro progetto
* Modifica dello stato del progetto da Completato a uno stato attivo

>[!NOTE]
>
>Quando si modifica lo stato del progetto, vengono ricalcolati solo i valori pianificati.

È inoltre possibile ricalcolare manualmente le finanze sotto la **Altro** menu ![](assets/qs-more-menu.png) a livello di progetto, facendo clic su **Ricalcola finanze**.
