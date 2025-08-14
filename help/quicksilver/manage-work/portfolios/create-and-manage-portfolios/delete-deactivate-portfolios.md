---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Eliminare e disattivare i portfolio
description: I portafogli sono raccolte di progetti o programmi in Adobe Workfront. Puoi eliminare o disattivare un portfolio se lo ritieni irrilevante per il tuo sistema.
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: 8a4668a568fde2ca7ee26714caae3cd33efe4eda
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 1%

---

# Eliminare e disattivare i portfolio

<!--Audited: 2/2024-->

I portafogli sono insiemi di progetti o programmi in [!DNL Adobe Workfront]. Puoi eliminare o disattivare un portfolio se lo ritieni irrilevante per il tuo sistema.

Consigliamo di disattivare un portfolio che non deve più essere associato a progetti futuri, invece di eliminarlo, per conservare le informazioni storiche sui progetti attualmente associati al portfolio e ai suoi programmi.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso a progetti e portafogli da [!UICONTROL Edit]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di [!UICONTROL Manage] per il portfolio </p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Panoramica sull’eliminazione e la disattivazione dei portfolio

Quando decidi se eliminare o disattivare i portfolio, considera quanto segue:

* L’eliminazione di un portfolio comporta l’eliminazione dei programmi ad esso associati.

  >[!IMPORTANT]
  >
  >Non è necessario disporre di autorizzazioni per i programmi per poter eliminare il portfolio.

* L’eliminazione di un portfolio non comporta l’eliminazione dei relativi progetti.
* Non puoi recuperare i portfolio eliminati.
* La disattivazione di un portfolio assicura che il nome del portfolio e dei relativi programmi non possano più essere assegnati ai progetti durante la creazione di un progetto.
* La disattivazione di un portfolio già associato a un progetto non ne comporta la rimozione dal progetto. Se rimuovi un portfolio disattivato da un progetto, devi riattivarlo prima di poterlo ricollegare al progetto.

## Disattivare un portfolio

Quando disattivi un portfolio, puoi comunque accedervi dall&#39;area [!UICONTROL Portfolio], ma non viene più visualizzato nell&#39;elenco dei portfolio quando gli utenti tentano di aggiungerlo a un progetto.

>[!NOTE]
>
>A seconda della configurazione del modello di layout da parte dell&#39;amministratore di [!DNL Workfront] o gruppo, l&#39;area [!UICONTROL Portfolio] potrebbe non essere visualizzata nel [!UICONTROL Menu principale]. Per ulteriori informazioni, vedere [Personalizzare il menu principale utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

{{step1-click-main-menu}}

1. Fare clic su **[!UICONTROL Portfolio]**.
1. Fai clic sul nome del portfolio.
1. Fai clic sul menu **Altro** ![Altro menu](assets/more-icon.png) a destra del nome del portfolio, quindi fai clic su **[!UICONTROL Disattiva Portfolio]**.
Il portfolio viene immediatamente disattivato.
1. (Facoltativo) Fai clic sul menu **Altro** ![Altro menu](assets/more-icon.png) a destra del nome del portfolio, quindi fai clic su **[!UICONTROL Attiva Portfolio]** per riattivarlo.

## Eliminare un portfolio

{{step1-to-portfolios}}

1. Esegui una delle operazioni seguenti:

   * Seleziona il portfolio nell&#39;elenco, quindi fai clic sull&#39;icona **[!UICONTROL Elimina]** ![Elimina](assets/delete.png).
   * Fai clic sul portfolio per aprirlo, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-icon.png) a destra del nome del portfolio, quindi **Elimina Portfolio**.
1. Fai clic su **[!UICONTROL Sì, elimina]** per confermare.

   Il portfolio viene eliminato e non può essere recuperato.
