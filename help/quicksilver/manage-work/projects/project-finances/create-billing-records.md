---
navigation-topic: financials
title: Creazione di record di fatturazione
description: Oltre a configurare i ricavi e le spese di tracciamento, puoi creare record di fatturazione per un progetto per le informazioni che devono essere fatturate.
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 1%

---

# Creazione di record di fatturazione

Oltre a configurare i ricavi e le spese di tracciamento, puoi creare record di fatturazione per un progetto per le informazioni che devono essere fatturate.

Non è possibile creare record di fatturazione per le attività. Puoi creare record di fatturazione solo per i progetti.

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

## Panoramica sui record di fatturazione

I record di fatturazione vengono creati come allegati a un progetto e contengono i dati finanziari del progetto, nonché alcune informazioni finanziarie per le attività di un progetto.

Quando si pianifica di utilizzare i record di fatturazione, tenere presente quanto segue:

* Creare un record di fatturazione quando si desidera fatturare un importo relativo al progetto a un fornitore o partner esterno. Oltre a fatturare un importo fisso a un&#39;origine esterna, ci sono momenti in cui è necessario fatturare la quantità di lavoro sul progetto (da ore registrate) a un appaltatore esterno, così come le spese sostenute o l&#39;importo dei ricavi fissi. Puoi includere tutte queste informazioni nello stesso record di fatturazione.
* Una volta che un record di fatturazione è impostato su Fatturato non può essere modificato.

   >[!IMPORTANT]
   >
   >Questo è importante quando le tariffe variano e si desidera bloccare le informazioni su ricavi e spese sul progetto. Aggiungendolo a un record di fatturazione e contrassegnandolo come Fatturato, non viene aggiornato quando le tariffe vengono aggiornate nel sistema.

* Impossibile eliminare un progetto con record di fatturazione contrassegnati come Fatturato.

## Creare un record di fatturazione

1. Passa a un progetto.
1. Fai clic su **Record di fatturazione** nel pannello a sinistra.

   Questa sezione potrebbe essere situata in **Mostra altro**.

1. Con **Dettagli record di fatturazione** nel pannello a sinistra, fai clic su **Nuovo record di fatturazione**.
1. In **Nuovo record di fatturazione** casella visualizzata, specificare le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Questo campo è obbligatorio. Specificare una descrizione per il record di fatturazione in modo da riflettere lo scopo o l'intento del record.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stato di Fatturazione</td> 
      <td> <p>Seleziona <strong>Non fatturato</strong>, se questo record non è ancora stato fatturato.</p> <p>Seleziona <strong>Fatturato</strong> quando viene fatturato il record di fatturazione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data Fatturazione</td> 
      <td>Seleziona la data in cui questo record di fatturazione viene fatturato facendo clic sull'icona del calendario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">N. ordine di acquisto</td> 
      <td>Se al record di fatturazione è associato un numero OA, specificare queste informazioni in questo campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID Fattura</td> 
      <td>Se al record di fatturazione è associata una fattura, specificare queste informazioni in questo campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importo aggiuntivo</td> 
      <td>Immettere l'importo fisso del record di fatturazione. Si tratta dell'importo che si intende fatturare a un cliente esterno, a un contraente o a un partner per questo progetto. Impossibile modificare l'importo dopo che lo stato del record di fatturazione è stato modificato in Fatturato.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) In **Forms personalizzato**, seleziona un modulo personalizzato per record di fatturazione da aggiungere al record di fatturazione.

   Prima di poter selezionare un modulo personalizzato per i record di fatturazione, è necessario creare un modulo personalizzato per i record di fatturazione (o un altro utente con accesso a moduli personalizzati). Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Per informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   È possibile ripetere questo passaggio per aggiungere altri moduli personalizzati necessari per il record di fatturazione.

1. Fai clic su **Salva.**

   Viene creato il record di fatturazione. Per includere nel record di fatturazione le ore fatturabili, le spese e i ricavi fissi, segui i passaggi descritti nella sottosezione seguente.

## Includi ore fatturabili, spese e ricavi fissi in un record di fatturazione

* [Includi ore fatturabili in un record di fatturazione](#include-billable-hours-in-a-billing-record)
* [Includi spese fatturabili in un record di fatturazione](#include-billable-expenses-in-a-billing-record)
* [Includi ricavi fissi in un record di fatturazione](#include-fixed-revenues-in-a-billing-record)

### Includi ore fatturabili in un record di fatturazione {#include-billable-hours-in-a-billing-record}

Nei record di fatturazione puoi includere ore che sono state registrate su attività, problemi o progetti.\
Se l’utente che registra le ore o il ruolo di lavoro principale è associato a un tasso di fatturazione per ora, i ricavi di queste ore vengono aggiunti al record di fatturazione.

* [Quali ore possono essere aggiunte a un record di fatturazione?](#what-hours-can-be-added-to-a-billing-record)
* [Aggiungi ore a un record di fatturazione](#add-hours-to-a-billing-record)

#### Quali ore possono essere aggiunte a un record di fatturazione? {#what-hours-can-be-added-to-a-billing-record}

Puoi aggiungere ore a un record di fatturazione quando sono soddisfatte le seguenti condizioni:

* Attività, problemi o il progetto ha ore registrate.
* Il tipo di ora delle ore registrate viene contrassegnato come Conteggio come Ricavo.

   Per ulteriori informazioni sui tipi di ora, consulta l’articolo [Gestione dei tipi di ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Tutte le ore registrate per i problemi o per il progetto possono essere aggiunte a un record di fatturazione se l’utente che registra l’ora ha un tasso di fatturazione per ora associato a essi o il ruolo principale del lavoro.
* Se le ore sono registrate su un&#39;attività, l&#39;attività deve avere il seguente tipo di ricavi:

   * Impossibile impostare il tipo di ricavi su Non fatturabile.
   * Se Tipo di ricavi è impostato su Orario utente, l’utente che registra il tempo deve avere un tasso di fatturazione per ora impostato nel proprio profilo.
   * Se Tipo di ricavi è impostato su Ruolo orario, il ruolo principale dell’utente che registra il tempo deve avere un tasso di fatturazione per ora.

      >[!NOTE]
      >
      >È possibile sostituire i tassi di fatturazione per i ruoli di lavoro a livello di progetto.\
      >Per ulteriori informazioni sull&#39;override dei tassi di fatturazione dei ruoli di lavoro, vedere la sezione &quot;Overrides Job Role Billing Rates at at the Project Level&quot; nell&#39;articolo [Panoramica sulla priorità dei tassi di fatturazione dei ruoli di lavoro e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Se **Richiedi tempo per l&#39;approvazione del progetto** è selezionato in Impostazioni progetto, quindi il proprietario del progetto deve approvare le ore registrate.\
   Per ulteriori informazioni sulla richiesta di approvazione per l’orario di progetto, consulta l’articolo [Richiedi tempo per l’approvazione di un progetto](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Aggiungi ore a un record di fatturazione {#add-hours-to-a-billing-record}

Per aggiungere ore fatturabili a un record di fatturazione:

1. Passa al progetto con i record di fatturazione.
1. Fai clic su **Record di fatturazione** nel pannello a sinistra.

   Questa sezione potrebbe essere situata in **Mostra altro**.

1. Fai clic sul pulsante **Descrizione** di un record di fatturazione per aprire **Dettagli record di fatturazione** scheda .

1. Fai clic su **Ore fatturabili** nel pannello a sinistra.
1. Se ci sono ore che possono essere incluse in un record di fatturazione, fai clic su **Aggiungi ore**.\
   La **Aggiungi ore fatturabili** si apre la casella.

   >[!NOTE]
   >
   >Se non ci sono ore registrate o se le ore registrate non soddisfano le condizioni necessarie per essere aggiunte a un record di fatturazione, il **Aggiungi ore** il pulsante non viene visualizzato. Per ulteriori informazioni sulle ore che possono essere registrate in un record di fatturazione, consulta la sezione . [Quali ore possono essere aggiunte a un record di fatturazione?](#what-hours-can-be-added-to-a-billing-record) in questo articolo.

1. Selezionare le ore da includere nel record di fatturazione e fare clic su **Aggiungi ore**.\
   Il costo effettivo delle ore viene aggiunto come **Ore fatturabili** l&#39;importo **Totale record di fatturazione**.

1. (Facoltativo) Fai clic su **Dettagli record di fatturazione** per rivedere **Ore fatturabili** e **Totale record di fatturazione** importi. Puoi anche vedere il totale del record di fatturazione nell’intestazione del record di fatturazione.

### Includi spese fatturabili in un record di fatturazione {#include-billable-expenses-in-a-billing-record}

Se si aggiungono spese fatturabili al record di fatturazione, assicurarsi che le spese relative alle attività e al progetto siano contrassegnate come fatturabili. Le spese non contrassegnate come fatturabili non sono disponibili per l’aggiunta in un record di fatturazione. Per ulteriori informazioni sull&#39;aggiunta delle spese, consulta l&#39;articolo [Gestione delle spese di progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Per aggiungere spese fatturabili a un record di fatturazione:

1. Passa al progetto con i record di fatturazione.
1. Fai clic su **Record di fatturazione** nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **Mostra altro**, quindi **Record di fatturazione**.

1. Fai clic sul pulsante **Descrizione** di un record di fatturazione per aprire **Dettagli record di fatturazione** scheda .

1. Fai clic su **Spese fatturabili** nel pannello a sinistra.
1. (Condizionale) Se hai aggiunto le spese alle attività o al progetto e le hai contrassegnate come fatturabili, fai clic su **Aggiungi spese**.

   >[!NOTE]
   >
   >Se hai delle spese ma queste non sono contrassegnate come fatturabili, il **Aggiungi spese** il pulsante non viene visualizzato. Solo le spese fatturabili con un importo effettivo maggiore di zero possono essere incluse in un record di fatturazione.

1. Selezionare le spese fatturabili disponibili da aggiungere al record di fatturazione, quindi fare clic su **Aggiungi spese**.\
   L&#39;importo effettivo delle spese viene aggiunto come **Spese fatturabili** l&#39;importo **Totale record di fatturazione**.

1. (Facoltativo) Fai clic su **Dettagli record di fatturazione** per rivedere **Spese fatturabili** e **Totale record di fatturazione** importi. Puoi anche vedere il totale del record di fatturazione nell’intestazione del record di fatturazione.

### Includi ricavi fissi in un record di fatturazione {#include-fixed-revenues-in-a-billing-record}

È possibile aggiungere i ricavi fissi ai record di fatturazione se sono disponibili attività con ricavi fissi. Nessun altro tipo di attività o ricavi di progetto è disponibile per essere aggiunto in un record di fatturazione. Per ulteriori informazioni sui tipi di ricavi, consulta la sezione [Panoramica di fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) sezione [Panoramica di fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Per aggiungere ricavi fissi a un record di fatturazione:

1. Passa al progetto con i record di fatturazione.
1. Fai clic su **Record di fatturazione** nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **Mostra altro**, quindi **Record di fatturazione**.

1. Fai clic sul pulsante **Descrizione** di un record di fatturazione per aprire **Dettagli record di fatturazione** scheda .

1. Seleziona la **Entrate fisse** scheda .
1. Se hai aggiunto ricavi fissi alle tue attività, fai clic su **Aggiungi ricavi fissi**.

   >[!NOTE]
   >
   >Se disponi di importi di ricavi per le attività ma non sono contrassegnati come &quot;Fisso&quot;, il **Aggiungi ricavi fissi** il pulsante non viene visualizzato.

1. Selezionare le attività di cui si desidera includere i ricavi fissi nel record di fatturazione, quindi fare clic su **Aggiungi attività**.\
   La **Entrate fisse** l&#39;importo delle attività viene aggiunto come **Entrate fatturabili** l&#39;importo **Totale record di fatturazione**.

1. (Facoltativo) Fai clic su **Dettagli record di fatturazione** per rivedere **Entrate fatturabili** e **Totale record di fatturazione** importi. Puoi anche vedere il totale del record di fatturazione nell’intestazione del record di fatturazione.

## Modificare un record di fatturazione

Dopo aver creato un record di fatturazione che include ore, spese e ricavi nel record di fatturazione, è possibile modificare alcune informazioni sul record esistente, prima che venga contrassegnato come Fatturato.

1. Passa al record di fatturazione.
1. Con **Dettagli record di fatturazione** selezionati nel pannello a sinistra , modifica le informazioni in tutti i campi disponibili

   Oppure

   Fai clic sul pulsante **Icona Modifica** ![](assets/edit-icon.png) nell’angolo in alto a destra, quindi modifica le informazioni in tutti i campi disponibili.

   Aggiorna quanto segue:

   * **Descrizione**
   * **Stato di Fatturazione**

      >[!TIP]
      >
      >Se si seleziona **Fatturato** per lo stato di fatturazione, il record di fatturazione non può essere modificato dopo aver salvato le modifiche.

   * **Data Fatturazione**
   * **N. ordine di acquisto**
   * **ID Fattura**
   * **Importo aggiuntivo**

   I campi seguenti non sono disponibili per la modifica:

   * **Ore fatturabili:** Totale dei ricavi effettivi delle ore incluse nel record di fatturazione. Per ulteriori informazioni sull&#39;inclusione delle ore in un record di fatturazione, consulta la sezione . [Includi ore fatturabili in un record di fatturazione](#include-billable-hours-in-a-billing-record) in questo articolo.

   * **Spese fatturabili**: Totale dell&#39;importo effettivo delle spese fatturabili incluse nel record di fatturazione. Per ulteriori informazioni sull&#39;inclusione delle spese fatturabili in un record di fatturazione, consulta la sezione . [Includi spese fatturabili in un record di fatturazione](#include-billable-expenses-in-a-billing-record) in questo articolo.

   * **Entrate fatturabili**: Totale dei ricavi fissi delle attività incluse nel record di fatturazione. Per ulteriori informazioni sull&#39;inclusione dei ricavi fissi in un record di fatturazione, consulta la sezione . [Includi ricavi fissi in un record di fatturazione](#include-fixed-revenues-in-a-billing-record) in questo articolo.

   * **Totale record di fatturazione**: Totale di tutti gli importi fatturabili. Viene calcolata con la seguente formula:

      ```
      Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
      ```


1. Fai clic su **Salva***modifiche**.
