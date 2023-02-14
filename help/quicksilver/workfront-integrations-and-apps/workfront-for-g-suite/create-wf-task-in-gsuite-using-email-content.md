---
product-area: workfront-integrations;projects
keywords: google,doc,documento,foglio,diapositiva
navigation-topic: workfront-for-g-suite
title: Crea un [!DNL Adobe Workfront] attività in G Suite utilizzando il contenuto e-mail
description: Puoi convertire un’e-mail esterna (non generata da Adobe) [!DNL Workfront]) a un’attività Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 0934ae23a8e80dd18872efef7d274bd57d227647
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# Crea un [!DNL Adobe Workfront] in [!DNL G Suite] utilizzo del contenuto e-mail

>[!NOTE]
>
>C&#39;è una [problema noto](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) con la versione corrente di [!DNL Workfront for G Suite] non funziona come previsto. Stiamo lavorando a una nuova versione e ci aspettiamo che venga rilasciata al [!DNL Google Marketplace] nel prossimo futuro.

Puoi convertire un’e-mail esterna (non generata da [!DNL Adobe Workfront]) a [!DNL Workfront] compito.

Puoi anche convertire un’e-mail esterna in un aggiornamento relativo a un’attività esistente. Per ulteriori informazioni, consulta [Aggiornare un [!DNL Adobe Workfront] elemento di [!DNL G Suite] tramite contenuto e-mail](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Per informazioni sull&#39;utilizzo [!DNL G Suite] per lavorare con le e-mail di notifica inviate da [!DNL Workfront], vedi [Gestisci [!DNL Adobe Workfront] dettagli di notifica da [!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

Prima di creare un [!DNL Workfront] in [!DNL G Suite], devi

* Installa [!DNL Workfront for G suite]\
   Per istruzioni, consulta [Installa [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Crea un [!DNL Adobe Workfront] in [!DNL G Suite] utilizzo del contenuto e-mail

1. Se la [!UICONTROL Workfront per G Suite] il pannello non è visualizzato, fai clic sul pulsante [!DNL Workfront] icona ![](assets/wf-lion-icon.png) in [!DNL G Suite] barra laterale dei componenti aggiuntivi all’estrema destra della pagina.
1. Con il messaggio e-mail aperto in [!DNL G Suite], fai clic su un’opzione in [!DNL Workfront for G Suite] per convertire l’e-mail in una nuova [!DNL Workfront] compito.

   ![](assets/convert-email-task-issue-update.png)

1. Seleziona una **[!UICONTROL Crea nuovo]** per indicare se l’attività farà parte di un progetto o di un’attività personale indipendente da un progetto.
1. Se desideri allegare l’attività a un progetto principale, fai clic su **[!UICONTROL Nome del progetto]**, inizia a digitare il nome del progetto in cui desideri eseguire l’attività, quindi fai clic sul nome del progetto quando viene visualizzato nell’elenco seguente.
1. Apporta una delle seguenti modifiche:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome attività]</td> 
      <td>Modifica qualsiasi parte di questo testo, prelevata dalla riga dell’oggetto dell’e-mail.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Modifica qualsiasi parte di questo testo, prelevata dal corpo dell'e-mail.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Assegna A]</td> 
      <td>Fai clic su <strong>[!UICONTROL Assegna A]</strong>, fai clic su <strong>[!UICONTROL Assegna a]</strong> viene visualizzata, quindi inizia a digitare il nome della persona e fai clic su di esso quando viene visualizzato nell'elenco seguente. Ripeti questa operazione per ogni persona che desideri aggiungere, quindi fai clic su <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Durata pianificata]</td> 
      <td> <p>Fai clic su <strong>[!UICONTROL Durata pianificata]</strong>, quindi digitare il numero di giorni desiderati per l’esecuzione dell’attività. </p> <p>Nota: Questa opzione può essere configurata per la tua organizzazione in diversi modi. Ad esempio, per la tua organizzazione, potrebbe essere necessario digitare un numero di ore anziché di giorni. Se hai bisogno di ulteriori informazioni, consulta la [!DNL Workfront] amministratore. Se desideri specificare un periodo di tempo diverso da quello predefinito configurato, digita <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong>oppure <strong>mo</strong> dopo il numero di minuti, ore, giorni, settimane o mesi da indicare.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Fare clic sulla freccia a discesa, quindi sulla priorità desiderata per l'attività.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Includi allegati e-mail]</td> 
      <td> <p>Disponibile solo se l’e-mail contiene almeno un allegato. Fai clic su questa opzione per salvare gli allegati nell’e-mail nell’area Documenti dell’attività. </p> <p>Se non si desidera salvare un allegato, fare clic sulla X a destra del nome. </p> <p>Se l’e-mail contiene collegamenti a documenti in [!DNL Google Drive], vengono salvate nella scheda [!UICONTROL Overview] dell’attività che si sta creando. </p> <p>Importante: Affinché questo funzioni, il tuo [!DNL Workfront] l'amministratore deve autorizzare [!DNL Google Drive] per lavorare con i documenti in [!DNL Workfront], come descritto nella sezione <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurare le integrazioni per gestire i documenti</a> nell'articolo <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurare le integrazioni di documenti</a>.</p> <p>Se abiliti questa opzione, rimane abilitata per altre e-mail che vengono convertite in attività, problemi e aggiornamenti.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email file]</td> 
      <td> <p>Fai clic su questa opzione per salvare l’e-mail originale come file e-mail (EML) <span>all'area Documenti</span> del compito. Da lì, puoi fare doppio clic sul file per aprire l’e-mail nell’applicazione e-mail.</p> <p>Se abiliti questa opzione, rimane abilitata per altre e-mail che vengono convertite in attività, problemi e aggiornamenti.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Crea attività]**.

   La **[!UICONTROL Dettagli]** nella scheda della nuova attività [!DNL Workfront for G Suite] pannello. Puoi fare clic su **[!UICONTROL Aggiornamenti]** e iniziare subito a comunicare con i collaboratori senza lasciare la tua casella in entrata.

   Nella parte inferiore del **[!UICONTROL Dettagli]** puoi anche fare clic su **[!UICONTROL Visualizza in[!DNL Workfront]]** per passare alla nuova attività in Workfront.

   Quando si aggiorna il browser, viene visualizzato un messaggio con un collegamento nella parte inferiore della sezione [!DNL Workfront for G Suite] Il pannello conferma che l’e-mail è stata convertita in un’attività :

   ![](assets/email-was-converted.png)

   Puoi fare clic sul collegamento per passare alla visualizzazione Dettagli all&#39;interno della [!DNL Workfront for G Suite] per l’attività creata.

   Puoi ripetere questi passaggi per convertire la stessa e-mail in più attività. Quando aggiorni il browser o ritorni all’e-mail in un altro momento, tutti i collegamenti creati per l’e-mail sono elencati nella parte inferiore della [!UICONTROL Workfront per G Suite] pannello.

1. (Facoltativo) Continua a lavorare con l’attività nel [!DNL Workfront for G Suite] eseguendo una delle operazioni seguenti:

   * Per aggiungere un aggiornamento al **[!UICONTROL Aggiornamenti]** scheda , fai clic su **[!UICONTROL Avvia un nuovo aggiornamento]** e digitare l&#39;aggiornamento.

   * Per rispondere a un aggiornamento sul **[!UICONTROL Aggiornamenti]** scheda , fai clic su **[!UICONTROL Rispondi]** e digita la risposta.

      Per entrambe le azioni di cui sopra, è possibile inviare a utenti particolari il proprio commento. Fai clic su **[!UICONTROL Notifica]**, inizia a digitare il nome di un utente, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa. Ripeti questo processo per gli altri utenti a cui desideri inviare una notifica, quindi fai clic su **[!UICONTROL Post]**.

   * Fai clic sul pulsante **[!UICONTROL Documenti]** per visualizzare tutti i documenti salvati con l&#39;attività.

Puoi ripetere questi passaggi per convertire la stessa e-mail in più attività. Quando aggiorni il browser o ritorni all’e-mail in un altro momento, tutti i collegamenti creati per l’e-mail sono elencati nella parte inferiore della [!DNL Workfront for G Suite] pannello.
