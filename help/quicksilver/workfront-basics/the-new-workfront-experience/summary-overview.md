---
content-type: overview
title: Panoramica di riepilogo
description: È possibile utilizzare il pannello Riepilogo per rivedere e aggiornare le informazioni sull'elemento di lavoro direttamente da un elenco di attività, documenti o da altre aree di [!DNL Adobe Workfront] che visualizzano attività e problemi.
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: ba81706f457e41c989bc34d9bdff81223b0d745e
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 1%

---

# [!UICONTROL Riepilogo] panoramica

{{highlighted-preview}}

È possibile utilizzare [!UICONTROL Riepilogo] pannello per rivedere e aggiornare le informazioni sull’elemento di lavoro direttamente da un elenco di attività, problemi, documenti o da altre aree di [!DNL Adobe Workfront] che visualizzano attività e problemi.

Nella tabella seguente vengono visualizzate le aree in cui è possibile individuare e utilizzare [!UICONTROL Riepilogo] pannello:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Attività</td> 
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
  <tr data-mc-conditions=""> 
   <td>Problemi</td> 
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
   <td>Problemi nell'area [!UICONTROL Assigned Work] (Lavoro assegnato) del Bilanciatore dei carichi di lavoro [!UICONTROL]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problemi nella sezione [!UICONTROL Submitted] dell'area [!UICONTROL Requests]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Documenti</td> 
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

Questo articolo descrive come accedere e utilizzare [!UICONTROL Riepilogo] pannello per attività e problemi negli elenchi.

Per informazioni sull&#39;accesso a [!UICONTROL Riepilogo] nel [!UICONTROL Bilanciatore dei carichi di lavoro], vedi [Aggiornare gli elementi di lavoro in [!UICONTROL Bilanciatore dei carichi di lavoro] utilizzando [!UICONTROL Riepilogo]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Per informazioni sull&#39;accesso a [!UICONTROL Riepilogo] per i documenti, consulta [[!UICONTROL Riepilogo] panoramica sui documenti](../../documents/managing-documents/summary-for-documents.md).

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
   <td> <p>Accesso a [!UICONTROL View] o versione successiva ad attività, problemi e documenti</p> <p>Accesso di [!UICONTROL View] o versione successiva a qualsiasi oggetto per il quale si desidera visualizzare il riepilogo dei documenti [!UICONTROL Summary]</p> <p>Nota: se non disponi ancora dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>[!UICONTROL View] o autorizzazioni superiori per un'attività, un problema o un documento</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Visualizza [!UICONTROL Riepilogo] in un elenco di attività o problemi

1. Vai a un’attività o a un problema e seleziona un elemento nell’elenco.
1. Fai clic su **[!UICONTROL Riepilogo]** icona ![](assets/qs-summary-in-new-toolbar-small.png)

   oppure

   Fai clic su **[!UICONTROL Apri riepilogo]** icona ![](assets/open-summary-with-text-nwe.png) nel [!UICONTROL Inviato] sezione del [!UICONTROL Richieste] area.

   Dopo aver aperto il riepilogo, rimane aperto quando si fa clic su o si selezionano altre attività o problemi e rimane aperto fino a quando non viene chiuso manualmente.

   >[!TIP]
   >
   >Puoi selezionare una sola attività o un solo problema alla volta per visualizzarne i dettagli in [!UICONTROL Riepilogo] pannello.

   <div class="preview">

   Esempio del pannello Riepilogo nell’ambiente di anteprima:
   ![Pannello Riepilogo](assets/summary-panel-for-task-new-comments.png)

   </div>

   Esempio del pannello Riepilogo nell’ambiente di produzione:
   ![Pannello Riepilogo](assets/summary-panel-for-task.png)

1. (Facoltativo) Per chiudere il [!UICONTROL Riepilogo] eseguire una delle operazioni seguenti:

   * In un elenco di attività o problemi, fai clic su **[!UICONTROL Apri riepilogo]** icona ![](assets/summary-panel-icon.png)

     Oppure

     Fai clic su **X** nell&#39;angolo superiore destro del [!UICONTROL Riepilogo] pannello.

   * In [!UICONTROL Inviato] sezione del [!UICONTROL Richieste] , fare clic sul pulsante **[!UICONTROL Chiudi riepilogo]** icona ![](assets/close-summary-with-text-nwe.png)

     Oppure

     Fai clic su **X** nell&#39;angolo superiore destro del pannello Riepilogo.

## [!UICONTROL Percentuale completato]

Utilizza la barra di avanzamento nella parte superiore della [!UICONTROL Riepilogo] per aggiornare la percentuale di completamento per l&#39;attività o il problema selezionato. Immetti un numero o trascina la barra fino alla percentuale corretta.

![Percentuale di completamento nel pannello Riepilogo](assets/summary-overview-percent-complete.png)

## [!UICONTROL Aggiornamenti]

Utilizza il [!UICONTROL Aggiornamenti] sezione del [!UICONTROL Riepilogo] per visualizzare gli aggiornamenti recenti e apportare aggiornamenti all’attività o al problema selezionato. Clic **[!UICONTROL Vedi tutto]** per passare direttamente al [!UICONTROL Aggiornamenti] sull&#39;attività.

<div class="preview">

Esempio di aggiornamenti nell’ambiente di anteprima:
![Sezione Aggiornamenti nel pannello Riepilogo](assets/summary-updates-section.png)

</div>

Esempio di aggiornamenti nell’ambiente di produzione:
![Sezione Aggiornamenti nel pannello Riepilogo](assets/summary-updates-with-block-quote-350x290.png)

## [!UICONTROL Documenti]

Utilizza il [!UICONTROL Documenti] sezione del [!UICONTROL Riepilogo] per visualizzare i documenti allegati all’attività o al problema selezionato. Fare clic sulla miniatura per aprire un&#39;anteprima del documento. Per passare direttamente al [!UICONTROL Documenti] sull’attività o sul problema, fai clic sulla scheda **[!UICONTROL Documenti]** titolo.

![Sezione Documenti nel pannello Riepilogo](assets/summary-documents-section.png)

## [!UICONTROL Dettagli]

Utilizza il [!UICONTROL Dettagli] sezione del [!UICONTROL Riepilogo] per visualizzare i dettagli degli elementi di lavoro di alto livello, effettuare assegnazioni o aggiungere date di inizio. Clic **[!UICONTROL Vedi tutto]** per passare direttamente al [!UICONTROL Dettagli] sull’attività o sul problema.

>[!NOTE]
>
>I campi visualizzati in questa sezione sono gli stessi campi visualizzati nel pannello destro della Home. Puoi personalizzare questi campi [Personalizza [!UICONTROL Home] e [!UICONTROL Riepilogo] utilizzo di un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

![Sezione Dettagli nel pannello Riepilogo](assets/summary-details-section.png)

## [!UICONTROL Sottoattività]

Questa sezione è disponibile solo per le attività. Utilizza il [!UICONTROL Sottoattività] sezione del [!UICONTROL Riepilogo] per visualizzare [!UICONTROL Nuovo], [!UICONTROL In corso], e [!UICONTROL Chiuso] sottoattività dell&#39;attività selezionata. Fai clic su **[!UICONTROL Stato]** menu a discesa per passare da uno stato all’altro. Per passare direttamente al [!UICONTROL Sottoattività] sull&#39;attività, fare clic sul pulsante **[!UICONTROL Sottoattività]**&#x200B;titolo.

Se non sono state aggiunte sottoattività all&#39;attività, fare clic su **[!UICONTROL Aggiungine qui]** per passare direttamente al [!UICONTROL Sottoattività] sull&#39;attività.

![Sezione delle sottoattività nel pannello Riepilogo](assets/summary-subtasks-section.png)

## [!UICONTROL Ore]

Utilizza il [!UICONTROL Ore] sezione del [!UICONTROL Riepilogo] per registrare le ore per l’attività o il problema selezionato. Clic **[!UICONTROL Tempo di connessione]** e inserisci le ore. Per passare direttamente alla scheda Ore sull’attività o sul problema, fai clic sul pulsante **[!UICONTROL Ore]** titolo.

Il conteggio delle ore nel [!UICONTROL Riepilogo] visualizza le ore registrate. Altri utenti avranno totali orari diversi nel [!UICONTROL Riepilogo] a seconda dell&#39;ora di accesso all&#39;attività.

Se non sono pianificati [!UICONTROL ore] sull’attività o sul problema e hai registrato l’ora, la barra delle ore viene visualizzata in rosso.

![Sezione ore nel pannello Riepilogo](assets/summary-hours-section.png)

## Approvazioni

Utilizza il [!UICONTROL Approvazioni] sezione del [!UICONTROL Riepilogo] per visualizzare le approvazioni associate all’attività o al problema selezionato. Se non hai aggiunto alcuna approvazione, seleziona un’approvazione esistente dal menu a discesa o fai clic su **[!UICONTROL Creare un processo di approvazione per singolo utilizzo]** per passare direttamente al [!UICONTROL Approvazioni] sull’attività o sul problema.

Per passare direttamente al [!UICONTROL Approvazioni] sull’attività o sul problema, fai clic sulla scheda **[!UICONTROL Approvazioni]** titolo.

![Sezione Approvazioni nel pannello Riepilogo](assets/summary-approvals-section.png)
