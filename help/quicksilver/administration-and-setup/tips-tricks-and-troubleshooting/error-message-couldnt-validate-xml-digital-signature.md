---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Messaggio di errore: impossibile convalidare la firma digitale XML'
description: Impossibile stabilire una connessione ad ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
TQID: https://experienceleague.adobe.com/lPAWprUiJA2ZJFUEdzXNTMTM1oXHEKNpc5VAadI-yqI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 274
ht-degree: 12%

---

# Messaggio di errore: impossibile convalidare la firma digitale XML

## Problema

Impossibile stabilire una connessione ad ADFS.

![messaggio di errore.png](assets/error-message.png)

>[!NOTE]
>
>Se stabilisci una connessione di prova riuscita e riscontri ancora problemi, potresti riscontrare mappature di attributi errate o problemi con gli ID federativi. Per eventuali domande, contatta l’assistenza clienti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Causa 1: il certificato non è corretto

### Soluzione

Recuperare manualmente il certificato di firma dal server ADFS:

1. In [!DNL Windows], fare clic su **[!UICONTROL Avvia]** > **[!UICONTROL Amministrazione]** > **[!UICONTROL Gestione ADFS 2.0]**.\
   Viene visualizzata la finestra di dialogo Gestione ADFS 2.0.

1. Selezionare **[!UICONTROL Relazione di trust]** > **[!UICONTROL Trust tra relatori]** nel riquadro di sinistra.

1. Fare clic con il pulsante destro del mouse su **[!UICONTROL Attendibilità componente]** e selezionare **[!UICONTROL Proprietà]**.

1. Fare clic sulla scheda **[!UICONTROL Firma]**.
1. Fai clic sul nome del certificato di firma e fai clic su **[!UICONTROL Visualizza]**.
1. Fare clic su Copia nel **[!UICONTROL file]**... e selezionare **[!UICONTROL Avanti]**.

1. Selezionare **[!UICONTROL Base-64 codificato x.509 (CER)]** e fare clic su **[!UICONTROL Avanti]**.

1. Specificare il nome del file e fare clic su **[!UICONTROL Avanti]**.
1. Fai clic su **[!UICONTROL Termina]**.
1. In [!DNL Adobe Workfront], passare a **[!UICONTROL Configurazione]** > **[!UICONTROL Sistema]** > **[!UICONTROL Single Sign-On (SSO)]** e caricare manualmente il certificato di firma.

## Causa 2: il certificato è firmato con DSA quando [!DNL Workfront] prevede una firma RSA

### Soluzione

Ricreare il certificato e utilizzare la firma RSA anziché DSA.

## Causa 3: dati XML non corretti

### Soluzione

Riesportare e importare i metadati XML dal sistema di gestione ADFS.

## Causa 4: impossibile eseguire la richiesta a causa di un errore sul lato SAML

### Soluzione

Contatta il provider SAML.
