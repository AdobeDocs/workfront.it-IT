---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Panoramica sul calcolo delle ore e dell'FTE per utenti e ruoli nella pianificazione risorse
description: Panoramica del calcolo delle ore e dell'FTE per utenti e ruoli nella pianificazione risorse
author: Lisa
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 0%

---

# Panoramica del calcolo delle ore e dell&#39;FTE per utenti e ruoli nella pianificazione risorse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

È possibile visualizzare l&#39;allocazione e la disponibilità delle risorse nella Pianificazione risorse in base alle ore, FTE o Costo.\
Per ulteriori informazioni sul calcolo dei costi nella programmazione delle risorse, vedere [Calcolare i costi nella programmazione delle risorse](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

&quot;FTE&quot; sta per Equivalente tempo pieno. Si tratta di una misura del tempo che rappresenta la quantità di ore dedicate al lavoro reale durante un giorno o una settimana per un utente o una mansione.

Le seguenti serie di informazioni sulle risorse vengono calcolate in modo diverso in Pianificazione risorse:

* I valori di Ore o FTE disponibili vengono calcolati in base al modo in cui l&#39;amministratore di sistema configura le preferenze di Gestione risorse nel sistema.\
  Per ulteriori informazioni sul calcolo dei valori delle ore e dell&#39;FTE disponibili, vedere [Calcolare le ore o l&#39;FTE disponibili per gli utenti e le mansioni in Pianificazione risorse](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
  Per ulteriori informazioni sulla definizione delle preferenze di Gestione risorse per Adobe Workfront, vedere [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* Tutti gli altri valori FTE vengono calcolati in base alla pianificazione predefinita del sistema.\
  Per ulteriori informazioni sulla visualizzazione di tutti gli altri valori nella pianificazione delle risorse quando si utilizza l&#39;FTE, vedere la sezione [Calcolare tutti gli altri valori di ore e FTE per gli utenti e le mansioni nella pianificazione delle risorse](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) in questo articolo.

È importante comprendere cos’è l’FTE per ciascuno degli utenti e i relativi ruoli per gestire in modo accurato le risorse mentre vengono assegnate al lavoro.

## Calcola le ore o l&#39;FTE disponibili per gli utenti e le mansioni in Pianificazione risorse {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [Calcola le ore e l&#39;FTE disponibili per un utente nella Programmazione risorse](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [Calcola le ore e l&#39;FTE disponibili per una mansione nella Programmazione risorse](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [Calcola le ore e l&#39;FTE disponibili per un utente nella Programmazione delle risorse (esempio)](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### Calcolare le ore e l&#39;FTE disponibili per un utente nella Programmazione delle risorse {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

L’amministratore di Workfront determina il modo in cui viene calcolato il tempo disponibile per un utente selezionando l’opzione per utilizzare una delle seguenti opzioni nell’area Gestione risorse di Configurazione:

* La pianificazione predefinita del sistema e l&#39;FTE dell&#39;utente.
* La pianificazione dell’utente.

![Impostazione di sistema per le pianificazioni utente](assets/setup-resource-mgmt.png)

>[!NOTE]
>
>Questo determina come calcolare la disponibilità delle risorse a livello di sistema. Per ulteriori informazioni sulla definizione delle preferenze di Gestione risorse per il sistema, vedere [Configurare le preferenze di Gestione risorse](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

In base alla configurazione di questa impostazione, la disponibilità degli utenti nella pianificazione risorse (ore e disponibilità FTE) viene calcolata utilizzando i metodi seguenti:

* **Pianificazione predefinita**: la pianificazione predefinita del sistema e l&#39;FTE dell&#39;utente vengono utilizzati per determinare le ore disponibili e il valore FTE dell&#39;utente nella pianificazione risorse. La pianificazione dell’utente viene ignorata. In questo caso:

   * Le **ore disponibili** nella Programmazione delle risorse vengono calcolate con la seguente formula:

     `User Available Hours = Default Schedule Hours * User FTE value`

     Ad esempio, se la programmazione predefinita prevede 40 ore settimanali disponibili per il lavoro e l&#39;FTE dell&#39;utente è 0,5, l&#39;utente è disponibile a lavorare 20 ore settimanali nella Programmazione delle risorse.

     Per ulteriori informazioni sulle pianificazioni, inclusa la pianificazione predefinita, vedere [Creare una pianificazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * L&#39;**FTE disponibile** per l&#39;utente nella Programmazione risorse è uguale all&#39;FTE utente specificato nelle impostazioni utente.

     Ad esempio, se l’FTE dell’utente è 0,5 nelle impostazioni utente, l’FTE disponibile dell’utente è 0,5 nella Programmazione delle risorse. Per ulteriori informazioni sul valore dell&#39;FTE utente visualizzato nelle impostazioni utente, vedere [Modifica del profilo di un utente](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* **Pianificazione dell&#39;utente**: la pianificazione dell&#39;utente viene utilizzata per determinare la disponibilità dell&#39;utente nella Programmazione delle risorse. Il valore dell&#39;FTE utente viene ignorato. In questo caso:

   * Le **ore disponibili** nella Programmazione delle risorse sono uguali alle ore della Pianificazione dell&#39;utente.

     Ad esempio, se la pianificazione dell&#39;utente dispone di 40 ore settimanali per lavorare, l&#39;utente è disponibile a lavorare per 40 ore settimanali nella pianificazione risorse.

   * L&#39;**FTE disponibile** nella Programmazione delle risorse viene calcolato con la seguente formula:

     `User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours`

     Ad esempio, se la pianificazione dell’utente ha 20 ore disponibili per lavorare e la pianificazione predefinita in Workfront ha 40 ore disponibili per lavorare, l’FTE dell’utente è 0,5.

     Per ulteriori informazioni sulle pianificazioni, inclusa la pianificazione predefinita, vedere [Creare una pianificazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

>[!NOTE]
>
>Se l&#39;utente non è associato a una pianificazione, le ore disponibili per l&#39;utente vengono calcolate utilizzando la pianificazione predefinita.

### Calcolare le ore e l&#39;FTE disponibili per una mansione nella Programmazione delle risorse {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

Prima di tutto è necessario calcolare la disponibilità dell&#39;utente, quindi è possibile calcolare la disponibilità di ciascuna mansione.

La disponibilità dei ruoli nella pianificazione risorse tiene conto della disponibilità totale dell&#39;utente e della **percentuale di disponibilità FTE** associata a ogni ruolo dell&#39;utente.\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

Per ulteriori informazioni sull&#39;associazione di un valore di **Percentuale di disponibilità FTE** a una mansione per un utente, vedere [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Ad esempio, se il valore di Ore disponibili per un utente è 40 e l&#39;utente può svolgere un Ruolo principale per il 75% del tempo, e un Altro Ruolo per il 25% del tempo, la Programmazione delle risorse mostra che il valore **Ore disponibili** per il Ruolo principale per una settimana è 30 ore e che il valore **Ore disponibili** per l&#39;Altro Ruolo è 10 ore. In questo caso, l’FTE per il ruolo principale è 0,75 e l’FTE per l’altro ruolo è 0,25.

>[!NOTE]
>
>Il tempo totale disponibile per l&#39;utente viene calcolato in base a uno dei due metodi descritti in [Calcolare le ore e l&#39;FTE disponibili per un utente nella sezione Pianificazione risorse](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) di questo articolo.

Quando si visualizza la Programmazione delle risorse nella Vista ruolo, la disponibilità di una mansione corrisponde al totale della disponibilità di tutti gli utenti che possono svolgere quella mansione.\
Per ulteriori informazioni sulla disponibilità delle risorse nella Programmazione delle risorse, vedere [Panoramica sulla programmazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Calcola le ore e l&#39;FTE disponibili per un utente nella Programmazione delle risorse (esempio) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

Nella tabella seguente viene illustrato come vengono calcolate le ore disponibili e l&#39;FTE disponibile per l&#39;utente nella Programmazione risorse, a seconda del metodo utilizzato dall&#39;amministratore di sistema per il calcolo dell&#39;FTE nelle Preferenze di gestione risorse.

Per questo esempio, usiamo i seguenti numeri:

* Una pianificazione predefinita di sistema di 40 ore
* Una pianificazione utente di 20 ore
* Un FTE utente di 0,8

| Metodo di calcolo FTE (impostazione di sistema) | **Ore dalla pianificazione utente** | **Ore dalla pianificazione predefinita** | **Campo FTE utente** | **Ore disponibili nella Programmazione delle risorse** | **FTE disponibile nella pianificazione risorse** |
|---|---|---|---|---|---|
| **Pianificazione predefinita** | Ignorato | 40 | 0,8 | **32** (calcolato) | **0,8** |
| **La pianificazione dell&#39;utente** | 20 | 40 | Ignorato | **20** | **0.5** (calcolato) |

Eccezioni alla pianificazione e indisponibilità potrebbero influire sulla quantità di ore pianificate o FTE. Per ulteriori informazioni, vedere [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Esempio di visualizzazione di Programmazione delle risorse per utente e ore:

![Visualizzazione Pianificazione risorse per utente e ore](assets/resource-planner-by-user-by-hours.png)

Esempio di visualizzazione di Programmazione delle risorse per utente e FTE:

![Visualizzazione Pianificazione risorse per utente e FTE](assets/resource-planner-by-user-by-fte.png)

## Calcola tutti gli altri valori di ore e FTE per gli utenti e le mansioni in Pianificazione risorse {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

Oltre alle ore o all&#39;FTE disponibili, nella Programmazione delle risorse vengono visualizzate anche le seguenti informazioni sull&#39;ora:

* Lavoro Necessario
* Ore preventivate
* Variazione ore
* Ore nette\
  Per ulteriori informazioni su questi valori, vedere [Panoramica su ore, FTE e informazioni sui costi nelle visualizzazioni Progetto e Ruolo della Programmazione delle risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* Differenza di Ore\
  Per ulteriori informazioni su questo valore, vedere [Panoramica su ore, FTE e informazioni sui costi nelle visualizzazioni Progetto e Ruolo della Programmazione delle risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

In Pianificazione risorse è possibile visualizzare le stesse informazioni come FTE o come ore.

Workfront utilizza la formula seguente per visualizzare tutti gli altri valori come FTE nella Programmazione delle risorse:

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>La pianificazione dell&#39;utente viene ignorata durante il calcolo dell&#39;FTE per tutti i valori eccetto i valori FTE disponibili (AVL) nella pianificazione delle risorse. Per il calcolo viene preso in considerazione solo lo Schedule predefinito.

Questo calcolo si applica ai seguenti valori:

* FTE pianificato (PLN)
* FTE preventivato (BDG)
* Varianza FTE (VAR)
* FTE NETTO
* Differenza FTE (DIF)
