---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Accesso necessario per utilizzare la Pianificazione scenario
description: Scenario Planner richiede una licenza separata da Adobe Workfront e accesso aggiuntivo.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Accesso necessario per utilizzare [!DNL Scenario Planner]

Il [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], vedi [Il [!DNL Scenario Planner] panoramica](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Senza l&#39;accesso o le autorizzazioni corrette, potrebbe non essere possibile visualizzare [!UICONTROL Scenari] area di[!DNL  Adobe Workfront] né gestire piani o iniziative per la tua organizzazione. La gestione di piani e iniziative include la creazione, la modifica e l&#39;eliminazione.

>[!IMPORTANT]
>
>Quando si accede a [!UICONTROL Scenari], è possibile visualizzare e gestire solo i piani creati. Se si desidera consentire ad altri utenti di visualizzare o gestire i piani creati, è necessario eseguire le operazioni seguenti:
>
>* Inviare un collegamento al piano ad altri utenti
>* Condividere il piano con altri utenti
>
>  Per informazioni sulla condivisione di un piano, consulta [Condividere un piano in [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>Quando un utente viene disattivato, i suoi piani non hanno alcun proprietario e non sono accessibili a meno che non siano stati condivisi in precedenza con un collegamento.

## Accesso necessario per visualizzare e utilizzare [!DNL Adobe Workfront Scenario Planner]

Prima di poter accedere a, è necessario verificare che siano soddisfatte tutte le seguenti condizioni [!DNL Workfront Scenario Planner]:

<!--drafted for P&P:

* Depending on whether you use the current or the legacy Workfront plans, your organization must have the following:

  * For the current plans:  

    * The [!UICONTROL Ultimate] [!DNL Workfront] plan.

      Or
  
    * The [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] plan, in addition to purchasing a separate [!DNL Scenario Planner] license.

  * For the legacy plans: (indent the bullets below, before the NOTE)

-->

* La tua organizzazione deve acquistare un [!DNL Workfront] [!UICONTROL Aziende] o superiore [!DNL Workfront] piano. Per informazioni su [!DNL Workfront] piani, vedi [Piani Workfront](https://workfront.com/plans).
* La tua organizzazione deve acquistare un [!DNL Workfront Scenario Planner] licenza, oltre a un [!DNL Workfront] licenza. Contatta il tuo [!DNL Workfront] Il rappresentante commerciale per saperne di più [!DNL Workfront Scenario Planner] licenze.

<!--drafted for P&P: 

* Depending on whether you use the current or legacy licenses, your [!DNL Workfront] administrator must assign you a license of any of the following types: 

  * For the current licenses: 
    * [!UICONTROL Standard]
    * [!UICONTROL Light]

  * For the legacy licenses: (re-indent the licenses below and reword the sentence)

-->



* Il tuo [!DNL Workfront] l&#39;amministratore deve assegnare all&#39;utente una licenza di uno dei seguenti elementi [!DNL Workfront] tipi:

   * [!UICONTROL Piano]
   * [!UICONTROL Lavoro]
   * [!UICONTROL Revisiona]

  >[!NOTE]
  >
  >Utenti con un [!UICONTROL Richiesta] o [!UICONTROL Esterno] il tipo di licenza non può accedere al [!DNL Workfront Scenario Planner].

<!--drafted - replace the note above with this at P&P release: 
  * When using the current licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
  * When using the legacy licenses, users with a Request or External license type cannot access the Scenario Planner. -->

* Il tuo [!DNL Workfront] l&#39;amministratore deve fornire [!UICONTROL Visualizza] o [!UICONTROL Modifica] accesso a [!DNL Scenario Planner] nel tuo livello di accesso.

  Per informazioni sulla concessione dell&#39;accesso al [!DNL Workfront Scenario Planner], vedi [Concedi l’accesso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* (Facoltativo e consigliato) Per visualizzare o aggiornare le informazioni finanziarie relative ai piani e alle iniziative, [!DNL Workfront] l&#39;amministratore deve inoltre concederti l&#39;accesso a [!UICONTROL Dati finanziari] nel tuo livello di accesso. Per informazioni sulla concessione di dati finanziari nel proprio livello di accesso, vedere [Concedere l’accesso ai dati finanziari](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  <!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

* Se è necessario accedere ai piani non creati, un creatore di piani deve assegnare le autorizzazioni corrette al proprio piano per accedervi. Per informazioni sulle autorizzazioni necessarie per accedere a piani e iniziative non creati, vedi [Autorizzazioni necessarie per accedere a piani e iniziative](#permissions-needed-to-access-plans-and-initiatives) in questo articolo.

## Accesso necessario per visualizzare piani e iniziative

Oltre all&#39;acquisizione della licenza corretta per [!DNL Workfront Scenario Planner], il tuo [!DNL Workfront] l&#39;amministratore deve inoltre assegnarti i seguenti diritti di accesso e configurazione in modo da poter visualizzare [!DNL Workfront Scenario Planner] e le informazioni in questo settore:

* Un livello di accesso con almeno [!UICONTROL Visualizza] accesso a [!DNL Scenario Planner].

  Per informazioni sul livello di accesso a [!DNL Scenario Planner], vedi [Concedi l’accesso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Un livello di accesso con almeno [!UICONTROL Visualizza] accesso a [!UICONTROL Dati finanziari] per visualizzare anche informazioni finanziarie sul piano e sulle iniziative. Alcuni esempi di informazioni finanziarie sono i budget, i costi o i tassi di ruolo.

  Per informazioni su [!UICONTROL Dati finanziari] livello di accesso, vedi [Concedere l’accesso ai dati finanziari](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Richiedenti] e [!UICONTROL Esterno] Gli utenti non hanno accesso alla visualizzazione [!DNL Scenario Planner].

* Visualizzare le autorizzazioni per il piano. Per informazioni sulle autorizzazioni necessarie per accedere a piani e iniziative non creati, vedi [Autorizzazioni necessarie per accedere a piani e iniziative](#permissions-needed-to-access-plans-and-initiatives) in questo articolo.

## Accesso necessario per gestire piani e iniziative

Il tuo [!DNL Workfront] l&#39;amministratore deve assegnare il seguente accesso in modo da poter gestire i piani e le relative informazioni in [!DNL Scenario Planner]:

* A [!UICONTROL Piano] o [!UICONTROL Lavoro] tipo di licenza con accesso di modifica a [!DNL Scenario Planner] nel tuo livello di accesso.

  Tutti gli altri tipi di licenza non dispongono dell&#39;accesso per gestire i piani.

  Per informazioni su come concedere l’accesso a [!DNL Scenario Planner] dal Livello d&#39;Accesso, vedi [Concedi l’accesso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Piano] tipo di licenza con [!UICONTROL Modifica] accesso a [!UICONTROL Dati finanziari] nel tuo livello di accesso, se devi aggiornare anche le informazioni finanziarie sul piano.

  Alcuni esempi di informazioni finanziarie che è possibile modificare sono [!UICONTROL Budget], [!UICONTROL Vantaggio pianificato], e [!UICONTROL Costi fissi].

  >[!TIP]
  >
  >Solo [!UICONTROL Piano] i titolari di licenza hanno [!UICONTROL Modifica] accesso a [!UICONTROL Dati finanziari].

  Per informazioni su [!UICONTROL Dati finanziari] livello di accesso, vedi [Concedere l’accesso ai dati finanziari](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Gestisci le autorizzazioni per un piano che non hai creato. Per informazioni sulle autorizzazioni necessarie per accedere a piani e iniziative non creati, vedi [Autorizzazioni necessarie per accedere a piani e iniziative](#permissions-needed-to-access-plans-and-initiatives) in questo articolo.

## Autorizzazioni necessarie per accedere a piani e iniziative

I livelli di accesso funzionano insieme alle autorizzazioni in [!DNL Workfront] per dare visibilità ai piani e alle iniziative che non sono stati creati. Oltre ad avere il corretto livello di accesso per accedere al [!DNL Scenario Planner], è inoltre necessario disporre delle autorizzazioni corrette per il piano che si desidera visualizzare o gestire, se non si è il creatore di tali piani.

Per impostazione predefinita, è possibile accedere solo ai piani creati. Per visualizzare i piani creati da altri utenti, è necessario condividerli con l&#39;utente. Per informazioni sulla condivisione dei piani, vedere [Condividere un piano in [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

Se un utente condivide un collegamento a un piano senza condividerlo, è possibile richiedere le autorizzazioni per il piano. Per informazioni sulla richiesta di autorizzazioni ai piani, consulta [Richiedere l’accesso a un piano in [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

