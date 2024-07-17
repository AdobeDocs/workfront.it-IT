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
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 1%

---

# Aggiungi utenti a [!DNL Adobe Workfront Fusion] tramite [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>Le procedure descritte in questa pagina si applicano solo alle organizzazioni che sono state caricate in [!DNL Adobe Admin Console].
>
>Se la tua organizzazione non è ancora stata integrata in [!DNL Adobe Admin Console], vedi [Aggiungere un utente a un&#39;organizzazione in [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>Per un elenco delle procedure che differiscono a seconda che l&#39;organizzazione sia stata integrata in [!DNL Adobe Admin Console], vedere [Differenze di amministrazione basate su Platform ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

È possibile aggiungere un utente a [!DNL Adobe Admin Console] e assegnarlo a [!DNL Adobe Workfront Fusion] oppure assegnare un utente esistente in [!DNL Adobe Admin Console] a [!DNL Workfront Fusion].

Per un video che descrive [!DNL Workfront Fusion] in [!DNL Adobe Admin Console], incluso come aggiungere utenti, vedi [[!DNL Fusion] su Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] diritti di amministratore</td> 
   <td>Devi essere un [!UICONTROL Product Configuration Administrator] di [!DNL Adobe] prodotti per la tua organizzazione.</td> 
  </tr>
  </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

&#42;&#42;Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Prerequisiti

Prima di utilizzare [!DNL Admin Console] per [!DNL Workfront], è necessario ricevere un&#39;e-mail di invito alla console.

1. Se sei alle prime armi con [!DNL Adobe] e hai ricevuto un&#39;e-mail che ti informa che ora disponi dei diritti di amministrazione per gestire software e servizi [!DNL Adobe] per la tua organizzazione, fai clic sul pulsante nell&#39;e-mail per creare un account [!DNL Adobe] e aprire [!DNL Admin Console].

   Oppure

   Se disponi già di un account Adobe, passa alla [[!DNL Adobe Admin Console] pagina](https://adminconsole.adobe.com/).


## Aggiungi un nuovo utente a [!DNL Adobe Admin Console] e [!DNL Workfront Fusion]

1. Dalla [[!DNL Adobe Admin Console] pagina](https://adminconsole.adobe.com/), seleziona la scheda **[!UICONTROL Prodotti]** nella barra di navigazione superiore, quindi fai clic sul riquadro del prodotto **[!DNL Workfront Fusion]**.

   ![Fusione in Admin Console](assets/fusion-product-admin-console.png)

1. Nell’elenco visualizzato, seleziona l’organizzazione in cui desideri aggiungere un utente.

   ![Istanza Fusion in Admin Console](assets/fusion-instances-admin-console.png)

1. Nell&#39;elenco visualizzato, con la scheda **[!UICONTROL Profili prodotto]** selezionata, fare clic sul collegamento [!DNL Workfront Fusion] [!UICONTROL Profilo prodotto].

   ![Profilo prodotto Workfront Fusion](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > Non apportare modifiche al [!UICONTROL profilo di prodotto] stesso.

1. Con la scheda **[!UICONTROL Utenti]** selezionata sopra l&#39;elenco, fare clic su **[!UICONTROL Aggiungi utente]**.

1. Nella casella **[!UICONTROL Aggiungi utenti a questo profilo di prodotto]**, immetti l&#39;indirizzo e-mail o il nome di un utente che desideri aggiungere, quindi seleziona l&#39;utente nell&#39;elenco visualizzato.

1. Fai clic su **[!UICONTROL Salva]**.

   L&#39;utente è stato creato in [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Facoltativo) Continua con [Modifica il livello di accesso di un utente in [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Modificare il livello di accesso di un utente in Workfront Fusion

### Cambia il ruolo di un utente in Amministratore

L&#39;assegnazione di un ruolo di amministratore a un utente deve essere eseguita in [!DNL Adobe Admin Console].

1. Nella pagina [!DNL Workfront Fusion] [!UICONTROL Profilo prodotto] in cui hai aggiunto l&#39;utente, seleziona la scheda **[!UICONTROL Amministratori]**.

1. Fai clic su **[!UICONTROL Aggiungi amministratore]**.

1. Nella casella **[!UICONTROL Aggiungi amministratori del profilo di prodotto]**, inserisci l&#39;indirizzo e-mail o il nome di un utente che desideri aggiungere, quindi seleziona l&#39;utente nell&#39;elenco visualizzato.

1. Fai clic su **[!UICONTROL Salva]**.

   L&#39;utente è ora un amministratore in [!DNL Workfront Fusion].

### Cambia il ruolo di un utente in [!UICONTROL Membro], [!UICONTROL Contabile] o [!UICONTROL Sviluppatore app].

I ruoli [!UICONTROL Membro], [!UICONTROL Contabile] e [!UICONTROL Sviluppatore app] sono gestiti in [!DNL Workfront Fusion].

Per istruzioni, consulta [Visualizzare o modificare i ruoli utente](../organizations/manage-fusion-users.md#view-or-edit-user-roles) nell&#39;articolo [Gestire [!DNL Adobe Workfront Fusion] gli utenti dell&#39;organizzazione](../organizations/manage-fusion-users.md)

## Assegna un utente esistente in [!DNL Adobe Admin Console] a [!DNL Workfront Fusion]

1. Inizia a modificare l&#39;utente come descritto nella sezione &quot;Modifica dettagli utente&quot; dell&#39;articolo [Gestisci gli utenti singolarmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) nella documentazione di [!DNL Adobe Admin Console].

1. Aggiungi **[!DNL Adobe Workfront Fusion]** ai prodotti assegnati all&#39;utente.
