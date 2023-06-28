---
product-area: workfront-integrations;projects
keywords: google,documento,documento,foglio,diapositiva
navigation-topic: workfront-for-g-suite
title: Aggiornare un [!DNL Adobe Workfront] elemento di G Suite tramite contenuti e-mail
description: È possibile aggiornare un progetto, un’attività o un problema esistente con informazioni provenienti da un messaggio e-mail non Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Aggiornare un [!DNL Adobe Workfront] elemento da [!DNL G Suite] utilizzo di contenuti e-mail

>[!NOTE]
>
>La versione più recente del plug-in Adobe Workfront per Google è stata rilasciata il 26 giugno 2023.

È possibile aggiornare un progetto, un’attività o un problema esistente con informazioni provenienti da un[!DNL Adobe Workfront] e-mail.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Lavoro], [!UICONTROL Piano]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Prerequisiti

Prima di aggiornare un [!DNL Workfront] elemento che utilizza il contenuto dell&#39;e-mail da [!DNL G Suite], è necessario

* Installa [!DNL Workfront for G suite]\
   Per istruzioni, consulta [Installa [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Aggiornare un [!DNL Workfront] elemento che utilizza il contenuto dell&#39;e-mail da [!DNL G Suite]

1. Se il [!UICONTROL Workfront per G Suite] non viene visualizzato, fai clic sull’icona Workfront ![](assets/wf-lion-icon.png) nel [!DNL G Suite] barra laterale dei componenti aggiuntivi all’estrema destra della pagina.
1. Con il messaggio e-mail aperto in [!DNL G Suite], fai clic su **[!UICONTROL Pubblica come nuovo aggiornamento]** nel [!DNL G Suite] pannello.
1. Sotto **[!UICONTROL Tipo]**, fare clic sulla freccia dell&#39;elenco a discesa, quindi sul tipo di oggetto in cui si desidera aggiungere l&#39;aggiornamento.
1. Fai clic su **[!UICONTROL Cerca]** , inizia a digitare il nome dell&#39;oggetto in cui desideri aggiungere l&#39;aggiornamento, quindi seleziona l&#39;elemento quando viene visualizzato nell&#39;elenco seguente.

   Questa opzione varia a seconda di quanto selezionato al punto 3. Potrebbe essere **[!UICONTROL Cercare un progetto]**, **[!UICONTROL Cercare un’attività]**, o **[!UICONTROL Cercare un problema]**.

   >[!NOTE]
   >
   >Quando si digita il nome di un&#39;attività, le attività personali ad hoc vengono escluse dall&#39;elenco dei nomi visualizzato di seguito.

1. Effettua una delle seguenti modifiche facoltative:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Update]</td> 
      <td>Modifica qualsiasi parte del testo, che viene presa dalla riga dell’oggetto e dal corpo del messaggio e-mail.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Includi allegati e-mail]</td> 
      <td><p>(Disponibile solo se l’e-mail contiene almeno un allegato). Fare clic su questa opzione per salvare gli allegati nella scheda [!UICONTROL Documents] per l'attività o il problema. </p><p>Se non si desidera salvare un allegato, fare clic sulla X a destra del nome. </p><p>Se l’e-mail contiene collegamenti a documenti in [!DNL Google Drive], i collegamenti vengono salvati nella scheda Panoramica dell'attività o del problema che si sta creando. </p><p>Importante: <span style="color: #ff1493;"><span style="color: #000000;">Affinché questo funzioni, il tuo</span></span>[!DNL Workfront] amministratore<span style="color: #ff1493;"><span style="color: #000000;"> deve autorizzare [!DNL Google Drive] per utilizzare [!DNL Workfront]</span></span></p>
      <p>Se abiliti questa opzione, questa rimane abilitata per altre e-mail convertite in attività, problemi e aggiornamenti.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notifica</td> 
      <td>Clic <strong>[!UICONTROL Notify]</strong>, fare clic su <strong>[!UICONTROL Cerca un utente o un team]</strong> , quindi inizia a digitare il nome della persona o del team e fai clic su di esso quando viene visualizzato nell’elenco seguente. Ripeti l’operazione per ogni persona e team che desideri aggiungere, quindi fai clic su <strong>[!UICONTROL Salva]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Aggiorna]**.

   Quando aggiorni il browser, un messaggio con un collegamento nella parte inferiore della [!DNL Workfront for G Suite] il pannello conferma che l’e-mail è stata convertita in aggiornamento:

   Puoi fare clic sul collegamento per passare alla [!UICONTROL Aggiornamenti] scheda in [!DNL Workfront] per l&#39;oggetto specificato nel passaggio 4.

   Puoi ripetere questi passaggi per convertire lo stesso messaggio e-mail in aggiornamenti, attività e problemi (consulta [Crea un problema Adobe Workfront in [!DNL G Suite] utilizzando il contenuto dell&#39;e-mail](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Quando aggiorni il browser o torni all’e-mail in un altro momento, tutti i collegamenti creati per l’e-mail sono elencati in fondo alla sezione [!UICONTROL Workfront per G Suite] pannello.

1. (Facoltativo) Continua a lavorare con l’aggiornamento nella sezione [!DNL Workfront] pannello dei componenti aggiuntivi eseguendo una delle operazioni seguenti:

   * Per aggiungere un altro aggiornamento al **[!UICONTROL Aggiornamenti]** , fare clic su **[!UICONTROL Avvia un nuovo aggiornamento]** e digita le informazioni.

   * Per rispondere a un aggiornamento sul **[!UICONTROL Aggiornamenti]** , fare clic su **[!UICONTROL Rispondi]** e digita la tua risposta.

     Per entrambe le opzioni precedenti, puoi fare clic su **[!UICONTROL Notifica]** per specificare i destinatari della risposta, come nel passaggio 5. Quando sei pronto, fai clic su **[!UICONTROL Pubblica]** per aggiungere l’aggiornamento o la risposta.

   * Fai clic su **[!UICONTROL Dettagli]** per visualizzare i dettagli del nuovo progetto, attività o problema.
