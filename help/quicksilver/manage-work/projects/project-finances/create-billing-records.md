---
navigation-topic: financials
title: Crea record fatturazione
description: Oltre a impostare le entrate e a tenere traccia delle spese, è possibile creare record di fatturazione in un progetto per le informazioni da fatturare.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 4805b93be7ce3dc098c7e160cdb872446f80ecbd
workflow-type: tm+mt
source-wordcount: '1645'
ht-degree: 1%

---

# Crea record fatturazione

<!-- Audited: 6/2025 -->

Oltre a impostare le entrate e a tenere traccia delle spese, è possibile creare record di fatturazione in un progetto per le informazioni da fatturare.

Non è possibile creare record di fatturazione per le attività, ma solo per i progetti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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

I record fatturazione vengono creati come allegati a un progetto e contengono dati finanziari del progetto e informazioni finanziarie sulle attività del progetto.

Quando si pianifica l&#39;utilizzo dei record di fatturazione, tenere presente quanto segue:

* Si crea un record di fatturazione quando si desidera fatturare una somma di denaro correlata al progetto a un fornitore o partner esterno. Oltre a fatturare un importo fisso a un&#39;origine esterna, in alcuni casi è necessario fatturare la quantità di lavoro sul progetto (dalle ore registrate) a un contraente esterno, nonché le spese sostenute o l&#39;importo dei ricavi fissi. Puoi includere tutte queste informazioni nello stesso record di fatturazione.
* Una volta impostato su Fatturato, il record di fatturazione non può essere modificato.

  >[!IMPORTANT]
  >
  >Questo è importante quando le tariffe variano e si desidera bloccare le informazioni su ricavi e spese sul progetto. Aggiungendolo a un record di fatturazione e contrassegnandolo come Fatturato, si impedisce che venga aggiornato quando le tariffe vengono aggiornate nel sistema.

* Un progetto con record fatturazione che sono stati contrassegnati come Fatturati non può essere eliminato.

## Creare un record di fatturazione

{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona un progetto.
1. Fai clic su **Record fatturazione** nel pannello a sinistra.
1. Fare clic su **Nuovo record fatturazione**.
1. Nella casella **Nuovo record fatturazione** visualizzata immettere le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>(Obbligatorio) Inserire una descrizione per il record fatturazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stato fatturazione</td> 
      <td> <p>Seleziona <strong>Non fatturato</strong> se questo record non è ancora stato fatturato.</p> <p>Seleziona <strong>Fatturato</strong> se il record di fatturazione è stato fatturato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data fatturazione</td> 
      <td>Seleziona la data di fatturazione di questo record di fatturazione facendo clic sull’icona del calendario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">N. ordine di acquisto</td> 
      <td>Inserire il numero OA associato a questo record di fatturazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID Fattura</td> 
      <td>Inserire la fattura associata a questo record fatturazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importo aggiuntivo</td> 
      <td>Inserire l'importo fisso del record fatturazione. Si tratta dell'importo che si intende fatturare a un cliente esterno, a un collaboratore esterno o a un partner per questo progetto. Questo importo non può essere modificato dopo che lo stato del record fatturazione è stato cambiato in Fatturato.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) In **Forms personalizzato**, selezionare un modulo personalizzato per i record di fatturazione che si desidera aggiungere al record.

   È necessario creare un modulo personalizzato per i record fatturazione prima di poterlo selezionare qui. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Per informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Fare clic su **Salva.** Record di fatturazione creato.

## Includi ore fatturabili, spese e retribuzioni fisse in un record di fatturazione

### Includi ore fatturabili in un record di fatturazione {#include-billable-hours-in-a-billing-record}

Puoi includere le ore registrate per attività, problemi o il progetto nei record di fatturazione.

Se l’utente che registra le ore o il suo ruolo lavorativo principale è associato a una tariffa di fatturazione ad ore, i ricavi derivanti da queste ore vengono aggiunti al record di fatturazione.

* [Quali ore possono essere aggiunte a un record di fatturazione](#what-hours-can-be-added-to-a-billing-record)
* [Aggiungere ore a un record fatturazione](#add-hours-to-a-billing-record)

#### Quali ore possono essere aggiunte a una fatturazione {#what-hours-can-be-added-to-a-billing-record}

Puoi aggiungere ore a una fatturazione quando sono soddisfatte le seguenti condizioni:

* Le ore per le attività, i problemi o il progetto sono state registrate.
* Il Tipo di Ora delle ore registrate è contrassegnato come Conteggio come Ricavi.

  Per ulteriori informazioni, vedere l&#39;articolo [Gestione dei tipi di lavoro](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Tutte le ore registrate per i problemi o il progetto possono essere aggiunte a una fatturazione se all&#39;utente che registra l&#39;ora è associata una tariffa Fatturazione ad Ore o la sua mansione principale.
* Se le ore sono registrate su un&#39;attività, l&#39;attività deve avere il seguente Tipo di Reddito:

   * Il Tipo di Reddito non può essere impostato su Non Fatturabile.
   * Se il tipo di retribuzione è impostato su Ore utente, l’utente che registra l’ora deve avere una tariffa di fatturazione ad ore impostata nel proprio profilo.
   * Se il Tipo di Reddito è impostato su Ore Ruolo, il ruolo principale dell&#39;utente che registra l&#39;ora deve avere una tariffa Fatturazione ad Ore.

     >[!NOTE]
     >
     >È possibile sostituire le tariffe di fatturazione per le mansioni a livello di progetto.\
     >Per ulteriori informazioni, vedere la sezione &quot;Override delle tariffe di fatturazione dei ruoli a livello di progetto&quot; nell&#39;articolo [Panoramica dell&#39;override delle tariffe di fatturazione dei ruoli e del calcolo dei ricavi su un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Se l&#39;opzione Richiedi l&#39;approvazione del tempo per questo progetto è selezionata in Impostazioni progetto, il proprietario del progetto deve approvare le ore registrate.\
  Per ulteriori informazioni, vedere [Richiedere l&#39;approvazione del tempo per un progetto](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Aggiungere ore a un record fatturazione {#add-hours-to-a-billing-record}

{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona un progetto.
1. Fai clic su **Record fatturazione** nel pannello a sinistra.
1. Fai clic sul record fatturazione **Descrizione** per aprire la scheda **Dettagli record fatturazione**.
1. Fai clic su **Ore fatturabili** nel pannello a sinistra.
1. Se ci sono ore che potrebbero essere incluse in un record di fatturazione, fai clic su **Aggiungi ore**. Viene visualizzata la casella **Aggiungi ore fatturabili**.

   >[!NOTE]
   >
   >Se non sono presenti ore registrate o se le ore registrate non soddisfano le condizioni richieste per essere aggiunte a un record di fatturazione, il pulsante **Aggiungi ore** non verrà visualizzato. Per ulteriori informazioni, vedere la seguente sezione in questo articolo: [Quali ore possono essere aggiunte a un record di fatturazione](#what-hours-can-be-added-to-a-billing-record).

1. Seleziona le ore da includere nel record di fatturazione, quindi fai clic su **Aggiungi ore**. Il costo effettivo delle ore viene aggiunto come **Ore fatturabili** al **Totale record fatturazione**.

1. (Facoltativo) Fai clic su **Dettagli record fatturazione** per esaminare gli importi di **Ore fatturabili** e **Totale record fatturazione** e il totale dei record fatturazione nell&#39;intestazione dei record fatturazione.

### Includi spese fatturabili in un record fatturazione {#include-billable-expenses-in-a-billing-record}

Se si aggiungono spese fatturabili al record fatturazione, assicurarsi che le spese relative alle attività e al progetto siano contrassegnate come fatturabili. Le spese non contrassegnate come fatturabili non sono disponibili per l&#39;aggiunta in un record di fatturazione. Per ulteriori informazioni sull&#39;aggiunta delle spese, vedere l&#39;articolo [Gestione delle spese del progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Per aggiungere spese fatturabili a un record fatturazione:

{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona un progetto.
1. Fai clic su **Record fatturazione** nel pannello a sinistra.
1. Fai clic sul record fatturazione **Descrizione** per aprire la scheda **Dettagli record fatturazione**.
1. Fai clic su **Spese fatturabili** nel pannello a sinistra.
1. (Condizionale) Se hai aggiunto delle spese alle attività o al progetto e le hai contrassegnate come Fatturabili, fai clic su **Aggiungi spese**.

   >[!NOTE]
   >
   >Se hai delle spese ma non sono contrassegnate come fatturabili, il pulsante **Aggiungi spese** non viene visualizzato. Solo le spese fatturabili con un importo effettivo maggiore di zero possono essere incluse in un record di fatturazione.

1. Seleziona le spese fatturabili disponibili per l&#39;aggiunta al record fatturazione, quindi fai clic su **Aggiungi spese**.  L&#39;importo effettivo delle spese viene aggiunto come importo **Spese fatturabili** al **Totale record fatturazione**.

1. (Facoltativo) Fai clic su **Dettagli record fatturazione** per esaminare gli importi **Spese fatturabili** e **Totale record fatturazione** e il totale dei record fatturazione nell&#39;intestazione dei record fatturazione.

### Includi i ricavi fissi in un record di fatturazione {#include-fixed-revenues-in-a-billing-record}

È possibile aggiungere i ricavi fissi ai record di fatturazione se sono disponibili attività con ricavi fissi. Nessun altro tipo di attività o di ricavi progetto è disponibile per l&#39;aggiunta in un record di fatturazione. Per ulteriori informazioni sui tipi di ricavi, vedere la sezione &quot;Panoramica sulla fatturazione e sui ricavi&quot; nell&#39;articolo [Panoramica sulla fatturazione e sui ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona un progetto.
1. Fai clic su **Record fatturazione** nel pannello a sinistra.
1. Fai clic sul **Descrizione** del record fatturazione per aprire la scheda **Dettagli record fatturazione**.
1. Selezionare la scheda **Redditi fissi**.
1. Se hai aggiunto ricavi fissi alle attività, fai clic su **Aggiungi ricavi fissi**.

   >[!NOTE]
   >
   >Se le attività contengono importi di ricavi ma non sono contrassegnati come fissi, il pulsante **Aggiungi ricavi fissi** non verrà visualizzato.

1. Selezionare le attività di cui si desidera includere i ricavi fissi nel record fatturazione, quindi fare clic su **Aggiungi attività**.  L&#39;importo di **retribuzione fissa** delle attività viene aggiunto come importo di **retribuzione fatturabile** al **totale record fatturazione**.

1. (Facoltativo) Fai clic su **Dettagli record fatturazione** per esaminare gli importi **Ricavi fatturabili** e **Totale record fatturazione** e il totale dei record fatturazione nell&#39;intestazione dei record fatturazione.

## Modificare un record di fatturazione

Dopo aver creato un record di fatturazione e aver aggiunto ad esso ore, spese e ricavi, puoi modificare alcune informazioni sul record esistente prima che sia contrassegnato come Fatturato.

1. Passa al record fatturazione.
1. Seleziona **Dettagli record fatturazione** nel pannello a sinistra.
1. Modificare le informazioni in qualsiasi campo disponibile.

   Oppure

   Fai clic sull&#39;icona **Modifica** ![Modifica icona](assets/edit-icon.png) nell&#39;angolo superiore destro, quindi modifica le informazioni in tutti i campi disponibili.

   Aggiorna quanto segue:

   * **Descrizione**
   * **Data di Fatturazione**
   * **Stato fatturazione**

     >[!TIP]
     >
     >Se selezioni **Fatturato** per lo stato di fatturazione, il record di fatturazione non può essere modificato dopo il salvataggio delle modifiche.

   * **ID fattura**
   * **Numero OA**
   * **Importo aggiuntivo**

   I campi seguenti non sono disponibili per la modifica:

   * **Ore fatturabili:** il totale delle retribuzioni effettive delle ore incluse nel record di fatturazione. Per ulteriori informazioni, vedere la seguente sezione in questo articolo: [Includere ore fatturabili in un record di fatturazione](#include-billable-hours-in-a-billing-record).

   * **Spese fatturabili**: il totale dell&#39;importo effettivo delle spese fatturabili incluse nel record di fatturazione. Per ulteriori informazioni, vedere la seguente sezione in questo articolo: [Includere le spese fatturabili in un record di fatturazione](#include-billable-expenses-in-a-billing-record).

   * **Retribuzioni fatturabili**: il totale delle retribuzioni fisse delle attività incluse nel record di fatturazione. Per ulteriori informazioni, vedere la seguente sezione in questo articolo: [Includere i ricavi fissi in un record di fatturazione](#include-fixed-revenues-in-a-billing-record).

   * **Totale record fatturazione**: il totale di tutti gli importi fatturabili. Viene calcolata con la seguente formula:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Fai clic su **Salva modifiche**.
