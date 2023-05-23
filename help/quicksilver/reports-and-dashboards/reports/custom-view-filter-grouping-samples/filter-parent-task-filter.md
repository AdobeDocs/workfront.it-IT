---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: visualizzare le attività principali"
description: È possibile applicare i filtri delle attività riportati di seguito per visualizzare le attività di lavoro. Le attività di lavoro sono attività che possono essere elaborate in modo indipendente e non sono attività padre di altre attività. In un esempio, un filtro identifica le attività secondarie che potrebbero essere padri stessi. In questo caso, non sono attività operative.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Filtro: visualizza le attività padre

È possibile applicare i filtri delle attività riportati di seguito per visualizzare le attività di lavoro. Le attività di lavoro sono attività che possono essere elaborate in modo indipendente e non sono attività padre di altre attività. In un esempio, un filtro identifica le attività secondarie che potrebbero essere padri stessi. In questo caso, non sono attività operative.

>[!TIP]
>
>* Se consideri di aggiungere più filtri a un rapporto, ti consigliamo di aggiungere tutti i filtri utilizzando l’interfaccia di Report Builder e di fare clic su Passa a modalità testo dopo aver aggiunto tutte le altre regole di filtro. Quindi, puoi aggiungere il codice per il filtro dell’attività principale come indicato sopra. 
* È inoltre consigliabile aggiungere un raggruppamento per Nome progetto per facilitare la lettura del rapporto. Per ulteriori informazioni sull’aggiunta di raggruppamenti ai rapporti, consulta l’articolo [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>


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
   <td> <p>Richiesta di modifica di un filtro </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Visualizza le attività senza elementi figlio (potrebbero avere un elemento padre)

Per visualizzare le attività senza elementi secondari, è possibile applicare il seguente filtro a un report di attività. Potrebbero avere genitori propri ed essere figli di altre mansioni.

1. Dalla sezione **Menu principale** ![](assets/main-menu-icon.png), fai clic su **Rapporti.**

1. Clic **Nuovo rapporto**.
1. Seleziona un **Report attività**.
1. Clic **Filtri**.
1. Clic **Aggiungere una regola di filtro**.
1. In **Inizia a digitare il nome del campo ...** riga, inizia a digitare **Numero di elementi figlio**.

1. Seleziona **Uguale (distinzione maiuscole/minuscole)** per il modificatore, quindi immetti **0** per il numero di figli.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   Oppure

   Clic **Passa alla modalità testo** e nella finestra di modifica del testo, copia e incolla il testo seguente: 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Clic **Salva e chiudi**.

   In questo modo viene estratto un report per tutte le attività in esecuzione nel sistema. Alcune di queste attività possono avere un elemento padre, ma non sono attività padre.

## Visualizza le attività con i genitori (potrebbero avere figli)

È possibile applicare il filtro seguente a un report di attività per visualizzare le attività con padre, ovvero le attività figlio. Tuttavia, queste attività possono anche avere figli propri, perché il filtro non esclude i loro figli. Le attività figlio che sono anche padri per altre attività non sono considerate attività di lavoro.

1. Dalla sezione **Menu principale** ![](assets/main-menu-icon.png), fare clic su **Rapporti.
1. Clic **Nuovo rapporto**.
1. Seleziona un **Report attività**.
1. Clic **Filtri**.
1. Clic **Aggiungere una regola di filtro**.
1. In **Inizia a digitare il nome del campo ...** riga, inizia a digitare **ID principale**.
1. Seleziona **Non è vuoto** per il modificatore.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   Oppure

   Clic **Passa alla modalità testo** e nella finestra di modifica del testo, copia e incolla il testo seguente: 

   `parentID_Mod=notblank`

1. Clic **Salva e chiudi**.

   In questo modo viene generato un report per tutte le attività del sistema che hanno i genitori e sono attività figlio di tali genitori. Alcune di queste attività potrebbero essere un genitore.

## Visualizza le attività senza elementi figlio e senza elementi padre (attività autonome)

È possibile applicare il filtro seguente a un report di attività per visualizzare le attività di lavoro autonome. Queste attività non hanno un genitore e non hanno figli propri.

1. Dalla sezione **Menu principale** ![](assets/main-menu-icon.png), fai clic su **Rapporti.**
1. Clic **Nuovo rapporto**.
1. Seleziona un **Report attività**.
1. Clic **Filtri**.
1. Clic **Aggiungere una regola di filtro** e nella **Inizia a digitare il nome del campo ...** inizio digitazione riga **Numero di elementi figlio** seleziona **Uguale (distinzione maiuscole/minuscole)** per il modificatore, quindi immetti **0** per il numero di figli.
1. Clic **Aggiungi un&#39;altra regola filtro** e nella **Inizia a digitare il nome del campo ...** inizio digitazione riga **ID principale**, quindi seleziona **È vuoto**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Oppure

   Anziché i passaggi 6-7, fai clic su **Passa alla modalità testo** e nella finestra di modifica del testo, copia e incolla il seguente testo: 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Clic **Salva e chiudi**.

   Questo consente di recuperare un report per tutte le attività del sistema che non hanno genitori né figli. Si tratta di attività di lavoro autonome.
