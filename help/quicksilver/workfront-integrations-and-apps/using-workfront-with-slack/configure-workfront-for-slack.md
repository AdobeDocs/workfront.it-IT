---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Configura [!DNL Adobe Workfront] per Slack
description: Integrazione [!DNL Adobe Workfront] con Slack consente di accedere e creare [!DNL Workfront] articoli da lavoro, approvazioni, preferiti, articoli recenti dallo Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Configura [!DNL Adobe Workfront for Slack]

Integrazione [!DNL Adobe Workfront] con [!DNL Slack] consente di effettuare le seguenti operazioni:

* Accedi alle [!DNL Workfront] articoli da lavoro, approvazioni, preferiti, articoli recenti da [!DNL Slack].
* Iscriviti, approva, assegna lavoro da [!DNL Slack].
* Crea attività e problemi da [!DNL Slack].
* Ricevi alcune [!DNL Workfront] notifiche in [!DNL Slack].

A seconda di come [!DNL Slack] l&#39;ambiente è configurato, è possibile installare e configurare [!DNL Workfront for Slack] tu o il tuo [!DNL Workfront] prima di configurarlo autonomamente, è necessario che l’amministratore lo installi e lo configuri.

Quando si integra il [!DNL Slack] istanza con [!DNL Workfront] gli utenti possono utilizzare [!DNL Workfront] collaborando nel loro [!DNL Slack] canali. L’integrazione può essere utilizzata da qualsiasi [!DNL Slack] ambiente, compresi [!DNL Slack] app mobile.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] piano]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.\

## Prerequisiti per l’utilizzo [!DNL Workfront] con [!DNL Slack]

* Devi avere un [!DNL Slack] istanza.
* Le [!DNL Slack] l&#39;amministratore di sistema deve consentire [!DNL Slack] utenti da installare [!DNL Workfront for Slack].
* Devi avere un [!DNL Workfront] per poter utilizzare le funzioni integrate in [!DNL Workfront].

   >[!NOTE]
   >
   >Utenti con qualsiasi [!DNL Workfront] tipo di licenza accessibile [!DNL Workfront] da [!DNL Slack]. Azioni eseguibili da [!DNL Slack] sono limitate alle [!DNL Workfront] livelli di licenza e autorizzazione.

Per ulteriori informazioni sulla gestione delle app in [!DNL Slack], vedi [Gestisci le app per il tuo spazio di lavoro.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Installa [!DNL Workfront for Slack]

Ogni [!DNL Slack] l&#39;utente deve installare [!DNL Workfront] per utilizzare [!DNL Workfront] da [!DNL Slack].

Puoi installare l’app nei seguenti modi:

* [Installa il [!DNL Workfront] app esterna [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Installa il [!DNL Workfront] all&#39;interno dell&#39;app [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Installa il [!DNL Workfront] app esterna [!DNL Slack] {#install-the-workfront-app-outside-slack}

Segui i passaggi seguenti per eseguire il processo di installazione e autorizzare [!DNL Workfront for Slack] sul tuo [!DNL Slack] istanza.

>[!IMPORTANT]
>
>Quando una nuova versione di [!DNL Workfront] per il rilascio dello Slack, è necessario riautorizzare l’app per continuare a utilizzarla.

1. Individua il [!DNL Adobe Workfront] componente aggiuntivo nel [[!DNL Slack] archiviare](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Fai clic su **[!UICONTROL Apri in[!DNL Slack]]**.

1. Accedi all’area di lavoro specificando il tuo [!DNL Slack] URL e clic **[!UICONTROL Continua]**.\

1. Esamina l’accesso che [!DNL Slack] richiede. Se accetti questo accesso, fai clic su **[!UICONTROL Consenti accesso]** autorizzare [!DNL Workfront] app.

Ora puoi accedere a [!DNL Workfront] da [!DNL Slack], come descritto nel [Accesso [!DNL Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Installa il [!DNL Workfront] all&#39;interno dell&#39;app [!DNL Slack] {#install-the-workfront-app-within-slack}

È possibile installare [!DNL Workfront] direttamente dall’app [!DNL Slack] domanda:

1. Passa alla [!DNL Slack] URL.

   Ad esempio: *`<YourTeamName>`.slack.com/apps*.

   Oppure

   Fai clic sul pulsante **[!UICONTROL Aggiungi app]** nella tua [!DNL Slack] istanza.

1. Inizia a digitare *[!DNL Workfront]* nel campo di ricerca.
1. Premere Invio.
1. Seleziona la **[!DNL Workfront]** app.
1. Fai clic su **[!UICONTROL Impostazioni]**.

   Viene visualizzata la pagina Directory app .

1. Fai clic su **[!UICONTROL Visita sito app]**.
1. Fai clic su **[!UICONTROL Aggiungi a[!DNL Slack]]**.
1. Segui i passaggi per completare l&#39;installazione.
1. Al termine dell&#39;installazione, puoi accedere a [!DNL Workfront] da [!DNL Slack], come descritto nel [Accesso a [!DNL Workfront] da [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
