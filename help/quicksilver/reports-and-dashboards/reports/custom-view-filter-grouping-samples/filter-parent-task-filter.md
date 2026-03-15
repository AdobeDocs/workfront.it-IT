---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: visualizzare le attività principali'
description: È possibile applicare i filtri delle attività riportati di seguito per visualizzare le attività di lavoro. Le attività di lavoro sono attività che possono essere elaborate in modo indipendente e non sono attività padre di altre attività. In un esempio, un filtro identifica le attività secondarie che potrebbero essere padri. In questo caso, non sono attività operative.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 7%

---

# Filtro: visualizzare le attività principali

<!--Audited: 10/2024-->

È possibile applicare i filtri delle attività riportati di seguito per visualizzare le attività di lavoro. Le attività di lavoro sono attività che possono essere elaborate in modo indipendente e non sono attività padre di altre attività. In un esempio, un filtro identifica le attività secondarie che potrebbero essere padri stessi. In questo caso, non sono attività operative.

>[!TIP]
>
>* Se consideri di aggiungere più filtri a un rapporto, ti consigliamo di aggiungere tutti i filtri utilizzando l’interfaccia di Report Builder e di fare clic su Passa a modalità testo dopo aver aggiunto tutte le altre regole di filtro. Quindi, puoi aggiungere il codice per il filtro dell’attività principale come indicato sopra. 
>* È inoltre consigliabile aggiungere un raggruppamento per Nome progetto per facilitare la lettura del rapporto. Per ulteriori informazioni sull&#39;aggiunta di raggruppamenti ai report, vedere l&#39;articolo [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>

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
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a report, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizza le attività senza elementi figlio (potrebbero avere un elemento padre)

È possibile applicare il seguente filtro a un report attività per visualizzare le attività senza figli. Potrebbero avere genitori propri ed essere figli di altre mansioni.

1. Dall&#39;**icona Menu principale** ![Icona Menu principale](assets/main-menu-icon.png) nell&#39;angolo superiore destro o dal **Menu principale** ![Linee menu principale](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibili, fare clic su **Report**.

1. Fare clic su **Nuovo report**.
1. Seleziona un **report attività**.
1. Fare clic su **Filtri**.
1. Fai clic su **Aggiungi una regola filtro**.
1. Nella riga **Inizia a digitare il nome del campo ...**, inizia a digitare **Number of Children**, quindi fai clic su **Task >> Number of Children** quando viene visualizzato nell&#39;elenco.

1. Seleziona **Uguale (distinzione maiuscole/minuscole)** per il modificatore, quindi immetti **0** per il numero di elementi figlio.\
   ![Filtro attività padre](assets/parent-task-filter-from-the-ui-350x76.png)

   Oppure

   Fare clic su **Passa alla modalità testo** e nella finestra di modifica del testo copiare e incollare il testo seguente

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Fai clic su **Salva e Chiudi**.

   In questo modo viene estratto un report per tutte le attività in esecuzione nel sistema. Alcune di queste attività possono avere un elemento padre, ma non sono di per sé attività padre.

## Visualizza le attività con i genitori (potrebbero avere figli)

È possibile applicare il seguente filtro a un report attività per visualizzare le attività con attività principali, ovvero attività secondarie. Tuttavia, queste attività possono anche avere figli propri, perché il filtro non esclude i loro figli. Le attività figlio che sono anche padre per altre attività non sono considerate attività lavorative.

1. Dall&#39;icona **Main Menu** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro o dalle **Main Menu** ![Main Menu lines](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibili, fare clic su **Reports**.

1. Fare clic su **Nuovo report**.
1. Seleziona un **report attività**.
1. Fai clic su **Filtri**.
1. Fare clic su **Aggiungi regola filtro**.
1. Nella riga **Inizia a digitare il nome del campo ...**, inizia a digitare **ID principale**, quindi seleziona **Attività >> ID principale** quando viene visualizzato nell&#39;elenco.
1. Selezionare **Non è vuoto** per il modificatore.

   ![L&#39;ID padre non è vuoto](assets/filter-parent-id-not-blank-350x100.png)

   Oppure

   Fare clic su **Passa alla modalità testo** e nella finestra di modifica del testo copiare e incollare il testo seguente: 

   `parentID_Mod=notblank`

1. Fai clic su **Salva e Chiudi**.

   In questo modo viene generato un report per tutte le attività del sistema che hanno i genitori e sono attività figlio di tali genitori. Alcune di queste attività potrebbero essere un genitore.

## Visualizza attività senza figli e senza padri (attività autonome)

È possibile applicare il seguente filtro a un report attività per visualizzare le attività di lavoro autonome. Queste attività non hanno un genitore e non hanno figli.

1. Dall&#39;**icona Menu principale** ![Icona Menu principale](assets/main-menu-icon.png) nell&#39;angolo superiore destro o dal **Menu principale** ![Linee menu principale](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibili, fare clic su **Report**.

1. Fai clic su **Nuovo report**.
1. Selezionare un **report attività**.
1. Fare clic su **Filtri**.
1. Fai clic su **Aggiungi una regola filtro**.
1. In **Inizia a digitare il nome del campo ...** la riga inizia a digitare **Numero di elementi figlio**, quindi seleziona **Attività >> Numero di elementi figlio** dall&#39;elenco.
1. Selezionare **Uguale (Maiuscole/minuscole)** per il modificatore, quindi immettere **0** per il numero di figli.
1. Fare clic su **Aggiungi un&#39;altra regola filtro**.
1. Nella riga **Inizia a digitare il nome del campo ...**, inizia a digitare **ID principale**, quindi seleziona **Attività >> ID principale** dall&#39;elenco.
1. Selezionare **È vuoto** per il modificatore.

   ![L&#39;ID padre è vuoto e non sono presenti elementi figlio](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Oppure

   Invece dei passaggi 6-10 <!--ensure steps above stay accurate-->, fai clic su **Passa alla modalità testo** e nella finestra di modifica del testo copia e incolla il testo seguente:

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Fai clic su **Salva e Chiudi**.

   Questo consente di recuperare un report per tutte le attività del sistema che non hanno genitori né figli. Si tratta di attività di lavoro autonome.
