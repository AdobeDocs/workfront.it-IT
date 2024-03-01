---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Accesso a oggetti e aree tramite nuove licenze
description: La tabella seguente indica il livello massimo di accesso (Modifica o Visualizza) consentito da ciascuna licenza Adobe Workfront per gli oggetti e le aree in Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: 7a9232f59e4c6f2eac2995be7d7862295b6bab2c
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 18%

---

# Accesso a oggetti e aree tramite nuove licenze

<!-- Audited: 2/2024 -->

La tabella seguente indica il livello massimo di accesso (Modifica o Visualizza) consentito da ciascuna licenza Adobe Workfront per gli oggetti e le aree in Workfront.

* **Visualizza**: l’utente può rivedere e condividere gli elementi.
* **Modifica**: l’utente può creare, modificare, eliminare e condividere elementi.

  >[!NOTE]
  >
  >Quando un altro utente condivide un oggetto, può specificare le autorizzazioni che limitano la possibilità di modificarlo. Per ulteriori informazioni, consulta [Panoramica delle autorizzazioni di condivisione sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>Standard</td>
        <td>Light</td>
        <td>Collaboratore</td>
        <td>Esterno</td>
    </tr>
    <tr>
        <td>Progetti</td>
        <td>Modifica</td>
        <td>Visualizza</td>
        <td>Visualizza (solo la pagina Dettagli)</td>
        <td>Nessun accesso</td>
    </tr>
    <tr>
        <td>Attività</td>
        <td>Modifica</td>
        <td>Visualizza</td>
        <td>Visualizza</td>
        <td>Visualizza</td>
    </tr>
    <tr>
        <td>Problemi</td>
        <td>Modifica</td>
        <td>Modifica</td>
        <td>Modifica</td>
        <td>Nessun accesso</td>
    </tr>
    <tr>
        <td>Portfolio</td>
        <td>Modifica</td>
        <td>Visualizza</td>
        <td>Nessun accesso</td>
        <td>Nessun accesso</td>
    </tr>
    <tr>
        <td>Programmi</td>
        <td>Modifica</td>
        <td>Visualizza</td>
        <td>Nessun accesso</td>
        <td>Nessun accesso</td>
    </tr>
    <tr>
        <td>Report, dashboard e calendari</td>
        <td>Modifica</td>
        <td>Visualizza</td>
        <td>Visualizza*</td>
        <td>Visualizza (solo per i calendari, nessuna autorizzazione di condivisione)</td>
    </tr>
    <tr>
        <td>Filtri, viste e raggruppamenti</td>
        <td>Modifica</td>
        <td>Modifica</td>
        <td>Modifica</td>
        <td>Nessun accesso</td>
    </tr>
    <tr>
        <td>Documenti</td>
        <td>Modifica</td>
        <td>Modifica</td>
        <td>Modifica</td>
        <td>Visualizza (nessuna autorizzazione di condivisione)</td>
    </tr>
    <tr>
        <td>Utenti</td>
        <td>Modifica</td>
        <td>Visualizza</td>
        <td>Visualizza</td>
        <td>Visualizza</td>
    </tr>
    <tr>
        <td>Team</td>
        <td>Modifica</td>
        <td>Visualizza</td>
        <td>Visualizza</td>
        <td>Nessun accesso</td>
    </tr>
    <tr>
        <td>Modelli</td>
        <td>Modifica</td>
        <td>Nessun accesso</td>
        <td>Nessun accesso</td>
        <td>Nessun accesso</td>
    </tr>
    <tr>
        <td>Dati finanziari</td>
        <td>Modifica</td>
        <td>Nessun accesso</td>
        <td>Nessun accesso</td>
        <td>Nessun accesso</td>
    </tr>
    <tr>
        <td>Gestione risorse</td>
        <td>Modifica</td>
        <td>Visualizza</td>
        <td>Nessun accesso</td>
        <td>Nessun accesso</td>
    </tr>
    <tr>
        <td>Pianificazione scenario</td>
        <td>Modifica</td>
        <td>Visualizza</td>
        <td>Nessun accesso</td>
        <td>Nessun accesso</td>
    </tr>
    <tr>
        <td>Workfront Goals</td>
        <td>Modifica</td>
        <td>Modifica</td>
        <td>Modifica</td>
        <td>Nessun accesso</td>
    </tr>
</table>

&#42; Gli utenti con una licenza Collaboratore possono visualizzare solo report, dashboard e calendari condivisi con loro.

>[!NOTE]
>
>Gli utenti con una licenza Light o una licenza Contributor dispongono di funzionalità di condivisione limitate. Per ulteriori informazioni, consulta [Panoramica sulle licenze](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>Gli utenti esterni non possono cercare elementi in Workfront. Possono visualizzare documenti e calendari condivisi in modo specifico con loro. Possono inoltre visualizzare gli utenti che condividono gli elementi con loro.

Nei seguenti articoli sono disponibili informazioni dettagliate sui livelli di accesso consentiti per ciascun oggetto e area:

* [Concedere l’accesso ai progetti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Concedere l’accesso ai problemi](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Concedere l’accesso ai documenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Concedere l’accesso ai portfolio](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Concedere l’accesso ai programmi](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Concedere l’accesso a rapporti, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Concedere l’accesso a filtri, viste e raggruppamenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Concedere l’accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Concedere l’accesso ai team](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Concedere l’accesso ai modelli](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Concedere l’accesso alla gestione delle risorse](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Concedere l’accesso a Scenario Planner](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Concedere l’accesso agli obiettivi di Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
