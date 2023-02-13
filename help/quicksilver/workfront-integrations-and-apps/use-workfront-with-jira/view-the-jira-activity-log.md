---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Visualizza il registro delle attività di Jira
description: Come [!DNL Jira] amministratore, puoi visualizzare le eccezioni e gli errori che si verificano durante la sincronizzazione o la creazione dei ticket tra [!DNL Adobe Workfront] e [!DNL Jira] in un registro delle attività.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Visualizza la [!UICONTROL [!DNL Jira] Registro attività]

Come [!DNL Jira] amministratore, puoi visualizzare le eccezioni e gli errori che si verificano durante la sincronizzazione o la creazione dei ticket tra [!DNL Adobe Workfront] e [!DNL Jira] in [!UICONTROL Registro attività].

Puoi visualizzare fino a 500 elementi nel Registro attività e sono elencati a partire da quelli più recenti.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] piano</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] panoramica delle licenze</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accesso</td> 
   <td> <p>Accesso amministratore di sistema</p> <p>Importante: È consigliabile creare account di amministratore di sistema separati in [!DNL Jira] e [!DNL Workfront] per dedicare a questa integrazione, anziché utilizzare quelle esistenti che potrebbero essere collegate agli utenti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Prerequisiti

Prima di poter collegare elementi tra [!DNL Workfront] e [!DNL Jira], devi

* Installa [!DNL Workfront for Jira]

   Per istruzioni sull’installazione [!DNL Workfront for Jira], vedi [Installa [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Accedere al [!UICONTROL [!DNL Jira] Registro attività]:

1. Accedi a Jira come amministratore di sistema.
1. Fai clic su **[!UICONTROL Impostazioni]** nella [!DNL Jira] menu.
1. Fai clic su **[!UICONTROL Componenti aggiuntivi]**, quindi **[!UICONTROL Gestire i componenti aggiuntivi]**.

1. Espandi la **[!DNL Workfront]** add-on.
1. Fai clic su **[!UICONTROL Configura]**.
1. Accedi a [!DNL Workfront] come amministratore di sistema.
1. Seleziona la **[!UICONTROL Registro attività]** scheda .

   Visualizza informazioni sulle eccezioni e gli errori che si sono verificati durante la creazione di elementi o la sincronizzazione di campi tra le due applicazioni.

   Il registro include i campi seguenti:

   * Data dell&#39;evento
   * Nome dell&#39;utente in Jira
   * Numero della partita
   * Breve descrizione dell’errore che si è verificato.
