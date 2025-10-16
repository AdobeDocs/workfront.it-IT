---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Panoramica sulla quadratura delle allocazioni di risorse tra progetti e iniziative
description: Panoramica sulla riconciliazione delle allocazioni di risorse tra progetti e iniziative
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Panoramica sulla riconciliazione delle allocazioni di risorse tra progetti e iniziative

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Puoi collegare i progetti con le iniziative per garantire che i piani strategici e il lavoro effettivo siano sincronizzati. Quando si delineano i piani e le iniziative strategiche in [!DNL Scenario Planner] e si pianifica il lavoro effettivo in un progetto, è possibile garantire che le risorse del progetto e delle iniziative corrispondano, in modo da non sovrassegnarle o sottoutilizzarle.

## Prerequisiti

Prima di iniziare, è necessario disporre dei seguenti elementi:

* Un piano in [!DNL Scenario Planner] con un&#39;iniziativa connessa a un progetto.
* Allocazioni di ruoli richieste per l’iniziativa.
* Attività o problemi del progetto che hanno ore pianificate e sono assegnati a uno dei seguenti:

   * Mansioni
   * Utenti associati a mansioni

## Collegare progetti e iniziative

>[!NOTE]
>
>È possibile creare iniziative e collegarle ai progetti solo se l&#39;organizzazione ha acquistato una licenza aggiuntiva per [!DNL Workfront Scenario Planner].

Per collegare i progetti alle iniziative, effettua una delle seguenti operazioni:

* Importa progetti in un piano, come nuove iniziative

  Per ulteriori informazioni, vedere [Importare progetti nei piani in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Pubblicare iniziative in progetti

  Per ulteriori informazioni, vedere [Aggiornare o creare progetti pubblicando iniziative in [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

Entrambi i processi creano una connessione tra i progetti e le iniziative corrispondenti. Dopo averli collegati, puoi gestirne le allocazioni di risorse confrontandole e verificandone la corrispondenza.

## Considerazioni sulla conciliazione delle risorse su progetti e iniziative collegati

>[!NOTE]
>
>È possibile visualizzare le iniziative, collegarle ai progetti e visualizzare le allocazioni delle risorse per un progetto solo se l&#39;organizzazione ha acquistato una licenza aggiuntiva per [!DNL Workfront Scenario Planner].

* È possibile assegnare utenti, team e ruoli agli elementi di lavoro di un progetto e ruoli alle iniziative. Di conseguenza, è possibile riconciliare solo i ruoli tra progetti e iniziative.

  >[!TIP]
  >
  >Per riconciliare il tempo degli utenti su un progetto con le allocazioni di ruoli sulle iniziative, è necessario associare gli utenti alle mansioni.

* Puoi visualizzare l’allocazione dei ruoli dell’iniziativa su un progetto collegato nelle seguenti aree del progetto:

   * [!DNL Scenario Planner] sezione dell&#39;area [!UICONTROL Dettagli progetto] in un progetto. Per ulteriori informazioni, consulta i seguenti articoli:

      * [Aggiorna o crea progetti pubblicando iniziative in [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Gestisci informazioni nell&#39;area [!UICONTROL Panoramica] del progetto](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >Non è possibile visualizzare le informazioni sulle mansioni dal progetto e dall&#39;iniziativa affiancate nella sezione [!DNL Scenario Planner] dei [!UICONTROL Dettagli progetto].

   * Il pannello [!UICONTROL Allocazione ruoli] nelle seguenti aree:

      * [!UICONTROL Bilanciatore dei carichi di lavoro] del progetto

        Per informazioni su come visualizzare e riconciliare le allocazioni di ruoli tra l&#39;iniziativa e il progetto collegato nel [!UICONTROL Bilanciatore dei carichi di lavoro], vedere [Mostra allocazione ruoli per progetti e iniziative nel [!UICONTROL Bilanciatore dei carichi di lavoro]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * Sezione [!UICONTROL Attività]

        Per informazioni su come riconciliare le allocazioni di ruoli tra l&#39;iniziativa e il progetto collegato nella sezione [!UICONTROL Attività], vedere [Mostra allocazione ruoli per progetti e iniziative nell&#39;elenco attività](../scenario-planner/show-role-allocation-task-list-nwe.md).

     >[!TIP]
     >
     >Puoi visualizzare le informazioni sui ruoli dal progetto e dall&#39;iniziativa nel pannello [!UICONTROL Allocazione ruoli].

* Non puoi visualizzare l’allocazione delle mansioni per un progetto su un’iniziativa collegata. Per ulteriori informazioni, vedere [Importare progetti nei piani in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
