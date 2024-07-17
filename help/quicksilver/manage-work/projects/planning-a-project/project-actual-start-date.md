---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica della data di inizio effettiva del progetto
description: I progetti, le attività e i problemi hanno una data di inizio effettiva in Adobe Workfront. Per le attività e i problemi, si tratta della data in cui sono stati contrassegnati come In corso. Per i progetti, questa è la data in cui la prima attività del progetto è contrassegnata come In corso o è stata completata.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Panoramica della data di inizio effettiva del progetto

I progetti, le attività e i problemi hanno una data di inizio effettiva in Adobe Workfront. Per le attività e i problemi, si tratta della data in cui sono stati contrassegnati come In corso. Per i progetti, questa è la data in cui la prima attività del progetto è contrassegnata come In corso o è stata completata.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso ai progetti di visualizzazione o superiore</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare o accedere ad autorizzazioni superiori per un progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

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
     >La data di inizio effettiva del progetto non viene compilata quando il progetto è contrassegnato come Corrente. Il lavoro effettivo deve iniziare dalle attività del progetto prima che venga compilata la Data di inizio effettiva del progetto.

     In questi casi, la data di inizio effettiva del progetto viene impostata sulla data e sull&#39;ora in cui si sono verificate queste azioni per la prima attività del progetto. Indica che il progetto è effettivamente iniziato in questa data e ora.

## Individuare la data di inizio effettiva di un progetto

È possibile individuare la data di inizio effettiva di un progetto nelle seguenti aree:

* Nella sezione Dettagli di un progetto.
* In un report o in una visualizzazione di progetto, quando si aggiunge la Data di inizio effettiva per l&#39;oggetto Project nel report.

  Per informazioni sulla creazione di report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Per individuare la data di inizio effettiva nella sezione Dettagli del progetto:

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Workfront, quindi fai clic su **Progetti**.
1. Fare clic sul progetto per il quale si desidera visualizzare la data di inizio effettiva.
1. Fai clic su **Dettagli progetto** nel pannello a sinistra, quindi vai alla sezione **Panoramica**.

   La data di inizio effettiva viene visualizzata insieme alle altre date del progetto.

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
