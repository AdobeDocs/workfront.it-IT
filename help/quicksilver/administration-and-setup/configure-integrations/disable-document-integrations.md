---
title: Disabilita integrazioni documenti
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: In qualità di amministratore  [!DNL anAdobe] [!DNL Workfront], puoi disabilitare la connessione tra Workfront e qualsiasi provider di documenti di terze parti.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 1%

---

# Disattiva integrazioni documenti

In qualità di amministratore [!DNL Adobe] [!DNL Workfront], puoi disabilitare la connessione tra [!DNL Workfront] e qualsiasi provider di documenti di terze parti.

Quando si disattiva la connessione tra [!DNL Workfront] e un provider di documenti, i collegamenti ai documenti scompaiono da [!DNL Workfront]. Gli utenti non possono più visualizzare i documenti collegati, non possono apportare modifiche ai documenti tramite i collegamenti [!DNL Workfront] e non possono aggiungere altri documenti a tale provider.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Devi essere un amministratore [!DNL Workfront]. Per informazioni sugli amministratori di [!DNL Workfront], vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

+++

## Disabilita integrazioni provider cloud

Per disabilitare le integrazioni dei documenti per [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Accedere a [!DNL Workfront] come amministratore [!DNL Workfront].

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Provider cloud]**.

1. Deselezionare uno dei provider cloud da cui si desidera disconnettersi da [!DNL Workfront].
1. Fai clic su **[!UICONTROL Salva]**.

   Gli utenti non possono connettersi al provider cloud specifico disabilitato e non possono più collegare i documenti da tale provider cloud a Workfront.

## Disattiva l&#39;integrazione di [!DNL SharePoint]

1. Accedere a [!DNL Workfront] come amministratore [!DNL Workfront].

{{step-1-to-setup}}

1. Espandere **[!UICONTROL Documenti]**, quindi fare clic su **[!UICONTROL [!DNL SharePoint]Integrazione]**.
1. Selezionare l&#39;integrazione di [!DNL SharePoint] da disabilitare.
1. Fare clic su **[!UICONTROL Disattiva]**.\
   Gli utenti non possono connettersi al sito [!DNL SharePoint] disabilitato e non possono più collegare documenti da [!DNL SharePoint] a [!DNL Workfront].

## Disattiva integrazioni personalizzate

1. Accedere a [!DNL Workfront] come amministratore.

{{step-1-to-setup}}

1. Fai clic su **[!UICONTROL Documenti]** > **[!UICONTROL Integrazione personalizzata]**.
1. Seleziona l’integrazione personalizzata da disabilitare.
1. Fare clic su **[!UICONTROL Disattiva]**.

   Gli utenti non possono connettersi al provider di documenti di terze parti disabilitato e non possono più collegare i documenti da tale provider di cloud a [!DNL Workfront].
