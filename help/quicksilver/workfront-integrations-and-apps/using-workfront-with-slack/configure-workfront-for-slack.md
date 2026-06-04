---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Configura [!DNL Adobe Workfront] per Slack
description: L'integrazione di [!DNL Adobe Workfront] con Slack consente di accedere e creare [!DNL Workfront] elementi di lavoro, approvazioni, preferiti ed elementi recenti di Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
TQID: https://experienceleague.adobe.com/rOccEnbPoWVh5LFVPCeX81S3Nl-VpEBGGfcNDNXEdPk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 417
ht-degree: 6%

---

# Configurare [!DNL Adobe Workfront for Slack]

L&#39;integrazione di [!DNL Adobe Workfront] con [!DNL Slack] consente di effettuare le seguenti operazioni:

* Accedi a [!DNL Workfront] elementi di lavoro, approvazioni, preferiti ed elementi recenti da [!DNL Slack].
* Iscriviti, approva, assegna lavoro da [!DNL Slack].
* Crea attività e problemi da [!DNL Slack].
* Ricevi [!DNL Workfront] notifiche in [!DNL Slack].

A seconda della configurazione dell&#39;ambiente [!DNL Slack], è possibile installare e configurare [!DNL Workfront for Slack] autonomamente oppure l&#39;amministratore di [!DNL Workfront] deve installarlo e configurarlo prima di poterlo configurare autonomamente.

Quando integri l&#39;istanza [!DNL Slack] con [!DNL Workfront], gli utenti possono utilizzare [!DNL Workfront] durante la collaborazione all&#39;interno dei loro canali [!DNL Slack]. L&#39;integrazione può essere utilizzata da qualsiasi ambiente [!DNL Slack], inclusa l&#39;app mobile [!DNL Slack]. ## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Qualsiasi</p>
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti per l&#39;utilizzo di [!DNL Workfront] con [!DNL Slack]

* È necessaria un&#39;istanza [!DNL Slack].
* L&#39;amministratore di sistema [!DNL Slack] deve consentire a tutti gli utenti [!DNL Slack] di installare [!DNL Workfront for Slack].
* È necessario disporre di una licenza [!DNL Workfront] per poter utilizzare le funzionalità integrate in [!DNL Workfront].

  >[!NOTE]
  >
  >Gli utenti con qualsiasi tipo di licenza [!DNL Workfront] possono accedere a [!DNL Workfront] da [!DNL Slack]. Le azioni eseguibili da [!DNL Slack] sono limitate ai livelli di licenza e autorizzazione di [!DNL Workfront].

Per ulteriori informazioni sulla gestione delle app in [!DNL Slack], consulta [Gestione delle app per il tuo Workspace.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Installa [!DNL Workfront for Slack]

Ogni utente [!DNL Slack] deve installare l&#39;app [!DNL Workfront] per utilizzare [!DNL Workfront] da [!DNL Slack].

Puoi installare l’app nei seguenti modi:

* [Installa l&#39; [!DNL Workfront] app all&#39;esterno [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Installa l&#39; [!DNL Workfront] app entro [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Installa l&#39;app [!DNL Workfront] fuori da [!DNL Slack] {#install-the-workfront-app-outside-slack}

Per eseguire il processo di installazione e autorizzare [!DNL Workfront for Slack] nell&#39;istanza di [!DNL Slack], attenersi alla procedura seguente.

>[!IMPORTANT]
>
>Quando viene rilasciata una nuova versione di [!DNL Workfront] per Slack, è necessario autorizzare nuovamente l&#39;app per continuare a utilizzarla.

1. Individua il componente aggiuntivo [!DNL Adobe Workfront] nell&#39;archivio [[!DNL Slack] store](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Fai clic su **[!UICONTROL Apri in[!DNL Slack]]**.

1. Accedi all&#39;area di lavoro specificando l&#39;URL [!DNL Slack] e facendo clic su **[!UICONTROL Continua]**.\

1. Esaminare l&#39;accesso richiesto da [!DNL Slack]. Se accetti questo accesso, fai clic su **[!UICONTROL Consenti accesso]** per autorizzare l&#39;app [!DNL Workfront].

È ora possibile accedere a [!DNL Workfront] da [!DNL Slack], come descritto in [Accesso [!DNL Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Installa l&#39;app [!DNL Workfront] in [!DNL Slack] {#install-the-workfront-app-within-slack}

È possibile installare l&#39;app [!DNL Workfront] direttamente dall&#39;applicazione [!DNL Slack]:

1. Passa all&#39;URL [!DNL Slack].

   Ad esempio: *`<YourTeamName>`.slack.com/apps*.

   Oppure

   Fai clic sull&#39;icona **[!UICONTROL Aggiungi app]** nella tua istanza di [!DNL Slack].

1. Inizia a digitare *[!DNL Workfront]* nel campo di ricerca.
1. Premere Invio.
1. Selezionare l&#39;app **[!DNL Workfront]**.
1. Fare clic su **[!UICONTROL Impostazioni]**.

   Viene visualizzata la pagina Directory app.

1. Fai clic su **[!UICONTROL Visita sito app]**.
1. Fare clic su **[!UICONTROL Aggiungi a[!DNL Slack]]**.
1. Seguire la procedura per completare l&#39;installazione.
1. Al termine dell&#39;installazione, è possibile accedere a [!DNL Workfront] da [!DNL Slack], come descritto in [[!UICONTROL Access [!DNL Workfront] from [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
