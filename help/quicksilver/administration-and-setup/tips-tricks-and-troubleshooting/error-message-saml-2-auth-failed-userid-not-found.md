---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '"Messaggio di errore: Autenticazione SAML 2.0 non riuscita: Identificatore utente non trovato'
description: Quando utilizzi SAML 2.0, l'errore "SAML 2.0 Authentication Failed-User Identifier Not Found" significa che un UID o un ID di nome non viene passato dalle regole di attestazione ADFS. In ADFS l'attendibilità del componente deve avere una regola di attestazione che trasmette un UID o un valore ID del nome. Quando si esegue un [!DNL Workfront] Prova connessione, questa deve essere visualizzata in caso di esito positivo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Messaggio di errore: Autenticazione SAML 2.0 non riuscita: Identificatore utente non trovato

## Problema

Ricevo questo errore quando si utilizza SAML 2.0: &quot;Autenticazione SAML 2.0 non riuscita: Identificatore utente non trovato.&quot;

## Causa

Questo accade quando una **UID** o **ID NOME** non viene passato dal **Regole di attestazione ADFS**.

In ADFS la funzione **Affidabilità del gruppo** deve avere un **Regola di richiesta** che passa una **UID** o **ID NOME** valore. Quando si esegue un **[!DNL Workfront]Prova connessione**, dovrebbe mostrarlo in caso di esito positivo.

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

## Soluzione

1. Durante la modifica del **[!UICONTROL INFORMAZIONI ADFS]**, nella **[!UICONTROL Fiducia nel partito]** > Seleziona oggetto >**[!UICONTROL Modifica regole di attestazione]**.

1. La **[!UICONTROL Attributo LDAP]** (colonna a sinistra) dovrebbe essere **[!UICONTROL Indirizzi di posta elettronica]** (o qualsiasi identificatore univoco).

1. La **[!UICONTROL Tipo di attestazione in uscita]** (colonna a destra) deve essere **[!UICONTROL ID nome]**.

   >[!NOTE]
   >
   >Non deve avere gli indirizzi e-mail dell&#39;attributo LDAP. È possibile utilizzare qualsiasi identificatore univoco che identifichi l’utente, ma deve essere trasmesso in [!DNL Adobe Workfront] come **ID NOME**.
