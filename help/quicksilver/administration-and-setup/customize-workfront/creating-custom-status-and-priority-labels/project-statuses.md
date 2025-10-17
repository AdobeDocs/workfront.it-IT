---
title: Accedere all'elenco degli stati dei progetti di sistema
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Gli utenti possono specificare lo stato di un progetto in modo che gli altri utenti possano visualizzare l’attuale fase di sviluppo del progetto in un determinato momento.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# Accedere all’elenco degli stati del progetto di sistema

Gli utenti possono specificare lo stato di un progetto in modo che gli altri utenti possano visualizzare l’attuale fase di sviluppo del progetto in un determinato momento.

Workfront viene fornito con 9 stati di progetto di sistema. È possibile modificare il nome di questi stati, ma non eliminarli.

Puoi anche aggiungere stati di progetto personalizzati in base alle esigenze della tua organizzazione.

In qualità di amministratore di Workfront, puoi configurare lo stato predefinito per tutti i nuovi progetti nel sistema. Per istruzioni, consulta [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Amministratore di Sistema</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Accedere agli stati del progetto

In qualità di amministratore di Workfront, puoi accedere all’elenco degli stati dei progetti a livello di sistema.

Per informazioni sulla modifica dello stato di un sistema e sulla creazione di stati personalizzati, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

{{step-1-to-setup}}

1. Fai clic su **Preferenze progetto** > **Stati**.

1. Fare clic sulla scheda **Progetto**.

   Gli stati del progetto disponibili in Workfront sono elencati in questa scheda.

   ![Stato progetto](assets/project-status.png)

   Per informazioni dettagliate su ciascuno degli stati predefiniti del progetto di sistema, vedere [Panoramica degli stati del progetto di sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## Creazione di stati di progetto personalizzati e personalizzazione degli stati di sistema

In qualità di amministratore di Workfront, puoi aggiungere gli stati del progetto di sistema a Workfront. In qualità di proprietario del gruppo, puoi aggiungere uno stato personalizzato specifico per un gruppo. Per ulteriori informazioni sulla creazione di stati personalizzati o sulla modifica di quelli di sistema, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Quando crei uno stato di progetto personalizzato, devi sempre equiparare il nuovo stato a uno stato di sistema esistente. È necessario comprendere il comportamento degli stati del sistema per sapere con quale stato è appropriato equiparare lo stato personalizzato. Dopo aver selezionato lo stato uguale, questa selezione non può essere modificata. Per ulteriori informazioni sugli stati del progetto di sistema, vedere [Panoramica degli stati del progetto di sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).
