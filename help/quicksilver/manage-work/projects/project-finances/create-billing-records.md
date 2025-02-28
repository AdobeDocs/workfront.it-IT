---
navigation-topic: financials
title: Crea record fatturazione
description: Oltre a impostare le entrate e a tenere traccia delle spese, è possibile creare record di fatturazione in un progetto per le informazioni da fatturare.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '1898'
ht-degree: 0%

---

# Crea record fatturazione

Oltre a impostare le entrate e a tenere traccia delle spese, è possibile creare record di fatturazione in un progetto per le informazioni da fatturare.

Non è possibile creare record di fatturazione per le attività. Puoi creare record di fatturazione solo per i progetti.

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
   <td>Modifica accesso a progetti e dati finanziari</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Gestire le autorizzazioni per il progetto con le autorizzazioni per Gestire le finanze</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Panoramica sui record fatturazione

I record fatturazione vengono creati come allegati di un progetto e contengono dati finanziari del progetto, nonché alcune informazioni finanziarie relative alle attività di un progetto.

Quando si pianifica l&#39;utilizzo dei record di fatturazione, tenere presente quanto segue:

* Si crea un record di fatturazione quando si desidera fatturare una somma di denaro correlata al progetto a un fornitore o partner esterno. Oltre a fatturare un importo fisso a un&#39;origine esterna, in alcuni casi è necessario fatturare la quantità di lavoro sul progetto (dalle ore registrate) a un contraente esterno, nonché le spese sostenute o l&#39;importo dei ricavi fissi. Puoi includere tutte queste informazioni nello stesso record di fatturazione.
* Una volta che un record di fatturazione è impostato su Fatturato, non può essere modificato.

  >[!IMPORTANT]
  >
  >Questo è importante quando le tariffe variano e si desidera bloccare le informazioni su ricavi e spese sul progetto. Aggiungendolo a un record di fatturazione e contrassegnandolo come Fatturato, si impedisce che venga aggiornato quando le tariffe vengono aggiornate nel sistema.

* Un progetto con record fatturazione che sono stati contrassegnati come Fatturati non può essere eliminato.

## Creare un record di fatturazione

1. Passa a un progetto.
1. Fai clic su **Record fatturazione** nel pannello a sinistra.

   Questa sezione potrebbe trovarsi in **Mostra altro**.

1. Con **Dettagli record fatturazione** selezionato nel pannello a sinistra, fai clic su **Nuovo record fatturazione**.
1. Nella casella **Nuovo record fatturazione** visualizzata, specificare le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Questo campo è obbligatorio. Specifica una descrizione per il record di fatturazione, che rifletta lo scopo o l’intento del record.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stato di Fatturazione</td> 
      <td> <p>Seleziona <strong>Non fatturato</strong>, se questo record non è ancora stato fatturato.</p> <p>Seleziona <strong>Fatturato</strong> quando il record di fatturazione viene fatturato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data fatturazione</td> 
      <td>Seleziona la data di fatturazione di questo record fatturazione facendo clic sull’icona del calendario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">N. ordine di acquisto</td> 
      <td>Se a questo record di fatturazione è associato un numero OA, specificare queste informazioni in questo campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID Fattura</td> 
      <td>Se a questo record di fatturazione è associata una fattura, specificare queste informazioni in questo campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importo aggiuntivo</td> 
      <td>Inserire l'importo fisso del record fatturazione. Questo è l'importo che intendi fatturare a un cliente esterno, fornitore o partner per questo progetto. Questo importo non può essere modificato dopo che lo stato del record di fatturazione è stato modificato in Fatturato.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) In **Forms personalizzato**, selezionare un modulo personalizzato per i record fatturazione che si desidera aggiungere al record fatturazione.

   Prima di poter essere selezionato qui, è necessario creare un modulo personalizzato per i record di fatturazione, o un altro utente con accesso ai moduli personalizzati. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Per informazioni sulla creazione di moduli personalizzati, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   È possibile ripetere questo passaggio per aggiungere altri moduli personalizzati necessari per il record di fatturazione.

1. Fai clic su **Salva.**

   Viene creato il record di fatturazione. Per includere le ore fatturabili, le spese e i ricavi fissi nel record di fatturazione, seguire i passaggi descritti nella seguente sottosezione.

## Includi ore fatturabili, spese e retribuzioni fisse in un record di fatturazione

* [Includi ore fatturabili in un record di fatturazione](#include-billable-hours-in-a-billing-record)
* [Includi spese fatturabili in un record fatturazione](#include-billable-expenses-in-a-billing-record)
* [Includi retribuzioni fisse in un record di fatturazione](#include-fixed-revenues-in-a-billing-record)

### Includi ore fatturabili in un record di fatturazione {#include-billable-hours-in-a-billing-record}

Puoi includere le ore registrate per attività, problemi o il progetto nei record di fatturazione.\
Se l’utente che registra le ore o la sua mansione principale è associato a una tariffa di fatturazione per ora, i ricavi derivanti da queste ore vengono aggiunti al record di fatturazione.

* [Quali ore possono essere aggiunte a un record di fatturazione](#what-hours-can-be-added-to-a-billing-record)
* [Aggiungi ore a un record fatturazione](#add-hours-to-a-billing-record)

#### Quali ore possono essere aggiunte a una fatturazione {#what-hours-can-be-added-to-a-billing-record}

Puoi aggiungere ore a una fatturazione quando sono soddisfatte le seguenti condizioni:

* Le attività, i problemi o il progetto hanno ore registrate.
* Il Tipo di Ora delle ore registrate è contrassegnato come Conteggio come Ricavi.

  Per ulteriori informazioni sui Tipi di Ora, vedere l&#39;articolo [Gestione dei Tipi di Ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Tutte le ore registrate per problemi o per il progetto possono essere aggiunte a una fatturazione se all&#39;utente che registra l&#39;ora è associata una tariffa di fatturazione ad ore o la sua mansione principale.
* Se le ore sono registrate su un&#39;attività, l&#39;attività deve avere il seguente Tipo di Reddito:

   * Il Tipo di Reddito non può essere impostato su Non Fatturabile.
   * Se il tipo di retribuzione è impostato su Ore utente, l’utente che registra l’ora deve avere una tariffa di fatturazione ad ore impostata nel proprio profilo.
   * Se il Tipo di Reddito è impostato su Ore Ruolo, il Ruolo Principale dell&#39;utente che registra l&#39;ora deve avere una tariffa di Fatturazione ad Ore.

     >[!NOTE]
     >
     >È possibile sostituire le tariffe di fatturazione per le mansioni a livello di progetto.\
     >Per ulteriori informazioni sull&#39;override delle tariffe di fatturazione dei ruoli, vedere la sezione &quot;Override Job Role Billing Rates at the Project Level&quot; nell&#39;articolo [Panoramica sull&#39;override delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi su un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Se **Richiedi l&#39;approvazione del tempo per questo progetto** è selezionato in Impostazioni progetto, il proprietario del progetto deve approvare le ore registrate.\
  Per ulteriori informazioni sulla richiesta di approvazione nelle ore del progetto, vedere l&#39;articolo [Richiedi approvazione del tempo per un progetto](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Aggiungi ore a un record fatturazione {#add-hours-to-a-billing-record}

Per aggiungere ore fatturabili a un record di fatturazione:

1. Vai al progetto con i record di fatturazione.
1. Fai clic su **Record fatturazione** nel pannello a sinistra.

   Questa sezione potrebbe trovarsi in **Mostra altro**.

1. Fai clic su **Descrizione** di un record di fatturazione per aprire la scheda **Dettagli record fatturazione**.

1. Fai clic su **Ore fatturabili** nel pannello a sinistra.
1. Se ci sono ore che potrebbero essere incluse in un record di fatturazione, fai clic su **Aggiungi ore**.\
   Viene visualizzata la casella **Aggiungi ore fatturabili**.

   >[!NOTE]
   >
   >Se non sono presenti ore registrate o se le ore registrate non soddisfano le condizioni richieste per essere aggiunte a un record di fatturazione, il pulsante **Aggiungi ore** non viene visualizzato. Per ulteriori informazioni sulle ore che possono essere registrate in un record di fatturazione, vedere la sezione [Quali ore possono essere aggiunte a un record di fatturazione](#what-hours-can-be-added-to-a-billing-record) in questo articolo.

1. Selezionare le ore da includere nel record fatturazione e fare clic su **Aggiungi ore**.\
   Il costo effettivo delle ore viene aggiunto come **Ore fatturabili** al **Totale record fatturazione**.

1. (Facoltativo) Fai clic su **Dettagli record fatturazione** per esaminare gli importi di **Ore fatturabili** e **Totale record fatturazione**. Puoi anche vedere il totale del record di fatturazione nell’intestazione del record di fatturazione.

### Includi spese fatturabili in un record di fatturazione {#include-billable-expenses-in-a-billing-record}

Se si aggiungono spese fatturabili al record fatturazione, assicurarsi che le spese relative alle attività e al progetto siano contrassegnate come fatturabili. Le spese non contrassegnate come fatturabili non sono disponibili per l&#39;aggiunta in un record di fatturazione. Per ulteriori informazioni sull&#39;aggiunta delle spese, vedere l&#39;articolo [Gestione delle spese del progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Per aggiungere spese fatturabili a un record fatturazione:

1. Vai al progetto con i record di fatturazione.
1. Fai clic su **Record fatturazione** nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **Mostra altro**, quindi su **Record fatturazione**.

1. Fai clic su **Descrizione** di un record di fatturazione per aprire la scheda **Dettagli record fatturazione**.

1. Fai clic su **Spese fatturabili** nel pannello a sinistra.
1. (Condizionale) Se hai aggiunto spese alle attività o al progetto e le hai contrassegnate come Fatturabili, fai clic su **Aggiungi spese**.

   >[!NOTE]
   >
   >Se sono presenti spese ma non sono contrassegnate come fatturabili, il pulsante **Aggiungi spese** non viene visualizzato. Solo le spese fatturabili con un importo effettivo maggiore di zero possono essere incluse in un record di fatturazione.

1. Seleziona le spese fatturabili disponibili per l&#39;aggiunta al record fatturazione, quindi fai clic su **Aggiungi spese**.\
   L&#39;importo effettivo delle spese viene aggiunto come importo **Spese fatturabili** al **Totale record fatturazione**.

1. (Facoltativo) Fai clic su **Dettagli record fatturazione** per esaminare gli importi **Spese fatturabili** e **Totale record fatturazione**. Puoi anche vedere il totale del record di fatturazione nell’intestazione del record di fatturazione.

### Includi retribuzioni fisse in un record di fatturazione {#include-fixed-revenues-in-a-billing-record}

È possibile aggiungere i Redditi Fissi ai record di fatturazione se sono disponibili attività con questo tipo di retribuzione. Non è disponibile nessun altro tipo di attività o di ricavi di progetto da aggiungere in un record di fatturazione. Per ulteriori informazioni sui tipi di ricavi, vedere la sezione [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) in [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Per aggiungere i ricavi fissi a un record di fatturazione:

1. Vai al progetto con i record di fatturazione.
1. Fai clic su **Record fatturazione** nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **Mostra altro**, quindi su **Record fatturazione**.

1. Fai clic su **Descrizione** di un record di fatturazione per aprire la scheda **Dettagli record fatturazione**.

1. Selezionare la scheda **Redditi fissi**.
1. Se hai aggiunto ricavi fissi alle attività, fai clic su **Aggiungi ricavi fissi**.

   >[!NOTE]
   >
   >Se le attività contengono importi di ricavi ma non sono contrassegnati come &quot;Fissi&quot;, il pulsante **Aggiungi retribuzione fissa** non viene visualizzato.

1. Selezionare le attività di cui si desidera includere i ricavi fissi nel record fatturazione, quindi fare clic su **Aggiungi attività**.\
   L&#39;importo di **retribuzione fissa** delle attività viene aggiunto come importo di **retribuzione fatturabile** al **totale record fatturazione**.

1. (Facoltativo) Fai clic su **Dettagli record fatturazione** per esaminare gli importi **Ricavi fatturabili** e **Totale record fatturazione**. Puoi anche vedere il totale del record di fatturazione nell’intestazione del record di fatturazione.

## Modificare un record di fatturazione

Dopo aver creato un record di fatturazione e aver incluso ore, spese e ricavi nel record di fatturazione, è possibile modificare alcune informazioni sul record esistente prima che venga contrassegnato come Fatturato.

1. Passa al record fatturazione.
1. Con **Dettagli record fatturazione** selezionato nel pannello a sinistra, modifica le informazioni in tutti i campi disponibili

   Oppure

   Fai clic sull&#39;icona **Modifica** ![Modifica](assets/edit-icon.png) nell&#39;angolo superiore destro, quindi modifica le informazioni in tutti i campi disponibili.

   Aggiorna quanto segue:

   * **Descrizione**
   * **Stato fatturazione**

     >[!TIP]
     >
     >Se selezioni **Fatturato** per lo stato di fatturazione, non potrai modificare il record di fatturazione dopo aver salvato le modifiche.

   * **Data di Fatturazione**
   * **Numero OA**
   * **ID fattura**
   * **Importo aggiuntivo**

   I campi seguenti non sono disponibili per la modifica:

   * **Ore fatturabili:** il totale delle retribuzioni effettive delle ore incluse nel record di fatturazione. Per ulteriori informazioni sull&#39;inclusione delle ore in un record di fatturazione, vedere la sezione [Includere le ore fatturabili in un record di fatturazione](#include-billable-hours-in-a-billing-record) in questo articolo.

   * **Spese fatturabili**: il totale dell&#39;importo effettivo delle spese fatturabili incluse nel record di fatturazione. Per ulteriori informazioni sull&#39;inclusione delle spese fatturabili in un record di fatturazione, vedere la sezione [Includere le spese fatturabili in un record di fatturazione](#include-billable-expenses-in-a-billing-record) in questo articolo.

   * **Retribuzioni fatturabili**: il totale delle retribuzioni fisse delle attività incluse nel record di fatturazione. Per ulteriori informazioni sull&#39;inclusione dei ricavi fissi in un record di fatturazione, vedere la sezione [Includere i ricavi fissi in un record di fatturazione](#include-fixed-revenues-in-a-billing-record) in questo articolo.

   * **Totale record fatturazione**: il totale di tutti gli importi fatturabili. Viene calcolata con la seguente formula:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Fai clic su **Salva****Modifiche**.
