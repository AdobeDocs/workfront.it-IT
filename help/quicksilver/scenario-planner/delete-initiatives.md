---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Eliminare le iniziative in Scenario Planner
description: È possibile eliminare le iniziative in base a un piano creato dall'utente o a un piano condiviso con l'utente. Non puoi recuperare le iniziative eliminate.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: ed179058cfec1332384ef76cb04598278109291b
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 1%

---

# Elimina iniziative in [!DNL Scenario Planner]

È possibile eliminare le iniziative in base a un piano creato dall&#39;utente o a un piano condiviso con l&#39;utente. Non puoi recuperare le iniziative eliminate.

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

## Elimina iniziative

Quando elimini le iniziative, tieni presente quanto segue:

* Se si elimina un&#39;iniziativa, la quantità richiesta di mansioni e le informazioni sui costi associate all&#39;iniziativa vengono rimosse dal piano.
* L’eliminazione di un’iniziativa creata importando un progetto non comporta l’eliminazione del progetto associato all’iniziativa.
* L’eliminazione di un’iniziativa pubblicata in un progetto comporta almeno una volta quanto segue:

   * L&#39;iniziativa è stata eliminata dallo scenario ma l&#39;area [!DNL Scenario Planner] rimane nella sezione [!UICONTROL Dettagli progetto].
   * Se l’iniziativa eliminata è l’unica iniziativa pubblicata nello scenario, viene rimosso anche l’indicatore che il piano è stato pubblicato.

     Per informazioni sulla pubblicazione di iniziative nei progetti, vedere [Aggiornare o creare progetti pubblicando iniziative in [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

     Per informazioni sulla creazione di iniziative mediante l&#39;importazione di progetti, vedere [Importare progetti nei piani in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

È possibile eliminare un&#39;iniziativa alla volta oppure più iniziative in blocco.

* [Elimina un&#39;iniziativa](#delete-one-initiative)
* [Elimina iniziative in blocco](#delete-initiatives-in-bulk)

### Elimina un&#39;iniziativa {#delete-one-initiative}

{{step1-to-scenario-planner}}

Viene visualizzato un elenco di piani.

1. Fare clic sul nome di un piano per aprirlo, quindi individuare l&#39;iniziativa che si desidera eliminare.
1. Esegui una delle operazioni seguenti:

   * Fai clic sul menu **[!UICONTROL Altro]** ![](assets/more-menu.png) a destra del nome dell&#39;iniziativa, quindi fai clic su **[!UICONTROL Elimina]** > **[!UICONTROL Sì, elimina]**.

   * Selezionare la casella a sinistra dell&#39;iniziativa, quindi fare clic su **[!UICONTROL Elimina]** nel menu mobile visualizzato nella parte inferiore del piano, quindi fare clic su **[!UICONTROL Sì, elimina]**.

   L&#39;iniziativa e il suo ruolo e le informazioni sui costi sono cancellati dal piano.

1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.

### Elimina iniziative in blocco {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

Viene visualizzato un elenco di piani.

1. Fare clic sul nome di un piano per aprirlo, quindi individuare l&#39;iniziativa che si desidera eliminare.
1. Selezionare le caselle a sinistra delle iniziative che si desidera eliminare, quindi fare clic su **[!UICONTROL Elimina]** dal menu visualizzato nella parte inferiore del piano, quindi fare clic su **[!UICONTROL Sì, eliminale]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   Le iniziative e le relative mansioni e informazioni sui costi vengono eliminate dal piano.

1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.
