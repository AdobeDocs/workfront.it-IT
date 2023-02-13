---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica della data di inizio effettiva del progetto
description: I progetti, le attività e i problemi hanno una data di inizio effettiva in Adobe Workfront. Per le attività e i problemi, si tratta della data in cui sono stati contrassegnati come in corso. Per i progetti, si tratta della data in cui la prima attività del progetto viene contrassegnata come In corso o è stata completata.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Panoramica della data di inizio effettiva del progetto

I progetti, le attività e i problemi hanno una data di inizio effettiva in Adobe Workfront. Per le attività e i problemi, si tratta della data in cui sono stati contrassegnati come in corso. Per i progetti, si tratta della data in cui la prima attività del progetto viene contrassegnata come In corso o è stata completata.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizzare o accedere in modo più rapido ai progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare o concedere autorizzazioni superiori a un progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sulle date di inizio effettive in Workfront

* La data di inizio effettiva si trova nella sezione Dettagli di progetti, attività e problemi. 
* La data di inizio effettivo di un progetto, di un&#39;attività o di un problema non viene compilata quando questi elementi vengono creati.
* La data di inizio effettiva viene compilata quando il lavoro inizia effettivamente sul progetto, sull&#39;attività o sul problema.
* La data di inizio effettivo non viene visualizzata nella scheda Dettagli progetto se il lavoro sul progetto non è ancora iniziato.

   Se il lavoro non è ancora iniziato, nelle schede Attività e Dettagli problema viene visualizzato vuoto.

* È possibile modificare manualmente la data di inizio effettivo di un&#39;attività o di un problema, ma non è possibile modificare la data di inizio effettivo di un progetto.

## Considerazioni sulle date di inizio effettive per i progetti

* Workfront imposta automaticamente la data effettiva di un progetto quando si verifica una delle situazioni seguenti:

   * Lo stato di un&#39;attività viene modificato da un assegnatario *Nuovo* a qualsiasi altro stato che non sia uguale a *Nuovo*.

   * L&#39;assegnatario di un&#39;attività modifica la percentuale di completamento di un&#39;attività.

      >[!IMPORTANT]
      >
      >La data di inizio effettivo del progetto non viene compilata se il progetto è contrassegnato come Corrente. Il lavoro effettivo deve iniziare sui task del progetto prima che la data di inizio effettivo del progetto venga compilata.

      In questi casi, la data di inizio effettivo del progetto viene impostata sulla data e l&#39;ora in cui si sono verificate queste azioni per il primo task del progetto. Ciò indica che il progetto è effettivamente iniziato in questa data e ora.

## Individuare la data di inizio effettivo di un progetto

È possibile individuare la data di inizio effettivo di un progetto nelle aree seguenti:

* Nella sezione Dettagli di un progetto.
* In un rapporto o in una visualizzazione del progetto, quando si aggiunge la data di inizio effettiva per l&#39;oggetto Progetto nel rapporto.

   Per informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Per individuare la data di inizio effettiva nella sezione Dettagli del progetto:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Progetti**.
1. Fare clic sul progetto per il quale si desidera visualizzare la data di inizio effettiva.
1. Fai clic su **Dettagli progetto** nel pannello a sinistra, quindi vai alla **Panoramica** sezione .

   La data di inizio effettivo viene visualizzata insieme alle altre date del progetto .

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
