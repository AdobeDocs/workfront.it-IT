---
title: Accedere all’elenco degli stati del progetto di sistema
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Gli utenti possono specificare lo stato di un progetto in modo che gli altri utenti possano vedere lo stato attuale di sviluppo del progetto in un dato momento.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Accedere all’elenco degli stati del progetto di sistema

Gli utenti possono specificare lo stato di un progetto in modo che gli altri utenti possano vedere lo stato attuale di sviluppo del progetto in un dato momento.

Workfront viene fornito con 9 stati del progetto di sistema. È possibile modificare il nome di questi stati, ma non è possibile eliminarli.

Puoi anche aggiungere stati di progetto personalizzati per soddisfare le esigenze della tua organizzazione.

In qualità di amministratore di Workfront, puoi configurare lo stato predefinito per tutti i nuovi progetti nel sistema. Per istruzioni, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Accedere agli stati del progetto

In qualità di amministratore di Workfront, puoi accedere all’elenco degli stati del progetto a livello di sistema.

Per informazioni sulla modifica dello stato di un sistema e sulla creazione di stati personalizzati, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Preferenze del progetto** > **Stati**.

1. Fai clic sul pulsante **Progetto** scheda .

   Gli stati del progetto disponibili in Workfront sono elencati in questa scheda.

   ![](assets/project-status.png)

   Per informazioni dettagliate su ciascuno stato del progetto di sistema integrato, consulta [Stato del progetto di sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## Creazione di stati di progetto personalizzati e personalizzazione degli stati del sistema

In qualità di amministratore di Workfront puoi aggiungere gli stati del progetto di sistema a Workfront. In qualità di proprietario del gruppo, puoi aggiungere uno stato personalizzato specifico per un gruppo. Per ulteriori informazioni sulla creazione di stati personalizzati o sulla modifica di quelli di sistema, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Quando crei uno stato di progetto personalizzato, devi sempre equiparare il nuovo stato a uno stato di sistema esistente. È necessario comprendere il comportamento degli stati del sistema per sapere con quale stato si desidera ottenere lo stato personalizzato. Dopo aver selezionato lo stato uguale, questa selezione non può essere modificata. Per ulteriori informazioni sugli stati del progetto di sistema, consulta [Stato del progetto di sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).
