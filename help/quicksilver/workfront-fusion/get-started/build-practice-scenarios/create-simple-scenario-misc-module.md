---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Crea uno scenario semplice in [!DNL Adobe Workfront Fusion]
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
hide: true
hidefromtoc: true
feature: Workfront Fusion
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 0%

---

# Crea uno scenario di base in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Crea uno scenario di base](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/create-basic-scenario.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

Il ruolo di [!DNL Adobe Workfront Fusion] consiste nell&#39;automatizzare i processi in modo da potersi concentrare su nuove attività anziché ripetere più volte le stesse attività. Funziona tramite il collegamento di azioni all’interno e tra app e servizi per creare uno scenario che trasferisce e trasforma automaticamente i dati. Lo scenario in cui si creano controlli i dati in un’app o in un servizio ed elabora tali dati in modo da fornire il risultato desiderato.

Questo esempio illustra come creare uno scenario che cerca un problema in Workfront e lo converte in un progetto.

<!--# Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Creare uno scenario di esercitazione

### Inizia a creare lo scenario

1. Nell&#39;area **Scenari**, fare clic su **Crea un nuovo scenario**.

   <!--To locate the Scenarios area, see navigation article-->

   Viene visualizzato l’editor scenario, contenente un modulo vuoto al centro.

   <!--picture?-->

1. Seleziona il nome del segnaposto **[!UICONTROL Nuovo scenario]** nell&#39;angolo superiore sinistro, quindi immetti un nome.
1. Continua con [Aggiungi e configura il primo modulo](#add-and-configure-the-first-module) di seguito.

### Aggiungere e configurare il primo modulo

1. Fai clic sul modulo vuoto per scegliere l’app dalla quale selezionare un modulo.

   A destra del modulo viene visualizzato un elenco di app.

1. Selezionare **[!DNL Adobe Workfront]**. Se non è visibile, fare clic sulla barra di ricerca nella parte inferiore dell&#39;elenco, digitare &quot;Workfront&quot; e selezionarla quando viene visualizzata nell&#39;elenco.

   L&#39;elenco viene modificato in modo da visualizzare tutti i moduli [!DNL Workfront] utilizzabili.

1. Fare clic sul modulo **[!UICONTROL Cerca]**.

   Viene visualizzata la finestra di configurazione del modulo.

1. Nella casella [!UICONTROL Connessione], seleziona la tua connessione Workfront.

   Se non disponi di una connessione Workfront, vedi [Creare una connessione a [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. Nella casella [!UICONTROL Tipo di record], seleziona **[!UICONTROL Problema]**. Questo imposta il modulo in modo che esegua la ricerca solo dei problemi.

   Puoi trovare **[!UICONTROL Issue]** nell&#39;elenco se inizi a digitare la parola &quot;[!UICONTROL issue].&quot;

1. Nella casella **[!UICONTROL Set di risultati]** selezionare **[!UICONTROL Primo record corrispondente]**.

   In questo modo il modulo restituirà solo il primo record che soddisfa i criteri.
1. Nell&#39;area **[!UICONTROL Criteri di ricerca]**, configura i criteri per restituire il problema specifico.

   1. Nella prima casella in [!UICONTROL Criteri di ricerca], selezionare il campo che si desidera includere nella ricerca. Per questo esempio, selezionare **[!UICONTROL Nome]**.

      Puoi trovare **[!UICONTROL Name]** nell&#39;elenco se inizi a digitare la parola &quot;[!UICONTROL name].&quot;
   1. Per l&#39;operatore, fare clic sulla freccia a discesa accanto a **Esiste** e modificarla in [!UICONTROL **Contiene (senza distinzione maiuscole/minuscole)**].

      Questo consente al modulo di trovare i progetti il cui nome contiene le parole scelte, anche se non si inserisce il nome completo o si inserisce il nome con lettere maiuscole non corrette.
   1. Nell&#39;ultimo campo in [!UICONTROL Criteri di ricerca], immettere una parola o una frase che si sa essere nel nome del problema che si sta cercando.

1. Nell&#39;elenco **[!UICONTROL Output]** selezionare i campi che si desidera vengano generati dal modulo. Per questo esempio, selezionare i campi **[!UICONTROL ID]** e **[!UICONTROL Nome]**.

   >[!TIP]
   >
   >È possibile utilizzare **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F** ([!DNL Windows] OS) per trovare rapidamente un campo.

1. Fare clic su **[!UICONTROL OK]** per salvare la configurazione del modulo.

1. Fare clic con il pulsante destro del mouse sul modulo, scegliere **[!UICONTROL Rinomina]**, quindi digitare un nome che descriva le operazioni che si desidera eseguire (ad esempio &quot;Cerca problema&quot;), quindi fare clic su **[!UICONTROL OK]**.

   Il nome viene visualizzato appena sotto il modulo. Di seguito, [!DNL Workfront Fusion] include una breve descrizione del tipo di azione eseguita dal modulo.

   ![](assets/)

1. Continua con [Aggiungi e configura il secondo modulo](#add-and-configure-the-second-module).

## Aggiungere e configurare il secondo modulo

1. Passa il puntatore del mouse sul cerchio parziale a destra della sezione del modulo, quindi fai clic su **[!UICONTROL Aggiungi un altro modulo]**.
1. Selezionare [!DNL Adobe Workfront] dall&#39;elenco delle applicazioni, quindi scegliere il modulo **[!UICONTROL Azione varie]**.

   Il modulo Azioni varie consente di eseguire in Workfront azioni che non dispongono di un modulo dedicato. In questo esempio, questo modulo viene utilizzato per convertire il problema in un progetto.
1. Nel campo [!UICONTROL Connessione], seleziona la stessa connessione Workfront utilizzata nel modulo precedente.
1. Nel campo **[!UICONTROL Tipo di record]**selezionare **[!UICONTROL Problema]**, poiché l&#39;azione da eseguire è correlata a un problema.
1. Nel campo **[!UICONTROL Azione]**, selezionare **convertToProject**. Questa è l&#39;azione che convertirà il problema selezionato in un progetto.
1. Fai clic sul campo **[!UICONTROL ID]**.

   Viene visualizzato un pannello che consente di selezionare cosa utilizzare come ID del problema da convertire in un progetto. Il pannello include l’output di tutti i moduli precedenti. Poiché hai selezionato ID come output del modulo precedente, ora è disponibile nel pannello.

   Questo pannello è denominato pannello di mappatura. Per ulteriori informazioni sul pannello di mappatura, vedere [Mappare le informazioni da un modulo all&#39;altro](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Seleziona **ID** nel pannello di mappatura.

   Nel campo ID viene visualizzato un blocco ID. Mostra il numero del modulo da cui è mappato e il campo mappato.

   ![ID mappa](assets/map-id.png)

1. (Facoltativo) Nella sezione Progetto, individua il campo ID proprietario e inizia a digitare il tuo nome nel campo, quindi selezionalo quando viene visualizzato. Questo ti imposta come proprietario del progetto e lo renderà più facile da trovare in Workfront.

   >[!TIP]
   >
   >È possibile utilizzare **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F** ([!DNL Windows] OS) per trovare rapidamente un campo.

1. Fare clic su **[!UICONTROL OK]** per salvare la configurazione del modulo.

1. Fare clic con il pulsante destro del mouse sul modulo, scegliere **[!UICONTROL Rinomina]**, quindi digitare un nome che descriva le operazioni che si desidera eseguire (ad esempio &quot;Converti in progetto&quot;), quindi fare clic su **[!UICONTROL OK]**.

1. Continua a [Verificare lo scenario](#test-the-scenario).

## Verifica lo scenario

Prima di attivare lo scenario, è importante testarlo eseguendolo almeno una volta e visualizzando i risultati. Questo ti aiuta a capire come i dati scorrono attraverso lo scenario e a trovare eventuali errori.

In questo caso, se il test ha esito positivo, il problema viene individuato e convertito in un progetto.

1. Fai clic su **[!UICONTROL Esegui una volta]** nell&#39;angolo inferiore sinistro dell&#39;editor scenari.
1. Al termine dell’esecuzione dello scenario, fai clic sul fumetto sopra il primo modulo per visualizzare informazioni sul bundle di dati elaborato dal modulo, inclusi i dati estratti dal problema restituito dal modulo.

1. Fai clic sul fumetto del controllo dell’esecuzione sopra il secondo modulo per visualizzare l’input (il problema) e l’output (il progetto convertito).

   Per ulteriori informazioni sui dati contenuti nelle bolle di ispezione, vedere:

   * Per informazioni generali, vedere [Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Per informazioni sui bundle elaborati, vedere [Esecuzione scenario, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. In [!DNL Workfront Fusion], fai clic su **[!UICONTROL Salva]** nell&#39;angolo inferiore sinistro per salvare l&#39;avanzamento dello scenario.

   >[!IMPORTANT]
   >
   >Risparmia spesso quando affili e testa uno scenario.

>[!TIP]
>
>È consigliabile aggiungere note su ciascun modulo in modo facoltativo ma utile.
>
>1. Fare clic con il pulsante destro del mouse su un modulo di [!DNL Workfront], quindi scegliere **[!UICONTROL Aggiungi nota]**.
>1. Nella nota visualizzata, digita una panoramica del modulo.
>
>    È possibile aggiungere più note per un modulo.
>
>1. Chiudi l&#39;area **[!UICONTROL Note]**.
>
>     Dopo aver aggiunto una nota a uno scenario, un punto arancione viene visualizzato sull&#39;icona **[!UICONTROL Note]** ![](assets/notes-icon-w-dot.png) nella parte inferiore dell&#39;editor dello scenario.
>
>1. Fai clic sull&#39;icona **[!UICONTROL Note]** ![](assets/notes-icon-w-dot.png) per visualizzare le note.
>

## Attiva lo scenario

L’ultimo passaggio nella creazione di uno scenario è quello di attivarlo.

Poiché questo scenario è alla ricerca di un problema specifico, non è necessario attivarlo. L’attivazione di uno scenario ne determina l’esecuzione secondo una pianificazione o quando si verifica un’azione specifica in un’applicazione. Dopo aver attivato uno scenario, per impostazione predefinita viene eseguito ogni 15 minuti. Puoi modificare questa impostazione definendo quando e con quale frequenza desideri che venga eseguita.

Per ulteriori informazioni sull&#39;attivazione degli scenari, vedere [Attivare o disattivare uno scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Per informazioni sulle pianificazioni, vedere [Pianificare uno scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
