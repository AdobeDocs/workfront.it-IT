---
product-area: workfront-integrations;projects
keywords: google,documento,documento,foglio,diapositiva
navigation-topic: workfront-for-g-suite
title: Aggiorna un  [!DNL Adobe Workfront]  elemento da Google Workspace utilizzando il contenuto dell'e-mail
description: È possibile aggiornare un progetto, un’attività o un problema esistente con informazioni provenienti da un messaggio e-mail non Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Aggiorna un elemento [!DNL Adobe Workfront] da [!DNL Google Workspace] utilizzando il contenuto dell&#39;e-mail

>[!NOTE]
>
>La versione più recente del plug-in Adobe Workfront per Google è stata rilasciata il 26 giugno 2023.

È possibile aggiornare un progetto, un&#39;attività o un problema esistente con informazioni provenienti da un&#39;e-mail non [!DNL Adobe Workfront].

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

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Prerequisiti

Prima di poter aggiornare un elemento [!DNL Workfront] utilizzando il contenuto dell&#39;e-mail di [!DNL Google Workspace], è necessario

* Installa [!DNL Workfront for Google Workspace]\
   Per istruzioni, vedere [Installa [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Aggiorna un elemento [!DNL Workfront] utilizzando il contenuto dell&#39;e-mail da [!DNL Google Workspace]

1. Se il pannello [!UICONTROL Workfront for Google Workspace] non è visualizzato, fare clic sull&#39;icona di Workfront ![icona Workfront](assets/wf-lion-icon.png) nella barra laterale dei componenti aggiuntivi [!DNL Google Workspace] all&#39;estrema destra della pagina.
1. Con il messaggio di posta elettronica aperto in [!DNL Google Workspace], fai clic su **[!UICONTROL Pubblica come nuovo aggiornamento]** nel pannello [!DNL Google Workspace].
1. In **[!UICONTROL Tipo]** fare clic sulla freccia dell&#39;elenco a discesa, quindi sul tipo di oggetto in cui si desidera aggiungere l&#39;aggiornamento.
1. Fai clic sull&#39;opzione **[!UICONTROL Cerca]**, inizia a digitare il nome dell&#39;oggetto in cui desideri aggiungere l&#39;aggiornamento, quindi seleziona l&#39;elemento quando viene visualizzato nell&#39;elenco seguente.

   Questa opzione varia a seconda di quanto selezionato al punto 3. Potrebbe essere **[!UICONTROL Cerca un progetto]**, **[!UICONTROL Cerca un&#39;attività]** o **[!UICONTROL Cerca un problema]**.

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
      <td><p>(Disponibile solo se l’e-mail contiene almeno un allegato). Fare clic su questa opzione per salvare gli allegati nella scheda [!UICONTROL Documents] per l'attività o il problema. </p><p>Se non si desidera salvare un allegato, fare clic sulla X a destra del nome. </p><p>Se l'e-mail contiene collegamenti a documenti in [!DNL Google Drive], tali collegamenti vengono salvati nella scheda Panoramica di [!UICONTROL] dell'attività o del problema che si sta creando. </p><p>Importante: <span style="color: #ff1493;"><span style="color: #000000;">Affinché questo funzioni, l'amministratore</span></span>[!DNL Workfront]<span style="color: #ff1493;"><span style="color: #000000;"> deve autorizzare [!DNL Google Drive] a lavorare con [!DNL Workfront]</span></span></p>
      <p>Se abiliti questa opzione, questa rimane abilitata per altre e-mail convertite in attività, problemi e aggiornamenti.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notifica</td> 
      <td>Fare clic su <strong>[!UICONTROL Notify]</strong>, fare clic sull'opzione <strong>[!UICONTROL Cerca un utente o un team]</strong> visualizzata, quindi iniziare a digitare il nome della persona o del team e fare clic su di esso quando viene visualizzato nell'elenco seguente. Ripetere questa operazione per ogni persona e team che si desidera aggiungere, quindi fare clic su <strong>[!UICONTROL Salva]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Aggiorna]**.

   Quando si aggiorna il browser, un messaggio con un collegamento nella parte inferiore del pannello [!DNL Workfront for Google Workspace] conferma che l&#39;e-mail è stata convertita in aggiornamento:

   È possibile fare clic sul collegamento per passare alla scheda [!UICONTROL Aggiornamenti] in [!DNL Workfront] per l&#39;oggetto specificato al passaggio 4.

   Puoi ripetere questi passaggi per convertire lo stesso messaggio e-mail in aggiornamenti, attività e problemi (vedi [Creare un problema Adobe Workfront in [!DNL Google Workspace] utilizzando il contenuto dell&#39;e-mail](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Quando si aggiorna il browser o si torna all&#39;e-mail in un secondo momento, tutti i collegamenti creati per l&#39;e-mail sono elencati nella parte inferiore del pannello [!UICONTROL Workfront for Google Workspace].

1. (Facoltativo) Continuare a lavorare con l&#39;aggiornamento nel pannello dei componenti aggiuntivi [!DNL Workfront] eseguendo una delle operazioni seguenti:

   * Per aggiungere un altro aggiornamento nella scheda **[!UICONTROL Aggiornamenti]**, fare clic su **[!UICONTROL Avvia un nuovo aggiornamento]** e digitare le informazioni.

   * Per rispondere a un aggiornamento nella scheda **[!UICONTROL Aggiornamenti]**, fai clic su **[!UICONTROL Rispondi]** e digita la tua risposta.

     Per entrambe le opzioni di cui sopra, è possibile fare clic su **[!UICONTROL Notifica]** per specificare i destinatari per la risposta, come nel passaggio 5. Quando sei pronto, fai clic su **[!UICONTROL Post]** per aggiungere l&#39;aggiornamento o rispondere.

   * Fai clic sulla scheda **[!UICONTROL Dettagli]** per visualizzare i dettagli del nuovo progetto, attività o problema.
