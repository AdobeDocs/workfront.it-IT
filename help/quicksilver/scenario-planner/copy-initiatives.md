---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copiare iniziative nella Pianificazione scenario
description: Puoi creare iniziative copiando quelle esistenti. È possibile copiare le iniziative in un piano creato dall'utente o in un piano condiviso con l'utente.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Copia iniziative in [!DNL Scenario Planner]

Puoi creare iniziative copiando quelle esistenti. È possibile copiare le iniziative in un piano creato dall&#39;utente o in un piano condiviso con l&#39;utente.

## Requisiti di accesso

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> piano*</b> </p> </td> 
   <td>[!UICONTROL Business] o versione successiva</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licenza</b>*</p> </td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td><b>Prodotto</b> </td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedere <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni del livello di accesso*</strong> </td> 
   <td> <p>Accesso di [!UICONTROL Edit] o versione successiva al [!DNL Scenario Planner]</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il livello di accesso, vedere <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Autorizzazioni [!UICONTROL Manage] per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedere <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedere accesso a un piano in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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

  Per informazioni sulla creazione di iniziative mediante l&#39;importazione di progetti, vedere [Importare progetti nei piani in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

## Copia iniziative

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]**, quindi fai clic su [!UICONTROL Scenari].

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
