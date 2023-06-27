---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Editor scenario in [!DNL Adobe] Workfront Fusion
description: L’editor degli scenari consente di creare e modificare scenari in un’interfaccia visiva.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Editor scenario in [!DNL Adobe Workfront Fusion]

L’editor degli scenari consente di creare e modificare scenari in un’interfaccia visiva.

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
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Apri l’editor scenario:

1. Clic **[!UICONTROL Scenari]** ![](assets/scenarios-icon.png) nel pannello a sinistra.

1. Per creare uno scenario, fai clic su **[!UICONTROL Crea un nuovo scenario]** nell’angolo superiore destro della pagina.

   Oppure

   Se si desidera modificare uno scenario esistente, fare clic su di esso.

   Nell’editor dello scenario visualizzato, puoi eseguire tutte le operazioni elencate nella tabella seguente. Per ulteriori informazioni, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Al termine della modifica di uno scenario (o in qualsiasi momento durante la modifica), fai clic su [!UICONTROL Salva] icona. ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >Dopo aver salvato lo scenario, sarà disponibile una nuova versione nel menu con tre punti, qualora tu debba accedervi in futuro. Le versioni degli scenari salvate in precedenza sono disponibili solo per 60 giorni.

## Azioni editor di scenari disponibili

Nell’editor scenario sono disponibili le seguenti azioni:

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Aggiungi il primo modulo</td>
     <td> <p>Fare clic sull'icona del punto interrogativo. <img src="assets/question-mark-full-size.png"></p> <p> Quindi individua e fai clic sull’app o sul servizio con cui desideri iniziare. Se hai selezionato delle app nel passaggio 2, sono disponibili qui per accedervi facilmente (e nel <strong>[!UICONTROL Preferiti]</strong> nella parte inferiore dello schermo).</p> </td>
  </tr>
  <tr>
     <td role="rowheader">Aggiungi un modulo</td>
     <td>Passa il puntatore del mouse su un modulo, fai clic sull’icona più a destra, quindi sul modulo desiderato nel menu visualizzato.</td>
  </tr>  
  <tr>   
     <td role="rowheader">Specifica quando e con quale frequenza verrà eseguito lo scenario</td>  
      <td> <p>Fai clic sull’icona dell’orologio. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Pianificare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">Impostare un ciclo di lavorazione</td>   
     <td> <p>Fai clic sull'icona [!UICONTROL chiave] <img src="assets/wrench-icon.gif"> tra i due moduli e utilizza una delle seguenti opzioni:</p>    
       <ul>
         <li><strong>[!UICONTROL Configura un filtro]</strong>: controlla quali bundle vengono utilizzati in determinati punti dello scenario. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Aggiungere un filtro a uno scenario in [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL Scollega]</strong>: rimuove una route.</li>     
         <li><strong>[!UICONTROL Aggiungi router]</strong>: aggiunge un router tra i moduli. </li>     
         <li><strong>[!UICONTROL Aggiungi un modulo]</strong>: aggiunge un nuovo modulo tra i moduli.</li>     
         <li><strong>[!UICONTROL Aggiungi una nota]</strong>: aggiunge una nota alla route.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Rimuovere un modulo</td>   
     <td>Fai clic con il pulsante destro del mouse sul modulo, quindi fai clic su <strong>[!UICONTROL Elimina modulo]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Visualizzare un registro di eventi che si verificano è uno scenario</td>     
     <td> 
       <p>Esegui uno scenario. Al termine dell'esecuzione dello scenario, il registro viene visualizzato nell'angolo inferiore destro dell'[!UICONTROL Scenario Editor]. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>A seconda dello scenario, il registro può contenere informazioni sulla difficoltà di ciascuna fase e su eventuali errori riscontrati durante l’esecuzione dello scenario.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Configurare le impostazioni dello scenario</td>   
     <td>Fai clic sull'icona [!UICONTROL Scenario settings] (Impostazioni scenario). <img src="assets/gear-icon-settings.png"> Queste impostazioni sono destinate principalmente agli utenti avanzati.</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Digita o visualizza le note sullo scenario</td>   
     <td>Fai clic sull'icona [!UICONTROL Notes]. <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Allineamento automatico del layout dei moduli </td>   
     <td>Fare clic sull'icona Allineamento automatico. <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">Visualizzare un’animazione che mostra il modo in cui i dati scorrono nello scenario</td>   <td>Fai clic sull'icona [!UICONTROL Spiega flusso]. <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Esporta lo scenario nel computer come blueprint</td>   
     <td>Fare clic sul menu Altro <img src="assets/more-icon.png">, quindi fare clic su [!UICONTROL Export Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Importa una blueprint di scenario dal computer</td>   
     <td>Fare clic sul menu Altro <img src="assets/more-icon.png">, quindi fare clic su [!UICONTROL Import Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Ripristina una versione precedente dello scenario</td>   
     <td>Vedi l’articolo <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Ripristinare una versione dello scenario in [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Configurare le impostazioni di [!UICONTROL Flow Control]</td>   
     <td> <p>Fare clic sull'icona [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> È possibile impostare un'attività in modo da ripetere un determinato numero di volte, convertire un array in una serie di bundle e unire più bundle in un singolo bundle. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Controllo del flusso in [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Migliorare lo scenario utilizzando strumenti avanzati</td>   
     <td>Fare clic sull'icona [!UICONTROL Tools]. <img src="assets/tools-icon.gif"> Puoi creare trigger, azioni, aggregatori e trasformatori. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Strumenti</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Utilizzare gli strumenti di analisi del testo</td>   
     <td>Fare clic sull'icona del parser di testo [!UICONTROL]. <img src="assets/text-parser-icon.gif"> Puoi recuperare elementi dal codice HTML, trovare ed estrarre elementi stringa che corrispondono a un pattern di ricerca, cercare e sostituire testo e dati di tipo "scrape" da un sito web. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Strumenti</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Accedi alle app e ai servizi più comunemente utilizzati</td>   
     <td> Fai clic su un’icona nella sezione <strong>[!UICONTROL Preferiti]</strong> nella parte inferiore dello schermo. Le icone vengono visualizzate automaticamente in questa sezione quando aggiungi app e servizi allo scenario. Puoi anche fare clic sull’icona Aggiungi <img src="assets/add-icon.gif"> per aggiungere manualmente app e servizi a quest'area.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Eseguire il test dello scenario</td>   
     <td>Clic <strong>[!UICONTROL Esegui una volta]</strong> per verificare che lo scenario venga eseguito come previsto prima di attivarlo. Una volta attivato, lo scenario viene eseguito in base alla sua pianificazione. Se tutto non funziona come previsto, consulta la sezione Gestione degli errori per scoprire come gestire gli errori.</td> 
   </tr> 
</tbody>
</table>
