---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Visualizzare il registro attività Jira
description: In qualità di amministratore di  [!DNL Jira] , puoi visualizzare le eccezioni e gli errori che si verificano durante la sincronizzazione o la creazione dei ticket tra [!DNL Adobe Workfront] e [!DNL Jira] in un registro attività.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 5%

---

# Visualizza il registro attività [!UICONTROL [!DNL Jira]]

>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Nell&#39;ambito di questo processo di transizione, l&#39;integrazione Workfront for Jira non sarà disponibile dopo il **28 febbraio 2026**.
>
>È consigliabile utilizzare l’automazione e l’integrazione di Workfront per le esigenze di integrazione della tua organizzazione con Jira.
>
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Jira, vedere [Moduli software Jira](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

In qualità di amministratore [!DNL Jira], puoi visualizzare le eccezioni e gli errori che si verificano durante la sincronizzazione o la creazione dei ticket tra [!DNL Adobe Workfront] e [!DNL Jira] in un [!UICONTROL registro attività].

Nel registro attività puoi trovare fino a 500 elementi, elencati a partire da quelli più recenti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard </p>
       <p>Piano </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Accesso Jira</td> 
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: è consigliabile creare account amministratore di sistema separati in Jira e Workfront per dedicarsi a questa integrazione, anziché utilizzare account esistenti che potrebbero essere collegati agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di collegare gli elementi tra [!DNL Workfront] e [!DNL Jira], è necessario

* Installa [!DNL Workfront for Jira]

  Per istruzioni sull&#39;installazione di [!DNL Workfront for Jira], vedere [Installa [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Accedere al registro attività [!UICONTROL [!DNL Jira]]:

1. Accedi a Jira come amministratore di sistema.
1. Fare clic su **[!UICONTROL Impostazioni]** nel menu principale di [!DNL Jira].
1. Fai clic su **[!UICONTROL Componenti aggiuntivi]**, quindi su **[!UICONTROL Gestisci componenti aggiuntivi]**.

1. Espandere il componente aggiuntivo **[!DNL Workfront]**.
1. Fare clic su **[!UICONTROL Configura]**.
1. Accedere a [!DNL Workfront] come amministratore di sistema.
1. Selezionare la scheda **[!UICONTROL Registro attività]**.

   Visualizzare informazioni sulle eccezioni e sugli errori che si sono verificati durante la creazione degli elementi o la sincronizzazione dei campi tra le due applicazioni.

   Il registro include i campi seguenti:

   * Data dell’occorrenza
   * Nome dell’utente in Jira
   * Numero problema Jira
   * Breve descrizione dell’errore che si è verificato.
