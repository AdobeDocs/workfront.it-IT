---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Messaggio di errore: Impossibile convalidare la firma digitale XML"
description: Impossibile stabilire una connessione ad ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Messaggio di errore: Impossibile convalidare la firma digitale XML

## Problema

Impossibile stabilire una connessione ad ADFS.

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>Se stabilisci una connessione di test riuscita e riscontri ancora problemi, potresti riscontrare mappature degli attributi non corrette o problemi con gli ID federativi. Per domande, contatta l’assistenza clienti.

## Requisiti di accesso

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Causa 1: Il certificato non è corretto

### Soluzione

Recupera manualmente il certificato di firma dal server ADFS:

1. In [!DNL Windows], fai clic su **[!UICONTROL Inizio]** > **[!UICONTROL Amministrazione]** > **[!UICONTROL Gestione ADFS 2.0]**.\
   Viene visualizzata la finestra di dialogo Gestione ADFS 2.0.

1. Seleziona **[!UICONTROL Relazione di trust]** > **[!UICONTROL Fiducia nel partito]** nel riquadro a sinistra.

1. Fai clic con il pulsante destro del mouse su **[!UICONTROL Affidabilità del gruppo]**, quindi seleziona **[!UICONTROL Proprietà]**.

1. Fai clic sul pulsante **[!UICONTROL Firma]** scheda .
1. Fare clic sul nome del certificato di firma e fare clic su **[!UICONTROL Visualizza]**.
1. Fai clic su Copia in **[!UICONTROL File]**... e seleziona **[!UICONTROL Successivo]**.

1. Seleziona **[!UICONTROL Codifica base 64 x.509 (CER)]** e fai clic su **[!UICONTROL Successivo]**.

1. Specifica il nome del file e fai clic su **[!UICONTROL Successivo]**.
1. Fai clic su **[!UICONTROL Fine]**.
1. In [!DNL Adobe Workfront], passa a **[!UICONTROL Configurazione]** > **[!UICONTROL Sistema]** > **[!UICONTROL Single Sign-On (SSO)]** e carica manualmente il certificato di firma.

## Causa 2: Il certificato viene firmato utilizzando DSA quando [!DNL Workfront] è in attesa di una firma RSA

### Soluzione

Ricrea il certificato e utilizza la firma RSA invece del DSA.

## Causa 3: Dati XML non corretti

### Soluzione

Esportazione e reimportazione dei metadati XML dal sistema di gestione ADFS.

## Causa 4: Impossibile eseguire la richiesta a causa di un errore sul lato SAML

### Soluzione

Contatta il tuo provider SAML.
