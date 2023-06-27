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
source-wordcount: '634'
ht-degree: 1%

---

# Aggiungi utenti a [!DNL Adobe Workfront Fusion] tramite [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>Le procedure descritte in questa pagina si applicano solo alle organizzazioni che sono state caricate in [!DNL Adobe Admin Console].
>
>Se la tua organizzazione non è ancora stata integrata in [!DNL Adobe Admin Console], vedi [Aggiungere un utente a un’organizzazione in [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>Per un elenco di procedure che differiscono in base al fatto che la tua organizzazione sia stata caricata su [!DNL Adobe Admin Console], vedi [Differenze di amministrazione basate sulla piattaforma ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

È possibile aggiungere un utente al [!DNL Adobe Admin Console] e assegnarli a [!DNL Adobe Workfront Fusion]o assegnare un utente esistente in [!DNL Adobe Admin Console] a [!DNL Workfront Fusion].

Per un video che descrive [!DNL Workfront Fusion] nel [!DNL Adobe Admin Console], tra cui come aggiungere utenti, vedi [[!DNL Fusion] su Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

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
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] diritti di amministratore</td> 
   <td>Devi essere un [!UICONTROL Product Configuration Administrator] di [!DNL Adobe] per la tua organizzazione.</td> 
  </tr>
  </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

&#42;&#42;Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Prerequisiti

Prima di utilizzare [!DNL Admin Console] per [!DNL Workfront], dovresti ricevere un’e-mail con l’invito a partecipare alla console.

1. Se non hai ancora utilizzato [!DNL Adobe] e hai ricevuto un’e-mail che ti diceva che ora disponi dei diritti di amministrazione per gestire [!DNL Adobe] software e servizi per la tua organizzazione, fai clic sul pulsante nell’e-mail per creare un’ [!DNL Adobe] e aprire il [!DNL Admin Console].

   Oppure

   Se disponi già di un account Adobe, vai al [[!DNL Adobe Admin Console] pagina](https://adminconsole.adobe.com/).


## Aggiungi un nuovo utente al [!DNL Adobe Admin Console] e [!DNL Workfront Fusion]

1. Dalla sezione [[!DNL Adobe Admin Console] pagina](https://adminconsole.adobe.com/), seleziona la **[!UICONTROL Prodotti]** nella barra di navigazione superiore, quindi selezionare la scheda **[!DNL Workfront Fusion]** riquadro del prodotto.

   ![Fusion in Admin Console](assets/fusion-product-admin-console.png)

1. Nell’elenco visualizzato, seleziona l’organizzazione in cui desideri aggiungere un utente.

   ![Istanza Fusion in Admin Console](assets/fusion-instances-admin-console.png)

1. Nell’elenco visualizzato, con il comando **[!UICONTROL Profili di prodotto]** , fare clic sul nome della scheda [!DNL Workfront Fusion] [!UICONTROL Profilo prodotto] collegamento.

   ![Profilo prodotto Workfront Fusion](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > Non apportare modifiche al [!UICONTROL Profilo prodotto] stesso.

1. Con il **[!UICONTROL Utenti]** selezionata sopra l’elenco, fai clic su **[!UICONTROL Aggiungi utente]**.

1. In **[!UICONTROL Aggiungi utenti a questo profilo di prodotto]** , immettere l&#39;indirizzo e-mail o il nome di un utente che si desidera aggiungere, quindi selezionare l&#39;utente nell&#39;elenco visualizzato.

1. Fai clic su **[!UICONTROL Salva]**.

   L’utente viene creato in [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Facoltativo) Continua con [Modificare il livello di accesso di un utente in [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Modificare il livello di accesso di un utente in Workfront Fusion

### Cambia il ruolo di un utente in Amministratore

L’assegnazione di un ruolo di amministratore a un utente deve essere eseguita nel [!DNL Adobe Admin Console].

1. Il giorno [!DNL Workfront Fusion] [!UICONTROL Profilo prodotto] pagina in cui è stato aggiunto l&#39;utente, selezionare la **[!UICONTROL Amministratori]** scheda.

1. Clic **[!UICONTROL Aggiungi amministratore]**.

1. In **[!UICONTROL Aggiungere amministratori del profilo di prodotto]** , immettere l&#39;indirizzo e-mail o il nome di un utente che si desidera aggiungere, quindi selezionare l&#39;utente nell&#39;elenco visualizzato.

1. Fai clic su **[!UICONTROL Salva]**.

   Questo utente è ora amministratore in [!DNL Workfront Fusion].

### Modificare il ruolo di un utente in [!UICONTROL Membro], [!UICONTROL Contabile], o [!UICONTROL Sviluppatore di app].

[!UICONTROL Membro], [!UICONTROL Contabile], e [!UICONTROL Sviluppatore di app] i ruoli vengono gestiti all&#39;interno di [!DNL Workfront Fusion].

Per istruzioni, consulta [Visualizzare o modificare i ruoli utente](../organizations/manage-fusion-users.md#view-or-edit-user-roles) nell’articolo [Gestisci [!DNL Adobe Workfront Fusion] utenti della tua organizzazione](../organizations/manage-fusion-users.md)

## Assegna un utente esistente in [!DNL Adobe Admin Console] a [!DNL Workfront Fusion]

1. Inizia a modificare l’utente come descritto nella sezione &quot;Modifica dettagli utente&quot; dell’articolo [Gestire gli utenti singolarmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) nel [!DNL Adobe Admin Console] documentazione.

1. Aggiungi **[!DNL Adobe Workfront Fusion]** ai prodotti assegnati all’utente.
