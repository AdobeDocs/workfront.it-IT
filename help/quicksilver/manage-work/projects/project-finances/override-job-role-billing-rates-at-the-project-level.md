---
product-area: projects
navigation-topic: financials
title: Sostituisci tariffe di fatturazione mansione a livello di progetto
description: In qualità di project manager, puoi specificare la tariffa di fatturazione per una mansione in un progetto specifico. Questa tariffa di fatturazione a livello di progetto sostituisce la tariffa di fatturazione a livello di sistema per questa mansione. Per calcolare i ricavi, Workfront utilizza la tariffa di fatturazione a livello di progetto della mansione, anziché la tariffa di fatturazione a livello di sistema.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: 1992e1c07e5e530a2e627ef5d2059b2384b31000
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# Sostituisci tariffe di fatturazione mansione a livello di progetto

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

In qualità di project manager, puoi specificare la tariffa di fatturazione per una mansione in un progetto specifico. Questa tariffa di fatturazione a livello di progetto sostituisce la tariffa di fatturazione a livello di sistema per questa mansione. Per calcolare i ricavi, Workfront utilizza la tariffa di fatturazione a livello di progetto della mansione, anziché la tariffa di fatturazione a livello di sistema.

Questo articolo descrive come sostituire le tariffe di fatturazione dei ruoli di sistema per un progetto.

Per informazioni generali sulla sostituzione delle tariffe di fatturazione dei ruoli per i progetti e sul calcolo dei ricavi del progetto, vedere [Panoramica sulla sostituzione delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Per ulteriori informazioni sulla mansione utilizzata per calcolare i ricavi sul progetto, vedere la sezione &quot;Informazioni sui calcoli dei ricavi per le attività basate sulle assegnazioni di utenti e ruoli&quot; nell&#39;articolo [Panoramica su fatturazione e ricavi](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>Nel caso del reddito effettivo, le tariffe di fatturazione applicate alle ore aggiunte a una fatturazione contrassegnata come Fatturata, non devono essere influenzate dalle sostituzioni delle tariffe di fatturazione che si verificano dopo la fatturazione della fatturazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a progetti e dati finanziari</p> <p>Accesso amministrativo per le mansioni</p></td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td> 
   <td>Gestisci le autorizzazioni per il progetto che includono Modifica dati finanziari </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Sostituisci tariffe di fatturazione mansione a livello di progetto

Puoi sovrascrivere la tariffa di fatturazione di una mansione su un progetto nei seguenti modi:

* Una volta, selezionando una nuova tariffa per la mansione.\
  Il nuovo tasso viene utilizzato per l&#39;intera durata del progetto, per calcolare le entrate.

* Più volte, selezionando diverse nuove tariffe per intervalli di date specifici.\
  È possibile utilizzare un tasso diverso durante ogni intervallo di date specificato.

* È possibile aggiungere nuove tariffe di fatturazione a un modello di progetto e queste diventano tariffe di fatturazione del progetto quando si crea il progetto da tale modello. Per informazioni sulla modifica dei modelli, vedere [Modifica modelli di progetto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!TIP]
>
>Non puoi sovrascrivere le tariffe di fatturazione degli utenti per un progetto.

Per sostituire una tariffa di fatturazione per un progetto:

1. Vai al progetto per il quale desideri sostituire le tariffe di fatturazione.
1. Fai clic su **Tariffe di fatturazione** nel pannello a sinistra.
1. Fai clic su **Aggiungi tariffa di fatturazione** > **Nuova tariffa di fatturazione**.

   Viene visualizzata la casella Nuova tariffa di fatturazione.

1. Nel campo **Mansione**, selezionare la mansione per la quale si desidera modificare la tariffa di fatturazione.

   Nel campo **Tariffa di fatturazione predefinita** viene visualizzata la tariffa a livello di sistema per questa mansione.

1. Nel campo **Tariffe di fatturazione 1**, inserisci la sostituzione della tariffa di fatturazione una tantum, quindi fai clic su **Salva** per sostituire la tariffa di fatturazione una volta

   Oppure

   Fai clic su **Aggiungi tariffa** per aggiungere altre sostituzioni della tariffa di fatturazione.

1. (Condizionale) Se stai aggiungendo più di una sostituzione della tariffa di fatturazione, specifica le seguenti informazioni:

   * **Tariffe di fatturazione 1**: il valore della tariffa di fatturazione dall&#39;inizio del progetto alla prima data della prima sostituzione. In genere si tratta della stessa quantità della **Tariffa predefinita**.
   * **Data inizio**: è la data in cui termina la tariffa predefinita.
   * **Data di fine**: la data in cui termina la nuova sostituzione della tariffa di fatturazione.

   <!--<span class="preview">Sample image in the Preview environment:</span>-->
   ![Tariffe di fatturazione con date di sostituzione](assets/billing-rates-093025.png)

   <!--Sample image in the Production environment:
   ![Billing rates with override dates](assets/new-billing-rate-with-adjustment-dates-350x266.png)-->

1. Il fuso orario per le date selezionate viene visualizzato nella parte inferiore della casella Nuova tariffa di fatturazione. Si tratta del fuso orario associato all’istanza Workfront, come mostrato nell’area Informazioni cliente di Configura. Per informazioni, vedere [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. Workfront applica il tasso di ruolo di sostituzione alle ore che si verificano durante gli intervalli di tempo specificati durante il calcolo dei ricavi sul progetto.
1. Non devono esserci intervalli tra gli intervalli di tempo di due tassi di sostituzione. La **Data inizio** di una tariffa di sostituzione deve essere il giorno immediatamente successivo alla **Data fine** della data di sostituzione precedente.

1. Non è possibile specificare una data di inizio per il primo tasso di sostituzione né una data di fine per l&#39;ultimo tasso di sostituzione.\
   È consigliabile utilizzare la tariffa predefinita per la prima tariffa di sostituzione.\
   Workfront presuppone che il primo tasso di sostituzione venga applicato a tutte le ore con una data precedente alla data di fine della prima sostituzione e che l’ultimo tasso di sostituzione venga applicato a tutte le ore con una data successiva alla data di inizio dell’ultima sostituzione.\
   Se viene registrata un’ora prima della data di inizio pianificata del progetto, viene utilizzata la prima tariffa di fatturazione.\
   Se viene registrata un’ora dopo la data di completamento pianificata del progetto, viene utilizzata l’ultima tariffa di fatturazione.

1. Fai clic su **Salva**.
