---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Panoramica sulla riconciliazione delle assegnazioni di risorse tra progetti e iniziative
description: Panoramica sulla riconciliazione delle assegnazioni di risorse tra progetti e iniziative
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Panoramica sulla riconciliazione delle assegnazioni di risorse tra progetti e iniziative

>[!IMPORTANT]
>
>La tua organizzazione deve acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per visualizzare le informazioni relative all’iniziativa su un progetto. Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi [Accesso necessario per utilizzare il planner dello scenario](../scenario-planner/access-needed-to-use-sp.md) .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Puoi collegare i progetti alle iniziative per garantire che i piani strategici e il lavoro effettivo siano sincronizzati. Come delineate i vostri piani strategici e le vostre iniziative nel [!DNL Scenario Planner] e si pianifica il lavoro effettivo in un progetto, è possibile garantire che le risorse del progetto e le iniziative corrispondano, in modo da non sovrascriverle o sottoutilizzarle.

## Prerequisiti

Prima di iniziare, è necessario disporre dei seguenti elementi:

* Un piano nel [!DNL Scenario Planner] con un&#39;iniziativa connessa a un progetto.
* Assegnazione obbligatoria dei ruoli di lavoro per l&#39;iniziativa.
* Attività o problemi relativi al progetto con orario pianificato e assegnati a una delle seguenti operazioni:

   * Mansioni
   * Utenti associati a ruoli di lavoro

## Collegare progetti e iniziative

>[!NOTE]
>
>Puoi creare iniziative e collegarle ai progetti solo se la tua organizzazione ha acquistato una licenza aggiuntiva per [!DNL Workfront Scenario Planner].

Per collegare i progetti alle iniziative, effettua una delle seguenti operazioni:

* Importare i progetti in un piano come nuove iniziative

   Per ulteriori informazioni, consulta [Importa progetti nei piani [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Pubblicare iniziative in progetti

   Per ulteriori informazioni, consulta [Aggiornare o creare progetti pubblicando iniziative nel [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

Entrambi i processi creano un collegamento tra i progetti e le relative iniziative. Dopo averli collegati, puoi gestire le loro allocazioni di risorse confrontandole e assicurandoti che corrispondano.

## Considerazioni sulla riconciliazione delle risorse su progetti e iniziative collegati

>[!NOTE]
>
>È possibile visualizzare le iniziative, collegarle ai progetti e visualizzare le relative allocazioni di risorse in un progetto solo se l&#39;organizzazione ha acquistato una licenza aggiuntiva per [!DNL Workfront Scenario Planner].

* È possibile assegnare utenti, team e ruoli di lavoro agli elementi di lavoro di un progetto e assegnare ruoli di lavoro alle iniziative. Di conseguenza, è possibile riconciliare i ruoli di lavoro solo tra progetti e iniziative.

   >[!TIP]
   >
   >Per riconciliare il tempo degli utenti in un progetto con le allocazioni di ruolo nelle iniziative, è necessario associare gli utenti ai ruoli di lavoro.

* Puoi visualizzare l’allocazione del ruolo di lavoro dell’iniziativa in un progetto collegato nelle seguenti aree del progetto:

   * [!DNL Scenario Planner] della sezione [!UICONTROL Dettagli progetto] area su un progetto. Per ulteriori informazioni, consulta i seguenti articoli:

      * [Aggiornare o creare progetti pubblicando iniziative nel [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Gestire le informazioni nel progetto [!UICONTROL Panoramica] area](../manage-work/projects/manage-projects/understand-project-overview-area.md)

      >[!TIP]
      >
      >Non è possibile visualizzare le informazioni sul ruolo di lavoro dal progetto e dall’iniziativa affiancate nella [!DNL Scenario Planner] della sezione [!UICONTROL Dettagli progetto].

   * La [!UICONTROL Assegnazione ruolo] nelle seguenti aree:

      * [!DNL Workload Balancer] del progetto

         Per informazioni su come visualizzare e riconciliare le allocazioni di ruoli tra l’iniziativa e il progetto collegato nel [!DNL Workload Balancer], vedi [Mostrare la ripartizione dei ruoli per progetti e iniziative [!DNL Workload Balancer]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * [!UICONTROL Attività] sezione

         Per informazioni su come riconciliare le allocazioni di ruoli tra l’iniziativa e il progetto collegato nel [!UICONTROL Attività] sezione [Mostra l&#39;allocazione dei ruoli per progetti e iniziative nell&#39;elenco dei task](../scenario-planner/show-role-allocation-task-list-nwe.md).
      >[!TIP]
      >
      >Puoi vedere le informazioni sul ruolo del lavoro dal progetto e dall’iniziativa affiancate in [!UICONTROL Assegnazione ruolo] pannello.



* Non è possibile visualizzare l&#39;allocazione dei ruoli di lavoro per un progetto su un&#39;iniziativa collegata. Per ulteriori informazioni, consulta [Importa progetti nei piani [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
