---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Fornire l'accesso alle code di richiesta
description: Quando si fornisce l’accesso a una coda di richiesta, si determina chi nell’organizzazione può visualizzare la coda di richiesta nell’area Richieste di Adobe Workfront.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Fornire l&#39;accesso alle code di richiesta

Quando si fornisce l’accesso a una coda di richiesta, si determina chi nell’organizzazione può visualizzare la coda di richiesta nell’area Richieste di Adobe Workfront.

È possibile fornire a utenti diversi l&#39;accesso a una coda di richiesta, a seconda che facciano parte del team di progetto, del gruppo di progetto o della società di progetto. Puoi anche fornire l’accesso a tutti gli utenti del sistema a una coda di richiesta. 

Questo è utile nelle organizzazioni che invitano soggetti interessati esterni in Workfront e desiderano limitare l’accesso degli utenti a aree specifiche. In questo caso, una coda di richiesta aperta solo agli utenti associati all’azienda o al gruppo del progetto limita la visibilità alle parti interessate esterne. L’accesso a chiunque rende la richiesta visibile sia alle parti interessate interne che a quelle esterne.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p> Gestisci le autorizzazioni per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere il piano, il tipo di licenza o l&#39;accesso a cui hai accesso, contatta il tuo amministratore Workfront

## Prerequisiti

Prima che la coda di richiesta sia disponibile per gli utenti nell’area Richieste , devi creare un progetto con le seguenti impostazioni:

* Designalo come coda di richiesta. Per ulteriori informazioni sulla creazione di una coda di richiesta, vedi [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Aggiorna lo stato del progetto a Corrente.

## Fornire l&#39;accesso a una coda di richiesta

1. Vai al progetto in cui desideri fornire l’accesso alle code di richiesta.

   >[!NOTE]
   >
   >Nell’area Richieste sono visibili solo i progetti con stato Corrente.

1. Fai clic su **Dettagli coda** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**, quindi **Dettagli coda**.
1. Seleziona **Pubblica come coda delle richieste di aiuto** per designare il progetto come coda richieste.
1. Seleziona tra le seguenti opzioni:

   * **Chiunque**: Qualsiasi utente può visualizzare e aggiungere richieste alla coda delle richieste.
   * **Utenti con accesso al progetto**: gli utenti che dispongono delle autorizzazioni di visualizzazione per il progetto possono visualizzare e aggiungere richieste alla coda delle richieste. 
   * **Persone nell&#39;azienda di questo progetto**: gli utenti associati all’azienda del progetto possono visualizzare e aggiungere richieste. L’azienda associata al progetto è elencata tra parentesi accanto a questa opzione. 
   * **Persone nel gruppo di questo progetto**: gli utenti associati al gruppo del progetto possono visualizzare e aggiungere richieste. Il gruppo associato al progetto è elencato tra parentesi accanto a questa opzione.

      Le code di gruppo sono utili quando diversi dipartimenti condividono un account Workfront per raggiungere obiettivi organizzativi unici. Ogni dipartimento può avere le proprie code che i membri di altri gruppi non dovrebbero essere in grado di vedere.

      Per informazioni su chi dispone delle autorizzazioni per un progetto, consulta [Condivisione di un progetto in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
      È possibile associare gruppi e aziende al progetto durante la modifica del progetto. Per ulteriori informazioni sulla modifica dei progetti, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Fai clic su **Salva**.
