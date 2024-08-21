---
title: Panoramica dei gruppi predefiniti
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Nel profilo dell’utente viene assegnato un Gruppo predefinito. Tutti gli utenti devono avere un Gruppo Predefinito.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Panoramica sui gruppi predefiniti

Nel profilo dell’utente viene assegnato un Gruppo predefinito. Tutti gli utenti devono avere un Gruppo Predefinito. Un utente può appartenere a più gruppi, ma può avere un solo gruppo predefinito. Per ulteriori informazioni sui gruppi, vedere [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Anche se qualsiasi gruppo esistente nel sistema può essere assegnato come Gruppo predefinito di un utente, si consiglia di creare e assegnare nuovi gruppi che rappresentino unità organizzative più grandi.

Quando stabilisci i gruppi predefiniti, considera in che modo l’organizzazione divide gli utenti Adobe Workfront. Di seguito sono riportati alcuni suggerimenti per determinare il tipo di gruppi da utilizzare come Gruppo predefinito:

* Gruppi che rappresentano reparti, ad esempio IT o Marketing
* Gruppi governati da budget diversi
* Gruppi situati in aree o regioni diverse
* Gruppi composti da più team che appartengono allo stesso centro di costo

>[!NOTE]
>
>Se devi riorganizzare i Gruppi predefiniti in unità organizzative, devi>
>1. Creare il nuovo gruppo, come descritto in [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).
>1. Riassegnare il nuovo gruppo come Gruppo predefinito dell&#39;utente, come spiegato in [Modifica il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>

## Gestione dei modelli di layout

Quando si assegna un modello di layout a un gruppo, tutti gli utenti a cui è assegnato il gruppo predefinito possono visualizzare le impostazioni specificate nel modello di layout.

Se un modello di layout è assegnato a un gruppo predefinito, è visibile solo agli utenti assegnati a tale gruppo.

Per ulteriori informazioni, vedere [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Gestione licenze

Ogni utente può essere assegnato a un solo Gruppo Predefinito, facilitando così la gestione del numero di licenze.

Gli amministratori di Workfront possono impostare il numero massimo di licenze per i gruppi predefiniti.

L&#39;impostazione di un numero massimo di licenze consente agli amministratori di Workfront di impedire a una business unit di utilizzare le licenze Workfront acquistate per altre business unit.

Per ulteriori informazioni, consulta [Gestire le licenze disponibili nel sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
