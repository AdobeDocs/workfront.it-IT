---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: visualizzare le attività principali"
description: È possibile applicare i filtri delle attività riportati di seguito per visualizzare le attività di lavoro. Le attività di lavoro sono attività che possono essere elaborate in modo indipendente e non sono attività padre di altre attività. In un esempio, un filtro identifica le attività secondarie che potrebbero essere padri stessi. In questo caso, non sono attività operative.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# Filtro: visualizza le attività padre

<!--Audited: 10/2024-->

È possibile applicare i filtri delle attività riportati di seguito per visualizzare le attività di lavoro. Le attività di lavoro sono attività che possono essere elaborate in modo indipendente e non sono attività padre di altre attività. In un esempio, un filtro identifica le attività secondarie che potrebbero essere padri stessi. In questo caso, non sono attività operative.

>[!TIP]
>
>* Se consideri di aggiungere più filtri a un rapporto, ti consigliamo di aggiungere tutti i filtri utilizzando l’interfaccia di Report Builder e di fare clic su Passa a modalità testo dopo aver aggiunto tutte le altre regole di filtro. Quindi, puoi aggiungere il codice per il filtro dell’attività principale come indicato sopra. 
>* È inoltre consigliabile aggiungere un raggruppamento per Nome progetto per facilitare la lettura del rapporto. Per ulteriori informazioni sull&#39;aggiunta di raggruppamenti ai report, vedere l&#39;articolo [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td> 
    <p>Nuovo:</p>
   <ul><li><p>Collaboratore per modificare un filtro </p></li>
   <li><p>Standard per modificare un rapporto</p></li> </ul>

<p>Corrente:</p>
   <ul><li><p>Richiesta di modifica di un filtro </p></li>
   <li><p>Pianificare la modifica di un rapporto</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizza le attività senza elementi figlio (potrebbero avere un elemento padre)

Per visualizzare le attività senza elementi secondari, è possibile applicare il seguente filtro a un report di attività. Potrebbero avere genitori propri ed essere figli di altre mansioni.

1. Dal **menu principale** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro o dal **menu principale** ![](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibile, fare clic su **Report**.

1. Fare clic su **Nuovo report**.
1. Seleziona un **report attività**.
1. Fare clic su **Filtri**.
1. Fai clic su **Aggiungi una regola filtro**.
1. Nella riga **Inizia a digitare il nome del campo ...**, inizia a digitare **Number of Children**, quindi fai clic su **Task >> Number of Children** quando viene visualizzato nell&#39;elenco.

1. Seleziona **Uguale (distinzione maiuscole/minuscole)** per il modificatore, quindi immetti **0** per il numero di elementi figlio.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   Oppure

   Fare clic su **Passa alla modalità testo** e nella finestra di modifica del testo copiare e incollare il testo seguente

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Fai clic su **Salva e Chiudi**.

   In questo modo viene estratto un report per tutte le attività in esecuzione nel sistema. Alcune di queste attività possono avere un elemento padre, ma non sono attività padre.

## Visualizza le attività con i genitori (potrebbero avere figli)

È possibile applicare il filtro seguente a un report di attività per visualizzare le attività con padre, ovvero le attività figlio. Tuttavia, queste attività possono anche avere figli propri, perché il filtro non esclude i loro figli. Le attività figlio che sono anche padri per altre attività non sono considerate attività di lavoro.

1. Dal **menu principale** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro o dal **menu principale** ![](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibile, fare clic su **Report**.

1. Fare clic su **Nuovo report**.
1. Seleziona un **report attività**.
1. Fare clic su **Filtri**.
1. Fai clic su **Aggiungi una regola filtro**.
1. Nella riga **Inizia a digitare il nome del campo ...**, inizia a digitare **ID padre**, quindi seleziona **Attività >> ID padre** quando viene visualizzato nell&#39;elenco.
1. Seleziona **Non è vuoto** per il modificatore.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   Oppure

   Fare clic su **Passa alla modalità testo** e nella finestra di modifica del testo copiare e incollare il testo seguente: 

   `parentID_Mod=notblank`

1. Fai clic su **Salva e Chiudi**.

   In questo modo viene generato un report per tutte le attività del sistema che hanno i genitori e sono attività figlio di tali genitori. Alcune di queste attività potrebbero essere un genitore.

## Visualizza le attività senza elementi figlio e senza elementi padre (attività autonome)

È possibile applicare il filtro seguente a un report di attività per visualizzare le attività di lavoro autonome. Queste attività non hanno un genitore e non hanno figli propri.

1. Dal **menu principale** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro o dal **menu principale** ![](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibile, fare clic su **Report**.

1. Fare clic su **Nuovo report**.
1. Seleziona un **report attività**.
1. Fare clic su **Filtri**.
1. Fai clic su **Aggiungi una regola filtro**.
1. In **Inizia a digitare il nome del campo ...** la riga inizia a digitare **Numero di elementi figlio**, quindi seleziona **Attività >> Numero di elementi figlio** dall&#39;elenco.
1. Seleziona **Uguale (distinzione maiuscole/minuscole)** per il modificatore, quindi immetti **0** per il numero di elementi figlio.
1. Fai clic su **Aggiungi un&#39;altra regola filtro**.
1. In **Inizia a digitare il nome del campo ...** la riga inizia a digitare **ID padre**, quindi seleziona **Attività >> ID padre** dall&#39;elenco.
1. Selezionare **È vuoto** per il modificatore.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Oppure

   Invece dei passaggi 6-10 <!--ensure steps above stay accurate-->, fai clic su **Passa alla modalità testo** e nella finestra di modifica del testo copia e incolla il testo seguente:

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Fai clic su **Salva e Chiudi**.

   Questo consente di recuperare un report per tutte le attività del sistema che non hanno genitori né figli. Si tratta di attività di lavoro autonome.
