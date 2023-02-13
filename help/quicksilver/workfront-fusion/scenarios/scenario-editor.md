---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Editor di scenari in [!DNL Adobe] Workfront Fusion
description: L’editor di scenari consente di creare e modificare scenari in un’interfaccia visiva.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: aa58a64ea6b09192f93fa89a42a4bf6731052d10
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Editor di scenari in [!DNL Adobe Workfront Fusion]

L’editor di scenari consente di creare e modificare scenari in un’interfaccia visiva.

![](assets/scenario-editor-350x228.jpg)

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Apri l’editor di scenari:

1. Fai clic su **[!UICONTROL Scenari]** ![](assets/scenarios-icon.png) nel pannello a sinistra.

1. Per creare uno scenario, fai clic su **[!UICONTROL Creare un nuovo scenario]** nell’angolo superiore destro della pagina.

   Oppure

   Se si desidera modificare uno scenario esistente, fare clic sullo scenario.

1. (Condizionale) Se stai creando un nuovo scenario, in **[!UICONTROL Quali servizi desideri integrare?]**, seleziona le app con cui desideri lavorare nello scenario, quindi fai clic su **[!UICONTROL Continua]**.

   Oppure

   Fai clic su **[!UICONTROL Salta]** se preferisci scegliere le app dall&#39;editor di scenari.

   Nell’editor dello scenario visualizzato, puoi eseguire tutte le operazioni elencate nella tabella seguente. Per ulteriori informazioni, consulta [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Al termine della modifica di uno scenario (o in qualsiasi momento durante la modifica), fai clic sul pulsante [!UICONTROL Salva] icona. ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >Dopo aver salvato lo scenario, sarà disponibile una nuova versione nel menu a tre punti nel caso sia necessario accedervi in futuro. Le versioni precedenti degli scenari salvati sono disponibili solo per 60 giorni.

## Azioni dell’editor di scenari disponibili

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Aggiungi il primo modulo</td>
     <td> <p>Fai clic sull’icona del punto interrogativo. <img src="assets/question-mark-full-size.png"></p> <p> Quindi trova e fai clic sull’app o sul servizio con cui vuoi iniziare. Se hai selezionato delle app al passaggio 2, queste appaiono qui per un facile accesso (e nel <strong>[!UICONTROL Preferiti]</strong> nella parte inferiore dello schermo).</p> </td>
  </tr>
  <tr>
     <td role="rowheader">Aggiungi un modulo</td>
     <td>Passa il puntatore del mouse su un modulo, fai clic sull'icona più a destra, quindi fai clic sul modulo desiderato nel menu visualizzato.</td>
  </tr>  
  <tr>   
     <td role="rowheader">Specificare quando e con quale frequenza verrà eseguito lo scenario</td>  
      <td> <p>Fai clic sull’icona dell’orologio. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Pianifica uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">Imposta un percorso</td>   
     <td> <p>Fai clic sull’icona a forma di chiave inglese [!UICONTROL] <img src="assets/wrench-icon.gif"> tra i due moduli e utilizzare una delle seguenti opzioni:</p>    
       <ul>
         <li><strong>[!UICONTROL Impostare un filtro]</strong>: Controlla quali bundle vengono utilizzati in determinati punti dello scenario. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Aggiungi un filtro a uno scenario in [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL Scollega]</strong>: Rimuove un percorso.</li>     
         <li><strong>[!UICONTROL Aggiungere un router]</strong>: Aggiunge un router tra i moduli. </li>     
         <li><strong>[!UICONTROL Aggiungi un modulo]</strong>: Aggiunge un nuovo modulo tra i moduli.</li>     
         <li><strong>[!UICONTROL Aggiungi una nota]</strong>: Aggiunge una nota alla route.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Rimuovere un modulo</td>   
     <td>Fai clic con il pulsante destro del mouse sul modulo, quindi fai clic su <strong>[!UICONTROL Elimina modulo]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Visualizza un registro degli eventi che si verificano in uno scenario</td>     
     <td> 
       <p>Esegui uno scenario. Al termine dell'esecuzione dello scenario, il registro viene visualizzato nell'angolo inferiore destro dell' [!UICONTROL Scenario Editor]. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>A seconda dello scenario, il registro può contenere informazioni sulla difficoltà di ogni fase e sugli eventuali errori riscontrati durante l’esecuzione dello scenario.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Configurare le impostazioni dello scenario</td>   
     <td>Fai clic sull'icona [!UICONTROL Scenario settings] . <img src="assets/gear-icon-settings.png"> Queste impostazioni sono destinate principalmente agli utenti avanzati.</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Digitare o visualizzare note sullo scenario</td>   
     <td>Fai clic sull’icona Note . <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Allineamento automatico del layout dei moduli </td>   
     <td>Fai clic sull’icona [!UICONTROL Auto-align]. <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">Visualizzare un'animazione che mostra il flusso dei dati nello scenario</td>   <td>Fai clic sull’icona [!UICONTROL Explain Flow]. <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Esportare lo scenario nel computer come blueprint</td>   
     <td>Fai clic sul menu Altro <img src="assets/more-icon.png">, quindi fai clic su [!UICONTROL Export Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Importare una blueprint dello scenario dal computer</td>   
     <td>Fai clic sul menu Altro <img src="assets/more-icon.png">, quindi fai clic su [!UICONTROL Import Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Ripristinare una versione precedente dello scenario</td>   
     <td>Vedi l'articolo <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Ripristinare una versione di uno scenario in [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Configurare le impostazioni di [!UICONTROL Flow Control]</td>   
     <td> <p>Fai clic sull’icona [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> È possibile impostare un'attività per ripetere un determinato numero di volte, convertire un array in una serie di bundle e unire diversi bundle in un unico bundle. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Controllo del flusso in [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Migliorare lo scenario utilizzando strumenti avanzati</td>   
     <td>Fai clic sull’icona [!UICONTROL Tools]. <img src="assets/tools-icon.gif"> Puoi creare attivatori, azioni, aggregatori e trasformatori. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Strumenti</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Utilizzare gli strumenti di analisi del testo</td>   
     <td>Fai clic sull’icona [!UICONTROL Text parser]. <img src="assets/text-parser-icon.gif"> È possibile recuperare elementi dal codice HTML, trovare ed estrarre elementi stringa che corrispondono a un pattern di ricerca, cercare e sostituire testo e dati "scraping" da un sito web. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Strumenti</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Accedere alle app e ai servizi più comunemente utilizzati</td>   
     <td> Fai clic su un’icona nella <strong>[!UICONTROL Preferiti]</strong> nella parte inferiore dello schermo. Le icone vengono visualizzate automaticamente in questa sezione quando aggiungi app e servizi al tuo scenario. Puoi anche fare clic sull’icona Aggiungi <img src="assets/add-icon.gif"> per aggiungere manualmente app e servizi a questa area.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Eseguire il test dello scenario</td>   
     <td>Fai clic su <strong>[!UICONTROL Esegui una volta)</strong> per verificare che lo scenario venga eseguito come previsto prima di attivarlo. Una volta attivato, lo scenario verrà eseguito in base alla sua pianificazione. Se tutto non funziona come previsto, puoi visitare la nostra sezione sulla gestione degli errori per scoprire come gestire gli errori.</td> 
   </tr> 
</tbody>
