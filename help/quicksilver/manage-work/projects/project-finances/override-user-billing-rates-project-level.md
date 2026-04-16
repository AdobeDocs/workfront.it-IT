---
content-type: overview
product-area: projects
navigation-topic: financials
title: Sostituisci tariffe di fatturazione utente a livello di progetto
description: Questo articolo descrive come sovrascrivere le tariffe di fatturazione degli utenti del sistema per un progetto.
author: Lisa
feature: Work Management
exl-id: eb7dbb6f-a31c-4569-be54-9a151dcf4135
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 4%

---

# Sostituire le tariffe di fatturazione degli utenti a livello di progetto

In qualità di project manager, puoi specificare la tariffa di fatturazione di un utente in un progetto specifico. Questa tariffa di fatturazione a livello di progetto sostituisce la tariffa di fatturazione a livello di sistema per questo utente. Per calcolare i ricavi, Workfront utilizza la tariffa di fatturazione dell’utente a livello di progetto, anziché la tariffa di fatturazione a livello di sistema.

Questo articolo descrive come sovrascrivere le tariffe di fatturazione degli utenti del sistema per un progetto.

Per informazioni generali sulla sostituzione delle tariffe di fatturazione per i progetti e sul calcolo dei ricavi del progetto, vedere [Panoramica sulla sostituzione delle tariffe di fatturazione e sul calcolo dei ricavi per un progetto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Per ulteriori informazioni sul calcolo dei ricavi per il progetto, vedere [Panoramica sulla gerarchia dei ricavi e dei costi](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) e la sezione [Calcoli dei ricavi per le attività basati sulle assegnazioni di utenti e ruoli](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) nell&#39;articolo [Panoramica sulla fatturazione e sui ricavi](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

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
   <td>Flusso di lavoro Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a progetti e dati finanziari</p>
       <p><p>È inoltre necessario disporre di uno dei seguenti elementi:</p> 
        <ul> 
          <li> <p>Livello di accesso Amministratore di sistema. </li> 
          <li> <p>Impostazione di <b>Utenti</b> nel livello di accesso configurato per l'accesso di <b>Modifica</b>, con <b>Crea</b> e almeno una delle due opzioni di <b>Amministratore utenti</b> abilitate in <b>Ottimizza le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se <b>User Admin (Group Users)</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Gestisci le autorizzazioni per il progetto che includono Modifica dati finanziari </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Sostituisci tariffe di fatturazione utente a livello di progetto

Quando sostituisci la tariffa di fatturazione di un utente in un progetto, puoi assegnare date di validità e ciascun intervallo di date ha una tariffa diversa. Se non si assegnano date di validità, la sostituzione della tariffa di fatturazione inserita viene utilizzata per l&#39;intera durata del progetto per calcolare i ricavi.

Per sostituire la tariffa di fatturazione di un utente per un progetto:

1. Vai al progetto per il quale desideri sostituire le tariffe di fatturazione.
1. Fai clic su **Tariffe** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**.
1. Fare clic sulla scheda **Fatturazione** se non è già selezionata.
1. Fai clic su **Aggiungi tariffa di fatturazione** > **Nuova tariffa di fatturazione utente**.

   Viene visualizzata la casella Nuova tariffa di fatturazione utente (New User Billing Rate).

1. Nel campo **Utente**, selezionare l&#39;utente per il quale si desidera modificare la tariffa di fatturazione.
1. Selezionare **Valuta** per la sostituzione della tariffa di fatturazione.
1. Nel campo **Tariffa di fatturazione** immettere la prima sostituzione della tariffa di fatturazione.
1. (Facoltativo) Fai clic su **Aggiungi tariffa effettiva data** per aggiungere altre sostituzioni della tariffa di fatturazione.
1. (Condizionale) Se stai aggiungendo più sostituzioni di tariffe di fatturazione, specifica le seguenti informazioni per ogni riga:

   * **Tariffa di fatturazione**: il valore della tariffa di fatturazione durante il periodo di tempo specificato.
   * **Data inizio**: la data di inizio della sostituzione della tariffa di fatturazione.
   * **Data di fine**: la data in cui termina la sostituzione della tariffa di fatturazione.

   ![La casella Tariffa di fatturazione nuovo utente mostra le date di validità](assets/new-user-billing-rate-on-project2.png)

   Workfront applica il tasso utente di sostituzione alle ore che si verificano durante questi intervalli di tempo durante il calcolo dei ricavi sul progetto.

   Workfront consente di lasciare degli spazi tra i tempi di override, ma riceverai un avviso per confermare che è intenzionale.

   Non è necessario specificare una data di inizio per il primo tasso di sostituzione né una data di fine per l&#39;ultimo tasso di sostituzione.

   Se si inserisce una sola sostituzione della tariffa di fatturazione, questa viene applicata per l&#39;intera durata del progetto. Se si aggiungono più sostituzioni valide per data, Workfront presuppone che la prima sostituzione venga applicata a tutte le ore precedenti alla data di fine e che l&#39;ultima sostituzione venga applicata a tutte le ore successive alla data di inizio.

   Workfront presuppone che il primo tasso di sostituzione venga applicato a tutte le ore con una data precedente alla data di fine della prima sostituzione e che l’ultimo tasso di sostituzione venga applicato a tutte le ore con una data successiva alla data di inizio dell’ultima sostituzione.

   Se viene registrata un’ora prima della data di inizio pianificata del progetto, viene utilizzata la prima tariffa di fatturazione.

   Se viene registrata un’ora dopo la data di completamento pianificata del progetto, viene utilizzata l’ultima tariffa di fatturazione.

1. Fai clic su **Salva**.
