---
content-type: overview
title: Panoramica di riepilogo
description: Puoi utilizzare il pannello Riepilogo per rivedere e aggiornare le informazioni sugli elementi di lavoro direttamente da un elenco di attività, documenti o da altre aree di [!DNL Adobe Workfront]  che visualizzano attività e problemi.
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 66fc75ed9a7fca4b44ac776c314a6e08a6fbd450
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 2%

---

# Panoramica di [!UICONTROL Riepilogo]

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span> -->

È possibile utilizzare il pannello [!UICONTROL Riepilogo] per rivedere e aggiornare le informazioni sugli elementi di lavoro direttamente da un elenco di attività, problemi, documenti o da altre aree di [!DNL Adobe Workfront] che visualizzano attività e problemi.

L’amministratore del Workfront o del gruppo può modificare le aree e i campi visualizzati nel pannello Riepilogo. Possono aggiungere fino a 16 campi al pannello Riepilogo.

>[!IMPORTANT]
>
>È consigliabile aggiungere al pannello Riepilogo i campi che è necessario aggiornare frequentemente, in modo da potervi accedere facilmente e aggiornarli senza dover accedere alla pagina principale dell’oggetto.
>
>Ad esempio, puoi aggiungere i seguenti campi aggiornati di frequente ai pannelli Riepilogo delle attività e dei problemi:
>
>* Stato
>* Percentuale completato
>* Conferma data
>* Data di completamento Pianificata
>* Condizione



Nella tabella seguente vengono visualizzate le aree in cui è possibile individuare e utilizzare il pannello [!UICONTROL Riepilogo]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td><b>Attività</b></td> 
  </tr> 
  <tr> 
   <td> <p>Elenchi di attività in una</p> 
    <ul> 
     <li>Progetto</li> 
     <li>Sottoattività</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Attività nelle aree di lavoro [!UICONTROL non assegnato] e [!UICONTROL assegnato] del Bilanciatore dei carichi di lavoro [!UICONTROL assegnato]</td> 
  </tr> 
   <tr> 
   <td>Attività in una scheda orario </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><b>Problemi</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Elenchi di problemi in una</p> 
    <ul> 
     <li>Progetto</li> 
     <li>Attività</li> 
     <li>Sottoattività</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problemi nell'area [!UICONTROL Assigned Work] (Lavoro assegnato) del Bilanciatore dei carichi di lavoro </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problemi nella sezione [!UICONTROL Submitted] dell'area [!UICONTROL Requests]</td> 
  </tr> 
</tr> 
   <tr> 
   <td>Problemi in una scheda orario </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td><b>Documenti</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Area [!UICONTROL Documents]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Sezione [!UICONTROL Documents] di qualsiasi oggetto (progetto, attività, problema, programma, portfolio, modello, attività modello, utente)</td> 
  </tr> 
 </tbody> 
</table>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront administrators can customize the Summary in the Layout Template. For more information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
-->

In questo articolo viene descritto come accedere e utilizzare il pannello [!UICONTROL Riepilogo] per le attività e i problemi negli elenchi.

Per informazioni sull&#39;accesso a [!UICONTROL Summary] nel [!UICONTROL Bilanciatore dei carichi di lavoro], vedere [Aggiornare gli elementi di lavoro nel [!UICONTROL Bilanciatore dei carichi di lavoro] utilizzando il [!UICONTROL Summary]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Per informazioni sull&#39;accesso a [!UICONTROL Riepilogo] per i documenti, vedere [[!UICONTROL Riepilogo] per la panoramica dei documenti](../../documents/managing-documents/summary-for-documents.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>Nuovo: Collaboratore o versione successiva</p>
   Oppure
   <p>Corrente:[!UICONTROL Request] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazione del livello di accesso</strong></td> 
   <td> <p>Accesso a [!UICONTROL View] o versione successiva ad attività, problemi e documenti</p> <p>Accesso di [!UICONTROL View] o versione successiva a qualsiasi oggetto per il quale si desidera visualizzare i documenti [!UICONTROL Summary]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>[!UICONTROL View] o autorizzazioni superiori per un'attività, un problema o un documento</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront]. Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Visualizza il pannello [!UICONTROL Riepilogo] in un elenco di attività o problemi

1. Vai a un’attività o a un problema e seleziona un elemento nell’elenco.
1. Fai clic sull&#39;icona **[!UICONTROL Riepilogo]** ![](assets/qs-summary-in-new-toolbar-small.png)

   oppure

   Fai clic sull&#39;icona ![](assets/open-summary-with-text-nwe.png) di **[!UICONTROL Apri riepilogo]** nella sezione [!UICONTROL Inviato] dell&#39;area [!UICONTROL Richieste].

   Dopo aver aperto il riepilogo, rimane aperto quando si fa clic su o si selezionano altre attività o problemi e rimane aperto fino a quando non viene chiuso manualmente.

   >[!TIP]
   >
   >Puoi selezionare una sola attività o un solo problema alla volta per visualizzarne i dettagli nel pannello [!UICONTROL Riepilogo].

   ![Pannello di riepilogo](assets/summary-panel-for-task-new-comments.png)

1. (Facoltativo) Per chiudere il pannello [!UICONTROL Riepilogo], eseguire una delle operazioni seguenti:

   * In un elenco di attività o problemi, fai clic sull&#39;icona **[!UICONTROL Apri riepilogo]** ![](assets/summary-panel-icon.png)

     Oppure

     Fai clic sull&#39;icona **X** nell&#39;angolo superiore destro del pannello [!UICONTROL Riepilogo].

   * Nella sezione [!UICONTROL Submitted] dell&#39;area [!UICONTROL Requests], fare clic sull&#39;icona **[!UICONTROL Close Summary]** ![](assets/close-summary-with-text-nwe.png)

     Oppure

     Fai clic sull&#39;icona **X** nell&#39;angolo superiore destro del pannello Riepilogo.

## [!UICONTROL Percentuale completato]

Utilizza il fumetto blu di avanzamento nella parte superiore del [!UICONTROL Riepilogo] per aggiornare la percentuale di completamento dell&#39;attività o del problema selezionato. Immetti un numero o trascina la bolla fino alla percentuale corretta.

Quando trascinate la bolla nel pannello Riepilogo, la percentuale di completamento viene aggiornata con incrementi di un punto. Impossibile immettere un numero decimale.

![Percentuale completata nel pannello Riepilogo](assets/summary-overview-percent-complete.png)

## [!UICONTROL Aggiornamenti]

Utilizza la sezione [!UICONTROL Aggiornamenti] del [!UICONTROL Riepilogo] per visualizzare gli aggiornamenti recenti e apportare aggiornamenti all&#39;attività o al problema selezionato. Fai clic su **[!UICONTROL Visualizza tutto]** per passare direttamente alla scheda [!UICONTROL Aggiornamenti] dell&#39;attività.

![Sezione Aggiornamenti nel pannello Riepilogo](assets/summary-updates-section.png)

## [!UICONTROL Documenti]

Utilizza la sezione [!UICONTROL Documenti] del [!UICONTROL Riepilogo] per visualizzare i documenti allegati all&#39;attività o al problema selezionato. Fare clic sulla miniatura per aprire un&#39;anteprima del documento. Per passare direttamente alla scheda [!UICONTROL Documenti] dell&#39;attività o del problema, fare clic sul titolo **[!UICONTROL Documenti]**.

![Sezione Documenti nel pannello Riepilogo](assets/summary-documents-section.png)

## [!UICONTROL Dettagli]

Utilizza la sezione [!UICONTROL Dettagli] del [!UICONTROL Riepilogo] per visualizzare i dettagli degli elementi di lavoro di alto livello, effettuare assegnazioni o aggiungere date di inizio. Fai clic su **[!UICONTROL Visualizza tutto]** per passare direttamente alla scheda [!UICONTROL Dettagli] sull&#39;attività o sul problema.



![Sezione Dettagli nel pannello Riepilogo](assets/summary-details-section.png)

## [!UICONTROL Attività secondarie]

Questa sezione è disponibile solo per le attività. Utilizza la sezione [!UICONTROL Sottoattività] del [!UICONTROL Riepilogo] per visualizzare [!UICONTROL Nuove], [!UICONTROL In corso] e [!UICONTROL Sottoattività chiuse] sull&#39;attività selezionata. Fai clic sul menu a discesa **[!UICONTROL Stato]** per passare da uno stato all&#39;altro. Per passare direttamente alla scheda [!UICONTROL Sottoattività] dell&#39;attività, fare clic sul titolo **[!UICONTROL &#x200B;]**.

Se non hai aggiunto alcuna sottoattività all&#39;attività, fai clic su **[!UICONTROL Aggiungi qui]** per passare direttamente alla scheda [!UICONTROL Sottoattività] dell&#39;attività.

![Sezione Sottoattività nel pannello Riepilogo](assets/summary-subtasks-section.png)

## [!UICONTROL Ore]

Utilizza la sezione [!UICONTROL Hours] del [!UICONTROL Summary] per registrare le ore per l&#39;attività o il problema selezionato. Fai clic su **[!UICONTROL Registra ora]** e immetti le tue ore. Per passare direttamente alla scheda Ore sull&#39;attività o sul problema, fai clic sul titolo **[!UICONTROL Ore]**.

Il conteggio delle ore nel [!UICONTROL Riepilogo] visualizza le ore registrate. Altri utenti avranno totali orari diversi in [!UICONTROL Riepilogo] a seconda dell&#39;ora di accesso all&#39;attività.

Se non sono presenti [!UICONTROL ore] pianificate per l&#39;attività o il problema e hai registrato l&#39;ora, la barra delle ore viene visualizzata in rosso.

![Sezione ore nel pannello Riepilogo](assets/summary-hours-section.png)

## Approvazioni

Utilizza la sezione [!UICONTROL Approvazioni] del [!UICONTROL Riepilogo] per visualizzare le approvazioni associate all&#39;attività o al problema selezionato. Se non hai aggiunto alcuna approvazione, seleziona un&#39;approvazione esistente dal menu a discesa o fai clic su **[!UICONTROL Crea processo di approvazione a utente singolo]** per passare direttamente alla scheda [!UICONTROL Approvazioni] sull&#39;attività o sul problema.

Per passare direttamente alla scheda [!UICONTROL Approvazioni] dell&#39;attività o del problema, fare clic sul titolo **[!UICONTROL Approvazioni]**.

![Sezione approvazioni nel pannello di riepilogo](assets/summary-approvals-section.png)
