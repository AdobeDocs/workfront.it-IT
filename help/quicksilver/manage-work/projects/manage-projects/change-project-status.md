---
product-area: projects
navigation-topic: manage-projects
title: Modificare lo stato di un progetto
description: Se necessario, puoi aggiornare manualmente lo stato di un progetto a qualsiasi altro stato. È possibile aggiornare manualmente lo stato di un progetto impostandolo su Completato solo quando la modalità di completamento del progetto è impostata su Manuale.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Modificare lo stato di un progetto

<!--Audited: 02/2024-->

Se necessario, puoi aggiornare manualmente lo stato di un progetto a qualsiasi altro stato.

È possibile aggiornare manualmente lo stato di un progetto impostandolo su Completato solo quando la modalità di completamento del progetto è impostata su Manuale.

In caso contrario, Adobe Workfront contrassegna automaticamente il progetto come Completato quando tutte le attività e i problemi del progetto sono completati e approvati.

Per ulteriori informazioni sulla modalità di completamento del progetto, vedere [Modifica progetti](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Standard </p> 
   Oppure
   <p>Corrente: Piano </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni sul progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront. Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considerazioni sull’aggiornamento a stati specifici

* **Quando si aggiorna un progetto a Completo:** Assicurarsi che tutte le attività e i problemi siano stati completati nel progetto. Non è possibile selezionare lo stato Completato per un progetto o qualsiasi altro stato che equivale a Completato quando sono presenti attività o problemi non completati nel progetto. Ciò include l&#39;approvazione di qualsiasi attività o problema con stato Completato-In attesa di approvazione.
* **Quando si aggiorna un progetto da Completo a Corrente:** Se tutte le attività e i problemi del progetto sono stati completati, assicurarsi che la Modalità di completamento del progetto sia impostata su Manuale. Se la Modalità di completamento del progetto è Automatica, lo stato del progetto rimane Completato.

## Modifica stato progetto

1. Vai al progetto di cui desideri aggiornare lo stato.
1. Nell&#39;intestazione del progetto, fai clic sul nome dello stato nel campo **Stato**, quindi seleziona un nuovo stato.

   ![Modifica stato progetto](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   Oppure

   Fai clic sul menu **Altro** ![Altro menu](assets/qs-more-menu.png) accanto al nome del progetto, quindi fai clic su **Modifica** e seleziona un nuovo stato nel campo **Stato**, quindi fai clic su **Salva**.

   Lo stato del progetto viene aggiornato in base allo stato selezionato.
