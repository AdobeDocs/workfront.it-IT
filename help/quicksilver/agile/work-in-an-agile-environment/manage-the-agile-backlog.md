---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: Gestire il backlog agile
description: Le attività e i problemi possono essere assegnati a un team agile e aggiunti al backlog del team come storie, a seconda della metodologia agile utilizzata dal team.
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: b855f032b24079ff27435fb833cd3ed8a382a77c
workflow-type: tm+mt
source-wordcount: '1376'
ht-degree: 0%

---

# Gestire il backlog agile

I seguenti elementi di lavoro possono essere assegnati a un team agile e aggiunti al backlog del team come storie, a seconda della metodologia agile utilizzata dal team:

* **[!UICONTROL Squadre agile di scrum]:** Le attività e i problemi possono essere assegnati al team agile e aggiunti al backlog.
* **[!UICONTROL Squadre mobili kanban]:** Le attività possono essere assegnate al team agile e aggiunte al backlog. Gli utenti possono visualizzare il backlog direttamente dalla bacheca di storie agili, come descritto in [[!UICONTROL Aggiungi il backlog] alla scheda Kanban](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). Il team utilizza questo backlog per assegnare priorità e gestire la coda di lavoro.

Le attività o i problemi possono essere assegnati al team (e successivamente aggiunti al backlog del team) da qualsiasi punto [!DNL Adobe Workfront]. Ad esempio, a un singolo team possono essere assegnate assegnazioni di lavoro da più progetti.

>[!NOTE]
>
>Se aggiungi più team a un elemento di backlog, l&#39;attività o il problema viene visualizzato solo nel backlog del team principale. Il team principale è il primo assegnato al team.

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
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superiore</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso a [!UICONTROL Gestire] il progetto su cui si trova la storia</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Creare e gestire le storie nel backlog

* [Riordina le storie](#reorder-stories)
* [[!UICONTROL Interruzione] storie in giù](#break-down-stories)
* [Modificare i brani](#edit-stories)
* [Crea nuove storie sul backlog](#create-new-stories-on-the-backlog)
* [Spostare le storie dal backlog a un&#39;iterazione o a una bacheca Kanban](#move-stories-from-the-backlog-to-an-iteration-or-kanban-board)

### Riordina le storie {#reorder-stories}

È possibile riordinare le storie nell’elenco dei backlog utilizzando il metodo di trascinamento della selezione.

1. Vai al backlog agile dove vuoi riordinare le storie.
1. In **[!UICONTROL Visualizza]** menu a discesa, seleziona il **[!UICONTROL Backlog]** visualizzazione o visualizzazione personalizzata che contiene **[!UICONTROL Ordine]** colonna.

   >[!NOTE]
   >
   >Se a un&#39;attività o a un problema è assegnato un team agile e il progetto non è in uno stato che corrisponde a Corrente, non viene visualizzato nel backlog. Tuttavia, influiscono comunque sul conteggio del backlog nella colonna Ordine.

1. Seleziona uno o più brani, quindi trascina i brani nell&#39;ordine in cui vuoi che vengano visualizzati nel backlog.\
   ![Trascinamento di elementi backlog](assets/agile-backlog-drag-and-drop.png)

### Rompere storie {#break-down-stories}

Poiché le storie in un backlog variano a seconda delle dimensioni, gli utenti possono suddividerle in dimensioni utilizzabili per un&#39;iterazione. Se si suddivide un brano, vengono create sottoattività dell&#39;attività rappresentata dal brano e viene sostituita l&#39;attività originale nel backlog. È possibile assegnare un&#39;attività padre o le relative sottoattività a un team agile, ma non è possibile assegnarle contemporaneamente a un team.

>[!NOTE]
>
>Considera le seguenti limitazioni durante la suddivisione di storie:
>
>* È possibile suddividere solo le storie che rappresentano attività. Non è possibile scomporre storie che rappresentano problemi.
>* Le storie possono essere suddivise solo se associate a un progetto.



Per scomporre una storia:

1. Vai al backlog che contiene la storia che vuoi scomporre.
1. Selezionate la storia da scomporre, quindi fate clic su **[!UICONTROL Storia di raggruppamento]**.\
   La [!UICONTROL Storia di raggruppamento] viene visualizzata la finestra di dialogo.\
   ![Finestra di dialogo Storia di suddivisione](assets/backlog-breakdown-dialog.png)

1. Specifica un nome e una stima per il brano, quindi seleziona se il brano è pronto.
1. Fai clic su **[!UICONTROL Aggiungi storia]** per creare un&#39;altra storia dalla storia originale.
1. Fai clic su **[!UICONTROL Salva]**.

### Modificare i brani {#edit-stories}

È possibile modificare i brani direttamente dal [!UICONTROL Storie] o [!UICONTROL Problemi] le schede nel backlog consentono di modificare in blocco tutte le attività o i problemi di un progetto, come descritto in [Modifica in blocco le attività](../../manage-work/tasks/manage-tasks/edit-tasks.md#editing-tasks-in-bulk) in [Modifica delle attività](../../manage-work/tasks/manage-tasks/edit-tasks.md) e [Modifica dei problemi](../../manage-work/issues/manage-issues/edit-issues.md#bulk-editing-issues) in [Modifica dei problemi](../../manage-work/issues/manage-issues/edit-issues.md).

## Crea nuove storie sul backlog {#create-new-stories-on-the-backlog}

Puoi creare nuove storie sul backlog creando la storia direttamente dal backlog o assegnando un&#39;attività o un problema esistente a un team agile.

* [Crea una storia dal backlog](#create-a-story-from-the-backlog)
* [Assegnare un&#39;attività o un problema a un team agile](#assign-a-task-or-issue-to-an-agile-team)

### Crea una storia dal backlog {#create-a-story-from-the-backlog}

Quando crei una storia dal backlog, questa viene creata come un&#39;attività o un problema all&#39;interno di un progetto. Non è possibile creare una storia dal backlog come problema.

Per creare una storia dal backlog:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona **[!UICONTROL Backlog]** dal pannello a sinistra.
1. Effettua una delle seguenti operazioni, a seconda che desideri creare un&#39;attività o un problema:

   * **Per creare un&#39;attività:** Fai clic su **[!UICONTROL Storie]**.

   * **Per creare un problema:** Fai clic su **[!UICONTROL Problemi]**.

1. Fai clic su **[!UICONTROL Nuova storia]** o **[!UICONTROL Nuovo problema]**.

1. Specifica le seguenti informazioni:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nome Story]</strong></td>
      <td> Digitate un nome per la storia.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Descrizione]</strong></td>
      <td>(Facoltativo) Immetti una descrizione della storia.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td> Seleziona se il brano è pronto per essere aggiunto a un'iterazione. Questa impostazione è solo informativo. Le storie possono essere aggiunte a un'iterazione indipendentemente dallo stato di questa impostazione.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>Specifica un punto o una stima oraria per la storia. Le stime influiscono sul grafico a discesa. Il grafico a discesa per un'iterazione è accurato solo se ogni storia contiene una stima accurata. Se fornisci una stima dei punti, devi aver già indicato nelle impostazioni del team quante ore rappresenta ogni punto.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Progetto padre]</strong></td>
      <td>Inizia a digitare il nome del progetto in cui verrà creato il brano, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.<br>Lo stato del progetto deve essere impostato su [!UICONTROL Current]. Se lo stato del progetto è diverso da [!UICONTROL Current], non viene visualizzato nel menu a discesa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Attività padre]</strong></td>
      <td>(Facoltativo) Inizia a digitare il nome dell'attività principale a cui il brano è subordinato, quindi fai clic sul nome quando viene visualizzato nell'elenco a discesa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td> (Facoltativo) Seleziona i moduli personalizzati da aggiungere a questa storia.</td>
     </tr>
    </tbody>
   </table>

1. Fai clic su **[!UICONTROL Salva storia]**.

### Assegnare un&#39;attività o un problema a un team agile {#assign-a-task-or-issue-to-an-agile-team}

Puoi assegnare un’attività o un problema a un team agile. Dopo l&#39;assegnazione, l&#39;attività o il problema viene visualizzato come una nuova storia nel backlog del team.

Per assegnare un&#39;attività o un problema a un team agile:

1. Passare al Progetto contenente l&#39;attività che si desidera riassegnare.
1. Seleziona l’attività o il problema nell’elenco.
1. Fai clic su **[!UICONTROL Modifica]**.
1. Fai clic su **[!UICONTROL Assegnazioni]**.
1. (Facoltativo) Elimina tutti gli assegnatari esistenti.
1. Fai clic su **[!UICONTROL Aggiungi assegnatario]**.
1. Inizia a digitare il nome del team agile che desideri assegnare all’attività o al problema, quindi fai clic sul nome del team quando viene visualizzato nell’elenco a discesa.
1. Fai clic su **[!UICONTROL Salva modifiche]**.\
   L&#39;attività o il problema è ora disponibile nel backlog del team.

## Spostare le storie dal backlog a un&#39;iterazione o a una bacheca + {#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [Spostare le storie esistenti nel backlog](#move-existing-stories-to-the-backlog)
* [Esportare storie dal backlog](#export-stories-from-the-backlog)

1. Vai al backlog del team agile.
1. Selezionate i brani da spostare in un&#39;iterazione o in una bacheca Kanban, quindi fate clic su **[!UICONTROL Altro]** > **[!UICONTROL Sposta a]**.\
   Se la storia viene spostata in un [!UICONTROL Kanban] la commissione [!UICONTROL Sposta la storia al Kanban] Viene visualizzata la bacheca.\
   Se si sposta la storia in un&#39;iterazione, la [!UICONTROL Sposta la storia a un&#39;iterazione] viene visualizzata la finestra di dialogo.\
   ![Finestra di dialogo Sposta storia](assets/agile-backlog-addtoiteration.png)

1. Effettua una delle seguenti operazioni:

   * **Per i team Scrum:** In **[!UICONTROL Seleziona iterazione]** selezionare l&#39;iterazione in cui si desidera spostare i brani.

   * **Per i team Kanban:** In **[!UICONTROL Seleziona bacheca kanban]** selezionare il team [!UICONTROL Kanban] consiglio di amministrazione. (I team Kanban possono avere un solo [!UICONTROL Kanban] scheda).

1. Fai clic su **[!UICONTROL Sposta storia]**.

### Spostare le storie esistenti nel backlog {#move-existing-stories-to-the-backlog}

Se decidi che il tuo team non è ancora pronto per lavorare su una storia, puoi spostare la storia nel backlog.

Per ulteriori informazioni, consulta [Spostare una storia agile](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Esportare storie dal backlog {#export-stories-from-the-backlog}

Puoi esportare uno o più brani (comprese attività e problemi) direttamente dal backlog.

Puoi esportare storie dal backlog nello stesso modo in cui esporti altri dati in [!DNL Workfront], come descritto in [Esportare i dati](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
