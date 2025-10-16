---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Fornire l’accesso alle code di richieste
description: Quando fornisci l’accesso a una coda di richieste, puoi determinare chi, nella tua organizzazione, può visualizzare la coda di richieste nell’area Richieste di Adobe Workfront.
author: Becky
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: 9cdf3d78e1d19f3d581f8d527919a608c5cc0ddc
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 1%

---

# Fornire l’accesso alle code di richieste

<!-- Audited: 6/2025 -->

Quando fornisci l’accesso a una coda di richieste, puoi determinare chi, nella tua organizzazione, può visualizzare la coda di richieste nell’area Richieste di Adobe Workfront.

Puoi fornire a utenti diversi l’accesso a una coda di richieste, a seconda che facciano parte del team di progetto, del gruppo di progetto o della società di progetto. Puoi anche fornire l’accesso alla coda di richieste a tutti gli utenti del sistema.

Ciò è utile nelle organizzazioni che invitano parti interessate esterne in Workfront e desiderano limitare l’accesso degli utenti ad aree specifiche. In questo caso, una coda di richieste aperta solo agli utenti associati all’azienda o al gruppo del progetto limita la visibilità alle parti interessate esterne. Dare accesso a chiunque rende la richiesta visibile alle parti interessate interne ed esterne.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Standard </p>
   <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p> Gestire le autorizzazioni per il progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima che la coda di richieste sia disponibile per gli utenti nell’area Richieste, è necessario creare un progetto con le seguenti impostazioni:

* Designalo come coda di richieste. Per ulteriori informazioni, vedere [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Aggiorna lo stato del progetto su Corrente.

## Fornire accesso a una coda di richieste

1. Vai al progetto in cui desideri fornire l’accesso alle code di richieste.

   >[!NOTE]
   >
   >Nell’area Richieste sono visibili solo i progetti con lo stato Attuale.

1. Fai clic su **Dettagli coda** nel pannello a sinistra.
1. Selezionare **Pubblica come coda di richieste della Guida** per designare il progetto come coda di richieste.
1. Seleziona tra le seguenti opzioni visualizzate:

   * **Chiunque**: qualsiasi utente può visualizzare e aggiungere richieste alla coda richieste.
   * **Persone con accesso di visualizzazione a questo progetto**: gli utenti con autorizzazioni di visualizzazione al progetto possono visualizzare e aggiungere richieste alla coda richieste.
   * **Persone nella società di questo progetto**: gli utenti associati alla società del progetto possono visualizzare e aggiungere richieste. La società associata al progetto è elencata tra parentesi accanto a questa opzione.
   * **Persone nel gruppo di questo progetto**: gli utenti associati al gruppo del progetto possono visualizzare e aggiungere richieste. Il Gruppo associato al progetto è elencato tra parentesi accanto a questa opzione.

     Le code di gruppo sono utili quando diversi reparti condividono un account Workfront per raggiungere obiettivi organizzativi univoci. Ogni reparto può disporre di code proprie che i membri di altri gruppi non dovrebbero essere in grado di visualizzare.

     Per informazioni su chi dispone delle autorizzazioni per un progetto, vedere [Condividere un progetto in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

     I gruppi e le società possono essere associati al progetto durante la modifica dello stesso. Per ulteriori informazioni, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Fai clic su **Salva**.
