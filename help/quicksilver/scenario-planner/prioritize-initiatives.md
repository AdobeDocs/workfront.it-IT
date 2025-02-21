---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Aggiornare le priorità dell’iniziativa nella Pianificazione scenario
description: La priorità delle iniziative è importante perché le iniziative ricevono mansioni e risorse di budget dal piano nell'ordine in cui sono elencate nel piano.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# Aggiorna le priorità dell&#39;iniziativa in [!DNL Scenario Planner]

La priorità delle iniziative è importante perché le iniziative ricevono mansioni e risorse di budget dal piano nell&#39;ordine in cui sono elencate nel piano.

Puoi assegnare un ordine di priorità alle iniziative in base a un piano creato personalmente o condiviso con te.

Per informazioni sulla creazione dei piani, vedere [Creare e modificare i piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Per informazioni sulla creazione delle iniziative, vedere [Creare e modificare le iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] piano*</p> </td> 
   <td> <ul></li>
   <li><p>Nuovo: Ultimate </p></li>
   <p>Pianificazione scenario non disponibile per i nuovi piani Workfront Select o Workfront Prime. </p>
   <li><p>Corrente: [!UICONTROL Business] o versione successiva</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td> <p>Nuovo: Chiaro o superiore</p> 
   <p>Corrente: [!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td>Prodotto* </td> 
   <td> <ul><li><p>Per i nuovi piani Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Per i piani Workfront correnti: </p>
   <p>Adobe Workfront</p> <p>Pianificazione scenario Adobe Workfront</p></li></ul>

<p>Per ulteriori informazioni, vedere <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
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

## Aggiornare le priorità dell’iniziativa

Quando si modifica la priorità delle iniziative, si modifica l&#39;ordine di visualizzazione delle iniziative nel piano.

Consigliamo di inserire iniziative più urgenti in cima a un piano e iniziative più fluide - che potrebbero essere realizzate in qualsiasi momento e solo se sono disponibili risorse - in fondo al piano.

>[!NOTE]
>
>[!DNL Workfront] alloca le risorse del piano alle iniziative nell&#39;ordine in cui sono elencate nel piano.
>
>Ad esempio, se il piano dispone di 3 tecnici disponibili e l&#39;Iniziativa 1 e l&#39;Iniziativa 2 richiedono il completamento di 2 tecnici e sono entrambi pianificati per lo stesso intervallo di tempo, Workfront associa 2 tecnici all&#39;Iniziativa 1 e un tecnico disponibile rimanente all&#39;Iniziativa 2. In questo caso, l&#39;iniziativa 2 presenta un conflitto in quanto manca un ingegnere. Talvolta, cambiare la priorità delle iniziative è l’unico modo per evitare conflitti su un piano.

Per aggiornare la priorità dell&#39;iniziativa:

{{step1-to-scenario-planner}}

Viene visualizzato un elenco di piani.

1. Fare clic sul nome di un piano per aprirlo, quindi individuare le iniziative da assegnare come priorità.
1. Fai clic sulla casella a sinistra del nome di una o più iniziative ed effettua una delle seguenti operazioni:

   * Fai clic sull’handle a sinistra del nome di una delle iniziative selezionate, quindi trascinalo verso l’alto o verso il basso nell’elenco per modificare la priorità dell’iniziativa.

     In Workfront viene visualizzato il numero di iniziative selezionate.

     ![Numero iniziativa a selezione multipla](assets/multi-select-initiative-number.png)

   * Fai clic sulla casella **[!UICONTROL Assegna priorità]** nella parte inferiore del piano, quindi scegli una delle seguenti opzioni:

      * **[!UICONTROL Principale]**: sposta le iniziative selezionate all&#39;inizio dell&#39;elenco delle iniziative. Le iniziative selezionate sono elencate per prime nel piano.
      * **[!UICONTROL Inferiore]**: sposta le iniziative selezionate in fondo all&#39;elenco delle iniziative. Le iniziative selezionate sono elencate per ultime nel piano.
      * **[!UICONTROL Seleziona un numero]**: sposta le iniziative selezionate dopo l&#39;iniziativa indicata.

        ![Assegna priorità alle iniziative](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] inserisce immediatamente le iniziative selezionate dove si indica e il numero di tutte le iniziative viene aggiornato di conseguenza.

1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.
