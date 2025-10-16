---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Accesso necessario per utilizzare Scenario Planner
description: Scenario Planner richiede una licenza separata da Adobe Workfront e accesso aggiuntivo.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 1b06589a705cf218239ff1273b865c05e4ceb96f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Accesso necessario per utilizzare [!DNL Scenario Planner]

<!--Audited: 04/2024-->

<!--The [!DNL Scenario Planner] has additional license requirements. For information about the [!DNL Workfront Scenario Planner], see [The [!DNL Scenario Planner] overview](../scenario-planner/scenario-planner-overview.md).-->

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Senza l&#39;accesso o le autorizzazioni corrette, potresti non essere in grado di visualizzare l&#39;area [!UICONTROL Scenari] di[!DNL  Adobe Workfront] né di gestire piani o iniziative per la tua organizzazione. La gestione di piani e iniziative include la creazione, la modifica e l&#39;eliminazione.

## Accesso necessario per visualizzare e utilizzare [!DNL Adobe Workfront Scenario Planner]

Prima di poter accedere a [!DNL Workfront Scenario Planner], è necessario verificare che siano soddisfatte tutte le seguenti condizioni:

1. La tua organizzazione deve disporre di un pacchetto Workfront Ultimate.

   La funzione Pianificazione scenario non è disponibile per i pacchetti flusso di lavoro di Workfront.

   Parla con il rappresentante del tuo account Workfront se stai rinnovando Workfront e desideri mantenere Scenario Planner.

   Se si è un nuovo cliente, Scenario Planner non è più disponibile per l&#39;acquisto.

   <!--Old: 
    Depending on whether you use the new or the current Workfront plan, your organization must have one of the following:
    * For the new plans, your organization must have the  [!UICONTROL Ultimate] [!DNL Workfront] plan. The Scenario Planner is included only in the [!UICONTROL Ultimate] plan. 
    * For the current Workfront plans, your organization must have both of the following: 
      * Your organization must purchase a [!DNL Workfront] [!UICONTROL Business] or higher [!DNL Workfront] plan. 
      
      * Your organization must purchase a [!DNL Workfront Scenario Planner] license, in addition to a [!DNL Workfront] license. Contact your [!DNL Workfront] Account Representative to learn about [!DNL Workfront Scenario Planner] licenses. -->

1. È necessario disporre di una delle seguenti licenze Workfront:

   * [!UICONTROL Chiaro] o versione successiva
   * [!UICONTROL Revisore] o versione successiva

   <!--Old: 
      * For the current licenses: 
        * [!UICONTROL Plan]
        * [!UICONTROL Work]
        * [!UICONTROL Review]-->
   <!--Old: 
      >[!NOTE]
      > 
      >* When using the new licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
      >
      >* When using the current licenses, users with a Request or External license type cannot access the Scenario Planner. -->

1. L&#39;amministratore di [!DNL Workfront] deve concedere a [!UICONTROL View] o [!UICONTROL Edit] l&#39;accesso a [!DNL Scenario Planner] nel proprio livello di accesso.

   Per informazioni sulla concessione dell&#39;accesso a [!DNL Workfront Scenario Planner], vedere [Concedere l&#39;accesso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Facoltativo e consigliato) Per visualizzare o aggiornare le informazioni finanziarie per i piani e le iniziative, l&#39;amministratore [!DNL Workfront] deve inoltre concedere l&#39;accesso a [!UICONTROL Dati finanziari] nel proprio livello di accesso. Per informazioni sulla concessione di dati finanziari nel proprio livello di accesso, vedere [Concedere l&#39;accesso ai dati finanziari](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).


<!--1. (Optional) If you need to access plans you didn't create, a plan creator must give you the correct permissions to their plan to access it. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.-->

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

<!--Repetitive from above?? 

## Access needed to view plans and initiatives

In addition to your company acquiring the correct license for the [!DNL Workfront Scenario Planner], your [!DNL Workfront] administrator must also assign you the following access and setup so you can view the [!DNL Workfront Scenario Planner] and the information in this area:

* An access level with at least [!UICONTROL View] access to [!DNL Scenario Planner].

  For information about the access level to [!DNL Scenario Planner], see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* An access level with at least [!UICONTROL View] access to [!UICONTROL Financial Data] if you need to also view financial information about the plan and the initiatives. Some examples of financial information are budgets, costs, or job role rates.

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Requestors] and [!UICONTROL External] Users do not have access to view the [!DNL Scenario Planner].

* View permissions to the plan. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

## Access needed to manage plans and initiatives

Your [!DNL Workfront] administrator must assign you the following access so you can manage plans and their information in the [!DNL Scenario Planner]:

* A [!UICONTROL Plan] or [!UICONTROL Work] license type with Edit access to the [!DNL Scenario Planner] in your access level.

  All other license types do not have access to manage plans.

  For information about granting access to [!DNL Scenario Planner] from the Access Level, see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Plan] license type with [!UICONTROL Edit] access to [!UICONTROL Financial Data] in your access level, if you need to also update financial information about the plan.

  Some examples of financial information that you can edit are [!UICONTROL Budget], [!UICONTROL Planned Benefit], and [!UICONTROL Fixed Costs].

  >[!TIP]
  >
  >Only [!UICONTROL Plan] license holders have [!UICONTROL Edit] access to [!UICONTROL Financial Data].

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Manage permissions to a plan that you didn't create. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

-->

## Autorizzazioni necessarie per accedere a piani e iniziative

I livelli di accesso collaborano con le autorizzazioni in [!DNL Workfront] per dare visibilità ai piani e alle iniziative non creati. Oltre a disporre del livello di accesso corretto per accedere a [!DNL Scenario Planner], è necessario disporre delle autorizzazioni corrette per i piani che si desidera visualizzare o gestire, se non si è il creatore di tali piani.

Tutti gli utenti, inclusi gli amministratori di sistema, possono accedere solo ai piani creati.

Per visualizzare i piani creati da altri utenti, è necessario condividerli con l&#39;utente nei modi seguenti:

* Condividi il piano con te

  Per informazioni sulla condivisione dei piani, vedere [Condividere un piano in [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

* Invia un collegamento a un piano creato

  Se un utente condivide un collegamento a un piano senza condividerlo, è possibile richiedere le autorizzazioni per il piano. Per informazioni sulla richiesta delle autorizzazioni per i piani, vedere [Richiedere l&#39;accesso a un piano in [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

>[!NOTE]
>
>Quando un utente viene disattivato, i suoi piani non hanno alcun proprietario e non sono accessibili a meno che non siano stati condivisi in precedenza con un collegamento.


