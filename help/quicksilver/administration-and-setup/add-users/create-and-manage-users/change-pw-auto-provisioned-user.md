---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Modificare la password per un utente con provisioning automatico
description: Spesso, quando un nuovo utente tenta di modificare la propria password temporanea, immette il proprio indirizzo e-mail e riceve un errore per un nome utente errato. Devono immettere il nome utente assegnato al sistema, ovvero il GUID (Globally Unique Identifier). Poiché un GUID è difficile da ricordare e utilizzare, è consigliabile modificare il nome utente di un nuovo utente con il relativo indirizzo di posta elettronica Workfront, quindi consentire loro di modificare la password.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Modificare la password per un utente con provisioning automatico

Quando crei utenti tramite il provisioning automatico, Adobe Workfront assegna loro un GUID (identificatore univoco globale) per un nome utente. Un GUID è una stringa univoca di numeri e lettere casuali, ad esempio *5489cb430012526e1ea635e8c29f377f*.

Spesso, quando un nuovo utente tenta di modificare la propria password temporanea, immette il proprio indirizzo e-mail per il proprio nome utente e riceve un errore per un nome utente errato. Affinché l’utente possa modificare la propria password, deve immettere il nome utente assegnato dal sistema, ovvero un GUID.

Poiché i nomi utente GUID possono essere difficili da utilizzare, si consiglia innanzitutto di modificare il nome utente di un utente con il proprio indirizzo di posta elettronica Workfront, quindi di consentire loro di modificare la password.

>[!TIP]
>
>È possibile trovare il GUID di un utente nei seguenti modi:
>
>* Passa al profilo dell’utente e copia il GUID dall’URL nel browser.
>
>  Ad esempio, nell’URL `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`, copi la stringa di numeri e lettere tra le ultime due barre: `61941ab1000af22d7104628efa1c738b`.
>
>  Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* Creare un rapporto utente con una colonna Utente > GUID . Per ulteriori informazioni, consulta [Creare un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* Esegui una query sull’API Workfront.
>


## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modificare la password per un utente con provisioning automatico

1. Determinare il nome utente GUID di un utente passando una richiesta API, come illustrato nell’esempio seguente:

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` Dove *`<domain>`* è di dominio della tua azienda e *`<ID of User>`* è l&#39;Workfront ID dell&#39;utente.

   Ricevi una risposta simile alla seguente:

   ![](assets/get-guid.png)

   Il valore restituito per &quot;username&quot; è il GUID dell&#39;utente.

1. Utilizzando il GUID come nome utente, modificare la password dell&#39;utente.

   Per ulteriori informazioni sulla modifica della password, consulta [Ripristino della password](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Se l&#39;organizzazione utilizza un sistema SSO, solo un amministratore di sistema Workfront può modificare la password di un utente. Per ulteriori informazioni, consulta [Panoramica del single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. Con l’utente che ha effettuato l’accesso a Workfront, passa a:

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. In **Indirizzo e-mail di accesso** verificare che l&#39;indirizzo e-mail dell&#39;utente sia corretto, quindi fare clic su **Aggiorna account**.

   ![](assets/guidusername-350x272.png)

   Il nome utente dell’utente viene modificato nell’indirizzo e-mail di Workfront.

>[!TIP]
>
>Per trovare l&#39;ID di un utente:
>
>1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).
>
>1. Seleziona l’utente.
>
>   Viene visualizzata la pagina del profilo dell’utente e il relativo ID utente nell’URL.
