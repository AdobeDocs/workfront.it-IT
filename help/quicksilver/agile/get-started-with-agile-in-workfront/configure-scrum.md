---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configura punteggio
description: Puoi configurare le seguenti opzioni per i team Scrum agile durante o dopo la creazione del team.
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 0%

---

# Configura [!UICONTROL Scratto]

Puoi configurare le seguenti opzioni per i team agili durante o dopo la creazione del team. Crea un team agile (Kanban o Scrum) in [!DNL Adobe Workfront] come descritto in [Creare un team agile](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Work] o superiore</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo [!DNL Workfront] amministratore.

## Configura se le storie sono stimate in punti o ore

>[!NOTE]
>
>Questa impostazione non può essere modificata se il team dispone di iterazioni attualmente in corso.

È possibile configurare le storie in modo da stimarle utilizzando punti o ore.

Per configurare la stima delle storie per il team agile:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!UICONTROL Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. Fai clic sul pulsante **[!UICONTROL Cambia team]** , quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.
1. Seleziona il team agile da gestire.
1. Fai clic sul pulsante **[!UICONTROL Altro]** quindi seleziona **[!UICONTROL Modifica]**.

   Solo i membri del team con una [!UICONTROL Pianificare] o [!UICONTROL Lavoro] licenza vedere questa opzione.\
   ![Modifica team](assets/edit-team-settings-350x205.png)

1. In **[!UICONTROL Agile]** nella sezione **[!UICONTROL Storie stimate in]** area, selezionare se si desidera utilizzare punti o ore per stimare la dimensione (carico di lavoro) delle storie. Se selezioni Punti, specifica quante ore sono uguali a 1 punto. (Il valore predefinito è 1 punto = 8 ore.) Questo è il numero di ore pianificate aggiunte alla storia.

   **Esempio:** Se hai selezionato per stimare le storie in punti e 1 punto è uguale a 8 ore, e una storia è stimata in 3 punti, alla storia vengono aggiunte 24 ore pianificate.

1. Fai clic su **[!UICONTROL Salva modifiche]**.

## Configurare le colonne di stato sulla bacheca di storie agile

È possibile configurare quali colonne vengono visualizzate sulla bacheca di storie agili per tutte le iterazioni assegnate al team o per un determinato progetto.

* [Configurare le colonne di stato per le iterazioni](#configure-status-columns-for-iterations)
* [Configurare le colonne di stato per i progetti](#configure-status-columns-for-projects)

### Configurare le colonne di stato per le iterazioni {#configure-status-columns-for-iterations}

È possibile definire gli stati esistenti sulla scheda della storia per il team agile. Questi sono gli unici stati visualizzati sulla lavagna.

Per definire gli stati disponibili per la storiella associata al team agile:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona il team agile da gestire.
1. Fai clic sul pulsante **[!UICONTROL Altro]** quindi seleziona **[!UICONTROL Modifica]**.

   Solo i membri del team con una [!UICONTROL Pianificare] o [!UICONTROL Lavoro] licenza vedere questa opzione.

   ![Modifica team](assets/edit-team-settings-350x205.png)

1. In **[!UICONTROL Agile]** , individua la sezione **[!UICONTROL Scheda Storia]** area.

1. (Facoltativo) Fai clic su **[!UICONTROL Aggiungi colonna]** per aggiungere una colonna di stato aggiuntiva alla storiella.
1. (Facoltativo) Trascinate una colonna di stato utilizzando l&#39;indicatore di trascinamento della selezione per riordinare le colonne di stato sulla storiella. Non è possibile spostare la prima colonna e trascinarne un’altra davanti alla prima colonna.

   ![Trascinamento della selezione](assets/agile-story-card-drag-and-drop.png)

1. Selezionare sia lo stato dell&#39;attività che quello del problema. Gli stati delle attività vengono visualizzati come titolo della colonna per ogni colonna del brano. Gli stati del problema selezionati vengono mappati sullo stato dell&#39;attività. Questo significa che quando si sposta un problema in un&#39;altra colonna della tabella delle storie, lo stato del problema cambia in base agli stati dei problemi qui mostrati e non in base al nome della colonna della tabella delle storie (che riflette lo stato dell&#39;attività).

   >[!IMPORTANT]
   >
   >Sono disponibili solo gli stati bloccati a livello di sistema; non è possibile selezionare gli stati specifici del gruppo. Inoltre, lo stato della prima colonna corrisponde sempre a **[!UICONTROL Nuovo]**.

   Puoi aggiungere stati personalizzati se [!DNL Workfront] l’amministratore li ha configurati; gli stati personalizzati possono essere configurati come descritto in [Creare o modificare uno stato](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   >[!NOTE]
   >
   >Quando selezioni lo stato del problema, per impostazione predefinita la terza colonna è sempre impostata su [!UICONTROL Chiuso]. Se hai più di tre colonne, assicurati di aggiornare manualmente le colonne per riflettere gli stati corretti.

1. Fai clic su **[!UICONTROL Salva modifiche]**.

### Configurare le colonne di stato per i progetti {#configure-status-columns-for-projects}

Per informazioni su come configurare le colonne di stato per un progetto, consulta la sezione . [Crea o personalizza un [!UICONTROL Agile] visualizzare](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) nell&#39;articolo [Creare o modificare visualizzazioni in [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Configura campi aggiuntivi da visualizzare sulle schede dei racconti sulla bacheca dei racconti Agile

Quando si aggiungono campi alle schede dei brani, i campi sono di sola visualizzazione e di sola visualizzazione quando il campo è compilato.

Per impostazione predefinita, nella scheda del brano vengono visualizzati i seguenti tipi di dati per attività e problemi:

* Nome della storia con un collegamento direttamente all’attività o al problema
* Nome del progetto con un collegamento diretto al progetto
* Questo collegamento viene visualizzato solo per i brani, non per le sottoattività
* Descrizione dell&#39;attività o del problema
* Impegno attuale
* Visualizza e modifica la percentuale di completamento regolando la percentuale di completamento oppure regolando il numero di punti o ore di completamento
* Utenti assegnati

È possibile visualizzare dati aggiuntivi (inclusi dati personalizzati) sulle schede delle storie. È possibile visualizzare campi aggiuntivi sulle schede delle storie per diversi motivi. Ad esempio, potrebbe essere utile visualizzare l&#39;ID cliente se si stanno lavorando a storie per più clienti nell&#39;iterazione, oppure se si desidera visualizzare la data di inizio del progetto o la data di completamento del progetto.

>[!NOTE]
>
>Se utilizzi un campo personalizzato su una scheda del brano, non può contenere un punto/punto nel nome.

Per configurare le schede delle storie assegnate al team agile in modo da visualizzare campi aggiuntivi:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!UICONTROL Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona il team agile da gestire.
1. Fai clic sul pulsante **[!UICONTROL Altro]** quindi seleziona **[!UICONTROL Modifica]**.\
   Solo i membri del team con una [!UICONTROL Pianificare] o [!UICONTROL Lavoro] licenza vedere questa opzione.

   ![Modifica team](assets/edit-team-settings-350x205.png)

1. In **[!UICONTROL Agile]** digitare un nome di campo per individuarlo.

   ![Campi aggiuntivi](assets/agile-additional-fields-scrum.png)

1. Seleziona il nome del campo da aggiungere.
1. Digita il **[!UICONTROL Nome visualizzato]** per mostrare il campo sulla storia o sulla scheda del rilascio.
1. Fai clic su **[!UICONTROL Salva modifiche]**.

## Configura come vengono utilizzati gli indicatori di colore per le storie sulla bacheca di storie agile

Per impostazione predefinita, i riquadri della storiella in un&#39;iterazione agile sono codificati in base al colore del progetto a cui è associata la storia. A ogni progetto viene assegnato arbitrariamente un colore sulla lavagna. Puoi modificare questo comportamento predefinito per ogni team agile. I colori per le storie agili possono essere legati alla priorità della storia, al proprietario e così via.

Per modificare il comportamento di come i colori vengono assegnati ai brani per un team agile:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona il team agile da gestire.
1. Fai clic sul pulsante **[!UICONTROL Altro]** quindi seleziona **[!UICONTROL Modifica]**.

   Solo i membri del team con una [!UICONTROL Pianificare] o [!UICONTROL Lavoro] licenza vedere questa opzione.

   ![Modifica team](assets/edit-team-settings-350x205.png)

1. In [!UICONTROL Agile] nella sezione [!UICONTROL Associa colore scheda a] seleziona una delle seguenti opzioni:

   * **[!UICONTROL Progetto]**: I colori sono associati al progetto a cui è legata la storia. (Quando viene creato un brano, deve essere associato a un progetto, come descritto in [Creare una storia di Agile](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). Tutte le attività dello stesso progetto vengono visualizzate con lo stesso colore.
   * **[!UICONTROL Forma libera]**: Tutte le schede sono visualizzate in blu per impostazione predefinita finché un utente non modifica manualmente il colore, come descritto in [[!UICONTROL Categorizzare le storie per colore] sulla scheda Scrum](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md).
   * **[!UICONTROL Priorità]**: I colori sono associati alla priorità della storia, come segue:

      * Alto = Rosso
      * Media = Giallo
      * Bassa = Verde\

         Se l&#39;amministratore di sistema ha configurato le priorità personalizzate per il tuo [!DNL Workfront] la priorità più alta è il rosso, la seconda il giallo e la terza il verde.
   * **[!UICONTROL Proprietario attività]**: Tutte le storie con lo stesso assegnatario primario sono dello stesso colore. L’assegnatario principale è l’utente che è stato assegnato per la prima volta all’attività.


1. Fai clic su **[!UICONTROL Salva modifiche]**.

## Configura come vengono applicate le date quando si aggiungono elementi di lavoro a un&#39;iterazione

Per impostazione predefinita, quando si aggiunge un elemento di lavoro a un&#39;iterazione Scrum, la data di inizio pianificata e la data di completamento pianificata sull&#39;elemento di lavoro vengono modificate in modo che corrispondano alle date di inizio e di fine dell&#39;iterazione. È possibile scegliere di mantenere le date originali su tutti gli elementi di lavoro del team.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Team]**.
1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.
1. Fai clic sul pulsante **[!UICONTROL Altro]** quindi seleziona **[!UICONTROL Modifica]**.\
   Solo i membri del team con una [!UICONTROL Pianificare] o [!UICONTROL Lavoro] licenza vedere questa opzione.
1. In [!UICONTROL Agile] nella sezione [!UICONTROL Quando un elemento di lavoro viene aggiunto a un&#39;iterazione] seleziona una delle seguenti opzioni:

   * **[!UICONTROL Modificare la data di inizio pianificata e la data di completamento pianificata in modo che corrispondano alle date di inizio e di fine dell&#39;iterazione]**: Quando gli elementi di lavoro vengono aggiunti a un&#39;iterazione, le date degli elementi di lavoro vengono modificate in date di iterazione.\

      Per ulteriori informazioni sulla modifica delle date, consulta la sezione . [Comprendere in che modo l&#39;aggiunta di storie influisce sulle date delle attività](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understa) nell&#39;articolo [Aggiungere storie a un&#39;iterazione esistente](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL Non modificare la data di inizio pianificata e la data di completamento pianificata in modo che corrispondano alle date di inizio e di fine dell&#39;iterazione]**: Quando gli elementi di lavoro vengono aggiunti a un&#39;iterazione, gli elementi di lavoro conservano le date originali.

   Se si modifica l&#39;opzione data, le date degli elementi di lavoro già presenti nell&#39;iterazione non vengono modificate.

   Queste opzioni possono influenzare le date in cui i team assegnano elementi di lavoro alle rispettive iterazioni. Ad esempio, il team A modifica le date degli elementi di lavoro nelle date di iterazione e il team B non modifica le date degli elementi di lavoro. Se il team B assegna un elemento di lavoro all&#39;iterazione del team A, le date dell&#39;elemento di lavoro verranno modificate. Tuttavia, se il team A assegna un elemento di lavoro all&#39;iterazione del team B, le date non verranno modificate.

1. Fai clic su **[!UICONTROL Salva modifiche]**.
