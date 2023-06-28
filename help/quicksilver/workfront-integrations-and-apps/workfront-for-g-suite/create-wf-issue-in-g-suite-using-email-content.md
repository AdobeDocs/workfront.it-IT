---
product-area: workfront-integrations;projects
keywords: google,documento,documento,foglio,diapositiva
navigation-topic: workfront-for-g-suite
title: Creare un [!DNL Adobe Workfront] problema in G Suite con l’utilizzo di contenuti e-mail
description: Puoi convertire un’e-mail esterna (non generata da [!DNL Adobe Workfront)] a un [!DNL Workfront] problema.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Creare un [!DNL Adobe Workfront] problema in [!DNL G Suite] utilizzo di contenuti e-mail

>[!NOTE]
>
>La versione più recente del plug-in Adobe Workfront per Google è stata rilasciata il 26 giugno 2023.

Puoi convertire un’e-mail esterna (non generata da [!DNL Adobe Workfront]) a un [!DNL Workfront] problema.

Puoi anche convertire un’e-mail esterna in un aggiornamento per un problema esistente. Per ulteriori informazioni, consulta [Aggiornare un [!DNL Adobe Workfront] elemento di [!DNL G Suite] che utilizza contenuto e-mail](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Per informazioni sull&#39;utilizzo di [!DNL G Suite] utilizzare le e-mail di notifica inviate da [!DNL Workfront], vedi [Gestisci [!DNL Adobe Workfront] dettagli di notifica da [!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

Prima di poter creare un problema da [!DNL G Suite], è necessario

* Installa [!DNL Workfront for G suite]\
   Per istruzioni, consulta [Installa [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Creare un [!DNL Adobe Workfront] problema in [!DNL G Suite] utilizzo di contenuti e-mail

1. Se il [!UICONTROL Workfront per G Suite] non viene visualizzato, fare clic sul pulsante [!DNL Workfront] icona ![](assets/wf-lion-icon.png) nel [!DNL G Suite] barra laterale dei componenti aggiuntivi all’estrema destra della pagina.
1. Con il messaggio e-mail aperto in [!DNL G Suite], fare clic su un&#39;opzione in [!DNL Workfront for G Suite] per convertire l’e-mail in una nuova [!DNL Workfront] problema.

   ![](assets/convert-email-task-issue-update.png)

1. Se desideri allegare il problema a un progetto principale, fai clic su **[!UICONTROL Nome progetto]**, inizia a digitare il nome del progetto in cui desideri risolvere il problema, quindi fai clic sul nome del progetto quando viene visualizzato nell’elenco seguente.
1. Effettua una delle seguenti modifiche:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Issue Name]</td> 
      <td>Modifica qualsiasi parte del testo, tratta dall’oggetto dell’e-mail.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Modifica qualsiasi parte del testo, tratta dal corpo dell’e-mail.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Assegna A]</td> 
      <td>Clic <strong>[!UICONTROL Assegna A]</strong>, fare clic su <strong>[!UICONTROL Assegna a]</strong> , quindi inizia a digitare il nome della persona e fai clic su di esso quando viene visualizzato nell’elenco seguente. Ripeti l’operazione per ogni persona che desideri aggiungere, quindi fai clic su <strong>[!UICONTROL Salva]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Priorità [!UICONTROL]</td> 
      <td>Fai clic sulla freccia a discesa, quindi fai clic sulla priorità desiderata per il problema.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Includi allegati e-mail]</td> 
      <td> <p>(Disponibile solo se l’e-mail contiene almeno un allegato). Fai clic su questa opzione per salvare gli allegati nel messaggio e-mail per l’area [!UICONTROL Documents] del problema. </p> <p>Se non si desidera salvare un allegato, fare clic sulla X a destra del nome. </p> <p>Se l’e-mail contiene collegamenti a documenti in [!DNL Google Drive], vengono salvate nella scheda Panoramica [!UICONTROL] del problema che si sta creando. </p> <p>Importante: affinché questo funzioni, il tuo [!DNL Workfront] l’amministratore deve autorizzare [!DNL Google Drive] per lavorare con i documenti in [!DNL Workfront], come descritto nella sezione <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurare le integrazioni per gestire i documenti</a> nell’articolo <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurare le integrazioni dei documenti</a>.</p> <p>Se abiliti questa opzione, questa rimane abilitata per altre e-mail convertite in attività, problemi e aggiornamenti.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Includi file e-mail</td> 
      <td> <p>Fai clic su questa opzione per salvare l’e-mail originale come file e-mail (EML) <span>nell'area [!UICONTROL Documents]</span> dell'emissione. A questo punto, puoi fare doppio clic sul file per aprire l’e-mail nell’applicazione e-mail.</p> <p>Se abiliti questa opzione, questa rimane abilitata per altre e-mail convertite in attività, problemi e aggiornamenti.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Crea un problema]**.

   Il **[!UICONTROL Dettagli]** per il nuovo problema viene visualizzata nella scheda [!DNL Workfront for G Suite] pannello. Puoi fare clic su **[!UICONTROL Aggiornamenti]** e iniziare a comunicare con i collaboratori immediatamente senza lasciare il tuo spazio nella casella.

   Nella parte inferiore della sezione **[!UICONTROL Dettagli]** , puoi anche fare clic su **[!UICONTROL Visualizza in Workfront]** per passare al nuovo problema in Workfront.

   Quando aggiorni il browser, un messaggio con un collegamento nella parte inferiore della [!UICONTROL Workfront per G Suite] il pannello conferma che l’e-mail è stata convertita in un problema:

   È possibile fare clic sul collegamento per passare alla visualizzazione Dettagli, all&#39;interno del [!DNL Workfront for G Suite] per il problema creato.

   Puoi ripetere questi passaggi per convertire la stessa e-mail in più problemi. Quando aggiorni il browser o torni all’e-mail in un altro momento, tutti i collegamenti creati per l’e-mail sono elencati in fondo alla sezione [!UICONTROL Workfront per G Suite] pannello.

1. (Facoltativo) Continua a lavorare con il problema nel [!DNL Workfront for G Suite] eseguendo una delle operazioni seguenti:

   * Per aggiungere un aggiornamento al **[!UICONTROL Aggiornamenti]** , fare clic su **[!UICONTROL Avvia un nuovo aggiornamento]** e digita l’aggiornamento.

   * Per rispondere a un aggiornamento sul **[!UICONTROL Aggiornamenti]** , fare clic su **[!UICONTROL Rispondi]** e digita la tua risposta.

     Per entrambe le azioni di cui sopra, puoi inviare una notifica a determinati utenti del commento. Clic **[!UICONTROL Notifica]**, inizia a digitare il nome di un utente, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa. Ripeti questo processo per altri utenti a cui desideri inviare la notifica, quindi fai clic su **[!UICONTROL Pubblica]**.

   * Fai clic su **[!UICONTROL Documenti]** per visualizzare tutti i documenti salvati con il problema.
