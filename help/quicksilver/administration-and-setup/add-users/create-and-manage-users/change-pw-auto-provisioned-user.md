---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Modificare la password per un utente con provisioning automatico
description: Spesso, quando un nuovo utente tenta di modificare la propria password temporanea, immette il proprio indirizzo e-mail e riceve un errore in caso di nome utente errato. Devono immettere il nome utente assegnato dal sistema, ovvero il GUID (Globally Unique Identifier). Poiché un GUID è difficile da ricordare e utilizzare, si consiglia di modificare il nome utente di un nuovo utente con il proprio indirizzo di posta elettronica Workfront, quindi di consentire la modifica della password.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# Modificare la password per un utente con provisioning automatico

Quando crei gli utenti tramite il provisioning automatico, Adobe Workfront assegna loro un GUID (Globally Unique Identifier) per un nome utente. Un GUID è una stringa univoca di numeri e lettere casuali, ad esempio *5489cb430012526e1ea635e8c29f377f*.

Spesso, quando un nuovo utente cerca di modificare la password temporanea, inserisce il proprio indirizzo e-mail per il nome utente e riceve un errore per un nome utente errato. Per poter modificare la password, l&#39;utente deve immettere il nome utente assegnato dal sistema, ovvero un GUID.

Poiché i nomi utente GUID possono essere difficili da utilizzare, si consiglia di modificare innanzitutto il nome utente di un utente con il proprio indirizzo di posta elettronica Workfront, quindi di consentire loro di modificare la password.

>[!TIP]
>
>È possibile trovare il GUID di un utente nei modi seguenti:
>
>* Vai al profilo dell’utente e copia il GUID dall’URL nel browser.
>
>  Ad esempio, nell&#39;URL `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`, si copia la stringa di numeri e lettere tra le ultime due barre: `61941ab1000af22d7104628efa1c738b`.
>
>  Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* Creare un report utente con una colonna Utente > GUID. Per ulteriori informazioni, vedere [Creare un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* Eseguire una query sull’API di Workfront.
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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modificare la password per un utente con provisioning automatico

1. Determinare il nome utente GUID di un utente trasmettendo una richiesta API, come illustrato nell&#39;esempio seguente:

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` Dove *`<domain>`* è il dominio della tua azienda e *`<ID of User>`* è l&#39;ID Workfront dell&#39;utente.

   Ricevi una risposta simile alla seguente:

   ![](assets/get-guid.png)

   Il valore restituito per &quot;username&quot; è il GUID dell&#39;utente.

1. Utilizzando il GUID come nome utente, modificare la password dell&#39;utente.

   Per ulteriori informazioni sulla modifica della password, vedere [Reimpostare la password](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Se l&#39;organizzazione utilizza un sistema SSO, solo un amministratore di sistema Workfront può modificare la password di un utente. Per ulteriori informazioni, vedere [Panoramica del Single Sign-On in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. Dopo che l’utente ha effettuato l’accesso a Workfront, passa a:

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. Nella casella **Indirizzo e-mail di accesso**, verifica che l&#39;indirizzo e-mail dell&#39;utente sia corretto, quindi fai clic su **Aggiorna account**.

   ![](assets/guidusername-350x272.png)

   Il nome utente dell’utente viene modificato nel relativo indirizzo e-mail Workfront.

>[!TIP]
>
>Per trovare l&#39;ID di un utente:
>
>1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).
>
>1. Seleziona l’utente.
>
>   Viene visualizzata la pagina del profilo dell’utente e il relativo ID utente nell’URL.
>
