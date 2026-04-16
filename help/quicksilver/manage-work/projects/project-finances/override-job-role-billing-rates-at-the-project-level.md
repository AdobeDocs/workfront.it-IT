---
product-area: projects
navigation-topic: financials
title: Sostituisci tariffe di fatturazione mansione a livello di progetto
description: Questo articolo descrive come sostituire le tariffe di fatturazione dei ruoli di sistema per un progetto.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: e3d4ffe2d42f9de3000df0ba1a924ca36fea9248
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 6%

---

# Sostituire tariffe di fatturazione della mansione a livello di progetto

In qualità di project manager, puoi specificare la tariffa di fatturazione per una mansione in un progetto specifico. Questa tariffa di fatturazione a livello di progetto sostituisce la tariffa di fatturazione a livello di sistema per questa mansione. Per calcolare i ricavi, Workfront utilizza la tariffa di fatturazione a livello di progetto della mansione, anziché la tariffa di fatturazione a livello di sistema.

Questo articolo descrive come sostituire le tariffe di fatturazione dei ruoli di sistema per un progetto.

Per informazioni generali sulla sostituzione delle tariffe di fatturazione dei ruoli per i progetti e sul calcolo dei ricavi del progetto, vedere [Panoramica sulla sostituzione delle tariffe di fatturazione e sul calcolo dei ricavi per un progetto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Per ulteriori informazioni sulla mansione utilizzata per calcolare i ricavi sul progetto, vedere [Panoramica sulla gerarchia dei ricavi e dei costi](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) e la sezione [Calcoli dei ricavi per le attività basati sulle assegnazioni di utenti e ruoli](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) nell&#39;articolo [Panoramica sulla fatturazione e sui ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>Nel caso del reddito effettivo, le tariffe di fatturazione applicate alle ore aggiunte a una fatturazione contrassegnata come Fatturata, non devono essere influenzate dalle sostituzioni delle tariffe di fatturazione che si verificano dopo la fatturazione della fatturazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td> <p>Per ignorare una tariffa di fatturazione di un ruolo per un progetto: Qualsiasi pacchetto Workfront o Workflow</p>
        <p>Per applicare gli attributi alla mansione: Workflow Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a progetti e dati finanziari</p> <p>Accesso amministrativo per le mansioni</p></td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Gestisci le autorizzazioni per il progetto che include Modifica tariffe di fatturazione </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Sostituire tariffe di fatturazione della mansione a livello di progetto

Quando si sostituisce la tariffa di fatturazione di un OdL in un progetto, è possibile assegnare date di validità e ciascun intervallo di date ha una tariffa diversa. Se non si assegnano date di validità, la sostituzione della tariffa di fatturazione inserita viene utilizzata per l&#39;intera durata del progetto per calcolare i ricavi.

È possibile aggiungere nuove tariffe di fatturazione a un modello di progetto e queste diventano tariffe di fatturazione del progetto quando si crea il progetto da tale modello. Per informazioni sulla modifica dei modelli, vedere [Modifica modelli di progetto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!TIP]
>
>Non puoi sovrascrivere le tariffe di fatturazione dell’utente per un progetto a meno che non disponi del pacchetto Workflow Ultimate.

Per sostituire una tariffa di fatturazione per un progetto:

1. Vai al progetto per il quale desideri sostituire le tariffe di fatturazione.
1. Fai clic su **Tariffe di fatturazione** nel pannello a sinistra.

   Oppure

   Fai clic su **Tariffe** nel pannello a sinistra, quindi sulla scheda **Fatturazione**, se non è già selezionata.

1. Fai clic su **Aggiungi tariffa di fatturazione > Nuova tariffa di fatturazione mansione**.

   Viene visualizzata la casella Nuova tariffa di fatturazione.

1. Nel campo **Mansione**, selezionare la mansione per la quale si desidera modificare la tariffa di fatturazione.

1. (Facoltativo) Seleziona gli attributi per la tariffa di fatturazione, ad esempio agenzia o ubicazione.

   L’amministratore di sistema definisce gli attributi della tariffa nell’area Setup (Configura).

1. Selezionare **Valuta** per la sostituzione della tariffa di fatturazione.
1. Nel campo **Tariffa di fatturazione**, inserisci la sostituzione della tariffa di fatturazione, quindi fai clic su **Salva** per sostituire la tariffa di fatturazione una volta

   Oppure

   Fai clic su **Aggiungi tariffa** per aggiungere altre sostituzioni della tariffa di fatturazione.

1. (Condizionale) Per le sostituzioni dei tassi di fatturazione effettivi per data, inserire le seguenti informazioni per ogni riga:

   * **Tariffa di fatturazione**: il valore della tariffa di fatturazione dall&#39;inizio del progetto alla prima data della prima sostituzione.
   * **Data inizio**: la data di inizio della sostituzione della tariffa di fatturazione.
   * **Data di fine**: la data di fine della sostituzione della tariffa di fatturazione.

   ![Tariffe di fatturazione con date di sostituzione](assets/new-job-role-billing-rate-on-project2.png)

   Workfront applica il tasso di ruolo di sostituzione alle ore che si verificano durante questi intervalli di tempo durante il calcolo dei ricavi sul progetto.

   Workfront consente di lasciare degli spazi tra i tempi di override, ma riceverai un avviso per confermare che è intenzionale.

   Non è necessario specificare una data di inizio per il primo tasso di sostituzione né una data di fine per l&#39;ultimo tasso di sostituzione.

   Se si inserisce una sola sostituzione della tariffa di fatturazione, questa viene applicata per l&#39;intera durata del progetto. Se si aggiungono più sostituzioni valide per data, Workfront presuppone che la prima sostituzione venga applicata a tutte le ore precedenti alla data di fine e che l&#39;ultima sostituzione venga applicata a tutte le ore successive alla data di inizio.

   Workfront presuppone che il primo tasso di sostituzione venga applicato a tutte le ore con una data precedente alla data di fine della prima sostituzione e che l’ultimo tasso di sostituzione venga applicato a tutte le ore con una data successiva alla data di inizio dell’ultima sostituzione.

   Se viene registrata un’ora prima della data di inizio pianificata del progetto, viene utilizzata la prima tariffa di fatturazione.

   Se viene registrata un’ora dopo la data di completamento pianificata del progetto, viene utilizzata l’ultima tariffa di fatturazione.

1. Fai clic su **Salva**.
