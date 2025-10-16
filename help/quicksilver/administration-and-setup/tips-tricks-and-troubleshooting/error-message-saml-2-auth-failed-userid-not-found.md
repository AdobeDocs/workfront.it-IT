---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Messaggio di errore: autenticazione SAML 2.0 non riuscita: identificatore utente non trovato'
description: Quando si utilizza SAML 2.0, l'errore "SAML 2.0 Authentication Failed-User Identifier Not Found" (Identificatore utente non riuscito con autenticazione SAML 2.0 non trovato) indica che un ID UID o NAME non viene passato dalle regole di attestazione ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 1%

---

# Messaggio di errore: autenticazione SAML 2.0 non riuscita: identificatore utente non trovato

## Problema

Viene visualizzato questo errore quando si utilizza SAML 2.0: &quot;Autenticazione SAML 2.0 non riuscita: Identificatore utente non trovato&quot;.

## Causa

Ciò si verifica quando **UID** o **NAME ID** non viene passato dalle **regole attestazione ADFS**.

In ADFS l&#39;attendibilità del componente **Relying Party** deve avere una **regola attestazione** che trasmette un valore **UID** o un valore **NAME ID**. Quando si esegue una connessione di prova **[!DNL Workfront]**, questa dovrebbe essere visualizzata in caso di esito positivo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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

## Soluzione

1. Durante la modifica di **[!UICONTROL INFORMAZIONI ADFS]**, in **[!UICONTROL Trust relying party]** > Seleziona oggetto >**[!UICONTROL Modifica regole attestazione]**.

1. L&#39;**[!UICONTROL attributo LDAP]** (colonna sinistra) deve avere **[!UICONTROL indirizzi di posta elettronica]** (o un identificatore univoco).

1. Il tipo di attestazione **[!UICONTROL in uscita]** (colonna a destra) deve essere **[!UICONTROL ID nome]**.

   >[!NOTE]
   >
   >Non è necessario che disponga degli indirizzi di posta elettronica degli attributi LDAP. Qualsiasi identificatore univoco che identificherà l&#39;utente può essere utilizzato, ma deve essere passato in [!DNL Adobe Workfront] come **ID NOME**.
