---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configura Scrum
description: Puoi configurare le seguenti opzioni per i team agili Scrum durante o dopo la creazione del team.
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '1725'
ht-degree: 0%

---

# Configura [!UICONTROL Scrum]

È possibile creare un team Agile in [!DNL Adobe Workfront] come descritto in [Creare un team Agile](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md). Durante la creazione di un team agile, puoi scegliere la metodologia utilizzata dal team per completare il lavoro. Puoi scegliere tra le seguenti opzioni:

* Scrum
* Kanban

Questo articolo descrive come configurare le impostazioni per un team Scrum. Dopo aver creato un team agile e aver scelto la metodologia Scrum, puoi fare riferimento a questo articolo per aggiornare le seguenti impostazioni:

* Se le storie vengono stimate in punti o ore
* Le colonne di stato sullo storyboard agile per iterazioni e progetti
* Campi aggiuntivi da visualizzare sulle schede delle storie sulla bacheca delle storie agile
* Come vengono utilizzati gli indicatori di colore per le storie sulla bacheca delle storie agile
* Applicazione delle date durante l&#39;aggiunta di elementi di lavoro a un&#39;iterazione

Per informazioni sulla configurazione di un team Kanban, vedere [Configurare Kanban](/help/quicksilver/agile/get-started-with-agile-in-workfront/configure-kanban.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Lavoro o superiore</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso ai team</p>  </td> 
  </tr>

</tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configura se le storie vengono stimate in punti o ore

>[!NOTE]
>
>Questa impostazione non può essere modificata se nel team sono presenti iterazioni attualmente in corso.

Puoi configurare le storie in modo che vengano stimate utilizzando punti o ore.

Per configurare il modo in cui le storie vengono stimate per il tuo team agile:

{{step1-to-team}}

1. Fai clic sull&#39;icona **[!UICONTROL Cambia team]**, quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.
1. Seleziona il team agile da gestire.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Modifica]**.

   Solo i membri del team con una licenza [!UICONTROL Standard], [!UICONTROL Piano] o [!UICONTROL Lavoro] possono vedere questa opzione.
   ![Modifica team](assets/edit-team-settings-350x205.png)

1. Nella sezione **[!UICONTROL Agile]**, nell&#39;area **[!UICONTROL Stima storie in]**, selezionare se si desidera utilizzare punti o ore per stimare la dimensione (carico di lavoro) delle storie. Se selezionate Punti (Points), specificate quante ore corrispondono a 1 punto. Il valore predefinito è 1 punto = 8 ore. Questo è il numero di ore pianificate che vengono aggiunte alla storia.

   **Esempio:** se hai selezionato di stimare le storie in punti e 1 punto equivale a 8 ore e una storia è stimata in 3 punti, alla storia vengono aggiunte 24 ore pianificate.

1. Fai clic su **[!UICONTROL Salva modifiche]**.

## Configurare le colonne di stato sullo storyboard Agile

Puoi configurare quali colonne vengono visualizzate sullo storyboard Agile per tutte le iterazioni assegnate al team o per un determinato progetto.

* [Configurare le colonne di stato per le iterazioni](#configure-status-columns-for-iterations)
* [Configurare le colonne di stato per i progetti](#configure-status-columns-for-projects)

### Configurare le colonne di stato per le iterazioni {#configure-status-columns-for-iterations}

Puoi definire gli stati che esistono sullo storyboard per il team agile. Questi sono gli unici stati visualizzati sullo storyboard.

Per definire gli stati disponibili per la bacheca delle storie associata al team Agile:

{{step1-to-team}}

1. Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team icona](assets/switch-team-icon.png), quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona il team agile da gestire.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Modifica]**.

   Solo i membri del team con una licenza di [!UICONTROL Piano] o [!UICONTROL Lavoro] possono visualizzare questa opzione.

   ![Modifica team](assets/edit-team-settings-350x205.png)

1. Nella sezione **[!UICONTROL Agile]**, individua l&#39;area **[!UICONTROL Storyboard]**.

1. (Facoltativo) Fai clic su **[!UICONTROL Aggiungi colonna]** per aggiungere una colonna di stato aggiuntiva alla bacheca delle storie.
1. (Facoltativo) Trascinate una colonna di stato utilizzando l&#39;indicatore di trascinamento per riordinare le colonne di stato sulla bacheca delle storie. Impossibile spostare la prima colonna e trascinare un&#39;altra colonna davanti alla prima colonna.

   ![Trascina](assets/agile-story-card-drag-and-drop.png)

1. Seleziona sia lo stato di attività che quello di problema. Gli stati delle attività vengono visualizzati come titolo della colonna per ogni colonna della bacheca delle storie. Gli stati del problema selezionati vengono mappati agli stati delle attività. Ciò significa che quando si sposta un problema in un&#39;altra colonna della bacheca delle storie, lo stato del problema cambia in base agli stati visualizzati qui e non al nome della colonna sulla bacheca delle storie (che riflette lo stato dell&#39;attività).

   >[!IMPORTANT]
   >
   >Solo gli stati bloccati a livello di sistema sono disponibili per la selezione; non è possibile selezionare stati specifici per il gruppo. Inoltre, lo stato della prima colonna corrisponde sempre a **[!UICONTROL Nuovo]**.

   È possibile aggiungere stati personalizzati se sono stati configurati dall&#39;amministratore di [!DNL Workfront]. Gli stati personalizzati possono essere configurati come descritto in [Creare o modificare uno stato](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   >[!NOTE]
   >
   >Quando si selezionano gli stati del problema, per impostazione predefinita la terza colonna viene [!UICONTROL Chiusa]. Se disponi di più di tre colonne, accertati di aggiornarle manualmente in modo da riflettere gli stati corretti.

1. Fai clic su **[!UICONTROL Salva modifiche]**.

### Configurare le colonne di stato per i progetti {#configure-status-columns-for-projects}

Per informazioni su come configurare le colonne di stato per un progetto, vedere la sezione [Creare o personalizzare una [!UICONTROL visualizzazione Agile]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) nell&#39;articolo [Creare o modificare le visualizzazioni in [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Configura campi aggiuntivi da visualizzare sulle schede delle storie sulla bacheca delle storie agile

Quando aggiungete campi alle schede delle storie, i campi sono di sola visualizzazione e di sola visualizzazione quando vengono compilati.

Per impostazione predefinita, nella scheda delle storie vengono visualizzati i seguenti tipi di dati per le attività e i problemi:

* Nome della storia con un collegamento diretto all’attività o al problema
* Il nome del progetto con un collegamento diretto al progetto
* Questo collegamento viene visualizzato solo per i brani, non per le sottoattività
* Descrizione dell’attività o del problema
* Impegno attuale
* Visualizzare e modificare la percentuale di completamento regolando la percentuale stessa o il numero di punti o ore completate
* Utenti assegnati

È possibile visualizzare dati aggiuntivi, inclusi dati personalizzati, sulle schede delle storie. È possibile visualizzare campi aggiuntivi sulle schede delle storie per diversi motivi. Ad esempio, potresti voler visualizzare l’ID cliente se stai lavorando su storie per più clienti all’interno dell’iterazione, oppure potresti voler visualizzare la Data di inizio del progetto o la Data di completamento del progetto.

>[!NOTE]
>
>Se si utilizza un campo personalizzato in una scheda brani, il nome non può contenere un punto o un punto.

Per configurare le schede delle storie assegnate al team Agile in modo da visualizzare campi aggiuntivi:

{{step1-to-team}}

1. Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team icona](assets/switch-team-icon.png), quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona il team agile da gestire.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Modifica]**.
Solo i membri del team con una licenza di [!UICONTROL Piano] o [!UICONTROL Lavoro] possono visualizzare questa opzione.

   ![Modifica team](assets/edit-team-settings-350x205.png)

1. Nella sezione **[!UICONTROL Agile]** digitare un nome di campo per individuarlo.

   ![Campi aggiuntivi](assets/agile-additional-fields-scrum.png)

1. Seleziona il nome del campo da aggiungere.
1. Digita **[!UICONTROL Nome visualizzato]** per il campo da visualizzare sulla storia o sulla scheda problema.
1. Fai clic su **[!UICONTROL Salva modifiche]**.

## Configurare il modo in cui gli indicatori di colore vengono utilizzati per le storie sulla bacheca delle storie agile

Per impostazione predefinita, le sezioni della bacheca delle storie in un’iterazione agile sono codificate con un colore in base al progetto a cui è associata la storia. A ogni progetto viene assegnato arbitrariamente un colore sulla bacheca delle storie. Puoi modificare questo comportamento predefinito per ogni team agile. I colori per le storie agili possono essere legati alla priorità della storia, al proprietario e così via.

Per modificare il comportamento di assegnazione dei colori alle storie per un team agile:

{{step1-to-team}}

1. Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team icona](assets/switch-team-icon.png), quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona il team agile da gestire.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Modifica]**.

   Solo i membri del team con una licenza di [!UICONTROL Piano] o [!UICONTROL Lavoro] possono visualizzare questa opzione.

   ![Modifica team](assets/edit-team-settings-350x205.png)

1. Nella sezione [!UICONTROL Agile], nell&#39;area [!UICONTROL Associa colore scheda a], selezionare una delle opzioni seguenti:

   * **[!UICONTROL Progetto]**: i colori sono associati al progetto a cui è associata la storia. Quando si crea una storia, è necessario associarla a un progetto, come descritto in [Creare una storia Agile](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). Tutte le attività dello stesso progetto vengono visualizzate con lo stesso colore.
   * **[!UICONTROL Modulo libero]**: per impostazione predefinita, tutte le schede sono visualizzate in blu finché l&#39;utente non cambia il colore manualmente, come descritto in [[!UICONTROL Categorizzare le storie per colore] sulla bacheca Scrum](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md).
   * **[!UICONTROL Priorità]**: i colori sono associati alla priorità della storia, come segue:

      * Alto = Rosso
      * Medium = Giallo
      * Basso = Verde

        Se l&#39;amministratore di sistema ha configurato le priorità personalizzate per il sistema [!DNL Workfront], la priorità più alta è rossa, la seconda più alta è gialla e la terza più alta è verde.
   * **[!UICONTROL Proprietario attività]**: tutti i brani con lo stesso assegnatario primario sono dello stesso colore. L&#39;assegnatario principale è l&#39;utente che è stato assegnato per primo all&#39;attività.


1. Fai clic su **[!UICONTROL Salva modifiche]**.

## Configurare la modalità di applicazione delle date quando si aggiungono elementi di lavoro a un’iterazione

Per impostazione predefinita, quando si aggiunge un elemento di lavoro a un&#39;iterazione Scrum, la Data inizio pianificata e la Data completamento pianificata dell&#39;elemento di lavoro vengono modificate in modo da corrispondere alle date di inizio e di fine dell&#39;iterazione. È possibile scegliere di mantenere le date originali su tutti gli elementi di lavoro del team.

{{step1-to-team}}

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Modifica]**.
Solo i membri del team con una licenza di [!UICONTROL Piano] o [!UICONTROL Lavoro] possono visualizzare questa opzione.
1. Nella sezione [!UICONTROL Agile], in [!UICONTROL Quando un elemento di lavoro viene aggiunto a un&#39;iterazione], selezionare una delle opzioni seguenti:

   * **[!UICONTROL Modificare la data di inizio pianificata e la data di completamento pianificata in modo che corrispondano alle date di inizio e di fine dell&#39;iterazione]**: quando si aggiungono elementi di lavoro a un&#39;iterazione, le date degli elementi di lavoro vengono modificate in base alle date dell&#39;iterazione.

     Per ulteriori informazioni sulla modifica delle date, vedere la sezione [Comprendere in che modo l&#39;aggiunta di storie influisce sulle date delle attività](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understand-how-adding-stories-affects-task-dates) nell&#39;articolo [Aggiungere storie a un&#39;iterazione esistente](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL Non modificare la Data inizio pianificata e la Data completamento pianificata in modo che corrispondano alle date di inizio e di fine dell&#39;iterazione]**: quando gli elementi di lavoro vengono aggiunti a un&#39;iterazione, gli elementi di lavoro mantengono le date originali.

   Se si modifica l&#39;opzione data, le date per gli elementi di lavoro già presenti nell&#39;iterazione non vengono modificate.

   Queste opzioni possono influenzare le date in cui i team assegnano elementi di lavoro alle rispettive iterazioni. Ad esempio, il team A modifica le date degli elementi di lavoro in base alle date di iterazione e il team B non modifica le date degli elementi di lavoro. Se il team B assegna un elemento di lavoro all&#39;iterazione del team A, le date dell&#39;elemento di lavoro verranno modificate. Tuttavia, se il team A assegna un elemento di lavoro all&#39;iterazione del team B, le date non cambieranno.

1. Fai clic su **[!UICONTROL Salva modifiche]**.
