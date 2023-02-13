---
title: Panoramica dei gruppi principali
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Un gruppo Home viene assegnato nel profilo dell’utente. Tutti gli utenti devono disporre di un gruppo Home. Un utente può appartenere a più di un gruppo, ma può avere un solo gruppo principale. Anche se qualsiasi gruppo esistente nel sistema può essere assegnato come gruppo principale dell’utente, si consiglia di creare e assegnare nuovi gruppi che rappresentano unità organizzative più grandi. Quando stabilisci i gruppi principali, considera come l’organizzazione divide gli utenti Adobe Workfront.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Panoramica dei gruppi principali

Un gruppo Home viene assegnato nel profilo dell’utente. Tutti gli utenti devono disporre di un gruppo Home. Un utente può appartenere a più di un gruppo, ma può avere un solo gruppo principale. Per ulteriori informazioni sui gruppi, consulta [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Anche se qualsiasi gruppo esistente nel sistema può essere assegnato come gruppo principale dell’utente, si consiglia di creare e assegnare nuovi gruppi che rappresentano unità organizzative più grandi.

Quando stabilisci i gruppi principali, considera come l’organizzazione divide gli utenti Adobe Workfront. Di seguito sono riportati alcuni suggerimenti per determinare quale tipo di gruppi deve essere utilizzato come gruppo principale:

* Gruppi che rappresentano dipartimenti, come IT o Marketing
* Gruppi governati da bilanci diversi
* Gruppi situati in aree o regioni diverse
* Gruppi composti da più team che appartengono allo stesso centro di costo

>[!NOTE]
>
>Se devi riorganizzare i gruppi principali in unità organizzative, devi>
>1. Crea il nuovo gruppo, come spiegato in [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).
>1. Riassegna il nuovo gruppo come gruppo principale dell’utente, come spiegato in [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>


## Gestione dei modelli di layout

Quando si assegna un modello di layout a un gruppo, tutti gli utenti a cui è assegnato il gruppo come gruppo principale possono visualizzare le impostazioni specificate nel modello di layout.

Se un modello di layout viene assegnato a un gruppo home, è visibile solo agli utenti assegnati a tale gruppo home.

Per ulteriori informazioni, consulta [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Gestione delle licenze

Ogni utente può essere assegnato a un solo gruppo principale, facilitando così la gestione dei conteggi delle licenze.

Gli amministratori di Workfront possono impostare il numero massimo di licenze per i gruppi principali.

L&#39;impostazione di un numero massimo di licenze consente agli amministratori di Workfront di impedire ad un&#39;unità aziendale di utilizzare le licenze Workfront acquistate per altre unità aziendali.

Per ulteriori informazioni, consulta [Gestione delle licenze disponibili nel sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
