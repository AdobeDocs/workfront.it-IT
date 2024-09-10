---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Messaggio di errore: errore SAML 2.0: identificatore utente non trovato"
description: Impossibile stabilire una connessione ad ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 1%

---

# Messaggio di errore: errore SAML 2.0: identificatore utente non trovato

## Problema

Impossibile stabilire una connessione ad ADFS.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>Se stabilisci una connessione di prova riuscita e riscontri ancora problemi, potresti riscontrare mappature di attributi errate o problemi con gli ID federativi. Per eventuali domande, contatta l’assistenza clienti.

## Causa:

Le dichiarazioni sul server ADFS non sono corrette.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td>
   <p>Nuovo: Standard</p>
   <p>oppure</p>
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Soluzione

Sul server ADFS verificare che sia presente una richiesta per l&#39;ID nome:

1. In Windows, fare clic su **[!UICONTROL Avvia]** > **[!UICONTROL Amministrazione]** > **[!UICONTROL Gestione ADFS 2.0]**.\
   Viene visualizzata la finestra di dialogo Gestione ADFS 2.0.

1. Selezionare **[!UICONTROL Relazione di trust]** > **[!UICONTROL Trust tra relatori]** nel riquadro di sinistra.

1. Fare clic con il pulsante destro del mouse sull&#39;attendibilità del componente correlata ad Adobe Workfront e selezionare **[!UICONTROL Modifica regole attestazione]**.
1. Verificare che l&#39;attestazione contenga un **[!UICONTROL Tipo di attestazione in uscita]** di **[!UICONTROL ID nome]**.

![1.png](assets/1-350x287.png)
