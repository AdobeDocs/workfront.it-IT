---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filtro: visualizzare le attività principali'
description: Per visualizzare le attività di lavoro, è possibile applicare i filtri attività riportati di seguito. Le attività di lavoro sono attività che possono essere lavorate in modo indipendente e non sono attività principali di altre attività. In un esempio, un filtro identifica le attività figlio che potrebbero essere gli stessi genitori. In questo caso, non sono attività di lavoro.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# Filtro: visualizzare le attività principali

Per visualizzare le attività di lavoro, è possibile applicare i filtri attività riportati di seguito. Le attività di lavoro sono attività che possono essere lavorate in modo indipendente e non sono attività principali di altre attività. In un esempio, un filtro identifica le attività figlio che potrebbero essere gli stessi genitori. In questo caso, non sono attività di lavoro.

>[!TIP]
>
>* Se desideri aggiungere più filtri a un rapporto, ti consigliamo di aggiungere tutti i filtri utilizzando l’interfaccia di Report Builder e di fare clic su Passa alla modalità testo dopo aver aggiunto tutte le altre regole di filtro. Quindi, puoi aggiungere il codice per il filtro attività principale come indicato sopra. 
* È inoltre consigliabile aggiungere un raggruppamento per Nome progetto per facilitare la lettura del rapporto. Per ulteriori informazioni sull’aggiunta di raggruppamenti ai rapporti, consulta l’articolo [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>


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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizza le attività senza elementi figlio (potrebbero avere un elemento padre)

È possibile applicare il filtro seguente a un report attività per visualizzare le attività senza elementi figlio. Potrebbero avere genitori propri e essere figli di altri compiti.

1. Da **Menu principale** ![](assets/main-menu-icon.png), fai clic su **Rapporti.**

1. Fai clic su **Nuovo rapporto**.
1. Seleziona una **Report attività**.
1. Fai clic su **Filtri**.
1. Fai clic su **Aggiungere una regola filtro**.
1. In **Inizia a digitare il nome del campo ...** riga, inizia a digitare **Numero di figli**.

1. Seleziona **Uguale (distinzione maiuscole/minuscole)** per il modificatore, immettere **0** per il numero di figli.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   Oppure

   Fai clic su **Passa alla modalità testo** e nella finestra di modifica del testo, copia e incolla il seguente testo: 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Fai clic su **Salva e chiudi**.

   Consente di richiamare un report per tutte le attività che funzionano nel sistema. Alcune di queste attività potrebbero avere un elemento padre, ma non sono attività principali.

## Visualizza le attività con i genitori (potrebbero avere figli)

È possibile applicare il filtro seguente a un rapporto di attività per visualizzare le attività con elementi principali, ovvero le attività secondarie. Tuttavia, queste attività potrebbero anche avere figli propri perché il filtro non esclude i loro figli. I compiti figlio che sono anche genitori per altri compiti non sono considerati compiti di lavoro.

1. Da **Menu principale** ![](assets/main-menu-icon.png), fai clic su **Rapporti.
1. Fai clic su **Nuovo rapporto**.
1. Seleziona una **Report attività**.
1. Fai clic su **Filtri**.
1. Fai clic su **Aggiungere una regola filtro**.
1. In **Inizia a digitare il nome del campo ...** riga, inizia a digitare **ID padre**.
1. Seleziona **Non vuoto** per il modificatore.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   Oppure

   Fai clic su **Passa alla modalità testo** e nella finestra di modifica del testo, copia e incolla il seguente testo: 

   `parentID_Mod=notblank`

1. Fai clic su **Salva e chiudi**.

   Questo richiama un report per tutte le attività del sistema che hanno genitori e sono compiti figli di tali genitori. Alcune di queste attività potrebbero essere un genitore stesso.

## Visualizza le attività senza figli e senza genitori (attività autonoma)

È possibile applicare il filtro seguente a un report attività per visualizzare le attività di lavoro autonome. Questi compiti non hanno un genitore e non hanno figli propri.

1. Da **Menu principale** ![](assets/main-menu-icon.png), fai clic su **Rapporti.**
1. Fai clic su **Nuovo rapporto**.
1. Seleziona una **Report attività**.
1. Fai clic su **Filtri**.
1. Fai clic su **Aggiungere una regola filtro** e **Inizia a digitare il nome del campo ...** battitura di inizio riga **Numero di figli** select **Uguale (distinzione maiuscole/minuscole)** per il modificatore, immettere **0** per il numero di figli.
1. Fai clic su **Aggiungi un’altra regola filtro** e **Inizia a digitare il nome del campo ...** battitura di inizio riga **ID padre**, quindi seleziona **È vuoto**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Oppure

   Invece dei passaggi 6-7, fai clic su **Passa alla modalità testo** e nella finestra di modifica del testo, copia e incolla il seguente testo: 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Fai clic su **Salva e chiudi**.

   Questo richiama un report per tutte le attività del sistema che non hanno genitori o figli. Si tratta di compiti di lavoro autonomi.
