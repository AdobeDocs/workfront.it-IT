---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Messaggio di errore: autenticazione SAML 2.0 non riuscita: identificatore utente non trovato"
description: Quando si utilizza SAML 2.0, l'errore "SAML 2.0 Authentication Failed-User Identifier Not Found" (Identificatore utente non riuscito con autenticazione SAML 2.0 non trovato) indica che un UID o un ID NAME non viene passato dalle regole di attestazione ADFS. In ADFS l'attendibilità della relying party deve disporre di una regola di attestazione che trasmette un UID o un valore di ID NAME. Quando esegui una connessione di prova  [!DNL Workfront] , questa dovrebbe essere visualizzata in caso di esito positivo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Messaggio di errore: autenticazione SAML 2.0 non riuscita: identificatore utente non trovato

## Problema

Viene visualizzato questo errore quando si utilizza SAML 2.0: &quot;Autenticazione SAML 2.0 non riuscita: Identificatore utente non trovato&quot;.

## Causa

Ciò si verifica quando un **UID** o un **ID NOME** non viene passato dalle **regole attestazione ADFS**.

In ADFS l&#39;attendibilità del componente **Relying Party** deve avere una **regola attestazione** che passa un valore **UID** o **NAME ID**. Quando si esegue una connessione di prova **[!DNL Workfront]**, questa dovrebbe essere visualizzata in caso di esito positivo.

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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore [!DNL Workfront]. Per ulteriori informazioni, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Soluzione

1. Durante la modifica di **[!UICONTROL INFORMAZIONI ADFS]**, in **[!UICONTROL Trust relying party]** > Seleziona oggetto >**[!UICONTROL Modifica regole attestazione]**.

1. L&#39;**[!UICONTROL attributo LDAP]** (colonna sinistra) deve avere **[!UICONTROL indirizzi di posta elettronica]** (o un identificatore univoco).

1. Il tipo di attestazione **[!UICONTROL in uscita]** (colonna a destra) deve essere **[!UICONTROL ID nome]**.

   >[!NOTE]
   >
   >Non è necessario che disponga degli indirizzi di posta elettronica degli attributi LDAP. Qualsiasi identificatore univoco che identificherà l&#39;utente può essere utilizzato, ma deve essere passato in [!DNL Adobe Workfront] come **ID NOME**.
