---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copiare iniziative nella Pianificazione scenario
description: Puoi creare iniziative copiando quelle esistenti. È possibile copiare le iniziative in un piano creato dall'utente o in un piano condiviso con l'utente.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Copia iniziative in [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Puoi creare iniziative copiando quelle esistenti. È possibile copiare le iniziative in un piano creato dall&#39;utente o in un piano condiviso con l&#39;utente.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] piano*</p> </td> 
   <td> <p>Corrente: [!UICONTROL Business] o versione successiva</p>
   <p>Nuovo: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td> <p>Nuovo: Chiaro o superiore</p> 
   <p>Corrente: [!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td>Prodotto* </td> 
   <td> 
   <p>Per i piani Workfront correnti: </p>
   <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni sull'accesso e sulle autorizzazioni per [!DNL Workfront Scenario Planner], vedere <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Livello di accesso </td> 
   <td> <p>Accesso di [!UICONTROL Edit] al [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>Autorizzazioni [!UICONTROL Manage] per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedere <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedere accesso a un piano in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Copia iniziative

Quando copi le iniziative, tieni presente quanto segue:

* Quando si copia un&#39;iniziativa, la copia viene posizionata sullo stesso piano dell&#39;iniziativa originale.
* Copiare un&#39;iniziativa copia e aggiunge le seguenti informazioni dall&#39;iniziativa originale alla nuova iniziativa:

   * [!UICONTROL Durata]
   * [!UICONTROL Ruoli]
   * [!UICONTROL Persone] e [!UICONTROL Costi fissi]
   * [!UICONTROL Vantaggio pianificato]

* Copiando un&#39;iniziativa è possibile modificare le seguenti informazioni per il piano, se disponibili nell&#39;iniziativa originale:

   * Quantità richiesta di mansioni
   * [!UICONTROL Costi]
   * [!UICONTROL Utilizzo piano]
   * Utilizzo ruolo
   * [!UICONTROL Valore Netto]

* Copiare un’iniziativa creata importando un progetto o che è stata pubblicata in un progetto almeno una volta ha le seguenti implicazioni:

   * Non duplica il progetto associato all’iniziativa.
   * Non collega l’iniziativa copiata al progetto.
   * Non modifica la sezione [!DNL Scenario Planner] del progetto, per i progetti che sono stati pubblicati almeno una volta.

  Per informazioni sulla pubblicazione di iniziative nei progetti, vedere [Aggiornare o creare progetti pubblicando iniziative in [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

  Per informazioni sulla creazione di iniziative mediante l&#39;importazione di progetti, vedere [Importare progetti nei piani in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

## Copia iniziative

{{step1-to-scenario-planner}}

Viene visualizzato un elenco di piani.

1. Fare clic sul nome di un piano per aprirlo, quindi individuare le iniziative da copiare.
1. Seleziona la casella a sinistra dell&#39;iniziativa o delle iniziative da copiare, quindi fai clic su **[!UICONTROL Copia]** dal menu visualizzato in fondo al piano.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] copia immediatamente le iniziative e le posiziona sotto l&#39;ultima iniziativa selezionata.

   Il nome dell&#39;iniziativa copiata è *[!UICONTROL Copia di]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >A seconda della posizione in cui vengono inserite le nuove iniziative, il numero di iniziative esistenti potrebbe cambiare.

1. Aggiorna il nome dell&#39;iniziativa copiata.

   >[!TIP]
   >
   >È consigliabile aggiornare sempre il nome dell’iniziativa per evitare confusione nel caso in cui si desideri copiarli nuovamente.

1. (Facoltativo) Aggiorna la priorità delle nuove iniziative create.

   Per informazioni sull&#39;assegnazione delle priorità alle iniziative, vedere [Aggiornare le priorità delle iniziative in  [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.
