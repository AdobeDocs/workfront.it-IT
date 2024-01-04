---
navigation-topic: use-lists
title: Introduzione agli elenchi in [!DNL Adobe Workfront]
description: È possibile visualizzare elenchi di oggetti in [!DNL Adobe Workfront] per ottenere informazioni su di essi, ad esempio le date di inizio e di scadenza, gli utenti assegnati e altri oggetti associati.
feature: Get Started with Workfront
author: Lisa
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '2397'
ht-degree: 0%

---

# Introduzione agli elenchi in [!DNL Adobe Workfront]

<!--
{{highlighted-preview}}
-->

È possibile visualizzare elenchi di oggetti in [!DNL Adobe Workfront] per ottenere informazioni su di essi, ad esempio le date di inizio e di scadenza, gli utenti assegnati e altri oggetti associati.

Di seguito sono riportate alcune caratteristiche degli elenchi in [!DNL Workfront]:

* Gli elenchi vengono aggiornati automaticamente ogni cinque minuti per aggiornare le informazioni che altri utenti del sistema stanno aggiornando altrove.
* Alcune aree in [!DNL Workfront] sono preconfigurate con elenchi predefiniti di oggetti.

  Puoi personalizzare la maggior parte di questi elenchi preconfigurati.

* A [!DNL Workfront] l&#39;amministratore può creare elenchi personalizzati da applicare a varie aree di [!DNL Workfront].

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
   <td> <p>[!UICONTROL Request] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL View] o versione successiva per l'accesso a filtri, viste, raggruppamenti</p> <P>Per gli elementi nell'area [!UICONTROL Setup] è necessario l'accesso amministrativo per l'elemento o il livello di accesso [!UICONTROL System Administrator].</P> <p>Nota: se non disponi ancora dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso.<br>Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>[!UICONTROL View] o versione successiva con accesso alla condivisione</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td>
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Elenchi di oggetti

Di seguito sono riportati alcuni tipi di elenchi di oggetti disponibili in [!DNL Workfront] e alcune delle aree in cui vengono visualizzate per impostazione predefinita quando si dispone dei diritti per visualizzare un oggetto.

>[!NOTE]
>
>* Questo elenco non è completo. Ciascuno di questi elenchi di oggetti può essere visualizzato anche in un report o in un dashboard. Ad esempio, un report di progetto o un dashboard contenente un report di progetto visualizza anche un elenco di progetti.
>* In questo elenco, &quot;seleziona&quot; significa che devi fare clic sul nome dell’elemento, non sulla casella di controllo a sinistra del nome.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] list</strong></th> 
   <th><strong>Posizione dell'elenco di oggetti</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Elenco dei portfolio</td> 
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
     <li> <p>[!UICONTROL Progetti]</p> </li> 
     <li> <p>[!UICONTROL Portfoli] &gt;[!UICONTROL seleziona un portfolio] &gt;[!UICONTROL Progetti]</p> </li> 
     <li> <p>[!UICONTROL Portfoli] &gt;[!UICONTROL seleziona un portfolio] &gt;[!UICONTROL Programmi] &gt;[!UICONTROL seleziona un programma] &gt;[!UICONTROL Progetti]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco delle attività</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Progetti] &gt;[!UICONTROL seleziona un progetto] &gt; [!UICONTROL Attività]</p> </li> 
     <li> <p>[!UICONTROL Progetti] &gt;[!UICONTROL seleziona un progetto] &gt;[!UICONTROL Attività] &gt;[!UICONTROL seleziona un'attività] &gt;[!UICONTROL Sottoattività]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Predecessors*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco delle Issues</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL select] a project &gt;[!UICONTROL Issues]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Issues]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt;[!UICONTROL Subtasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Issues]</p> </li> 
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
     <li> <p>[!UICONTROL Teams] &gt; [!UICONTROL Iterations]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco degli utenti</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Utenti]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco dei documenti</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Documenti]</p> </li> 
     <li> <p>[!UICONTROL Portfoli] &gt;[!UICONTROL seleziona un portfolio] &gt; [!UICONTROL Documenti]</p> </li> 
     <li> <p>[!UICONTROL Portfoli] &gt; [!UICONTROL seleziona un portfolio] &gt;[!UICONTROL Programmi] &gt;[!UICONTROL seleziona un programma] &gt;[!UICONTROL Documenti]</p> </li> 
     <li> <p>[!UICONTROL Progetti] &gt;[!UICONTROL seleziona un progetto] &gt;[!UICONTROL Documenti]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt; [!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt; [!UICONTROL select] a project &gt; [!UICONTROL Issues] &gt;[!UICONTROL select an issue] &gt; [!UICONTROL Documents]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco delle schede orario</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL] s &gt; [!UICONTROL Tutte le schede orario]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco delle tariffe di fatturazione</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] (Seleziona un progetto) &gt;[!UICONTROL Billing Rates*] (Tariffe di fatturazione UICONTROL)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco dei record di fatturazione</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Progetti] &gt; [!UICONTROL seleziona un progetto] &gt; [!UICONTROL Record fatturazione]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco dei rischi</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Progetti] &gt;[!UICONTROL seleziona un progetto] &gt;[!UICONTROL Rischi]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco delle spese</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Progetti] &gt;[!UICONTROL seleziona] un progetto &gt;[!UICONTROL Spese]</p> </li> 
     <li> <p>[!UICONTROL Progetti] &gt; [!UICONTROL seleziona un progetto] &gt;[!UICONTROL Attività] &gt;[!UICONTROL seleziona un'attività] &gt;[!UICONTROL Spese]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Elenco delle ore</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Progetti] &gt;[!UICONTROL seleziona] un progetto</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select a project] &gt;[!UICONTROL Tasks] &gt;[!UICONTROL select a task] &gt;[!UICONTROL Hours] (Seleziona un'attività)</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL select] un progetto &gt;[!UICONTROL Issues] &gt;[!UICONTROL select] un problema &gt;[!UICONTROL Hours]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td class="preview">Elenco dei moduli personalizzati</td> 
   <td> 
    <ul> 
     <li class="preview"> <p>[!UICONTROL Setup] &gt;[!UICONTROL Custom Forms]</p>
     <!--Remove the following note box when this goes to Production. Or do this when the Preview highlighting becomes available.-->
     <p><b>NOTA</b>: attualmente disponibile solo nell’ambiente di anteprima</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>Elenco di gruppi o sottogruppi</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups]</p> </li>
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups] &gt;[!UICONTROL select the parent group] &gt;[!UICONTROL Subgroups] (Seleziona il gruppo padre) </li> 
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
   <td>Elenco delle pianificazioni</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Schedules]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Elenco dei modelli di layout</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Layout Templates]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

Non è possibile personalizzare l&#39;elenco nell&#39;area specificata. A [!DNL Workfront] l&#39;amministratore può creare un elenco personalizzato a livello di sistema oppure un report per questo oggetto se il livello di accesso ti consente di accedere alla modifica dei report.

## Elementi elenco

Un elenco contiene alcuni elementi che ne definiscono il formato e le informazioni visualizzate. Per impostazione predefinita, sono disponibili diversi elementi dell&#39;elenco di sistema. Puoi anche creare elementi personalizzati in base alle tue esigenze.

>[!NOTE]
>
>Quando selezioni un nuovo filtro, una nuova vista o un nuovo raggruppamento da un elenco, tale selezione viene mantenuta anche se esci da [!DNL Workfront] o chiudi il browser.

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
   <td><strong>[!UICONTROL Filtro]</strong></td> 
   <td> <p>I filtri escludono le informazioni non necessarie da un elenco, in base ai criteri specificati. </p> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Panoramica sui filtri</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Visualizzazione [!UICONTROL]</strong></td> 
   <td> <p>Le visualizzazioni definiscono quali campi (colonne) vengono visualizzati sullo schermo.</p> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Panoramica delle visualizzazioni in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Raggruppamento]</strong></td> 
   <td> <p>I raggruppamenti separano gli oggetti dell'elenco in aree in base ai criteri specificati.</p> <p>Ad esempio, i problemi di un elenco possono essere visualizzati in sezioni in base allo stato o alla priorità.</p> <p>È possibile avere fino a tre livelli di raggruppamenti in un raggruppamento standard e aggiungere un quarto livello se si sta configurando un raggruppamento in modalità testo.</p> <p>Per ulteriori informazioni sui raggruppamenti, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Panoramica sui raggruppamenti in [!DNL Adobe Workfront]</a>.</p> <p>Per ulteriori informazioni sulla modalità testo, consulta <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Panoramica sulla modalità testo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per impostazione predefinita, questi elementi vengono visualizzati nella parte superiore di ogni elenco. Sono permanenti e non si spostano mentre scorri l’elenco. Passa il puntatore del mouse sull&#39;icona di ogni elemento per identificarli.

![](assets/nwe-list-elements.png)

È possibile personalizzare gli elementi di un elenco nelle seguenti aree e condividerli con altri utenti:

* Qualsiasi elenco predefinito del sistema trovato nella sezione [Introduzione agli elenchi in [!DNL Adobe Workfront]](#default-workfront-lists) in questo articolo
* Qualsiasi rapporto condiviso con te

Gli elementi di costruzione per gli elenchi sono gli stessi elementi di costruzione per i rapporti.

Per ulteriori informazioni sulla creazione e la personalizzazione degli elementi di creazione di elenchi e rapporti, vedere [Elementi di reporting: filtri, viste e raggruppamenti](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Elencare azioni

È possibile completare le azioni seguenti in un elenco:

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
   <td> <p>Modificare gli oggetti e le relative informazioni direttamente nell'elenco.</p> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">Modifica in linea di elementi in un elenco in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>Aggiorna con il riepilogo [!UICONTROL]</strong> </td> 
   <td> <p>Aggiorna attività e problemi a livello di progetto utilizzando il pannello [!UICONTROL Summary].</p> <p>Suggerimento: il riepilogo non è disponibile per tutti gli oggetti e non è disponibile nei report Attività o Problemi.</p> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Panoramica di riepilogo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Personalizza visualizzazione elenco</strong> </td> 
   <td> <p>Personalizza l’aspetto di un elenco, la disposizione delle colonne, l’ordinamento degli elementi o il numero di elementi visualizzati.</p> <p>Nota: le modifiche apportate al numero di elementi da visualizzare in una pagina vengono ripristinate quando si esce da [!DNL Workfront] o chiudi il browser. Le modifiche possono anche essere ripristinate dopo un periodo di 8 ore.</p> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">Modificare la modalità di visualizzazione di un elenco</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Filtro rapido</strong> </td> 
   <td> <p>Applica un filtro rapido per trovare solo gli elementi che ti interessano in modo da poterli rivedere, aggiornare o condividere rapidamente con altri utenti.</p> <p>Importante: è possibile trovare gli elementi che contengono una parola di ricerca utilizzando il filtro rapido, sia che l'elemento sia visibile sullo schermo o che venga visualizzato dopo lo scorrimento verso il fondo della pagina. Utilizzando le funzionalità di ricerca del browser, è possibile trovare solo gli elementi già visibili sullo schermo. Se l'elenco contiene più pagine, i filtri rapidi individuano solo gli elementi della pagina corrente.</p> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Applicare il filtro rapido a un elenco</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Esporta</strong> </td> 
   <td> <p>Esporta un elenco di oggetti da [!DNL Workfront]. Se un elenco contiene più di 2.000 elementi, l'esportazione dell'elenco è l'unico modo per esaminare tutti gli elementi di una pagina.</p> <p>Per ulteriori informazioni sull'esportazione di un elenco, vedere <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Esportare un elenco</a>. Per ulteriori informazioni sui formati e i limiti di esportazione, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Esporta dati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Barra degli strumenti Elenco

Nella tabella seguente sono elencate molte delle icone disponibili nella barra degli strumenti e viene indicato cosa accade quando si fa clic su di esse:

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
   <td>Apri altre opzioni, incluso l’aggiunta di un nuovo elemento o utente.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Inserisci attività in alto]</td> 
   <td> <p>Consente di inserire un'attività sopra l'attività selezionata.</p> <p>Questa opzione è disponibile solo per le attività. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Inserisci attività di seguito]</td> 
   <td> <p>Inserisce un'attività sotto l'attività selezionata.</p> <p>Questa opzione è disponibile solo per le attività. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL Modifica]</td> 
   <td>Modifica l'elemento selezionato.</td> 
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
   <td> <p>Apri la finestra di dialogo per aggiungere il problema selezionato a un’iterazione.</p> <p>Questa opzione è disponibile solo per problemi.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[!UICONTROL Share]</td> 
   <td>Condividi l'elemento selezionato.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Rientra e rimuove rientro attività] </td> 
   <td> <p>Rientro o rientro negativo dell'attività selezionata. </p> <p>Questa opzione è disponibile solo per le attività. </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL Altro]</td> 
   <td>Apri altre opzioni per l’elemento selezionato.</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL Filtro rapido] </p> </td> 
   <td> <p>Aprire la casella di ricerca a filtro rapido per trovare gli elementi nell'elenco visualizzato.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL Export]</td> 
   <td>Esporta l’elenco in file PDF, Excel o delimitati da tabulazioni.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Visualizzazione Agile]</td> 
   <td>Visualizzare l'elenco nella visualizzazione Agile.<br>Questa opzione è disponibile solo per le attività.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>Grafico di Gantt [!UICONTROL]</td> 
   <td> <p>Visualizza l'elenco nella visualizzazione Diagramma di Gantt [!UICONTROL].</p> <p>Questa opzione è disponibile solo per i progetti e le attività.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>Menu a discesa [!UICONTROL Filter]</td> 
   <td> <p>Visualizza un elenco di filtri e opzioni aggiuntive per la gestione dei filtri, inclusa la creazione di un filtro. </p> <p>In una piccola schermata, il nome del filtro viene sostituito dall’icona del filtro. Quando applichi un filtro diverso da "[!UICONTROL All]", sull’icona Filtro viene visualizzato un punto blu.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menu a discesa [!UICONTROL View]</td> 
   <td> <p>Visualizzare un elenco di viste e opzioni aggiuntive per gestire le viste, inclusa la creazione di una vista. </p> <p>In una piccola schermata, il nome della visualizzazione viene sostituito dall'icona [!UICONTROL view]. Quando si applica una visualizzazione diversa da "[!UICONTROL Standard]", sull'icona [!UICONTROL View] viene visualizzato un punto blu.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Menu a discesa di [!UICONTROL Grouping]</td> 
   <td> <p>Visualizza un elenco di raggruppamenti e opzioni aggiuntive per gestirli, inclusa la creazione di un gruppo. </p> <p>In una piccola schermata, il nome del raggruppamento viene sostituito dall'icona [!UICONTROL grouping]. Quando si applica un raggruppamento diverso da "[!UICONTROL Nothing]", sull'icona [!UICONTROL Grouping] viene visualizzato un punto blu."</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL Modalità piano]</p> </td> 
   <td> <p>Scegliere se si desidera salvare le modifiche apportate in un elenco di attività automaticamente o manualmente. </p> <p>Per informazioni sulla modifica delle attività in un elenco, vedere <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Modificare le attività in un elenco</a>. </p> <p>Questa opzione è disponibile solo per le attività.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>Riepilogo [!UICONTROL]</td> 
   <td> <p>Visualizza o nasconde la casella Riepilogo [!UICONTROL] per l'elemento selezionato.</p> <p>Questa opzione è disponibile solo per le attività e i problemi.</p> <p>Per informazioni sul pannello Riepilogo di [!UICONTROL] nel nuovo [!DNL Adobe Workfront] esperienza, vedi <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Panoramica di riepilogo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Rimuovi]</td> 
   <td>Rimuovi qualcosa dall’elenco. Ad esempio, in qualità di amministratore di un gruppo che gestisce le appartenenze a un gruppo o a un sottogruppo, rimuovere un membro del gruppo come descritto in <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">Visualizzare e gestire le appartenenze di un gruppo</a>.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL Comment] /[!UICONTROL Update]</td> 
   <td> <p>Digita un commento o un aggiornamento.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Differenza tra elenchi e rapporti

Sia gli elenchi che i report sono griglie contenenti informazioni su un tipo di oggetto.

La tabella seguente illustra le somiglianze e le differenze tra elenchi e rapporti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Funzionalità</strong> </th> 
   <th><strong>Elenco</strong> </th> 
   <th><strong>Report</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Chiunque può crearli</p> </td> 
   <td><span>✓*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Solo un [!DNL Workfront] Gli amministratori e gli utenti con una licenza di [!UICONTROL Plan] possono crearli</p> </td> 
   <td> </td> 
   <td>✓ **</td> 
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
   <td> <p>Puoi condividerli a livello di sistema</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Puoi condividerli al di fuori del sistema</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Puoi esportare in .pdf, [!DNL Excel]Formati delimitati da tabulazioni, e</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Puoi pianificarli per la consegna tramite e-mail</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>È possibile aggiungere elementi a un modello di layout</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Puoi aggiungerli alle sezioni personalizzate </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puoi aggiungerli a una dashboard</p> </td> 
   <td> ✓ *** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>È possibile utilizzare i prompt per personalizzare la visualizzazione</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Puoi visualizzarli in un grafico</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>È possibile modificare gli oggetti in linea al loro interno</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Per poterli creare, è necessario avere accesso a filtri, viste e raggruppamenti. Per ulteriori informazioni, consulta [Concedere l’accesso a filtri, viste e raggruppamenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

Per poterli creare, è necessario avere accesso a filtri, viste e raggruppamenti, nonché a rapporti, dashboard e calendari. Per ulteriori informazioni, consulta [Concedere l’accesso a rapporti, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Puoi personalizzare gli elenchi per i rapporti inseriti in un dashboard solo se l’autore del rapporto ha configurato gli elementi dell’elenco in modo che siano visibili nel dashboard.

>[!NOTE]
>
>Non è possibile aggiungere un elenco a un dashboard senza prima creare un report e aggiungerlo al dashboard.

Per ulteriori informazioni sulla creazione di un rapporto, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Per informazioni sulla creazione di sezioni personalizzate, consulta [Creare schede o sezioni personalizzate](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## Differenza tra gli elenchi aggiornati e quelli legacy

Esistono due tipi di elenchi in [!DNL Workfront]:

* Elenchi legacy

  ![](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* Elenchi aggiornati

  ![](assets/updated-list-screen-shot-gray-groupings-350x71.png)

Entrambi i tipi di elenchi vengono visualizzati nel [!DNL Adobe Workfront].

Tutti gli elenchi e i report in [!DNL Adobe Workfront] sono elenchi aggiornati, ad eccezione dei seguenti:

* Elenchi in [!UICONTROL Configurazione] area
* Elenchi in [!UICONTROL Rapporti] area

Nella tabella seguente sono illustrate alcune delle differenze tra gli elenchi legacy e aggiornato di [!DNL Workfront]:

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
   <td> <p>Font legacy, intestazioni di colonna, combinazione di colori di raggruppamento blu</p> </td> 
   <td> <p>Font aggiornati, intestazioni di colonna, combinazione di colori per il raggruppamento dei grigi</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifica in linea più lenta</p> </td> 
   <td> <p>Editing in linea più rapido</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Visualizzazione <strong>100</strong> elementi per impostazione predefinita</p> </td> 
   <td> <p>Visualizzazione <strong>Tutti</strong> o fino a <strong>2000</strong> elementi per impostazione predefinita</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utilizzare CTRL+F per trovare elementi in un elenco</p> </td> 
   <td> <p>Utilizzare i filtri rapidi per trovare rapidamente le informazioni in un elenco di grandi dimensioni</p> <p>Per informazioni sull’utilizzo dei filtri rapidi negli elenchi, consulta <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Applicare il filtro rapido a un elenco</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Non è possibile modificare i campi personalizzati in linea con la formattazione RTF.</td> 
   <td> <p>Il testo nei campi personalizzati con formattazione può essere configurato per consentire grassetto, corsivo, sottolineatura, punti elenco, numerazione, collegamenti ipertestuali e virgolette.</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Creare o modificare un modulo personalizzato</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>La formattazione condizionale può modificare il colore del testo dei collegamenti in un elenco</td> 
   <td>Impossibile applicare le modifiche al colore del testo ai collegamenti di un elenco</td> 
  </tr> 
 </tbody> 
</table>
