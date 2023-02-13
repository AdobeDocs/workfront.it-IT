---
title: Disattivazione delle integrazioni di documenti
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Come [!DNL anAdobe] [!DNL Workfront] amministratore, è possibile disattivare la connessione tra Workfront e qualsiasi provider di documenti di terze parti.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Disattivazione delle integrazioni di documenti

Come [!DNL Adobe] [!DNL Workfront] amministratore, puoi disattivare la connessione tra [!DNL Workfront] e di qualsiasi fornitore di documenti di terze parti.

Quando si disattiva la connessione tra [!DNL Workfront] e un provider di documenti, i collegamenti ai documenti scompaiono [!DNL Workfront]. Gli utenti non possono più visualizzare i documenti collegati, non possono apportare alcuna modifica ai documenti tramite il [!DNL Workfront] e non possono aggiungere altri documenti a tale provider.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Disattivazione delle integrazioni del provider cloud

Per disabilitare le integrazioni di documenti per [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Accedi a [!DNL Workfront] come [!DNL Workfront] amministratore.
1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Provider cloud]**.

1. Deseleziona uno dei provider cloud da cui vuoi disconnetterti [!DNL Workfront].
1. Fai clic su **[!UICONTROL Salva]**.

   Gli utenti non sono in grado di connettersi al provider cloud specifico disabilitato e non possono più collegare documenti da tale provider cloud a Workfront.

## Disattiva la [!DNL SharePoint] integrazione

1. Accedi a [!DNL Workfront] come [!DNL Workfront] amministratore.
1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Espandi **[!UICONTROL Documenti]**, quindi fai clic su **[!UICONTROL [!DNL SharePoint]Integrazione]**.
1. Seleziona la [!DNL SharePoint] integrazione da disattivare.
1. Fai clic su **[!UICONTROL Disattiva]**.\
   Gli utenti non sono in grado di connettersi al [!DNL SharePoint] sito disabilitato e non possono più collegare documenti da [!DNL SharePoint] a [!DNL Workfront].

## Disattivazione delle integrazioni personalizzate

1. Accedi a [!DNL Workfront] come amministratore.
1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Integrazione personalizzata]**.
1. Seleziona l’integrazione personalizzata da disabilitare.
1. Fai clic su **[!UICONTROL Disattiva]**.

   Gli utenti non sono in grado di connettersi al provider di documenti di terze parti disabilitato e non possono più collegare documenti da tale provider cloud a [!DNL Workfront].
