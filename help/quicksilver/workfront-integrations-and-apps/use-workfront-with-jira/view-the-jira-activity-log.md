---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Visualizzare il registro attività Jira
description: In qualità di amministratore di  [!DNL Jira] , puoi visualizzare le eccezioni e gli errori che si verificano durante la sincronizzazione o la creazione dei ticket tra [!DNL Adobe Workfront] e [!DNL Jira] in un registro attività.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Visualizza il registro attività [!UICONTROL [!DNL Jira]]

In qualità di amministratore [!DNL Jira], puoi visualizzare le eccezioni e gli errori che si verificano durante la sincronizzazione o la creazione dei ticket tra [!DNL Adobe Workfront] e [!DNL Jira] in un [!UICONTROL registro attività].

Nel registro attività puoi trovare fino a 500 elementi, elencati a partire da quelli più recenti.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] piano</a>*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica licenze Adobe [!DNL Workfront]</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accesso</td> 
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: è consigliabile creare account di amministratore di sistema separati in [!DNL Jira] e [!DNL Workfront] per dedicarsi a questa integrazione, anziché utilizzare account esistenti che potrebbero essere collegati agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Devi essere un amministratore [!DNL Workfront]. Per informazioni sugli amministratori di [!DNL Workfront], vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

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
