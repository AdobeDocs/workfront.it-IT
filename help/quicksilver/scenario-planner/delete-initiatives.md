---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Eliminare le iniziative nel Planner scenario
description: Puoi eliminare le iniziative in un piano creato o in un piano condiviso con te. Non è possibile recuperare le iniziative eliminate.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# Eliminare le iniziative nel [!DNL Scenario Planner]

Puoi eliminare le iniziative in un piano creato o in un piano condiviso con te. Non è possibile recuperare le iniziative eliminate.

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
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo. </p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!UICONTROL Scenario Planner]</a>. </p> </td> 
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

## Eliminare le iniziative

Quando elimini le iniziative, considera quanto segue:

* L&#39;eliminazione di un&#39;iniziativa rimuove dal piano la quantità richiesta di ruoli di lavoro e le informazioni sui costi associate all&#39;iniziativa.
* L’eliminazione di un’iniziativa creata importando un progetto non comporta l’eliminazione del progetto associato all’iniziativa.
* L’eliminazione di un’iniziativa pubblicata su un progetto almeno una volta determina quanto segue:

   * L&#39;iniziativa è cancellata dallo scenario ma [!DNL Scenario Planner] la zona rimane [!UICONTROL Dettagli progetto] sezione .
   * Se l&#39;iniziativa che elimini è l&#39;unica iniziativa pubblicata sullo scenario, viene rimosso anche l&#39;indicatore che il piano è stato pubblicato.

      Per informazioni sulla pubblicazione di iniziative in progetti, consulta [Aggiornare o creare progetti pubblicando iniziative nel [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

      Per informazioni sulla creazione di iniziative importando progetti, consulta [Importa progetti nei piani [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

Puoi eliminare un’iniziativa alla volta oppure più iniziative in blocco.

* [Elimina un&#39;iniziativa](#delete-one-initiative)
* [Eliminare iniziative in blocco](#delete-initiatives-in-bulk)

### Elimina un&#39;iniziativa {#delete-one-initiative}

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png), quindi fai clic su [!UICONTROL Scenari].

   Viene visualizzato un elenco di piani.

1. Fai clic sul nome di un piano per aprirlo, quindi individua l’iniziativa da eliminare.
1. Esegui una delle operazioni seguenti:

   * Fai clic sul pulsante **[!UICONTROL Menu Altro]** ![](assets/more-menu.png) a destra del nome dell&#39;iniziativa, quindi fai clic su **[!UICONTROL Elimina]** > **[!UICONTROL Sì, eliminalo]**.

   * Seleziona la casella a sinistra dell’iniziativa, quindi fai clic su **[!UICONTROL Elimina]** nel menu mobile visualizzato in fondo al piano, quindi fare clic su **[!UICONTROL Sì, eliminalo]**.

   L&#39;iniziativa e il suo ruolo e le informazioni sui costi vengono cancellati dal piano.

1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.

### Eliminare iniziative in blocco {#delete-initiatives-in-bulk}

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png), quindi fai clic su [!UICONTROL Scenari].

   Viene visualizzato un elenco di piani.

1. Fai clic sul nome di un piano per aprirlo, quindi individua l’iniziativa da eliminare.
1. Seleziona le caselle a sinistra delle iniziative da eliminare, quindi fai clic su **[!UICONTROL Elimina]** dal menu visualizzato nella parte inferiore del piano, quindi fare clic su **[!UICONTROL Sì, eliminali]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   Le iniziative, il loro ruolo e le informazioni sui costi vengono cancellate dal piano.

1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche.
