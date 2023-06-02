---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Panoramica sulla riconciliazione delle allocazioni di risorse tra progetti e iniziative
description: Panoramica sulla riconciliazione delle allocazioni di risorse tra progetti e iniziative
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Panoramica sulla riconciliazione delle allocazioni di risorse tra progetti e iniziative

>[!IMPORTANT]
>
>La tua organizzazione deve acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] in modo da poter visualizzare le informazioni sull’iniziativa su un progetto. Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi [Accesso necessario per utilizzare la Pianificazione scenario](../scenario-planner/access-needed-to-use-sp.md) .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Puoi collegare i progetti con le iniziative per garantire che i piani strategici e il lavoro effettivo siano sincronizzati. delineando i piani strategici e le iniziative nel [!DNL Scenario Planner] se si pianifica il lavoro effettivo di un progetto, è possibile assicurarsi che le risorse del progetto e delle iniziative corrispondano, in modo da non sovrassegnarle o sottoutilizzarle.

## Prerequisiti

Prima di iniziare, è necessario disporre dei seguenti elementi:

* Un piano in [!DNL Scenario Planner] con un’iniziativa connessa a un progetto.
* Allocazioni di ruoli richieste per l’iniziativa.
* Attività o problemi del progetto che hanno ore pianificate e sono assegnati a uno dei seguenti:

   * Mansioni
   * Utenti associati a mansioni

## Collegare progetti e iniziative

>[!NOTE]
>
>Puoi creare iniziative e collegarle ai progetti solo se la tua organizzazione ha acquistato una licenza aggiuntiva per [!DNL Workfront Scenario Planner].

È possibile collegare i progetti alle iniziative eseguendo una delle operazioni seguenti:

* Importa progetti in un piano, come nuove iniziative

   Per ulteriori informazioni, consulta [Importa progetti nei piani in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Pubblicare iniziative in progetti

   Per ulteriori informazioni, consulta [Aggiornare o creare progetti pubblicando iniziative in [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

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

   * [!DNL Scenario Planner] sezione del [!UICONTROL Dettagli progetto] in un progetto. Per ulteriori informazioni, consulta i seguenti articoli:

      * [Aggiornare o creare progetti pubblicando iniziative in [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Gestire le informazioni nel progetto [!UICONTROL Panoramica] area](../manage-work/projects/manage-projects/understand-project-overview-area.md)

      >[!TIP]
      >
      >Non è possibile visualizzare informazioni sui ruoli dal progetto e dall’iniziativa affiancate nel [!DNL Scenario Planner] sezione del [!UICONTROL Dettagli progetto].

   * Il [!UICONTROL Allocazione mansioni] nelle seguenti aree:

      * [!UICONTROL Bilanciatore dei carichi di lavoro] del progetto

         Per informazioni su come visualizzare e riconciliare le allocazioni di ruoli tra l’iniziativa e il progetto collegato in [!UICONTROL Bilanciatore dei carichi di lavoro], vedi [Mostra l’allocazione dei ruoli per progetti e iniziative in [!UICONTROL Bilanciatore dei carichi di lavoro]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * [!UICONTROL Attività] sezione

         Per informazioni su come riconciliare le allocazioni di ruoli tra l’iniziativa e il progetto collegato in [!UICONTROL Attività] sezione, vedi [Mostra assegnazione ruoli per progetti e iniziative nell&#39;elenco delle attività](../scenario-planner/show-role-allocation-task-list-nwe.md).
      >[!TIP]
      >
      >Puoi visualizzare le informazioni sui ruoli dal progetto e dall’iniziativa in [!UICONTROL Allocazione mansioni] pannello.



* Non puoi visualizzare l’allocazione delle mansioni per un progetto su un’iniziativa collegata. Per ulteriori informazioni, consulta [Importa progetti nei piani in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
