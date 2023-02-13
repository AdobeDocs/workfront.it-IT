---
product-area: projects
navigation-topic: financials
title: Ignora tassi di fatturazione ruolo lavoro a livello di progetto
description: In qualità di project manager, puoi specificare il tasso di fatturazione per un ruolo di lavoro in un progetto specifico. Questo tasso di fatturazione a livello di progetto sostituisce il tasso di fatturazione a livello di sistema per questo ruolo di lavoro. Workfront utilizza il tasso di fatturazione a livello di progetto del ruolo di processo per calcolare i ricavi, invece di utilizzare il tasso di fatturazione a livello di sistema.
author: Alina
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# Ignora tassi di fatturazione ruolo lavoro a livello di progetto

In qualità di project manager, puoi specificare il tasso di fatturazione per un ruolo di lavoro in un progetto specifico. Questo tasso di fatturazione a livello di progetto sostituisce il tasso di fatturazione a livello di sistema per questo ruolo di lavoro. Workfront utilizza il tasso di fatturazione a livello di progetto del ruolo di processo per calcolare i ricavi, invece di utilizzare il tasso di fatturazione a livello di sistema.

Questo articolo descrive come ignorare le tariffe di fatturazione dei ruoli di lavoro del sistema per un progetto.

Per informazioni generali sull&#39;override dei tassi di fatturazione dei ruoli di lavoro per i progetti e sul calcolo dei ricavi dei progetti, consulta [Panoramica sulla priorità dei tassi di fatturazione dei ruoli di lavoro e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Per ulteriori informazioni sul ruolo del lavoro utilizzato per calcolare i ricavi del progetto, consulta la sezione &quot;Informazioni sui calcoli dei ricavi per le attività in base alle assegnazioni di utenti e ruoli&quot; nell’articolo [Panoramica di fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>Nel caso dei ricavi effettivi, i tassi di fatturazione applicati alle ore aggiunte a un record di fatturazione contrassegnato come Fatturato non devono essere influenzati dalle sostituzioni dei tassi di fatturazione che si verificano dopo la fatturazione del record di fatturazione.

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
   <td> <p>Modifica l’accesso a progetti e dati finanziari</p> <p>Accesso amministrativo per i ruoli di lavoro</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per il progetto che include Modifica dati finanziari </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Ignora tassi di fatturazione ruolo lavoro a livello di progetto

È possibile ignorare il tasso di fatturazione di un ruolo di lavoro in un progetto nei seguenti modi:

* Una volta, selezionando un nuovo tasso per il ruolo di lavoro.\
   Il nuovo tasso viene utilizzato per l’intera durata del progetto, per calcolare i ricavi.

* Più volte, selezionando diversi nuovi tassi per specifici intervalli di date.\
   È possibile utilizzare un tasso diverso per ogni intervallo di date specificato.

>[!TIP]
>
>Non è possibile ignorare le tariffe di fatturazione utente per un progetto.

Per ignorare un tasso di fatturazione per un progetto:

1. Passa al progetto per il quale desideri ignorare le tariffe di fatturazione.
1. Fai clic su **Tassi di fatturazione** nel pannello a sinistra. Potrebbe essere necessario fare clic **Mostra altro**.
1. Fai clic su **Aggiungi tasso di fatturazione** > **Nuovo tasso di fatturazione**.

   Viene visualizzata la casella Nuovo tasso di fatturazione.

1. In **Ruolo** selezionare il ruolo del processo per il quale si desidera modificare il tasso di fatturazione.

   ![](assets/override-billing-rate-on-project-nwe-350x310.png)

   La **Tasso di fatturazione predefinito** visualizza la frequenza a livello di sistema per questo ruolo di processo.

1. In **Tassi di fatturazione 1** immettere l&#39;override del tasso di fatturazione una tantum, quindi fare clic su **Salva** per ignorare una volta il tasso di fatturazione

   Oppure

   Fai clic su **Aggiungi tasso** per aggiungere più sostituzioni del tasso di fatturazione.

1. (Condizionale) Se stai aggiungendo più di una sostituzione del tasso di fatturazione, specifica le seguenti informazioni:

   * **Tassi di fatturazione 1**: il valore del tasso di fatturazione dall&#39;inizio del progetto alla prima data della prima sostituzione. In genere si tratta della stessa quantità di **Frequenza predefinita**.
   * **Data di inizio**: si tratta della data in cui termina il tasso predefinito.
   * **Data di fine**: la data in cui termina l&#39;override del nuovo tasso di fatturazione.

   ![new_billing_rate_with_adjustment_date.png](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. Il fuso orario per le date selezionate viene visualizzato nella parte inferiore della casella Nuovo tasso di fatturazione. Questo è il fuso orario associato all’istanza Workfront, come mostrato nell’area Informazioni cliente di Configurazione. Per informazioni, consulta [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. Workfront applica la percentuale di ruolo di sostituzione alle ore che si verificano durante i periodi di tempo specificati durante il calcolo dei ricavi del progetto.
1. Non dovrebbero esserci divari tra i fotogrammi temporali di due tassi di sostituzione. La **Data di inizio** di un tasso di sostituzione deve essere il giorno immediatamente successivo al **Data di fine** della data di sostituzione precedente.

1. Non è possibile specificare una data di inizio per il primo tasso di sostituzione, né una data di fine per l&#39;ultimo tasso di sostituzione.\
   È consigliabile utilizzare il tasso predefinito per il primo tasso di sostituzione.\
   Workfront presuppone che il primo tasso di sostituzione sia applicato per tutte le ore con una data precedente alla data di fine della prima sostituzione e che l&#39;ultimo tasso di sostituzione sia applicato per tutte le ore con una data successiva alla data di inizio dell&#39;ultima sostituzione.\
   Se viene registrata un&#39;ora prima della data di inizio prevista del progetto, viene utilizzata la prima tariffa di fatturazione.\
   Se dopo la data di completamento pianificata del progetto viene registrata un’ora, viene utilizzato l’ultimo tasso di fatturazione.

1. Fai clic su **Salva**.
