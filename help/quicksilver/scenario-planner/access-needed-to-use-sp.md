---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Accesso necessario per utilizzare la Pianificazione scenario
description: Scenario Planner richiede una licenza separata da Adobe Workfront e accesso aggiuntivo.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: cf3b5d3f8e3a8a1922da757a41b4c5e0ee84e6fd
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# Accesso necessario per utilizzare [!DNL Scenario Planner]

<!--Audited: 04/2024-->

[!DNL Scenario Planner] ha requisiti di licenza aggiuntivi. Per informazioni su [!DNL Workfront Scenario Planner], vedere [The [!DNL Scenario Planner] overview](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Senza l&#39;accesso o le autorizzazioni corrette, potresti non essere in grado di visualizzare l&#39;area [!UICONTROL Scenari] di[!DNL  Adobe Workfront] né di gestire piani o iniziative per la tua organizzazione. La gestione di piani e iniziative include la creazione, la modifica e l&#39;eliminazione.

## Accesso necessario per visualizzare e utilizzare [!DNL Adobe Workfront Scenario Planner]

Prima di poter accedere a [!DNL Workfront Scenario Planner], è necessario verificare che siano soddisfatte tutte le seguenti condizioni:

1. L&#39;organizzazione deve disporre di uno dei piani Workfront descritti di seguito.

   A seconda che si utilizzi il piano Workfront nuovo o corrente, l&#39;organizzazione deve disporre di uno dei seguenti elementi:

   * Per i nuovi piani, l&#39;organizzazione deve disporre del piano [!UICONTROL Ultimate] [!DNL Workfront]. Pianificazione scenario incluso solo nel piano [!UICONTROL Ultimate].

   * Per i piani Workfront correnti, l&#39;organizzazione deve disporre di entrambi i seguenti elementi:

      * La tua organizzazione deve acquistare un piano [!DNL Workfront] [!UICONTROL Business] o superiore [!DNL Workfront]. Per informazioni sui piani [!DNL Workfront], vedere [Piani Workfront](https://www.workfront.com/plans).

      * La tua organizzazione deve acquistare una licenza di [!DNL Workfront Scenario Planner], oltre a una licenza di [!DNL Workfront]. Contatta il rappresentante commerciale [!DNL Workfront] per informazioni sulle licenze di [!DNL Workfront Scenario Planner].

1. È necessario disporre di una delle licenze Workfront descritte di seguito.

   A seconda che si utilizzino le licenze nuove o correnti, l&#39;amministratore [!DNL Workfront] deve assegnare all&#39;utente una licenza di uno dei seguenti tipi:

   * Per le nuove licenze:
      * [!UICONTROL Standard]
      * [!UICONTROL Chiaro]

   * Per le licenze correnti:

      * [!UICONTROL Piano]
      * [!UICONTROL Lavoro]
      * [!UICONTROL Revisione]

   >[!NOTE]
   > 
   >* Quando si utilizzano le nuove licenze, gli utenti con un tipo di licenza [!UICONTROL Collaboratore] o [!UICONTROL Esterno] non possono accedere a [!DNL Scenario Planner].
   >
   >* Quando si utilizzano le licenze correnti, gli utenti con un tipo di licenza Request (Richiesta) o External (Esterno) non possono accedere alla Pianificazione scenario.

1. L&#39;amministratore di [!DNL Workfront] deve concedere a [!UICONTROL View] o [!UICONTROL Edit] l&#39;accesso a [!DNL Scenario Planner] nel proprio livello di accesso.

   Per informazioni sulla concessione dell&#39;accesso a [!DNL Workfront Scenario Planner], vedere [Concedere l&#39;accesso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Facoltativo e consigliato) Per visualizzare o aggiornare le informazioni finanziarie per i piani e le iniziative, l&#39;amministratore [!DNL Workfront] deve inoltre concedere l&#39;accesso a [!UICONTROL Dati finanziari] nel proprio livello di accesso. Per informazioni sulla concessione di dati finanziari nel proprio livello di accesso, vedere [Concedere l&#39;accesso ai dati finanziari](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

1. (Facoltativo) Se devi accedere ai piani che non hai creato, un creatore di piani deve darti le autorizzazioni corrette per il proprio piano per accedervi. Per informazioni sulle autorizzazioni necessarie per accedere a piani e iniziative non creati, vedere la sezione [Autorizzazioni necessarie per accedere a piani e iniziative](#permissions-needed-to-access-plans-and-initiatives) in questo articolo.

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## Accesso necessario per visualizzare piani e iniziative

Oltre all&#39;acquisizione della licenza corretta per [!DNL Workfront Scenario Planner] da parte dell&#39;azienda, l&#39;amministratore di [!DNL Workfront] deve anche assegnare il seguente accesso e la seguente configurazione in modo da poter visualizzare [!DNL Workfront Scenario Planner] e le informazioni in quest&#39;area:

* Livello di accesso con almeno [!UICONTROL Visualizzazione] di accesso a [!DNL Scenario Planner].

  Per informazioni sul livello di accesso a [!DNL Scenario Planner], vedere [Concedere l&#39;accesso a  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Un livello di accesso con almeno l&#39;accesso [!UICONTROL Visualizzazione] a [!UICONTROL Dati finanziari] per visualizzare anche le informazioni finanziarie sul piano e sulle iniziative. Alcuni esempi di informazioni finanziarie sono i budget, i costi o i tassi di ruolo.

  Per informazioni sul livello di accesso [!UICONTROL Dati finanziari], vedere [Concedere l&#39;accesso ai dati finanziari](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Richiedenti] e [!UICONTROL Utenti esterni] non hanno accesso alla visualizzazione di [!DNL Scenario Planner].

* Visualizzare le autorizzazioni per il piano. Per informazioni sulle autorizzazioni necessarie per accedere a piani e iniziative non creati, vedere la sezione [Autorizzazioni necessarie per accedere a piani e iniziative](#permissions-needed-to-access-plans-and-initiatives) in questo articolo.

## Accesso necessario per gestire piani e iniziative

L&#39;amministratore di [!DNL Workfront] deve assegnare il seguente accesso in modo da poter gestire i piani e le relative informazioni in [!DNL Scenario Planner]:

* Un tipo di licenza [!UICONTROL Piano] o [!UICONTROL Lavoro] con accesso di modifica a [!DNL Scenario Planner] nel tuo livello di accesso.

  Tutti gli altri tipi di licenza non dispongono dell&#39;accesso per gestire i piani.

  Per informazioni sulla concessione dell&#39;accesso a [!DNL Scenario Planner] dal livello di accesso, vedere [Concedere l&#39;accesso a  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Un tipo di licenza [!UICONTROL Plan] con accesso [!UICONTROL Edit] a [!UICONTROL Financial Data] nel tuo livello di accesso, se devi aggiornare anche le informazioni finanziarie sul piano.

  Alcuni esempi di informazioni finanziarie che è possibile modificare sono [!UICONTROL Budget], [!UICONTROL Vantaggio pianificato] e [!UICONTROL Costi fissi].

  >[!TIP]
  >
  >Solo i [!UICONTROL titolari di licenza Pianificazione] dispongono dell&#39;accesso [!UICONTROL Modifica] a [!UICONTROL Dati finanziari].

  Per informazioni sul livello di accesso [!UICONTROL Dati finanziari], vedere [Concedere l&#39;accesso ai dati finanziari](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Gestisci le autorizzazioni per un piano che non hai creato. Per informazioni sulle autorizzazioni necessarie per accedere a piani e iniziative non creati, vedere la sezione [Autorizzazioni necessarie per accedere a piani e iniziative](#permissions-needed-to-access-plans-and-initiatives) in questo articolo.

## Autorizzazioni necessarie per accedere a piani e iniziative

I livelli di accesso collaborano con le autorizzazioni in [!DNL Workfront] per dare visibilità ai piani e alle iniziative non creati. Oltre a disporre del livello di accesso corretto per accedere a [!DNL Scenario Planner], è necessario disporre delle autorizzazioni corrette per il piano che si desidera visualizzare o gestire, se non si è il creatore di tali piani.

Tutti gli utenti, inclusi gli amministratori di sistema, possono accedere solo ai piani creati.

Per visualizzare i piani creati da altri utenti, è necessario condividerli con l&#39;utente nei modi seguenti:

* Condividi il piano con te

  Per informazioni sulla condivisione dei piani, vedere [Condividere un piano in [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

* Invia un collegamento a un piano creato

  Se un utente condivide un collegamento a un piano senza condividerlo, è possibile richiedere le autorizzazioni per il piano. Per informazioni sulla richiesta delle autorizzazioni per i piani, vedere [Richiedere l&#39;accesso a un piano in [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

>[!NOTE]
>
>Quando un utente viene disattivato, i suoi piani non hanno alcun proprietario e non sono accessibili a meno che non siano stati condivisi in precedenza con un collegamento.


