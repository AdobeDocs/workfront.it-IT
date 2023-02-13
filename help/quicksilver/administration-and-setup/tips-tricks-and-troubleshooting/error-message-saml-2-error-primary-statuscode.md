---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Messaggio di errore: Errore SAML 2.0: StatusCode principale"
description: Impossibile stabilire una connessione ad ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Messaggio di errore: Errore SAML 2.0: Codice di stato principale

## Problema

Impossibile stabilire una connessione ad ADFS.

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

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

## Causa 1: L&#39;algoritmo hash sicuro è impostato su SHA-256

### Soluzione

1. In Windows, fai clic su **[!UICONTROL Inizio]** > **[!UICONTROL Amministrazione]** > **[!UICONTROL Gestione ADFS 2.0]**.\
   Viene visualizzata la finestra di dialogo Gestione ADFS 2.0.

1. Seleziona **[!UICONTROL Relazione di trust]** > **[!UICONTROL Fiducia nel partito]** nel riquadro a sinistra.

1. Fai clic con il pulsante destro del mouse sull’attendibilità del componente correlata a [!DNL Adobe Workfront], quindi seleziona **[!UICONTROL Proprietà]**.
1. Fai clic sul pulsante **[!UICONTROL Avanzate]** , quindi seleziona **[!UICONTROL SHA-1]** dal **[!UICONTROL Algoritmo hash sicuro]** menu a discesa.\
   ![](assets/1-350x287.png)

## Causa 2: Il certificato di firma ADFS sta per scadere ed è stato sostituito da un nuovo certificato con date sovrapposte

### Soluzione

La [!DNL Workfront] Nella pagina Configurazione SSO è elencata la data di scadenza del certificato. Se il certificato sta per scadere, è necessario estrarre manualmente il nuovo certificato di firma dal server ADFS:

1. In Windows, fai clic su **[!UICONTROL Inizio]** > **[!UICONTROL Amministrazione]** > **[!UICONTROL Gestione ADFS 2.0]**.\
   Viene visualizzata la finestra di dialogo Gestione ADFS 2.0.

1. Seleziona **[!UICONTROL Relazione di trust]** > **[!UICONTROL Fiducia nel partito]** nel riquadro a sinistra.

1. Fai clic con il pulsante destro del mouse sull’attendibilità del componente correlata a [!DNL Workfront], quindi seleziona **[!UICONTROL Proprietà]**.
1. Fai clic sul pulsante **[!UICONTROL Firma]** scheda .
1. Fare clic sul nome del certificato di firma e fare clic su **[!UICONTROL Visualizza]**.
1. Fai clic su Copia in **[!UICONTROL File]**... e seleziona **[!UICONTROL Successivo]**.

1. Seleziona **[!UICONTROL Codifica base 64 x.509 (CER)]** e fai clic su **[!UICONTROL Successivo]**.

1. Specifica il nome del file e fai clic su **[!UICONTROL Successivo]**.
1. Fai clic su **[!UICONTROL Fine]**.
1. In [!DNL Workfront], passa a **[!UICONTROL Configurazione]** > **[!UICONTROL Sistema]** > **[!UICONTROL Single Sign-On (SSO)]** e carica manualmente il certificato di firma.

## Causa 3: Controllo di revoca del certificato non riuscito

La soluzione dipende dalla versione di [!DNL Microsoft] ADFS in uso. Consulta [!DNL Microsoft]Documentazione per ottenere i comandi appropriati per la tua versione.
