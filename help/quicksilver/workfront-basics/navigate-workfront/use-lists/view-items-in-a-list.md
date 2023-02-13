---
navigation-topic: use-lists
title: Guida introduttiva agli elenchi in [!DNL Adobe Workfront]
description: È possibile visualizzare gli elenchi degli oggetti in [!DNL Adobe Workfront] per ottenere informazioni su di essi, ad esempio le date di inizio e di scadenza, gli utenti assegnati e altri oggetti associati ad essi.
feature: Get Started with Workfront
author: Lisa
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '2370'
ht-degree: 0%

---

# Guida introduttiva agli elenchi in [!DNL Adobe Workfront]

<!--
{{highlighted-preview}}
-->

È possibile visualizzare gli elenchi degli oggetti in [!DNL Adobe Workfront] per ottenere informazioni su di essi, ad esempio le date di inizio e di scadenza, gli utenti assegnati e altri oggetti associati ad essi.

Di seguito sono riportate alcune caratteristiche degli elenchi in [!DNL Workfront]:

* Elenca l&#39;aggiornamento automatico ogni cinque minuti per aggiornare le informazioni che altri utenti del sistema stanno aggiornando altrove.
* Alcune aree in [!DNL Workfront] sono preconfigurati con elenchi di oggetti predefiniti.

   È possibile personalizzare la maggior parte di questi elenchi preconfigurati.

* A [!DNL Workfront] l’amministratore può creare elenchi personalizzati da applicare a varie aree di [!DNL Workfront].

   Per ulteriori informazioni sulla creazione di elenchi a livello di sistema, consulta l’articolo [Creare, modificare e condividere filtri, viste e raggruppamenti predefiniti](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Request] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Visualizzazione o accesso successivo a filtri, viste, raggruppamenti</p> <P>Per gli elementi nell'area [!UICONTROL Setup], è necessario l'accesso amministrativo per l'elemento o per il livello di accesso [!UICONTROL System Administrator].</P> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso.<br>Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Visualizzazione [!UICONTROL] o autorizzazioni successive con accesso alla condivisione</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td>
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Elenchi di oggetti

Di seguito sono riportati alcuni tipi di elenchi di oggetti che è possibile trovare in [!DNL Workfront] e alcune delle aree in cui vengono visualizzate per impostazione predefinita quando si dispone dei diritti per visualizzare un oggetto.

>[!NOTE]
>
>* Questo elenco non è completo. Ognuno di questi elenchi di oggetti può essere visualizzato anche in un report o in un dashboard. Ad esempio, un rapporto Progetto o una dashboard contenente un rapporto Progetto visualizza anche un elenco di progetti.
>* In questo elenco, &quot;select&quot; significa che è necessario fare clic sul nome dell’elemento, non sulla casella di controllo a sinistra del nome.



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] elenco</strong></th> 
   <th><strong>Posizione dell’elenco di oggetti</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Elenco dei portafogli</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfoli]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco dei programmi</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfoli] &gt;[!UICONTROL seleziona un portfolio] &gt;[!UICONTROL Programmi]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL Programmi]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco dei progetti</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]</p> </li> 
     <li> <p>[!UICONTROL Portfoli] &gt;[!UICONTROL seleziona un portfolio] &gt;[!UICONTROL Projects]</p> </li> 
     <li> <p>[!UICONTROL Portfoli] &gt;[!UICONTROL seleziona un portfolio] &gt;[!UICONTROL Programmi] &gt;[!UICONTROL seleziona un programma] &gt;[!UICONTROL Progetti]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco delle attività</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleziona un progetto] &gt; [!UICONTROL Tasks] (Attività)</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt;[!UICONTROL SubTasks] (Selezionare un’attività) &gt;[!UICONTROL Subtask]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Predecessori*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco dei problemi</td> 
   <td> 
    <ul> 
     <li> <p>Progetti &gt; [!UICONTROL seleziona] un progetto &gt;[!UICONTROL Problemi]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Issues]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleziona un progetto] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL seleziona un’attività] &gt;[!UICONTROL SubTasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Issues]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco dei rapporti</td> 
   <td> 
    <ul> 
     <li> <p>  Rapporti di [!UICONTROL]  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco delle dashboard</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Dashboards]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco di iterazioni</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Team] &gt; [!UICONTROL Iterazioni]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco degli utenti</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Users]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco dei documenti</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Portfoli] &gt;[!UICONTROL seleziona un portfolio] &gt; [!UICONTROL Documenti]</p> </li> 
     <li> <p>[!UICONTROL Portfoli] &gt; [!UICONTROL seleziona un portfolio] &gt;[!UICONTROL Programmi] &gt;[!UICONTROL seleziona un programma] &gt;[!UICONTROL Documenti]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleziona un progetto] &gt;[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Documents]</p> </li> 
     <li> <p>Progetti &gt; [!UICONTROL seleziona] un progetto &gt; [!UICONTROL Problemi] &gt;[!UICONTROL seleziona un problema] &gt; [!UICONTROL Documenti]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco dei fogli presenze</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Scheda attività] &gt; [!UICONTROL Tutti i fogli presenze]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco delle tariffe di fatturazione</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleziona un progetto] &gt;[!UICONTROL Billing Rates*] (Percentuali di fatturazione)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco dei record di fatturazione</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL seleziona un progetto] &gt; [!UICONTROL Billing Records]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco dei rischi</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleziona un progetto] &gt;[!UICONTROL Risks]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco delle spese</td> 
   <td> 
    <ul> 
     <li> <p>Progetti &gt;[!UICONTROL seleziona] un progetto &gt;[!UICONTROL Spese]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt;[!UICONTROL Expenses]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco delle ore</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleziona] un progetto</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL seleziona un progetto] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL seleziona un'attività] &gt;[!UICONTROL Hours]</p> </li> 
     <li> <p>Progetti &gt;[!UICONTROL seleziona] un progetto &gt;[!UICONTROL Problemi] &gt;[!UICONTROL seleziona] un problema &gt;[!UICONTROL Ore]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td class="preview">Elenco dei moduli personalizzati</td> 
   <td> 
    <ul> 
     <li class="preview"> <p>[!UICONTROL Setup] &gt;[!UICONTROL Custom Forms]</p>
     <!--Remove the following note box when this goes to Production. Or do this when the Preview highlighting becomes available.-->
     <p><b>NOTA</b>: Attualmente disponibile solo nell’ambiente Anteprima</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>Elenco dei gruppi o sottogruppi</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups]</p> </li>
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups] &gt;[!UICONTROL seleziona il gruppo padre] &gt;[!UICONTROL Subgroups] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco dei team</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Teams]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Elenco delle società</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Companies]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Elenco dei programmi</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Schedules]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Elenco di modelli di layout</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Layout Templates]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

Non è possibile personalizzare l’elenco nell’area specificata. A [!DNL Workfront] l&#39;amministratore può creare un elenco personalizzato a livello di sistema oppure è possibile creare un report per questo oggetto se il livello di accesso consente di accedere alle funzioni di modifica dei report.

## Elementi elenco

Un elenco contiene alcuni elementi che ne definiscono il formato e le informazioni visualizzate. È possibile trovare diversi elementi dell’elenco di sistema disponibili per impostazione predefinita. Puoi anche creare elementi personalizzati per soddisfare le tue esigenze.

>[!NOTE]
>
>Quando si seleziona un nuovo filtro, visualizzazione o raggruppamento da un elenco, tale selezione viene mantenuta anche se si disconnette da [!DNL Workfront] o chiudi il browser.

Di seguito sono riportati gli elementi di un elenco:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Elemento</strong></th> 
   <th><strong>Spiegazione</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Filter]</strong></td> 
   <td> <p>I filtri tengono informazioni superflue da un elenco, in base ai criteri specificati. </p> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Panoramica dei filtri in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL View]</strong></td> 
   <td> <p>Le visualizzazioni definiscono i campi (colonne) visualizzati sullo schermo.</p> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Panoramica delle visualizzazioni in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Grouping]</strong></td> 
   <td> <p>I raggruppamenti separano gli oggetti dell’elenco in aree in base ai criteri specificati.</p> <p>Ad esempio, i problemi contenuti in un elenco possono essere visualizzati nelle sezioni in base allo stato o alla priorità.</p> <p>Potete avere fino a tre livelli di raggruppamenti in un raggruppamento standard e aggiungere un quarto livello se configurate un raggruppamento in modalità testo.</p> <p>Per ulteriori informazioni sui raggruppamenti, vedi <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Panoramica sui raggruppamenti in [!DNL Adobe Workfront]</a>.</p> <p>Per ulteriori informazioni sulla modalità testo, consulta <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Panoramica della modalità testo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per impostazione predefinita, questi elementi vengono visualizzati nella parte superiore di ogni elenco. Sono permanenti e non si spostano quando si scorre l’elenco. Passa il puntatore del mouse sull&#39;icona di ciascun elemento per identificarli.

![](assets/nwe-list-elements.png)

Puoi personalizzare gli elementi dell’elenco nelle aree seguenti e condividerli con altri utenti:

* Qualsiasi elenco predefinito di sistema trovato nella sezione [Guida introduttiva agli elenchi in [!DNL Adobe Workfront]](#default-workfront-lists) nel presente articolo
* Qualsiasi rapporto condiviso con te

Gli elementi costitutivi degli elenchi sono gli stessi degli elementi costitutivi dei rapporti.

Per ulteriori informazioni sulla creazione e la personalizzazione degli elementi costitutivi di elenchi e rapporti, consulta [Elementi di reporting: filtri, visualizzazioni e raggruppamenti](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Elencare azioni

È possibile completare le seguenti azioni in un elenco:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Azione</strong></th> 
   <th><strong>Informazione</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Modifica in linea</strong> </td> 
   <td> <p>Modificare gli oggetti e le relative informazioni direttamente nell’elenco.</p> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">Elementi di modifica in linea in un elenco in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>Aggiornamento con [!UICONTROL Summary]</strong> </td> 
   <td> <p>Aggiorna attività e problemi a livello di progetto utilizzando il pannello [!UICONTROL Summary] .</p> <p>Suggerimento: Il Riepilogo non è disponibile per tutti gli oggetti e non è disponibile nei rapporti Attività o Problema.</p> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Panoramica di riepilogo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Personalizzare la visualizzazione degli elenchi</strong> </td> 
   <td> <p>Personalizza l’aspetto di un elenco, la disposizione delle colonne, l’ordine di ordinamento degli elementi o il numero di elementi visualizzati.</p> <p>Nota: Le modifiche apportate al numero di elementi da visualizzare su una pagina vengono ripristinate al momento della disconnessione [!DNL Workfront] o chiudi il browser. Le modifiche potrebbero anche essere ripristinate dopo un periodo di 8 ore.</p> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">Modificare la visualizzazione di un elenco</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Filtro rapido</strong> </td> 
   <td> <p>Applica un filtro rapido per trovare solo gli elementi importanti per te in modo da poterli rivedere, aggiornare o condividere rapidamente con altri.</p> <p>Importante: È possibile trovare gli elementi che contengono una parola di ricerca utilizzando il filtro rapido, sia che l'elemento sia visibile sullo schermo o che venga visualizzato dopo lo scorrimento verso il fondo della pagina. Quando utilizzi le funzionalità di ricerca del browser, puoi trovare solo gli elementi già visibili sullo schermo. Se l’elenco include più pagine, i filtri rapidi individuano solo gli elementi nella pagina corrente.</p> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Applicare il filtro rapido a un elenco</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Esporta</strong> </td> 
   <td> <p>Esportare un elenco di oggetti da [!DNL Workfront]. Quando un elenco contiene più di 2000 elementi, esportare l’elenco è l’unico modo per esaminare tutti gli elementi in una pagina.</p> <p>Per ulteriori informazioni sull’esportazione di un elenco, consulta <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Esportare un elenco</a>. Per ulteriori informazioni sui formati e i limiti di esportazione, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Esportare i dati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Barra degli strumenti dell’elenco

La tabella seguente elenca molte delle icone disponibili nella barra degli strumenti e indica cosa accade quando fai clic su di esse:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Icona</strong></td> 
   <td><strong>Descrizione</strong></td> 
   <td><strong>Al clic</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/add-icon-plus-in-circle.png"> </td> 
   <td>[!UICONTROL Aggiungi elemento o utente]</td> 
   <td>Apri altre opzioni, tra cui l’aggiunta di un nuovo elemento o utente.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Inserisci attività sopra]</td> 
   <td> <p>Inserire un'attività sopra l'attività selezionata.</p> <p>Questa opzione è disponibile solo per le attività. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Inserisci attività di seguito]</td> 
   <td> <p>Inserire un'attività sotto l'attività selezionata.</p> <p>Questa opzione è disponibile solo per le attività. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL Edit]</td> 
   <td>Modifica l’elemento selezionato.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/copy-icon.png"> </td> 
   <td>[!UICONTROL Copy]</td> 
   <td>Copia l'elemento selezionato.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/delete.png"> </td> 
   <td>[!UICONTROL Elimina]</td> 
   <td>Elimina l'elemento selezionato.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-add-to-iteration-icon-in-new-toolbar-for-issues.png"> </td> 
   <td>[!UICONTROL Aggiungi a]</td> 
   <td> <p>Apri la finestra di dialogo per aggiungere il problema selezionato a un'iterazione.</p> <p>Questa funzione è disponibile solo per i problemi.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[!UICONTROL Share]</td> 
   <td>Condividi l'elemento selezionato.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Attività rientro e rientro] </td> 
   <td> <p>Consente di rientro o rientro dell'attività selezionata. </p> <p>Questa opzione è disponibile solo per le attività. </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL Altro]</td> 
   <td>Apri altre opzioni per l’elemento selezionato.</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL Filtro rapido] </p> </td> 
   <td> <p>Apri la casella di ricerca del filtro rapido per individuare gli elementi nell’elenco visualizzato.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL Export]</td> 
   <td>Esporta l’elenco in file PDF, Excel o delimitati da tabulazioni.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Agile View]</td> 
   <td>Visualizza l’elenco nella vista Agile.<br>Questa opzione è disponibile solo per le attività.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>Diagramma di Gantt [!UICONTROL]</td> 
   <td> <p>Visualizza l'elenco nella visualizzazione Diagramma di Gantt.</p> <p>Questa opzione è disponibile solo per progetti e attività.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>Menu a discesa [!UICONTROL Filter]</td> 
   <td> <p>Visualizza un elenco di filtri e opzioni aggiuntive per la gestione dei filtri, inclusa la creazione di uno. </p> <p>In una schermata piccola, il nome del filtro viene sostituito dall’icona del filtro. Un punto blu viene visualizzato sull’icona Filtro quando si applica un filtro diverso da "[!UICONTROL All]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menu a discesa [!UICONTROL View]</td> 
   <td> <p>Visualizza un elenco di viste e opzioni aggiuntive per gestire le viste, inclusa la creazione di una. </p> <p>In una schermata piccola, il nome della visualizzazione viene sostituito dall’icona [!UICONTROL view]. Un punto blu viene visualizzato sull’icona [!UICONTROL View] quando si applica una visualizzazione diversa da "[!UICONTROL Standard]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menu a discesa Raggruppamento</td> 
   <td> <p>Visualizza un elenco di raggruppamenti e opzioni aggiuntive per la gestione dei raggruppamenti, inclusa la creazione di uno. </p> <p>In una schermata piccola, il nome del raggruppamento viene sostituito dall’icona di raggruppamento (!UICONTROL raggruppamento). Un punto blu viene visualizzato sull’icona [!UICONTROL Grouping] quando si applica un raggruppamento diverso da "[!UICONTROL Nothing]".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL Modalità piano]</p> </td> 
   <td> <p>Scegliere se salvare automaticamente o manualmente le modifiche apportate in un elenco di attività. </p> <p>Per informazioni sulla modifica delle attività in un elenco, consulta <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Modificare le attività in un elenco</a>. </p> <p>Questa opzione è disponibile solo per le attività.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL Riepilogo]</td> 
   <td> <p>Visualizza o nasconde la casella [!UICONTROL Summary] per l’elemento selezionato.</p> <p>Questa funzione è disponibile solo per attività e problemi.</p> <p>Per informazioni sul pannello [!UICONTROL Summary] nel nuovo [!DNL Adobe Workfront] esperienza, vedi <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Panoramica di riepilogo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Rimuovi]</td> 
   <td>Rimuovi qualcosa dall'elenco. Ad esempio, in qualità di amministratore del gruppo che gestisce le appartenenze a un gruppo o a un sottogruppo, rimuovere un membro del gruppo come spiegato in <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">Visualizzare e gestire le appartenenze a un gruppo</a>.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL Commento] /[!UICONTROL Aggiorna]</td> 
   <td> <p>Digita un commento o un aggiornamento.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Differenza tra elenchi e rapporti

Gli elenchi e i rapporti sono griglie che contengono informazioni su un tipo di oggetto.

La tabella seguente illustra le somiglianze e le differenze tra elenchi e rapporti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Funzionalità</strong> </th> 
   <th><strong>Lista</strong> </th> 
   <th><strong>Rapporto</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Chiunque può crearle</p> </td> 
   <td><span>✓*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Solo un [!DNL Workfront] gli amministratori e gli utenti con una licenza [!UICONTROL Plan] possono crearli</p> </td> 
   <td> </td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td> <p>Un set predefinito è disponibile da [!DNL Workfront]</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Personalizzabile in modalità standard</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Personalizzabile in modalità testo</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puoi condividerli con altri utenti</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puoi condividerle a livello di sistema</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Puoi condividerle al di fuori del sistema</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>È possibile esportare in formato .pdf, [!DNL Excel], e formati delimitati da tabulazioni</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Puoi pianificarle per la consegna in un’e-mail</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>È possibile aggiungere a un modello di layout</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Puoi aggiungerli a sezioni personalizzate </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puoi aggiungerli a un dashboard</p> </td> 
   <td> ✓*** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>È possibile utilizzare i prompt per personalizzare la visualizzazione</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>È possibile visualizzarli in un grafico</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>È possibile inserire in linea gli oggetti di modifica</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Per poterli creare, devi disporre dell’accesso a filtri, visualizzazioni e raggruppamenti. Per ulteriori informazioni, consulta [Consentire l’accesso a filtri, visualizzazioni e raggruppamenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

Per poterli creare, devi disporre dell’accesso a filtri, visualizzazioni e raggruppamenti, nonché a rapporti, dashboard e calendari. Per ulteriori informazioni, consulta [Consentire l’accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

È possibile personalizzare gli elenchi per i rapporti posizionati su un dashboard solo se l’autore del rapporto ha configurato gli elementi elenco in modo che siano visibili sul dashboard.

>[!NOTE]
>
>Non è possibile aggiungere un elenco a un dashboard senza creare un rapporto e aggiungerlo prima al dashboard.

Per ulteriori informazioni sulla creazione di un rapporto, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Per informazioni sulla creazione di sezioni personalizzate , consulta [Creare schede o sezioni personalizzate](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## Differenza tra gli elenchi aggiornati e quelli legacy

Esistono due tipi di elenchi in [!DNL Workfront]:

* Elenchi legacy

   ![](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* Elenchi aggiornati

   ![](assets/updated-list-screen-shot-gray-groupings-350x71.png)

Entrambi i tipi di elenchi vengono visualizzati nella [!DNL Adobe Workfront].

Tutti gli elenchi e i rapporti nel [!DNL Adobe Workfront] sono elenchi aggiornati, ad eccezione dei seguenti elementi:

* Elenchi nel [!UICONTROL Configurazione] area
* Elenchi nel [!UICONTROL Rapporti] area

La tabella seguente mostra alcune delle differenze tra gli elenchi legacy e aggiornati in [!DNL Workfront]:

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> [Legacy does not equal Classic. Legacy lists appear in NWE and Classic. Updated lists appear in NWE and Classic.]</span>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Elenchi legacy</b></td> 
   <td><b>Elenchi aggiornati</b></td> 
  </tr> 
  <tr> 
   <td> <p>Font legacy, intestazioni di colonna, schema di colori di raggruppamento blu</p> </td> 
   <td> <p>Font aggiornati, intestazioni di colonna, schema di colori di raggruppamento dei grigi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Editing in linea più lento</p> </td> 
   <td> <p>Editing in linea più rapido</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visualizzazione <strong>100</strong> elementi per impostazione predefinita</p> </td> 
   <td> <p>Visualizzazione <strong>Tutto</strong> o fino a <strong>2000</strong> elementi per impostazione predefinita</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilizzare CTRL+F per trovare elementi in un elenco</p> </td> 
   <td> <p>Utilizza i filtri rapidi per trovare rapidamente le informazioni in un elenco di grandi dimensioni</p> <p>Per informazioni sull’utilizzo dei filtri rapidi negli elenchi, consulta <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Applicare il filtro rapido a un elenco</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Non è possibile modificare in linea campi personalizzati con formattazione RTF.</td> 
   <td> <p>Il testo nei campi personalizzati con formattazione può essere configurato in modo da consentire l’uso di grassetto, corsivo, sottolineato, punti elenco, numerazione, collegamenti ipertestuali e virgolette di blocco.</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>La formattazione condizionale può modificare il colore del testo dei collegamenti in un elenco</td> 
   <td>Impossibile applicare modifiche al colore del testo ai collegamenti in un elenco</td> 
  </tr> 
 </tbody> 
</table>
