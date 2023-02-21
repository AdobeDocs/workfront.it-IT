---
product-area: workfront-integrations;projects
keywords: google,doc,documento,foglio,diapositiva
navigation-topic: workfront-for-g-suite
title: Aggiornare un [!DNL Adobe Workfront] elemento da G Suite utilizzando il contenuto e-mail
description: Puoi aggiornare un progetto, un’attività o un problema esistente con le informazioni provenienti da un’e-mail non Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 925e8f9d57d65fcb44068274800450d9db5c9d34
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Aggiornare un [!DNL Adobe Workfront] elemento da [!DNL G Suite] utilizzo del contenuto e-mail

>[!NOTE]
>
>C&#39;è una [problema noto](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) con la versione corrente di [!DNL Workfront for G Suite] non funziona come previsto. Stiamo lavorando a una nuova versione e ci aspettiamo che venga rilasciata al [!DNL Google Marketplace] nel prossimo futuro.

È possibile aggiornare un progetto, un&#39;attività o un problema esistente con le informazioni di un[!DNL Adobe Workfront] e-mail.

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
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Prerequisiti

Prima di poter aggiornare un [!DNL Workfront] elemento che utilizza il contenuto di e-mail da [!DNL G Suite], devi

* Installa [!DNL Workfront for G suite]\
   Per istruzioni, consulta [Installa [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Aggiornare un [!DNL Workfront] elemento che utilizza il contenuto di e-mail da [!DNL G Suite]

1. Se la [!UICONTROL Workfront per G Suite] Il pannello non è visualizzato, fai clic sull’icona Workfront ![](assets/wf-lion-icon.png) in [!DNL G Suite] barra laterale dei componenti aggiuntivi all’estrema destra della pagina.
1. Con il messaggio e-mail aperto in [!DNL G Suite], fai clic su **[!UICONTROL Pubblica come nuovo aggiornamento]** in [!DNL G Suite] pannello.
1. Sotto **[!UICONTROL Tipo]**, fai clic sulla freccia a discesa, quindi fai clic sul tipo di oggetto in cui desideri aggiungere l’aggiornamento.
1. Fai clic sul pulsante **[!UICONTROL Cerca]** inizia a digitare il nome dell&#39;oggetto in cui desideri aggiungere l&#39;aggiornamento, quindi seleziona l&#39;elemento quando viene visualizzato nell&#39;elenco seguente.

   Questa opzione varia a seconda di quanto selezionato al punto 3. Potrebbe essere **[!UICONTROL Cercare un progetto]**, **[!UICONTROL Ricerca di un’attività]** oppure **[!UICONTROL Cercare un problema]**.

   >[!NOTE]
   >
   >Quando si digita il nome di un&#39;attività, le attività personali ad hoc vengono escluse dall&#39;elenco di nomi riportato di seguito.

1. Apporta una delle seguenti modifiche facoltative:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Update]</td> 
      <td>Modifica qualsiasi parte di questo testo, prelevata dalla riga dell’oggetto e dal testo del corpo dell’e-mail.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Includi allegati e-mail]</td> 
      <td><p>Disponibile solo se l’e-mail contiene almeno un allegato. Fai clic su questa opzione per salvare gli allegati nella scheda [!UICONTROL Documents] per l’attività o il problema. </p><p>Se non si desidera salvare un allegato, fare clic sulla X a destra del nome. </p><p>Se l’e-mail contiene collegamenti a documenti in [!DNL Google Drive], i collegamenti vengono salvati nella scheda [!UICONTROL Overview] dell’attività o del problema che si sta creando. </p><p>Importante: <span style="color: #ff1493;"><span style="color: #000000;">Affinché questo funzioni, il tuo</span></span>[!DNL Workfront] amministratore<span style="color: #ff1493;"><span style="color: #000000;"> deve autorizzare [!DNL Google Drive] per lavorare con [!DNL Workfront]</span></span></p>
      <p>Se abiliti questa opzione, rimane abilitata per altre e-mail che vengono convertite in attività, problemi e aggiornamenti.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notifica</td> 
      <td>Fai clic su <strong>Notifica di [!UICONTROL]</strong>, fai clic su <strong>[!UICONTROL Cerca un utente o un team]</strong> viene visualizzata l'opzione , quindi inizia a digitare il nome della persona o del team e fai clic su di esso quando viene visualizzato nell'elenco seguente. Ripeti questa operazione per ogni persona e team che desideri aggiungere, quindi fai clic su <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Aggiorna]**.

   Quando si aggiorna il browser, viene visualizzato un messaggio con un collegamento nella parte inferiore della sezione [!DNL Workfront for G Suite] Il pannello conferma che l’e-mail è stata convertita in un aggiornamento:

   Puoi fare clic sul collegamento per passare alla [!UICONTROL Aggiornamenti] scheda in [!DNL Workfront] per l&#39;oggetto specificato al punto 4.

   Puoi ripetere questi passaggi per convertire la stessa e-mail in aggiornamenti, attività e problemi (vedi [Creare un problema Adobe Workfront in [!DNL G Suite] utilizzando il contenuto e-mail](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Quando aggiorni il browser o ritorni all’e-mail in un altro momento, tutti i collegamenti creati per l’e-mail sono elencati nella parte inferiore della [!UICONTROL Workfront per G Suite] pannello.

1. (Facoltativo) Continua a lavorare con l’aggiornamento nel [!DNL Workfront] pannello aggiuntivo eseguendo una delle operazioni seguenti:

   * Per aggiungere un altro aggiornamento nel **[!UICONTROL Aggiornamenti]** scheda , fai clic su **[!UICONTROL Avvia un nuovo aggiornamento]** e digitare le informazioni.

   * Per rispondere a un aggiornamento sul **[!UICONTROL Aggiornamenti]** scheda , fai clic su **[!UICONTROL Rispondi]** e digita la risposta.

      Per entrambe le opzioni di cui sopra, puoi fare clic su **[!UICONTROL Notifica]** specificare i destinatari della risposta come al punto 5. Quando sei pronto, fai clic su **[!UICONTROL Post]** per aggiungere l&#39;aggiornamento o la risposta.

   * Fai clic sul pulsante **[!UICONTROL Dettagli]** scheda per visualizzare i dettagli del nuovo progetto, attività o problema.
