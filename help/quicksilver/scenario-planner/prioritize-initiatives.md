---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Aggiornare le priorità dell'iniziativa nel planner dello scenario
description: La priorità alle iniziative è importante perché le iniziative ricevono ruoli e risorse di budget dal piano nell’ordine in cui sono elencate nel piano.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Aggiornare le priorità dell&#39;iniziativa [!DNL Scenario Planner]

La priorità alle iniziative è importante perché le iniziative ricevono ruoli e risorse di budget dal piano nell’ordine in cui sono elencate nel piano.

Puoi assegnare priorità alle iniziative in base a un piano creato o a un piano condiviso con te.

Per informazioni sulla creazione dei piani, consulta [Crea e modifica piani in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Per informazioni sulla creazione di iniziative, consulta [Creare e modificare iniziative in [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

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
   <td> <p>[!DNL Adobe Workfront]<b> licenza*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td><b>Prodotto</b> </td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Accesso o superiore a [!DNL Scenario Planner]</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Autorizzazioni di gestione per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedi <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedi l'accesso a un piano nel [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aggiorna le priorità dell&#39;iniziativa

Quando modifichi la priorità delle iniziative, modificane l’ordine di inserimento nel piano.

Vi consigliamo di inserire iniziative più urgenti in cima a un piano e quelle più fluide - che potrebbero essere fatte in qualsiasi momento e solo se le risorse sono disponibili - in fondo al piano.

>[!NOTE]
>
>[!DNL Workfront] assegna le risorse del piano alle iniziative nell&#39;ordine in cui sono elencate nel piano.
>
>Ad esempio, se il piano dispone di 3 ingegneri disponibili e di Iniziativa 1 e Iniziativa 2 ciascuno richiede il completamento di 2 ingegneri e sono entrambi programmati per lo stesso periodo di tempo, Workfront associa 2 ingegneri con Iniziativa 1 e uno ancora disponibile ingegnere con Iniziativa 2. In questo caso, l&#39;iniziativa 2 indica un conflitto, perché manca un ingegnere. A volte, cambiare la priorità delle tue iniziative è l&#39;unico modo per evitare conflitti su un piano.

Per aggiornare la priorità dell&#39;iniziativa:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png), quindi fai clic su [!UICONTROL Scenari].

   Viene visualizzato un elenco di piani.

1. Fai clic sul nome di un piano per aprirlo, quindi individua le iniziative da assegnare come priorità.
1. Fai clic sulla casella a sinistra del nome di una o più iniziative ed effettua una delle seguenti operazioni:

   * Fai clic sul quadratino a sinistra dei nomi di una delle iniziative selezionate, quindi trascinalo verso l’alto o il basso nell’elenco per modificare la priorità dell’iniziativa.

      Workfront mostra il numero di iniziative selezionate.

      ![](assets/multi-select-initiative-number.png)

   * Fai clic sul pulsante **[!UICONTROL Priorità]** nella parte inferiore del piano, quindi scegliere tra le seguenti opzioni:

      * **[!UICONTROL Top]**: Sposta le iniziative selezionate all’inizio dell’elenco delle iniziative. Le iniziative selezionate sono elencate per prime nel piano.
      * **[!UICONTROL In basso]**: Sposta le iniziative selezionate in fondo all’elenco delle iniziative. Le iniziative selezionate sono elencate per ultime sul piano.
      * **[!UICONTROL Seleziona un numero]**: Sposta le iniziative selezionate dopo l&#39;iniziativa indicata qui.

         ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)
      [!DNL Workfront] posiziona immediatamente le iniziative selezionate in corrispondenza del punto in cui vengono indicate e il numero di tutte le iniziative viene aggiornato di conseguenza.


1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.
