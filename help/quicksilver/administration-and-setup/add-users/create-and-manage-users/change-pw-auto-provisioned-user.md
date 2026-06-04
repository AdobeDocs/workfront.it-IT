---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Modificare la password per un utente con provisioning automatico
description: È consigliabile modificare il nome utente di un nuovo utente con il proprio indirizzo di posta Workfront, quindi consentire agli utenti di modificare la password.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
TQID: https://experienceleague.adobe.com/rC6FrOsS-RttMBDmncvjSbt-n7X9--DblMlHM3sq2Jk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 456
ht-degree: 11%

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

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Amministratore di sistema</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificare la password per un utente con provisioning automatico

1. Determinare il nome utente GUID di un utente trasmettendo una richiesta API, come illustrato nell&#39;esempio seguente:

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&ID=`<ID of User>` Dove *`<domain>`* è il dominio della tua azienda e *`<ID of User>`* è l'ID Workfront dell'utente.

   Ricevi una risposta simile alla seguente:

   ![Ottieni GUID](assets/get-guid.png)

   Il valore restituito per &quot;username&quot; è il GUID dell&#39;utente.

1. Utilizzando il GUID come nome utente, modificare la password dell&#39;utente.

   Per ulteriori informazioni sulla modifica della password, vedere [Reimpostare la password](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Se l&#39;organizzazione utilizza un sistema SSO, solo un amministratore di sistema Workfront può modificare la password di un utente. Per ulteriori informazioni, vedere [Panoramica del Single Sign-On in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. Dopo che l’utente ha effettuato l’accesso a Workfront, passa a:

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. Nella casella **Indirizzo e-mail di accesso**, verifica che l&#39;indirizzo e-mail dell&#39;utente sia corretto, quindi fai clic su **Aggiorna account**.

   ![Nome utente](assets/guidusername-350x272.png)

   Il nome utente dell’utente viene modificato nel relativo indirizzo e-mail Workfront.

>[!TIP]
>
>Per trovare l&#39;ID di un utente:
>
>1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic sull&#39;icona **Users** ![Users](assets/users-icon-in-main-menu.png).
>
>1. Seleziona l’utente.
>
>   Viene visualizzata la pagina del profilo dell’utente e il relativo ID utente nell’URL.
>
