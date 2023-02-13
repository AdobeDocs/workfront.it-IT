---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Esamina i grafici per comprendere le tendenze di avanzamento degli obiettivi negli obiettivi di Adobe Workfront
description: Puoi visualizzare lo stato generale dei tuoi obiettivi e la loro tendenza nel tempo nella sezione Grafici degli obiettivi di Adobe Workfront. I grafici di questa sezione non suddividono l'avanzamento di ciascun obiettivo, ma forniscono invece un'istantanea olistica dello stato di avanzamento di tutti gli obiettivi e della loro tendenza di avanzamento nel tempo durante un determinato periodo.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 3989903687f2ea64ebd5ad754119ce1a9d70b9f3
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# Esamina i grafici per comprendere le tendenze di avanzamento degli obiettivi negli obiettivi di Adobe Workfront

<!-- drafted mostly for P&P release-->

Puoi visualizzare lo stato generale dei tuoi obiettivi e la loro tendenza nel tempo nella sezione Grafici degli obiettivi di Adobe Workfront. I grafici di questa sezione non suddividono l&#39;avanzamento di ciascun obiettivo, ma forniscono invece un&#39;istantanea olistica dello stato di avanzamento di tutti gli obiettivi e della loro tendenza di avanzamento nel tempo durante un determinato periodo.

>[!IMPORTANT]
>
>Puoi visualizzare un conteggio totale degli obiettivi nella sezione Grafici per un periodo di tempo selezionato. Tuttavia, gli obiettivi di Workfront tengono conto solo degli obiettivi con stato Attivo e Chiuso quando si calcola lo stato di avanzamento dell’obiettivo complessivo e della percentuale di completamento.

## Requisiti di accesso

<!--drafted for P&P release: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>

-->

Per eseguire le azioni descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze di Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td> <p>Devi acquistare una licenza aggiuntiva per la funzionalità Obiettivi di Adobe Workfront per accedere alla descritta in questo articolo. </p> <p>Per informazioni, consulta <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Visualizzare o accedere in modo più rapido agli obiettivi</p> <p><b>NOTA</b><p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Concedere l’accesso agli obiettivi di Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> 
    <div> 
     <p>Visualizza o autorizzazioni superiori per gli obiettivi</p> 
     <p>Per informazioni sulla condivisione degli obiettivi, vedi <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario disporre dei seguenti elementi prima di poter iniziare:

* Modello di layout che include l’area Obiettivi del menu principale.

## Tipi di grafici negli obiettivi di Workfront

I seguenti grafici sono disponibili nella sezione Grafici o Obiettivi di Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">La tabella dello stato di salute dell'obiettivo</td> 
   <td> <p>Grafico a indicatori che mostra quanto segue:</p> 
    <ul> 
     <li>Numero totale di obiettivi per il periodo di tempo selezionato. Vengono presi in considerazione gli obiettivi con qualsiasi stato. </li> 
     <li>Stato di avanzamento degli obiettivi con stato Attivo e Chiuso.</li> 
    </ul> <p>Per informazioni sul modo in cui gli obiettivi di Workfront calcolano lo stato di avanzamento, consulta <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Panoramica dell’avanzamento e della condizione dell’obiettivo in Obiettivi di Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Grafico di avanzamento dell'obiettivo</td> 
   <td> <p>Grafico a linee che visualizza gli aggiornamenti apportati agli obiettivi con incrementi settimanali durante la durata dell'obiettivo. Il grafico di avanzamento dell’obiettivo mostra quanto segue:</p> 
    <ul> 
     <li>Una percentuale media prevista ed effettiva di completamento di tutti gli obiettivi attivi e chiusi nel periodo selezionato. L'avanzamento percentuale completo è suddiviso in incrementi settimanali contrassegnati da nodi. </li> 
     <li>La percentuale media complessiva di progressi per gli obiettivi attivi e chiusi rispetto alla settimana precedente. </li> 
    </ul> <p>Suggerimento: Il grafico di avanzamento obiettivo potrebbe non visualizzare alcuna informazione quando vengono effettuati aggiornamenti sugli obiettivi al di fuori del periodo di tempo selezionato. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Esamina l’avanzamento dell’obiettivo nei grafici

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) > **Obiettivi** nell&#39;angolo in alto a destra.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Viene aperta l’area Obiettivi di Workfront.

1. Fai clic su **Grafici** nel pannello a sinistra.

   ![](assets/graphs-in-left-panel.png)

   Viene visualizzata la sezione Grafici.

   Per impostazione predefinita, gli obiettivi visualizzati nella sezione Grafici sono limitati dai seguenti criteri:

   * Filtri applicati all’area Grafici.
   * Obiettivi con stato Attivo e Bozza.

1. (Facoltativo) Seleziona il tipo di informazioni da visualizzare aggiornando i filtri nell’angolo in alto a destra della sezione Grafici.

   Per ulteriori informazioni sul filtro degli obiettivi, vedi [Filtrare le informazioni negli obiettivi di Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   Se si è scelto di visualizzare più di un periodo di tempo, per ciascun periodo vengono visualizzati sia un grafico dello stato di salute (indicatore) che un grafico dell&#39;avanzamento (linea).

1. Rivedi le informazioni nella tabella seguente quando rivedi il grafico di integrità degli obiettivi.

   ![](assets/gauge-graph-wf-align-350x230.png)

   | Numero totale di obiettivi | Il numero nella parte inferiore del grafico indica il numero di tutti gli obiettivi del periodo selezionato, in tutti gli stati selezionati. |
   |---|---|
   | Percentuale media completata | Nella parte superiore del grafico, questo numero indica la percentuale media di completamento degli obiettivi attivi e chiusi nel periodo di tempo selezionato. |
   | Obiettivi e loro progressi | Numero di obiettivi per ogni segmento di stato di avanzamento, quando passi il cursore del mouse sui segmenti del grafico. Solo gli obiettivi nello stato Attivo o Chiuso vengono conteggiati nei segmenti. |


1. Rivedi le informazioni nella tabella seguente quando rivedi il grafico di avanzamento obiettivo.

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Avanzamento linea di base</td> 
      <td>La linea di pendenza verde indica la percentuale totale di completamento prevista per gli obiettivi attivi e chiusi per il periodo di tempo selezionato. Tutti gli obiettivi entro un periodo sono attesi per essere completati, quindi il progresso previsto è sempre del 100% alla fine del periodo. </td> 
     </tr> 
     <tr> 
      <td>Avanzamento effettivo</td> 
      <td> <p>La linea blu indica la percentuale totale effettiva di completamento della media degli obiettivi attivi e chiusi per il periodo di tempo selezionato in incrementi settimanali. Ogni settimana durante la durata dell'obiettivo viene contrassegnato da un nodo nella riga. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Passa il puntatore del mouse su un nodo della settimana nel grafico di avanzamento dell&#39;obiettivo e controlla quanto segue:

   * **Data della settimana**: Mese, giorno e anno della settimana selezionata.
   * **Avanzamento**: Una media della percentuale effettiva di completamento di tutti gli obiettivi per la settimana selezionata.
   * **Linea**: Una media della percentuale di completamento prevista di tutti gli obiettivi per la settimana selezionata.

1. (Facoltativo) Fai clic su **Avanzamento** nella parte inferiore del grafico di avanzamento per rimuovere la linea di avanzamento generale effettiva

   Oppure

   Fai clic su **Linea** nella parte inferiore del grafico di avanzamento per rimuovere lo stato di avanzamento previsto dal grafico.

 
