---
product-area: workfront-integrations;projects
keywords: google,documento,documento,foglio,diapositiva
navigation-topic: workfront-for-g-suite
title: Crea un  [!DNL Adobe Workfront]  problema in Google Workspace utilizzando il contenuto dell'e-mail
description: Puoi convertire un'e-mail esterna (non generata da [!DNL Adobe Workfront)] in un [!DNL Workfront] problema.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# Crea un problema [!DNL Adobe Workfront] in [!DNL Google Workspace] utilizzando il contenuto dell&#39;e-mail

>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Nell&#39;ambito di questo processo di transizione, le seguenti funzionalità di Workfront per Google Workspace non saranno disponibili dopo il **28 febbraio 2026**:
>
>* Accesso alle funzionalità di Google Workspace da Workfront
>
>* Visualizzazione e gestione delle attività di Workfront da Gmail o dal pannello del sito Calendario di Google
>
>È consigliabile utilizzare l&#39;automazione e l&#39;integrazione di Workfront per le esigenze di integrazione dell&#39;organizzazione con Google Workspace.
>
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Google Workspace, vedere [Moduli Gmail](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) e [Moduli calendario Google](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

È possibile convertire un&#39;e-mail esterna (non generata da [!DNL Adobe Workfront]) in un problema [!DNL Workfront].

Puoi anche convertire un’e-mail esterna in un aggiornamento per un problema esistente. Per ulteriori informazioni, vedere [Aggiornare un [!DNL Adobe Workfront] elemento da [!DNL Google Workspace] utilizzando contenuto e-mail](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Per informazioni sull&#39;utilizzo di [!DNL Google Workspace] per utilizzare le e-mail di notifica inviate da [!DNL Workfront], vedere [Gestisci [!DNL Adobe Workfront] dettagli notifica da [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

Prima di poter creare un problema da [!DNL Google Workspace], è necessario

* Installa [!DNL Workfront for Google Workspace]\
   Per istruzioni, vedere [Installa [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Crea un problema di [!DNL Adobe Workfront] in [!DNL Google Workspace] utilizzando il contenuto dell&#39;e-mail

1. Se il pannello [!UICONTROL Workfront for Google Workspace] non è visualizzato, fare clic sull&#39;icona [!DNL Workfront] ![icona Workfront](assets/wf-lion-icon.png) nella barra laterale dei componenti aggiuntivi [!DNL Google Workspace] all&#39;estrema destra della pagina.
1. Con il messaggio e-mail aperto in [!DNL Google Workspace], fai clic su un&#39;opzione in [!DNL Workfront for Google Workspace] per convertire l&#39;e-mail in un nuovo problema di [!DNL Workfront].

   ![Converti e-mail](assets/convert-email-task-issue-update.png)

1. Se si desidera allegare il problema a un progetto padre, fare clic su **[!UICONTROL Nome progetto]**, iniziare a digitare il nome del progetto in cui si desidera inserire il problema, quindi fare clic sul nome del progetto quando viene visualizzato nell&#39;elenco seguente.
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
      <td>Fare clic su <strong>[!UICONTROL Assegna a]</strong>, fare clic sull'opzione <strong>[!UICONTROL Assegna a]</strong> visualizzata, quindi iniziare a digitare il nome della persona e fare clic su di esso quando viene visualizzato nell'elenco seguente. Ripetere l'operazione per ogni persona che si desidera aggiungere, quindi fare clic su <strong>[!UICONTROL Salva]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Priorità </td> 
      <td>Fai clic sulla freccia a discesa, quindi fai clic sulla priorità desiderata per il problema.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Includi allegati e-mail]</td> 
      <td> <p>(Disponibile solo se l’e-mail contiene almeno un allegato). Fai clic su questa opzione per salvare gli allegati nel messaggio e-mail per l’area [!UICONTROL Documents] del problema. </p> <p>Se non si desidera salvare un allegato, fare clic sulla X a destra del nome. </p> <p>Se l'e-mail contiene collegamenti a documenti in [!DNL Google Drive], questi verranno salvati nella scheda [!UICONTROL Overview] (Panoramica) del problema che si sta creando. </p> <p>Importante: affinché questo funzioni, l'amministratore di [!DNL Workfront] deve autorizzare [!DNL Google Drive] a utilizzare i documenti in [!DNL Workfront], come descritto nella sezione <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurare le integrazioni per la gestione dei documenti</a> nell'articolo <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurare le integrazioni dei documenti</a>.</p> <p>Se abiliti questa opzione, questa rimane abilitata per altre e-mail convertite in attività, problemi e aggiornamenti.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Includi file e-mail</td> 
      <td> <p>Fai clic su questa opzione per salvare l'e-mail originale come file e-mail (EML) <span>nell'area [!UICONTROL Documents]</span> del problema. A questo punto, puoi fare doppio clic sul file per aprire l’e-mail nell’applicazione e-mail.</p> <p>Se abiliti questa opzione, questa rimane abilitata per altre e-mail convertite in attività, problemi e aggiornamenti.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Crea problema]**.

   La scheda **[!UICONTROL Dettagli]** per il nuovo problema viene visualizzata nel pannello [!DNL Workfront for Google Workspace]. Puoi fare clic su **[!UICONTROL Aggiornamenti]** e iniziare subito a comunicare con i collaboratori senza lasciare la casella in entrata.

   Nella parte inferiore della scheda **[!UICONTROL Dettagli]**, puoi anche fare clic su **[!UICONTROL Visualizza in Workfront]** per passare al nuovo problema in Workfront.

   Quando aggiorni il browser, un messaggio con un collegamento nella parte inferiore del pannello [!UICONTROL Workfront for Google Workspace] conferma che l&#39;e-mail è stata convertita in un problema:

   È possibile fare clic sul collegamento per passare alla visualizzazione Dettagli, nel pannello [!DNL Workfront for Google Workspace], per il problema creato.

   Puoi ripetere questi passaggi per convertire la stessa e-mail in più problemi. Quando si aggiorna il browser o si torna all&#39;e-mail in un secondo momento, tutti i collegamenti creati per l&#39;e-mail sono elencati nella parte inferiore del pannello [!UICONTROL Workfront for Google Workspace].

1. (Facoltativo) Continuare a lavorare con il problema nel pannello [!DNL Workfront for Google Workspace] eseguendo una delle operazioni seguenti:

   * Per aggiungere un aggiornamento nella scheda **[!UICONTROL Aggiornamenti]**, fare clic su **[!UICONTROL Avvia un nuovo aggiornamento]** e digitare l&#39;aggiornamento.

   * Per rispondere a un aggiornamento nella scheda **[!UICONTROL Aggiornamenti]**, fai clic su **[!UICONTROL Rispondi]** e digita la tua risposta.

     Per entrambe le azioni di cui sopra, puoi inviare una notifica a determinati utenti del commento. Fare clic su **[!UICONTROL Notifica]**, iniziare a digitare il nome di un utente, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa. Ripeti questo processo per gli altri utenti a cui vuoi inviare la notifica, quindi fai clic su **[!UICONTROL Post]**.

   * Fai clic sulla scheda **[!UICONTROL Documenti]** per visualizzare tutti i documenti salvati con il problema.
