---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Creare uno scenario semplice in [!DNL Adobe Workfront Fusion]
description: Scopri come creare uno scenario di automazione semplice con Adobe Workfront Fusion. Gli scenari di automazione automatizzano i processi Workfront, inclusa la manipolazione e la trasformazione dei dati. Questo esempio illustra il processo di creazione di uno scenario che cerca un problema e lo converte in un progetto.
author: Becky
hide: true
hidefromtoc: true
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '1260'
ht-degree: 0%

---

# Creare uno scenario di base in [!DNL Adobe Workfront Fusion]

Il ruolo di [!DNL Adobe Workfront Fusion] automatizzare i processi in modo da potersi concentrare su nuove attività anziché ripetere più volte le stesse attività. Funziona tramite il collegamento di azioni all’interno e tra app e servizi per creare uno scenario che trasferisce e trasforma automaticamente i dati. Lo scenario in cui si creano controlli i dati in un’app o in un servizio ed elabora tali dati in modo da fornire il risultato desiderato.

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

1. In **Scenari** , fare clic su **Crea un nuovo scenario**.

   <!--To locate the Scenarios area, see navigation article-->

   Viene visualizzato l’editor scenario, contenente un modulo vuoto al centro.

   <!--picture?-->

1. Seleziona la **[!UICONTROL Nuovo scenario]** nome segnaposto nell&#39;angolo superiore sinistro, quindi immettere un nome.
1. Continua con [Aggiungere e configurare il primo modulo](#add-and-configure-the-first-module) di seguito.

### Aggiungere e configurare il primo modulo

1. Fai clic sul modulo vuoto per scegliere l’app dalla quale selezionare un modulo.

   A destra del modulo viene visualizzato un elenco di app.

1. Seleziona **[!DNL Adobe Workfront]**. Se non è visibile, fare clic sulla barra di ricerca nella parte inferiore dell&#39;elenco, digitare &quot;Workfront&quot; e selezionarla quando viene visualizzata nell&#39;elenco.

   L’elenco viene modificato in visualizza tutto [!DNL Workfront] moduli che è possibile utilizzare.

1. Fai clic su **[!UICONTROL Ricerca]** modulo.

   Viene visualizzata la finestra di configurazione del modulo.

1. In [!UICONTROL Connessione] selezionare la connessione Workfront.

   Se non disponi di una connessione Workfront, consulta [Creare una connessione a [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. In [!UICONTROL Tipo di record] , seleziona **[!UICONTROL Problema]**. Questo imposta il modulo in modo che esegua la ricerca solo dei problemi.

   Puoi trovare **[!UICONTROL Problema]** nell’elenco, se inizi a digitare la parola &quot;[!UICONTROL problema].&quot;

1. In **[!UICONTROL Set di risultati]** , seleziona **[!UICONTROL Primo record corrispondente]**.

   In questo modo il modulo restituirà solo il primo record che soddisfa i criteri.
1. In **[!UICONTROL Criteri di ricerca]** , configura i criteri per restituire il problema specifico.

   1. Nella prima casella sotto [!UICONTROL Criteri di ricerca], seleziona il campo da includere nella ricerca. Per questo esempio, seleziona **[!UICONTROL Nome]**.

      Puoi trovare **[!UICONTROL Nome]** nell’elenco, se inizi a digitare la parola &quot;[!UICONTROL nome].&quot;
   1. Per l’operatore, fai clic sulla freccia a discesa accanto a **Esiste** e cambiarlo in [!UICONTROL **Contiene (senza distinzione maiuscole/minuscole)**].

      Questo consente al modulo di trovare i progetti il cui nome contiene le parole scelte, anche se non si inserisce il nome completo o si inserisce il nome con lettere maiuscole non corrette.
   1. Nell’ultimo campo in [!UICONTROL Criteri di ricerca], immetti una parola o una frase che sai essere nel nome del problema che stai cercando.

1. In **[!UICONTROL Uscite]** selezionare i campi che si desidera vengano generati dal modulo. Per questo esempio, seleziona la **[!UICONTROL ID]** e **[!UICONTROL Nome]** campi.

   >[!TIP]
   >
   >È possibile utilizzare **Cmd+F** ([!DNL Mac] OS) o **Ctrl+F** ([!DNL Windows] OS) per trovare rapidamente un campo.

1. Clic **[!UICONTROL OK]** per salvare la configurazione del modulo.

1. Fai clic con il pulsante destro del mouse sul modulo e fai clic su **[!UICONTROL Rinomina]**, quindi digita un nome che descriva le operazioni che desideri eseguire il modulo (ad esempio, &quot;Ricerca problema&quot;), quindi fai clic su **[!UICONTROL OK]**.

   Il nome viene visualizzato appena sotto il modulo. Sotto, [!DNL Workfront Fusion] include una breve descrizione del tipo di azione eseguita dal modulo.

   ![](assets/)

1. Continua con [Aggiungere e configurare il secondo modulo](#add-and-configure-the-second-module).

## Aggiungere e configurare il secondo modulo

1. Passa il puntatore del mouse sul cerchio parziale a destra della sezione del modulo, quindi fai clic su **[!UICONTROL Aggiungi un altro modulo]**.
1. Seleziona [!DNL Adobe Workfront] dall’elenco delle applicazioni, scegli il modulo **[!UICONTROL Azione Varie]**.

   Il modulo Azioni varie consente di eseguire in Workfront azioni che non dispongono di un modulo dedicato. In questo esempio, questo modulo viene utilizzato per convertire il problema in un progetto.
1. In [!UICONTROL Connessione] , seleziona la stessa connessione Workfront utilizzata nel modulo precedente .
1. Nel **[!UICONTROL Tipo di record]**campo, seleziona **[!UICONTROL Problema]**, perché l’azione da eseguire è correlata a un problema.
1. In **[!UICONTROL Azione]** campo, seleziona **convertToProject**. Questa è l&#39;azione che convertirà il problema selezionato in un progetto.
1. Fai clic su **[!UICONTROL ID]** campo.

   Viene visualizzato un pannello che consente di selezionare cosa utilizzare come ID del problema da convertire in un progetto. Il pannello include l’output di tutti i moduli precedenti. Poiché hai selezionato ID come output del modulo precedente, ora è disponibile nel pannello.

   Questo pannello è denominato pannello di mappatura. Per ulteriori informazioni sul pannello di mappatura, consulta [Mappare le informazioni da un modulo all&#39;altro](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Seleziona **ID** nel pannello mappatura.

   Nel campo ID viene visualizzato un blocco ID. Mostra il numero del modulo da cui è mappato e il campo mappato.

   ![ID mappa](assets/map-id.png)

1. (Facoltativo) Nella sezione Progetto, individua il campo ID proprietario e inizia a digitare il tuo nome nel campo, quindi selezionalo quando viene visualizzato. Questo ti imposta come proprietario del progetto e lo renderà più facile da trovare in Workfront.

   >[!TIP]
   >
   >È possibile utilizzare **Cmd+F** ([!DNL Mac] OS) o **Ctrl+F** ([!DNL Windows] OS) per trovare rapidamente un campo.

1. Clic **[!UICONTROL OK]** per salvare la configurazione del modulo.

1. Fai clic con il pulsante destro del mouse sul modulo e fai clic su **[!UICONTROL Rinomina]**, quindi digita un nome che descriva le operazioni che desideri eseguire il modulo (ad esempio &quot;Converti in progetto&quot;), quindi fai clic su **[!UICONTROL OK]**.

1. Continua con [Verifica lo scenario](#test-the-scenario).

## Verifica lo scenario

Prima di attivare lo scenario, è importante testarlo eseguendolo almeno una volta e visualizzando i risultati. Questo ti aiuta a capire come i dati scorrono attraverso lo scenario e a trovare eventuali errori.

In questo caso, se il test ha esito positivo, il problema viene individuato e convertito in un progetto.

1. Clic **[!UICONTROL Esegui una volta]** nell’angolo inferiore sinistro dell’editor di scenari.
1. Al termine dell’esecuzione dello scenario, fai clic sul fumetto sopra il primo modulo per visualizzare informazioni sul bundle di dati elaborato dal modulo, inclusi i dati estratti dal problema restituito dal modulo.

1. Fai clic sul fumetto del controllo dell’esecuzione sopra il secondo modulo per visualizzare l’input (il problema) e l’output (il progetto convertito).

   Per ulteriori informazioni sui dati contenuti nelle bolle di ispezione, vedere:

   * Per informazioni generali, consulta [Flusso di esecuzione dello scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Per informazioni sui bundle elaborati, consulta [Esecuzione di scenari, cicli e fasi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. In entrata [!DNL Workfront Fusion], fai clic su **[!UICONTROL Salva]** nell’angolo in basso a sinistra per salvare i progressi sullo scenario.

   >[!IMPORTANT]
   >
   >Risparmia spesso quando affili e testa uno scenario.

>[!TIP]
>
>È consigliabile aggiungere note su ciascun modulo in modo facoltativo ma utile.
>
>1. Fare clic con il pulsante destro del mouse su una [!DNL Workfront] , quindi fai clic su **[!UICONTROL Aggiungi una nota]**.
>1. Nella nota visualizzata, digita una panoramica del modulo.
>
>    È possibile aggiungere più note per un modulo.
>
>1. Chiudi **[!UICONTROL Note]** area.
>
>     Dopo aver aggiunto una nota a uno scenario, sulla schermata viene visualizzato un punto arancione **[!UICONTROL Note]** icona ![](assets/notes-icon-w-dot.png) nella parte inferiore dell’editor dello scenario.
>
>1. Fai clic su **[!UICONTROL Note]** icona ![](assets/notes-icon-w-dot.png) per visualizzare le note.
>

## Attiva lo scenario

L’ultimo passaggio nella creazione di uno scenario è quello di attivarlo.

Poiché questo scenario è alla ricerca di un problema specifico, non è necessario attivarlo. L’attivazione di uno scenario ne determina l’esecuzione secondo una pianificazione o quando si verifica un’azione specifica in un’applicazione. Dopo aver attivato uno scenario, per impostazione predefinita viene eseguito ogni 15 minuti. Puoi modificare questa impostazione definendo quando e con quale frequenza desideri che venga eseguita.

Per ulteriori informazioni sull’attivazione degli scenari, consulta [Attivare o disattivare uno scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Per informazioni sulle pianificazioni, consulta [Pianificare uno scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
