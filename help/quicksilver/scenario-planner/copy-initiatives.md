---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copiare le iniziative nel planner dello scenario
description: Puoi creare iniziative copiandone quelle esistenti. Puoi copiare le iniziative su un piano creato o su un piano condiviso da un utente.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# Copia le iniziative nel [!DNL Scenario Planner]

Puoi creare iniziative copiandone quelle esistenti. Puoi copiare le iniziative su un piano creato o su un piano condiviso da un utente.

## Requisiti di accesso

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> piano*</b> </p> </td> 
   <td>[!UICONTROL Business] o superiore</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licenza</b>*</p> </td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td><b>Prodotto</b> </td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Accesso o superiore a [!DNL Scenario Planner]</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Autorizzazioni di gestione per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedi <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedi l'accesso a un piano nel [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Copia delle iniziative

Quando copi le iniziative, considera quanto segue:

* Copiare un&#39;iniziativa posiziona la copia sullo stesso piano dell&#39;iniziativa originale.
* Copiare un&#39;iniziativa e aggiungere le seguenti informazioni dell&#39;iniziativa originale alla nuova iniziativa:

   * [!UICONTROL Durata]
   * [!UICONTROL Mansioni]
   * [!UICONTROL Persone] e [!UICONTROL Costi fissi]
   * [!UICONTROL Benef Pian]

* Copiare un&#39;iniziativa può modificare le seguenti informazioni per il piano, se le informazioni sono presenti nell&#39;iniziativa originale:

   * Quantità necessaria di ruoli di lavoro
   * [!UICONTROL Costi]
   * [!UICONTROL Utilizzo del piano]
   * Utilizzo del ruolo di lavoro
   * [!UICONTROL Valore Netto]

* La copia di un&#39;iniziativa creata importando un progetto o pubblicata in un progetto almeno una volta ha le seguenti implicazioni:

   * Non duplica il progetto associato all&#39;iniziativa.
   * Non collega l&#39;iniziativa copiata al progetto.
   * Non modifica la [!DNL Scenario Planner] sezione sul progetto, per i progetti pubblicati almeno una volta.

   Per informazioni sulla pubblicazione di iniziative in progetti, consulta [Aggiornare o creare progetti pubblicando iniziative nel [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

   Per informazioni sulla creazione di iniziative importando progetti, consulta [Importa progetti nei piani [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

## Copia delle iniziative

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png), quindi fai clic su [!UICONTROL Scenari].

   Viene visualizzato un elenco di piani.

1. Fai clic sul nome di un piano per aprirlo, quindi individua le iniziative da copiare.
1. Seleziona la casella a sinistra dell&#39;iniziativa o delle iniziative da copiare, quindi fai clic su **[!UICONTROL Copia]** dal menu visualizzato nella parte inferiore del piano.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] copia immediatamente le iniziative e le pone sotto l&#39;ultima iniziativa selezionata.

   Il nome dell&#39;iniziativa copiata è *[!UICONTROL Copia di]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >A seconda di dove si inseriscono le nuove iniziative, il numero di iniziative esistenti potrebbe cambiare.

1. Aggiorna il nome dell&#39;iniziativa copiata.

   >[!TIP]
   >
   >Si consiglia di aggiornare sempre il nome dell’iniziativa per evitare confusione nel caso in cui si desideri copiarli di nuovo.

1. (Facoltativo) Aggiorna la priorità delle iniziative appena create.

   Per informazioni sulla priorità delle iniziative, consulta [Aggiornare le priorità dell&#39;iniziativa [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.
