---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Panoramica del calcolo delle ore e degli FTE per utenti e ruoli nel Planner risorse
description: Panoramica del calcolo delle ore e degli FTE per utenti e ruoli nel Planner risorse
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# Panoramica del calcolo delle ore e degli FTE per utenti e ruoli nel Planner risorse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

È possibile visualizzare l&#39;allocazione e la disponibilità delle risorse nel Planner risorse per ore, FTE o Costo.\
Per ulteriori informazioni sul calcolo dei costi nel Planner risorse, vedere [Calcolare i costi nel planner risorse](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

&quot;FTE&quot; sta per Full Time Equivalent. Si tratta di una misura di tempo che rappresenta la quantità di ore dedicate al lavoro reale durante un giorno o una settimana per un utente o un ruolo di lavoro.

I seguenti set di informazioni sulle risorse vengono calcolati in modo diverso nel Planner risorse:

* I valori Orari disponibili o FTE vengono calcolati in base al modo in cui l’amministratore di sistema configura le preferenze di Gestione risorse nel sistema.\
   Per ulteriori informazioni sul calcolo dei valori Orari disponibili e FTE, consulta [Calcola le ore disponibili o FTE per gli utenti e i ruoli di lavoro nel planner risorse](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
   Per ulteriori informazioni sulla definizione delle preferenze di Gestione risorse per il sistema Adobe Workfront, consulta [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* Tutti gli altri valori FTE vengono calcolati in base alla pianificazione Predefinito di sistema.\
   Per ulteriori informazioni sulla visualizzazione di tutti gli altri valori nel planner risorse quando si utilizza l’ETP, consulta la sezione . [Calcolare tutti gli altri valori ora e FTE per gli utenti e i ruoli di lavoro nel Planner risorse](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) in questo articolo.

È importante comprendere cosa sia l’ETP per ciascuno dei tuoi utenti e i loro ruoli di lavoro per gestire con precisione le risorse mentre le stai assegnando al lavoro.

## Calcola le ore disponibili o FTE per gli utenti e i ruoli di lavoro nel planner risorse {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [Calcolare le ore disponibili e l’FTE per un utente nel planner risorse](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [Calcolare le ore disponibili e l&#39;FTE per un ruolo di lavoro nel planner risorse](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [Calcolare le ore disponibili e l’FTE per un utente nel Planner risorse (esempio)](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### Calcolare le ore disponibili e l’FTE per un utente nel planner risorse {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

L’amministratore di Workfront determina il modo in cui viene calcolato il tempo disponibile per un utente selezionando di utilizzare una delle opzioni seguenti nell’area Gestione risorse in Configurazione:

* La pianificazione predefinita del sistema e l’FTE dell’utente.
* La pianificazione dell&#39;utente.

Per ulteriori informazioni, consulta [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><br></p>
<p> <img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p>
<p>(NOTE: The determines how to calculate resource availability at the system level.For more information about defining the Resource Management preferences for the system, see Configure Resource Management preferences.)</p>
<p>Based on how this setting is configured, the availability of the users in the Resource Planner (hours as well as FTE availability) is calculated by using the following methods: </p>
<ul>
<li><strong>The Default Schedule</strong>: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user in the Resource Planner. The Schedule of the user is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE value</code> <span style="color: #dc143c;">( NOTE: this is the correct value. If this shows as a division in other articles, that is wrong. It's a multiplication between these 2 values).</span><br>For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Resource Planner.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a></li>
<li style="font-weight: normal;"> The <strong>Available FTE</strong> for the user in the<strong>Resource Planner</strong> is the same as the user FTE specified in the user settings. <br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner. For more information about the value of the user FTE as it displays in the user settings, see <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><strong>The User's Schedule</strong>: The Schedule of the user is used to determine the availability of the user in the Resource Planner. The value of the user FTE is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the Resource Planner. </li>
<li> The <strong>Available FTE</strong> in the<strong>Resource Planner</strong> is calculated by the following formula:<br><em><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in Workfront has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul></li>
</ul> <note type="note">
If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note>
</div>
-->

### Calcolare le ore disponibili e l&#39;FTE per un ruolo di lavoro nel planner risorse {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

È innanzitutto necessario calcolare la disponibilità dell’utente e quindi è possibile calcolare la disponibilità di ciascuno dei ruoli di lavoro.

La disponibilità dei ruoli di lavoro nel Planner risorse tiene conto della disponibilità totale dell&#39;utente e della **Percentuale di disponibilità FTE** associato a ogni ruolo dell&#39;utente.\
![percent_of_fte_available_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

Per ulteriori informazioni sull’associazione di un **Percentuale di disponibilità FTE** valore con un ruolo di lavoro per un utente, vedi [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Ad esempio, se il valore di Ore disponibili per un utente è 40 e può svolgere un ruolo primario per il 75% di tale tempo e un altro ruolo per il 25% di tale tempo, il planner risorse mostra che il **Ore disponibili** il valore per il ruolo principale per una settimana è di 30 ore e che il **Ore disponibili** Il valore per Altro ruolo è 10 ore. In questo caso, l’ETP per il ruolo principale è 0,75 e l’ETP per l’altro ruolo è 0,25.

>[!NOTE]
>
>Il tempo totale disponibile per l’utente viene calcolato in base a uno dei due metodi descritti nel [Calcolare le ore disponibili e l’FTE per un utente nel planner risorse](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) in questo articolo.

Quando si visualizza il planner risorse nella Vista ruolo, la disponibilità di un ruolo di lavoro è un totale della disponibilità di tutti gli utenti che possono svolgere quel ruolo di lavoro.\
Per ulteriori informazioni sulla disponibilità delle risorse nel Planner risorse, consulta la sezione [Panoramica di Resource Planner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Calcolare le ore disponibili e l’FTE per un utente nel Planner risorse (esempio) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

Nella tabella seguente viene illustrato come vengono calcolati gli orari disponibili e gli FTE disponibili per l&#39;utente nel Planner risorse, a seconda del metodo utilizzato dall&#39;amministratore di sistema per il calcolo FTE nelle Preferenze di Gestione risorse.

In questo esempio, utilizziamo i seguenti numeri:

* Un programma predefinito del sistema di 40 ore
* Un programma utente di 20 ore
* Un FTE utente di 0.75.

| Metodo per il calcolo FTE (impostazione del sistema) | **Ore dalla pianificazione dell’utente** | **Ore dalla pianificazione predefinita** | **Campo FTE utente** | **Ore disponibili nel planner risorse** | **FTE disponibile nel planner risorse** |
|---|---|---|---|---|---|
| **La pianificazione predefinita** | Ignorato | 40 | 0.75 | **30** (calcolato) | **0.75** |
| **La pianificazione dell&#39;utente** | 20 | 40 | Ignorato | **20** | **0,5** (calcolato) |

Le eccezioni di pianificazione e il tempo di inattività potrebbero influire sulla quantità di ore pianificate o FTE. Per ulteriori informazioni, consulta [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Calcolare tutti gli altri valori ora e FTE per gli utenti e i ruoli di lavoro nel Planner risorse {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

Oltre alle ore disponibili o all’FTE, nel Planner risorse vengono visualizzate anche le seguenti informazioni sull’ora:

* Lavoro Necessario
* Ore preventivate
* Varianza ore
* Ore nette\
   Per ulteriori informazioni su questi valori consulta [Panoramica delle informazioni su ore, FTE e costi nelle visualizzazioni Progetto e Ruolo del Planner risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* Differenza oraria\
   Per ulteriori informazioni su cosa rappresenta questo valore, consulta [Panoramica delle informazioni su ore, FTE e costi nelle visualizzazioni Progetto e Ruolo del Planner risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

È possibile visualizzare le stesse informazioni nel Planner risorse come FTE o come ore.

Workfront utilizza la seguente formula per visualizzare tutti gli altri valori come FTE nel planner risorse:

```
FTE = Resource Planner Hours/ Default Schedule Hours
```

>[!NOTE]
>
>La pianificazione dell’utente viene ignorata durante il calcolo dell’ETP per tutti i valori, ad eccezione dei valori FTE disponibili (AVL), nel Planner risorse. Per il calcolo viene preso in considerazione solo il programma predefinito.

Questo calcolo si applica ai seguenti valori:

* FTE pianificato (PLN)
* FTE a budget (BDG)
* Varianza FTE (VAR)
* FTE NETTE
* Differenza FTE (DIF)
