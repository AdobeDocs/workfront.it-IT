---
product-area: workfront-integrations;projects
keywords: google,documento,documento,foglio,diapositiva
navigation-topic: workfront-for-g-suite
title: Crea un'attività  [!DNL Adobe Workfront]  in Google Workspace utilizzando il contenuto dell'e-mail
description: È possibile convertire un'e-mail esterna (non generata da Adobe [!DNL Workfront]) in un'attività di Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Crea un&#39;attività [!DNL Adobe Workfront] in [!DNL Google Workspace] utilizzando il contenuto e-mail

>[!NOTE]
>
>La versione più recente del plug-in Adobe Workfront per Google è stata rilasciata il 26 giugno 2023.

È possibile convertire un&#39;e-mail esterna (non generata da [!DNL Adobe Workfront]) in un&#39;attività [!DNL Workfront].

Puoi anche convertire un’e-mail esterna in un aggiornamento per un’attività esistente. Per ulteriori informazioni, vedere [Aggiornare un [!DNL Adobe Workfront] elemento da [!DNL Google Workspace] utilizzando contenuto e-mail](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

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

Prima di poter creare un&#39;attività [!DNL Workfront] in [!DNL Google Workspace], è necessario

* Installa [!DNL Workfront for Google Workspace]\
   Per istruzioni, vedere [Installa [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Crea un&#39;attività [!DNL Adobe Workfront] in [!DNL Google Workspace] utilizzando il contenuto e-mail

1. Se il pannello [!UICONTROL Workfront for Google Workspace] non è visualizzato, fare clic sull&#39;icona [!DNL Workfront] ![icona Workfront](assets/wf-lion-icon.png) nella barra laterale dei componenti aggiuntivi [!DNL Google Workspace] all&#39;estrema destra della pagina.
1. Con il messaggio di posta elettronica aperto in [!DNL Google Workspace], fare clic su un&#39;opzione in [!DNL Workfront for Google Workspace] per convertire il messaggio in una nuova attività [!DNL Workfront].

1. Selezionare un&#39;opzione **[!UICONTROL Crea nuovo]** per indicare se l&#39;attività farà parte di un progetto o di un&#39;attività personale indipendente da un progetto.
1. Se si desidera allegare l&#39;attività a un progetto padre, fare clic su **[!UICONTROL Nome progetto]**, iniziare a digitare il nome del progetto in cui si desidera inserire l&#39;attività, quindi fare clic sul nome del progetto quando viene visualizzato nell&#39;elenco seguente.
1. Effettua una delle seguenti modifiche:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome attività]</td> 
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
      <td role="rowheader">[!UICONTROL Durata pianificata]</td> 
      <td> <p>Fai clic su <strong>[!UICONTROL Planned duration]</strong> (Durata pianificata), quindi digita il numero di giorni desiderati per l'attività. </p> <p>Nota: questa opzione può essere configurata per la tua organizzazione in modi diversi. Ad esempio, per la tua organizzazione, potrebbe essere necessario digitare un numero di ore invece di giorni. Per ulteriori informazioni, contattare l'amministratore [!DNL Workfront]. Se si desidera specificare un periodo di tempo diverso da quello predefinito configurato, digitare <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong> o <strong>mo</strong> dopo il numero per indicare minuti, ore, giorni, settimane o mesi.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Priorità </td> 
      <td>Fare clic sulla freccia dell'elenco a discesa, quindi selezionare la priorità desiderata per l'attività.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Includi allegati e-mail]</td> 
      <td> <p>(Disponibile solo se l’e-mail contiene almeno un allegato). Fare clic su questa opzione per salvare gli allegati nel messaggio di posta elettronica nell'area [!UICONTROL Documents] dell'attività. </p> <p>Se non si desidera salvare un allegato, fare clic sulla X a destra del nome. </p> <p>Se l'e-mail contiene collegamenti a documenti in [!DNL Google Drive], questi verranno salvati nella scheda [!UICONTROL Overview] (Panoramica) dell'attività che si sta creando. </p> <p>Importante: affinché questo funzioni, l'amministratore di [!DNL Workfront] deve autorizzare [!DNL Google Drive] a utilizzare i documenti in [!DNL Workfront], come descritto nella sezione <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurare le integrazioni per la gestione dei documenti</a> nell'articolo <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurare le integrazioni dei documenti</a>.</p> <p>Se abiliti questa opzione, questa rimane abilitata per altre e-mail convertite in attività, problemi e aggiornamenti.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email file]</td> 
      <td> <p>Fare clic su questa opzione per salvare l'e-mail originale come file e-mail (EML) <span>nell'area [!UICONTROL Documents]</span> dell'attività. A questo punto, puoi fare doppio clic sul file per aprire l’e-mail nell’applicazione e-mail.</p> <p>Se abiliti questa opzione, questa rimane abilitata per altre e-mail convertite in attività, problemi e aggiornamenti.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Crea attività]**.

   La scheda **[!UICONTROL Dettagli]** per la nuova attività viene visualizzata nel pannello [!DNL Workfront for Google Workspace]. Puoi fare clic su **[!UICONTROL Aggiornamenti]** e iniziare subito a comunicare con i collaboratori senza lasciare la casella in entrata.

   Nella parte inferiore della scheda **[!UICONTROL Dettagli]**, è inoltre possibile fare clic su **[!UICONTROL Visualizza in[!DNL Workfront]]** per passare alla nuova attività in Workfront.

   Quando aggiorni il browser, un messaggio con un collegamento nella parte inferiore del pannello [!DNL Workfront for Google Workspace] conferma che l&#39;e-mail è stata convertita in un&#39;attività:

   È possibile fare clic sul collegamento per passare alla visualizzazione Dettagli, nel pannello [!DNL Workfront for Google Workspace], per l&#39;attività creata.

   Puoi ripetere questi passaggi per convertire lo stesso messaggio e-mail in più attività. Quando si aggiorna il browser o si torna all&#39;e-mail in un secondo momento, tutti i collegamenti creati per l&#39;e-mail sono elencati nella parte inferiore del pannello [!UICONTROL Workfront for Google Workspace].

1. (Facoltativo) Continuare a lavorare con l&#39;attività nel pannello [!DNL Workfront for Google Workspace] eseguendo una delle operazioni seguenti:

   * Per aggiungere un aggiornamento nella scheda **[!UICONTROL Aggiornamenti]**, fare clic su **[!UICONTROL Avvia un nuovo aggiornamento]** e digitare l&#39;aggiornamento.

   * Per rispondere a un aggiornamento nella scheda **[!UICONTROL Aggiornamenti]**, fai clic su **[!UICONTROL Rispondi]** e digita la tua risposta.

     Per entrambe le azioni di cui sopra, puoi inviare una notifica a determinati utenti del commento. Fare clic su **[!UICONTROL Notifica]**, iniziare a digitare il nome di un utente, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa. Ripeti questo processo per gli altri utenti a cui vuoi inviare la notifica, quindi fai clic su **[!UICONTROL Post]**.

   * Fai clic sulla scheda **[!UICONTROL Documenti]** per visualizzare tutti i documenti salvati con l&#39;attività.

Puoi ripetere questi passaggi per convertire lo stesso messaggio e-mail in più attività. Quando si aggiorna il browser o si torna all&#39;e-mail in un secondo momento, tutti i collegamenti creati per l&#39;e-mail sono elencati nella parte inferiore del pannello [!DNL Workfront for Google Workspace].
