---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Accesso necessario per utilizzare il planner dello scenario
description: Il planner scenario richiede una licenza separata da Adobe Workfront e un accesso aggiuntivo.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Accesso necessario per utilizzare [!DNL Scenario Planner]

La [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni sulla [!DNL Workfront Scenario Planner], vedi [La [!DNL Scenario Planner] panoramica](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Senza l&#39;accesso o le autorizzazioni corrette, potresti non essere in grado di visualizzare il [!UICONTROL Scenari] area[!DNL  Adobe Workfront] né gestire piani o iniziative per la tua organizzazione. La gestione di piani e iniziative prevede la creazione, la modifica e l’eliminazione di piani e iniziative.

>[!IMPORTANT]
>
>Quando accedi [!UICONTROL Scenari], puoi visualizzare e gestire solo i piani creati. Per consentire ad altri utenti di visualizzare o gestire i piani creati, è necessario effettuare le seguenti operazioni:
>
>* Invia un collegamento al tuo piano ad altri utenti
>* Condividi il piano con altri utenti
>
>  Per informazioni sulla condivisione di un piano, vedi [Condividi un piano in [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>Quando un utente è disattivato, i suoi piani non dispongono di un proprietario e non sono accessibili a meno che non sia precedentemente condiviso con un collegamento.

## Accesso necessario per visualizzare e utilizzare il [!DNL Adobe Workfront Scenario Planner]

È necessario assicurarsi che siano soddisfatte tutte le seguenti condizioni prima di poter accedere al [!DNL Workfront Scenario Planner]:

<!--drafted for P&P:

* Depending on whether you use the current or the legacy Workfront plans, your organization must have the following:

  * For the current plans:  

    * The [!UICONTROL Ultimate] [!DNL Workfront] plan.

      Or
  
    * The [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] plan, in addition to purchasing a separate [!DNL Scenario Planner] license.

  * For the legacy plans: (indent the bullets below, before the NOTE)

-->

* La tua organizzazione deve acquistare un [!DNL Workfront] [!UICONTROL Business] o superiore [!DNL Workfront] piano. Per informazioni sulla [!DNL Workfront] piani, vedi [Piani Workfront](http://workfront.com/plans).
* La tua organizzazione deve acquistare un [!DNL Workfront Scenario Planner] in aggiunta a una licenza [!DNL Workfront] licenza. Contatta il tuo [!DNL Workfront] Rappresentante account per informazioni [!DNL Workfront Scenario Planner] licenze.

<!--drafted for P&P: 

* Depending on whether you use the current or legacy licenses, your [!DNL Workfront] administrator must assign you a license of any of the following types: 

  * For the current licenses: 
    * [!UICONTROL Standard]
    * [!UICONTROL Light]

  * For the legacy licenses: (re-indent the licenses below and reword the sentence)

-->



* Le [!DNL Workfront] l&#39;amministratore deve assegnare una licenza per uno dei seguenti [!DNL Workfront] tipi:

   * [!UICONTROL Piano]
   * [!UICONTROL Lavoro]
   * [!UICONTROL Revisiona]

   >[!NOTE]
   >
   >Utenti con un [!UICONTROL Richiesta] o [!UICONTROL Esterno] impossibile accedere al tipo di licenza [!DNL Workfront Scenario Planner].

<!--drafted - replace the note above with this at P&P release: 
  * When using the current licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
  * When using the legacy licenses, users with a Request or External license type cannot access the Scenario Planner. -->

* Le [!DNL Workfront] l&#39;amministratore deve [!UICONTROL Visualizza] o [!UICONTROL Modifica] accesso [!DNL Scenario Planner] nel livello di accesso.

   Per informazioni sulla concessione dell&#39;accesso al [!DNL Workfront Scenario Planner], vedi [Concedere l’accesso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* (Facoltativo e consigliato) Per visualizzare o aggiornare le informazioni finanziarie relative ai piani e alle iniziative, [!DNL Workfront] l&#39;amministratore deve inoltre concedere l&#39;accesso a [!UICONTROL Dati finanziari] nel livello di accesso. Per informazioni sulla concessione di dati finanziari nel livello di accesso, consulta [Concedere l’accesso ai dati finanziari](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

   <!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

* Se devi accedere ai piani che non hai creato, un creatore di piani deve concederti le autorizzazioni corrette per il suo piano per accedervi. Per informazioni sulle autorizzazioni necessarie per accedere ai piani e alle iniziative che non hai creato, consulta [Autorizzazioni necessarie per accedere a piani e iniziative](#permissions-needed-to-access-plans-and-initiatives) in questo articolo.

## Accesso necessario per visualizzare piani e iniziative

Oltre all&#39;acquisizione della licenza corretta per il [!DNL Workfront Scenario Planner], il [!DNL Workfront] l&#39;amministratore deve inoltre assegnarti i seguenti accessi e impostazioni in modo da poter visualizzare il [!DNL Workfront Scenario Planner] e le informazioni in materia:

* Un livello di accesso con almeno [!UICONTROL Visualizza] accesso [!DNL Scenario Planner].

   Per informazioni sul livello di accesso a [!DNL Scenario Planner], vedi [Concedere l’accesso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Un livello di accesso con almeno [!UICONTROL Visualizza] accesso [!UICONTROL Dati finanziari] se è necessario visualizzare anche informazioni finanziarie sul piano e le iniziative. Alcuni esempi di informazioni finanziarie sono budget, costi o tassi di ruolo del lavoro.

   Per informazioni sulla [!UICONTROL Dati finanziari] livello di accesso, vedi [Concedere l’accesso ai dati finanziari](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

   >[!TIP]
   >
   >[!UICONTROL Richiedenti] e [!UICONTROL Esterno] Gli utenti non hanno accesso alla visualizzazione del [!DNL Scenario Planner].

* Visualizza le autorizzazioni per il piano. Per informazioni sulle autorizzazioni necessarie per accedere ai piani e alle iniziative che non hai creato, consulta [Autorizzazioni necessarie per accedere a piani e iniziative](#permissions-needed-to-access-plans-and-initiatives) in questo articolo.

## Accesso necessario per la gestione dei piani e delle iniziative

Le [!DNL Workfront] l&#39;amministratore deve assegnare il seguente accesso per gestire i piani e le relative informazioni nel [!DNL Scenario Planner]:

* A [!UICONTROL Pianificare] o [!UICONTROL Lavoro] tipo di licenza con accesso Modifica al [!DNL Scenario Planner] nel livello di accesso.

   Tutti gli altri tipi di licenza non hanno accesso alla gestione dei piani.

   Per informazioni sulla concessione dell&#39;accesso a [!DNL Scenario Planner] dal livello di accesso, vedi [Concedere l’accesso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Pianificare] tipo di licenza con [!UICONTROL Modifica] accesso [!UICONTROL Dati finanziari] nel livello di accesso, se è necessario aggiornare anche le informazioni finanziarie sul piano.

   Alcuni esempi di informazioni finanziarie modificabili sono [!UICONTROL Bilancio], [!UICONTROL Vantaggio pianificato]e [!UICONTROL Costi fissi].

   >[!TIP]
   >
   >Solo [!UICONTROL Pianificare] i titolari delle licenze [!UICONTROL Modifica] accesso [!UICONTROL Dati finanziari].

   Per informazioni sulla [!UICONTROL Dati finanziari] livello di accesso, vedi [Concedere l’accesso ai dati finanziari](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Gestisci le autorizzazioni per un piano che non hai creato. Per informazioni sulle autorizzazioni necessarie per accedere ai piani e alle iniziative che non hai creato, consulta [Autorizzazioni necessarie per accedere a piani e iniziative](#permissions-needed-to-access-plans-and-initiatives) in questo articolo.

## Autorizzazioni necessarie per accedere a piani e iniziative

I livelli di accesso funzionano insieme alle autorizzazioni in [!DNL Workfront] per dare visibilità a piani e iniziative che non hai creato. Oltre ad avere il livello di accesso corretto per accedere al [!DNL Scenario Planner], se non sei il creatore di tali piani, devi anche disporre delle autorizzazioni corrette per il piano che desideri visualizzare o gestire.

Per impostazione predefinita, è possibile accedere solo ai piani creati. Per visualizzare i piani creati da altri utenti, è necessario che questi condividano i loro piani con te. Per informazioni sui piani di condivisione, vedi [Condividi un piano in [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

Se un utente condivide un collegamento a un piano senza condividerlo, è possibile richiedere le autorizzazioni per il piano. Per informazioni sulla richiesta di autorizzazioni ai piani, consulta [Richiedi l&#39;accesso a un piano nel [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

