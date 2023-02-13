---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Aggiungere utenti ad Adobe Workfront Fusion tramite Adobe Admin Console
description: È possibile aggiungere un utente a Adobe Admin Console e assegnarlo ad Adobe Workfront Fusion oppure assegnare un utente esistente in Adobe Admin Console a Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
hidefromtoc: true
source-git-commit: 6cd6b1433fb56b92872f0ad80bb1a700fc0854cc
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 1%

---

# Aggiungi utenti a [!DNL Adobe Workfront Fusion] attraverso [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>Le procedure descritte in questa pagina si applicano solo alle organizzazioni che sono state integrate nel [!DNL Adobe Admin Console].
>
>Se la tua organizzazione non è ancora stata effettuata l&#39;onboarding nel [!DNL Adobe Admin Console], vedi [Aggiungi un utente a un&#39;organizzazione in [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>Per un elenco delle procedure che variano a seconda che l&#39;organizzazione sia stata integrata o meno nel [!DNL Adobe Admin Console], vedi [Differenze di amministrazione basate su piattaforma ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

È possibile aggiungere un utente al [!DNL Adobe Admin Console] e assegnarle a [!DNL Adobe Workfront Fusion]oppure assegna un utente esistente nella [!DNL Adobe Admin Console] a [!DNL Workfront Fusion].

Per un video che descrive [!DNL Workfront Fusion] in [!DNL Adobe Admin Console], tra cui come aggiungere utenti, consulta [[!DNL Fusion] su Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> <p>[!UICONTROL Workfront Fusion for Work Automation] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] diritti di amministratore</td> 
   <td>Devi essere un [!UICONTROL Product Configuration Administrator] di [!DNL Adobe] prodotti per la tua organizzazione.</td> 
  </tr>
  </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

&#42;&#42;Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Prerequisiti

Prima di utilizzare [!DNL Admin Console] per [!DNL Workfront], riceverai un messaggio e-mail che ti invita alla console.

1. Se non hai mai utilizzato [!DNL Adobe] e hai ricevuto un&#39;e-mail che ti dice che ora hai i diritti di amministrazione per gestire [!DNL Adobe] software e servizi per la tua organizzazione, fai clic sul pulsante nell’e-mail per creare un [!DNL Adobe] e aprire [!DNL Admin Console].

   Oppure

   Se disponi già di un account di Adobe, passa alla pagina [[!DNL Adobe Admin Console] page](https://adminconsole.adobe.com/).


## Aggiungi un nuovo utente al [!DNL Adobe Admin Console] e [!DNL Workfront Fusion]

1. Da [[!DNL Adobe Admin Console] page](https://adminconsole.adobe.com/), seleziona **[!UICONTROL Prodotti]** nella barra di navigazione superiore, quindi seleziona la **[!DNL Workfront Fusion]** riquadro del prodotto.

   ![Fusione in Admin Console](assets/fusion-product-admin-console.png)

1. Nell’elenco visualizzato, seleziona l’organizzazione in cui desideri aggiungere un utente.

   ![Istanza di fusione in Admin Console](assets/fusion-instances-admin-console.png)

1. Nell’elenco visualizzato, con la **[!UICONTROL Profili di prodotto]** scheda selezionata, fai clic sul nome della [!DNL Workfront Fusion] [!UICONTROL Profilo prodotto] link.

   ![Profilo del prodotto Workfront Fusion](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > Non apportare alcuna modifica al [!UICONTROL Profilo prodotto] stesso.

1. Con la **[!UICONTROL Utenti]** scheda selezionata sopra l’elenco, fai clic su **[!UICONTROL Aggiungi utente]**.

1. In **[!UICONTROL Aggiungi utenti a questo profilo di prodotto]** immettere l&#39;indirizzo e-mail o il nome dell&#39;utente che si desidera aggiungere, quindi selezionare l&#39;utente nell&#39;elenco visualizzato.

1. Fai clic su **[!UICONTROL Salva]**.

   L’utente viene creato in [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Facoltativo) Continua a [Modificare il livello di accesso di un utente in [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Modificare il livello di accesso di un utente in Workfront Fusion

### Modificare il ruolo di un utente in Amministratore

Assegnare a un utente un ruolo Amministratore deve essere fatto nel [!DNL Adobe Admin Console].

1. Sulla [!DNL Workfront Fusion] [!UICONTROL Profilo prodotto] nella pagina in cui hai aggiunto l’utente, seleziona la **[!UICONTROL Amministratori]** scheda .

1. Fai clic su **[!UICONTROL Aggiungi amministratore]**.

1. In **[!UICONTROL Aggiungi amministratori del profilo di prodotto]** immettere l&#39;indirizzo e-mail o il nome dell&#39;utente che si desidera aggiungere, quindi selezionare l&#39;utente nell&#39;elenco visualizzato.

1. Fai clic su **[!UICONTROL Salva]**.

   Questo utente ora è un amministratore in [!DNL Workfront Fusion].

### Modificare il ruolo di un utente in [!UICONTROL Membro], [!UICONTROL Ragioniere]oppure [!UICONTROL Sviluppatore di app].

[!UICONTROL Membro], [!UICONTROL Ragioniere]e [!UICONTROL Sviluppatore di app] i ruoli vengono gestiti all’interno di [!DNL Workfront Fusion].

Per istruzioni, consulta [Visualizzare o modificare i ruoli utente](../organizations/manage-fusion-users.md#view-or-edit-user-roles) nell&#39;articolo [Gestisci [!DNL Adobe Workfront Fusion] utenti della tua organizzazione](../organizations/manage-fusion-users.md)

## Assegna un utente esistente nella [!DNL Adobe Admin Console] a [!DNL Workfront Fusion]

1. Inizia a modificare l’utente come descritto nella sezione &quot;Modifica dettagli utente&quot; dell’articolo [Gestire gli utenti individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) in [!DNL Adobe Admin Console] documentazione.

1. Aggiungi **[!DNL Adobe Workfront Fusion]** ai prodotti assegnati all&#39;utente.
