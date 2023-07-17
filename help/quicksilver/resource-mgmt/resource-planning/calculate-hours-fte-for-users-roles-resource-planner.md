---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Panoramica del calcolo delle ore e dell'FTE per utenti e ruoli nella pianificazione risorse
description: Panoramica del calcolo delle ore e dell'FTE per utenti e ruoli nella pianificazione risorse
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 4331917d133c52cf727f148b75a213853c1e5679
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# Panoramica del calcolo delle ore e dell&#39;FTE per utenti e ruoli nella pianificazione risorse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

È possibile visualizzare l&#39;allocazione e la disponibilità delle risorse nella Pianificazione risorse in base alle ore, FTE o Costo.\
Per ulteriori informazioni sul calcolo dei costi nella Programmazione delle risorse, vedere [Calcola i costi nella Programmazione delle risorse](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

&quot;FTE&quot; sta per Equivalente tempo pieno. Si tratta di una misura del tempo che rappresenta la quantità di ore dedicate al lavoro reale durante un giorno o una settimana per un utente o una mansione.

Le seguenti serie di informazioni sulle risorse vengono calcolate in modo diverso in Pianificazione risorse:

* I valori di Ore o FTE disponibili vengono calcolati in base al modo in cui l&#39;amministratore di sistema configura le preferenze di Gestione risorse nel sistema.\
  Per ulteriori informazioni sul calcolo dei valori delle ore e dell&#39;FTE disponibili, vedere [Calcola le ore o l&#39;FTE disponibili per gli utenti e le mansioni in Pianificazione risorse](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
  Per ulteriori informazioni sulla definizione delle preferenze di Gestione risorse per il sistema Adobe Workfront, vedere [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* Tutti gli altri valori FTE vengono calcolati in base alla pianificazione predefinita del sistema.\
  Per ulteriori informazioni sulla visualizzazione di tutti gli altri valori nella pianificazione delle risorse quando si utilizza FTE, vedere la sezione [Calcola tutti gli altri valori di ore e FTE per gli utenti e le mansioni in Pianificazione risorse](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) in questo articolo.

È importante comprendere cos’è l’FTE per ciascuno degli utenti e i relativi ruoli per gestire in modo accurato le risorse mentre vengono assegnate al lavoro.

## Calcola le ore o l&#39;FTE disponibili per gli utenti e le mansioni in Pianificazione risorse {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [Calcolare le ore e l&#39;FTE disponibili per un utente nella Programmazione delle risorse](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [Calcolare le ore e l&#39;FTE disponibili per una mansione nella Programmazione delle risorse](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [Calcola le ore e l&#39;FTE disponibili per un utente nella Programmazione delle risorse (esempio)](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### Calcolare le ore e l&#39;FTE disponibili per un utente nella Programmazione delle risorse {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

L’amministratore di Workfront determina il modo in cui viene calcolato il tempo disponibile per un utente selezionando l’opzione per utilizzare una delle seguenti opzioni nell’area Gestione risorse di Configurazione:

* La pianificazione predefinita del sistema e l&#39;FTE dell&#39;utente.
* La pianificazione dell’utente.

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

### Calcolare le ore e l&#39;FTE disponibili per una mansione nella Programmazione delle risorse {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

Prima di tutto è necessario calcolare la disponibilità dell&#39;utente, quindi è possibile calcolare la disponibilità di ciascuna mansione.

La disponibilità delle mansioni nella Programmazione delle risorse tiene conto della disponibilità totale dell&#39;utente e della **Percentuale di disponibilità FTE** associato a ciascun ruolo dell’utente.\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

Per ulteriori informazioni sull&#39;associazione di un **Percentuale di disponibilità FTE** con una mansione per un utente, vedi [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Ad esempio, se il valore di Ore disponibili per un utente è 40 e l&#39;utente può ricoprire un Ruolo principale per il 75% del tempo, e un Altro Ruolo per il 25% del tempo, la Programmazione delle risorse mostra che il **Ore disponibili** per il Ruolo principale per una settimana è di 30 ore e che il **Ore disponibili** Il valore per l’Altro Ruolo è 10 ore. In questo caso, l’FTE per il ruolo principale è 0,75 e l’FTE per l’altro ruolo è 0,25.

>[!NOTE]
>
>Il tempo totale disponibile per l&#39;utente viene calcolato in base a uno dei due metodi descritti nel [Calcolare le ore e l&#39;FTE disponibili per un utente nella Programmazione delle risorse](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) in questo articolo.

Quando si visualizza la Programmazione delle risorse nella Vista ruolo, la disponibilità di una mansione corrisponde al totale della disponibilità di tutti gli utenti che possono svolgere quella mansione.\
Per ulteriori informazioni sulla disponibilità delle risorse nella Programmazione delle risorse, vedi [Panoramica di Programmazione delle risorse](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Calcola le ore e l&#39;FTE disponibili per un utente nella Programmazione delle risorse (esempio) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

Nella tabella seguente viene illustrato come vengono calcolate le ore disponibili e l&#39;FTE disponibile per l&#39;utente nella Programmazione risorse, a seconda del metodo utilizzato dall&#39;amministratore di sistema per il calcolo dell&#39;FTE nelle Preferenze di gestione risorse.

Per questo esempio, usiamo i seguenti numeri:

* Una pianificazione predefinita di sistema di 40 ore
* Una pianificazione utente di 20 ore
* Un FTE utente di 0,75

| Metodo di calcolo FTE (impostazione di sistema) | **Ore dalla pianificazione dell&#39;utente** | **Ore dalla pianificazione predefinita** | **Campo FTE utente** | **Ore disponibili nella pianificazione risorse** | **FTE disponibile nella pianificazione risorse** |
|---|---|---|---|---|---|
| **La pianificazione predefinita** | Ignorato | 40 | 0.75 | **30** (calcolato) | **0.75** |
| **La pianificazione dell&#39;utente** | 20 | 40 | Ignorato | **20** | **0,5** (calcolato) |

Eccezioni alla pianificazione e indisponibilità potrebbero influire sulla quantità di ore pianificate o FTE. Per ulteriori informazioni, consulta [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Calcola tutti gli altri valori di ore e FTE per gli utenti e le mansioni in Pianificazione risorse {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

Oltre alle ore o all&#39;FTE disponibili, nella Programmazione delle risorse vengono visualizzate anche le seguenti informazioni sull&#39;ora:

* Lavoro Necessario
* Ore preventivate
* Variazione ore
* Ore nette\
  Per ulteriori informazioni su questi valori, consulta [Panoramica di ore, FTE e informazioni sui costi nelle visualizzazioni Progetto e Ruolo della Programmazione delle risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* Differenza di Ore\
  Per ulteriori informazioni su cosa rappresenta questo valore, consulta [Panoramica di ore, FTE e informazioni sui costi nelle visualizzazioni Progetto e Ruolo della Programmazione delle risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

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
