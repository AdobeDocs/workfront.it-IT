---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configura Kanban
description: Crea un team agile Kanban o Scrum in [!DNL Adobe Workfront].
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 3c5bcb85080a882a8b69bffcd01563a0479f98a5
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 0%

---

# Configura [!UICONTROL Kanban]

Puoi creare un team agile in [!DNL Adobe Workfront] come descritto in [Creare un team agile](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md). Durante la creazione di un team agile, puoi scegliere la metodologia utilizzata dal team per completare il lavoro. Puoi scegliere tra le seguenti opzioni:

* Scrum
* Kanban

Questo articolo descrive come configurare le impostazioni per un team Kanban. Dopo aver creato un team agile e scelto la metodologia Kanban, puoi fare riferimento a questo articolo per aggiornare le seguenti impostazioni:

* Se le storie vengono stimate in punti o ore
* Le colonne di stato sullo storyboard Agile
* Campi aggiuntivi da visualizzare sulle schede delle storie sulla bacheca delle storie agile
* Limite WIP (Work In Progress)
* Come aggiungere automaticamente brani dal backlog
* Per quanto tempo le carte rimangono sul Kanban Board

Per informazioni sulla configurazione di un team Scrum, consulta [Configura Scrum](../get-started-with-agile-in-workfront/configure-scrum.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>Nuovo: [!UICONTROL Standard]</p> 
   oppure
   <p>Corrente: [!UICONTROL Work] o versione successiva</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> <p>Modificare l’accesso ai team</p>  </td> 
  </tr>

</tbody> 
</table>

*Per sapere quale piano o tipo di licenza si dispone, contattare il [!DNL Workfront] amministratore.

## Configura se le storie vengono stimate in punti o ore

Puoi configurare le storie in modo che vengano stimate utilizzando punti o ore.

Per configurare il modo in cui le storie vengono stimate per il tuo team agile:

{{step1-to-team}}

1. Fai clic su **[!UICONTROL Cambia team]** icona ![](assets/switch-team-icon.png), quindi selezionare un nuovo team dal menu a discesa o cercare un team nella casella di ricerca.
1. Seleziona il team agile da gestire.
1. Fai clic su **[!UICONTROL Altro]** menu ![](assets/more-menu.png) , quindi seleziona **[!UICONTROL Modifica]**.

   ![Modifica team](assets/edit-team-settings-350x205.png)

1. In **[!UICONTROL Agile]** , nella sezione **[!UICONTROL Stima storie in]** selezionare se si desidera utilizzare punti o ore per stimare la dimensione (carico di lavoro) dei brani. Se selezionate Punti (Points), specificate quante ore corrispondono a 1 punto. Il valore predefinito è 1 punto = 8 ore. Questo è il numero di ore pianificate che vengono aggiunte alla storia.

   **Esempio:** Se hai selezionato di stimare le storie in punti e 1 punto equivale a 8 ore e una storia è stimata in 3 punti, alla storia vengono aggiunte 24 ore pianificate.

1. Clic **[!UICONTROL Salva modifiche]**.

## Configurare le colonne di stato sullo storyboard Agile

Puoi definire gli stati che esistono sullo storyboard per il team agile. Questi sono gli unici stati visualizzati sullo storyboard.

Per definire gli stati disponibili per la bacheca delle storie associata al team Agile:

{{step1-to-team}}

1. Fai clic su **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi selezionare un nuovo team dal menu a discesa o cercare un team nella barra di ricerca.

1. Seleziona il team agile da gestire.
1. Fai clic su **[!UICONTROL Altro]** , quindi seleziona **[!UICONTROL Modifica]**.

   ![Modifica team](assets/edit-team-settings-350x205.png)

1. In **[!UICONTROL Agile]** , individuare la sezione **[!UICONTROL Storyboard]** area.

1. (Facoltativo) Fai clic su **[!UICONTROL Aggiungi colonna]** per aggiungere una colonna di stato aggiuntiva allo storyboard.
1. (Facoltativo) Trascinate una colonna di stato utilizzando l&#39;indicatore di trascinamento per riordinare le colonne di stato sulla bacheca delle storie. Impossibile spostare la prima colonna e trascinare un&#39;altra colonna davanti alla prima colonna.

   ![Trascina](assets/agile-story-card-drag-and-drop.png)

1. Selezionare gli stati delle attività.

   >[!IMPORTANT]
   >
   >Solo gli stati bloccati a livello di sistema sono disponibili per la selezione. Non è possibile selezionare stati specifici del gruppo. Lo stato della prima colonna corrisponde sempre a **[!UICONTROL Nuovo]**.

   È possibile aggiungere stati personalizzati se [!DNL Workfront] configurati dall&#39;amministratore. Per ulteriori informazioni, consulta [Creare o modificare uno stato](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Clic **[!UICONTROL Salva modifiche]**.

## Configura campi aggiuntivi da visualizzare sulle schede delle storie sulla bacheca delle storie agile

Quando si aggiungono campi alle schede delle storie, i campi sono di sola visualizzazione e vengono visualizzati solo quando il campo è popolato.

Per impostazione predefinita, nella scheda delle storie per le attività e i problemi vengono visualizzati i seguenti tipi di dati:

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
>Se si utilizza un campo personalizzato in una scheda brani, il nome non può contenere un punto.

Per configurare le schede delle storie assegnate al team Agile in modo da visualizzare campi aggiuntivi:

{{step1-to-team}}

1. Fai clic su **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi selezionare un nuovo team dal menu a discesa o cercare un team nella barra di ricerca.

1. Seleziona il team agile da gestire.
1. Fai clic su **[!UICONTROL Altro]** , quindi seleziona **[!UICONTROL Modifica]**.\

   ![Modifica team](assets/edit-team-settings-350x205.png)

1. In **[!UICONTROL Agile]** , digitare un nome di campo per individuarlo.

   ![Campi aggiuntivi](assets/agile-additional-fields-kanban.png)

1. Seleziona il nome del campo da aggiungere.
1. Digita il **[!UICONTROL Nome visualizzato]** il campo da mostrare sulla storia o sulla scheda problema.
1. Clic **[!UICONTROL Salva modifiche]**.

## Configurare il limite WIP

Quando si definisce il limite WIP di un team Kanban, è possibile controllare il numero di elementi su cui il team sta attualmente lavorando limitando il numero di attività che possono essere visualizzate nel [!UICONTROL Nuovo] o [!UICONTROL In corso] colonna sulla [!UICONTROL Kanban] bacheca

Dopo aver configurato il limite WIP per un team Kanban, è possibile visualizzarlo e aggiornarlo dalla sezione [!UICONTROL Kanban] storyboard agile, come descritto in [Gestire il limite WIP (Work In Progress) per [!UICONTROL Kanban] scheda](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Per limitare WIP per il team Kanban:

{{step1-to-team}}

1. Fai clic su **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi selezionare un nuovo team dal menu a discesa o cercare un team nella barra di ricerca.

1. Seleziona il team Kanban da gestire.
1. Fai clic su **[!UICONTROL Altro]** menu ![](assets/more-menu.png), quindi seleziona **[!UICONTROL Modifica]**.

   ![Modifica team](assets/edit-team-settings-350x205.png)

1. In **[!UICONTROL Agile]** , nella sezione **[!UICONTROL Metodologia]** , verificare che sia selezionato Kanban.

1. In **[!UICONTROL Storyboard]** , nella sezione **[!UICONTROL Limite WIP]** , specificare il numero massimo di elementi consentito in ciascuna colonna del [!UICONTROL Kanban] storyboard agile. È possibile impostare un limite diverso per ogni colonna. Il limite massimo che è possibile impostare per ogni colonna è 100.\
   Se impostato, il limite WIP visualizza un messaggio di avvertenza sul [!UICONTROL Kanban] storyboard agile ogni volta che viene superato il limite per qualsiasi colonna dello storyboard. Questo messaggio di avviso viene visualizzato solo la prima volta che viene superato il limite WIP. Questo messaggio di avvertenza non viene visualizzato nelle colonne con uno stato che equivale a [!UICONTROL Completa].\
   Il limite WIP è semplicemente un&#39;avvertenza visiva e non impedisce al team di avere più elementi in una singola colonna rispetto al limite impostato.

   ![Limite WIP](assets/wip-limit-350x193.png)

1. Clic **Salva modifiche**.

## Configurare l’aggiunta automatica di brani dal backlog

<!-- this functionality needs to be verified-->

Puoi configurare i brani dal backlog in modo che vengano aggiunti automaticamente alla prima colonna del [!UICONTROL Kanban] bacheca immediatamente dopo lo spostamento di un elemento da tale colonna.

{{step1-to-team}}

1. Fai clic su **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi selezionare un nuovo team dal menu a discesa o cercare un team nella barra di ricerca.

1. Seleziona il team Kanban da gestire.
1. Fai clic su **[!UICONTROL Altro]** menu ![](assets/more-menu.png), quindi seleziona **[!UICONTROL Modifica]**.

   ![Modifica team](assets/edit-team-settings-350x205.png)

1. Seleziona **[!UICONTROL Aggiungi automaticamente la storia successiva dal backlog]** per configurare l&#39;aggiunta automatica dell&#39;elemento successivo dal backlog al **[!UICONTROL Nuovo]** quando un elemento viene spostato fuori dal **[!UICONTROL In corso]** colonna.

   Gli utenti devono abilitare **Mostra backlog** impostazione su [!UICONTROL Kanban] affinché questa funzionalità diventi effettiva. Quando gli utenti abilitano [!UICONTROL Mostra backlog] impostazione su [!UICONTROL Kanban Board], si verifica la seguente funzionalità:

   Ogni volta che una storia viene spostata da [!UICONTROL In corso] colonna in una colonna sullo storyboard che rappresenta un [!UICONTROL Completa] stato (o uno stato che equivale a [!UICONTROL Completa]), un brano della colonna Backlog si sposta automaticamente nel [!UICONTROL Nuovo] colonna del [!UICONTROL Kanban Board].
Quando viene aggiunta dal backlog, la storia con la priorità più alta viene aggiunta alla bacheca delle storie.

1. Clic **[!UICONTROL Salva modifiche]**.

## Configurare la durata delle schede [!UICONTROL Kanban] scheda

Puoi scegliere per quanto tempo le schede completate rimangono sul [!UICONTROL Kanban] bacheca Attività che non rientrano nel [!UICONTROL Kanban] è ancora possibile accedere alla bacheca nel loro progetto originale.

{{step1-to-team}}

1. (Facoltativo) Fai clic su **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi selezionare un nuovo team Kanban dal menu a discesa o cercare un team nella barra di ricerca.
1. Seleziona il team Kanban.
1. Fai clic su **[!UICONTROL Altro]** menu ![](assets/more-menu.png) , quindi seleziona **[!UICONTROL Modifica]**.

   ![Modifica team](assets/edit-team-settings-350x205.png)

1. In **[!UICONTROL Numero di giorni in cui le schede completate rimangono sulla bacheca Kanban]** , selezionare un valore.

   Puoi scegliere un numero da 1 a 30 giorni.
1. Clic **[!UICONTROL Salva modifiche]**.
