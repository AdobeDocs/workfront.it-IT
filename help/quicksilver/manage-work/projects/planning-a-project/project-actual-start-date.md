---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica della data di inizio effettiva del progetto
description: I progetti, le attività e i problemi hanno una data di inizio effettiva in Adobe Workfront. Per le attività e i problemi, si tratta della data in cui sono stati contrassegnati come In corso. Per i progetti, questa è la data in cui la prima attività del progetto è contrassegnata come In corso o è stata completata.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 3%

---

# Panoramica della data di inizio effettiva del progetto

I progetti, le attività e i problemi hanno una data di inizio effettiva in Adobe Workfront. Per le attività e i problemi, si tratta della data in cui sono stati contrassegnati come In corso. Per i progetti, questa è la data in cui la prima attività del progetto è contrassegnata come In corso o è stata completata.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Chiaro o superiore</p> 
   <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso ai progetti di visualizzazione o superiore</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare o accedere ad autorizzazioni superiori per un progetto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Considerazioni sulle date di inizio effettive in Workfront

* La data di inizio effettiva si trova nella sezione Dettagli dei progetti, delle attività e dei problemi.
* La data di inizio effettiva di un progetto, attività o problema non viene compilata al momento della creazione di questi elementi.
* La data di inizio effettiva viene compilata quando il lavoro inizia effettivamente per il progetto, l&#39;attività o il problema.
* La data di inizio effettiva non viene visualizzata nella scheda Dettagli progetto se il lavoro sul progetto non è ancora iniziato.

  Se il lavoro non è ancora iniziato, nelle schede Dettagli attività e Dettagli problema viene visualizzato vuoto il campo Data di inizio effettiva.

* È possibile modificare manualmente la Data di inizio effettiva di un&#39;attività o di un problema, ma non la Data di inizio effettiva di un progetto.

## Considerazioni sulle date di inizio effettive per i progetti

* Workfront imposta automaticamente la data effettiva di un progetto quando si verifica una delle seguenti situazioni:

   * Un assegnatario dell&#39;attività cambia lo stato di un&#39;attività da *Nuovo* a qualsiasi altro stato che non corrisponda a *Nuovo*.

   * L&#39;assegnatario di un&#39;attività modifica la percentuale di completamento di un&#39;attività.

     >[!IMPORTANT]
     >
     >La data di inizio effettiva del progetto non viene compilata quando il progetto è contrassegnato come Corrente. Il lavoro effettivo deve iniziare dalle attività del progetto prima che venga compilata la Data di inizio effettiva del progetto.

     In questi casi, la data di inizio effettiva del progetto viene impostata sulla data e sull&#39;ora in cui si sono verificate queste azioni per la prima attività del progetto. Indica che il progetto è effettivamente iniziato in questa data e ora.

## Individuare la data di inizio effettiva di un progetto

È possibile individuare la data di inizio effettiva di un progetto nelle seguenti aree:

* Nella sezione Dettagli di un progetto.
* In un report o in una visualizzazione di progetto, quando si aggiunge la Data di inizio effettiva per l&#39;oggetto Project nel report.

  Per informazioni sulla creazione di report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Per individuare la data di inizio effettiva nella sezione Dettagli del progetto:

{{step1-to-projects}}

1. Fare clic sul progetto per il quale si desidera visualizzare la data di inizio effettiva.
1. Fai clic su **Dettagli progetto** nel pannello a sinistra, quindi vai alla sezione **Panoramica**.

   La data di inizio effettiva viene visualizzata insieme alle altre date del progetto.

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)


