---
product-previous: workfront-proof
product-area: documents;system-administration;setup
navigation-topic: satellite-accounts
title: Configurare un account satellite in [!DNL Workfront Proof]
description: Gli account satellitari sono account a pagamento che puoi configurare e gestire dall'interno del tuo [!DNL Workfront] account di verifica. Per ulteriori informazioni, vedere "Account satellite in [!DNL Workfront] Proof.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 82c6dff3-6187-4145-951c-3f5312049b59
source-git-commit: 5be053a6ee99404673f6f3258a423ef5e5c7f431
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 0%

---

# Configurare un account satellite in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Gli account satellite sono account a pagamento configurati e gestiti dall&#39;account [!DNL Workfront Proof]. Per ulteriori informazioni, vedere [Account satellite in [!DNL Workfront] Bozza](../../../workfront-proof/wp-acct-admin/satellite-accounts/sat-accts-in-wp.md).

Qualsiasi amministratore di fatturazione può creare un account satellite. Per informazioni sugli amministratori di fatturazione, vedere [[!UICONTROL Profili autorizzazioni bozza] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
> Gli account satellite devono essere impostati su uno dei [!UICONTROL Standard] o piani superiori.

## Creazione di un account Satellite {#creating-a-satellite-account}

Per creare un account Satellite:

1. Vai alla pagina [!UICONTROL Fatturazione].\
   Per ulteriori informazioni sulla pagina di fatturazione, vedere [La [!DNL Workfront Proof] [!UICONTROL Fatturazione] pagina](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

1. Fare clic sul pulsante **[!UICONTROL Nuovo account Satellite]**. 1)

   Viene visualizzata una finestra popup.

   ![Nuovo_account_satellite.png](assets/new-satellite-account-350x156.png)

1. Immetti i dettagli del cliente, compresi eventuali codici promozionali pertinenti.
1. Fai clic su **[!UICONTROL Salva]**. L&#39;account Satellite viene visualizzato automaticamente nel menu a discesa [!UICONTROL Account] nella parte superiore della pagina [!UICONTROL Fatturazione].
1. Seleziona il nuovo account Satellite dal menu a discesa.
1. Continua con [Selezionare un piano per il tuo account Satellite](#selecting-a-plan-for-your-satellite-account) per aggiornare il tuo account Satellite.

## Selezione di un piano per il tuo account Satellite {#selecting-a-plan-for-your-satellite-account}

Dopo aver configurato l&#39;account Satellite come descritto in [Creazione di un account Satellite](#creating-a-satellite-account), è necessario aggiornarlo al piano desiderato.

1. Vai alla pagina [!UICONTROL Fatturazione].\
   Per ulteriori informazioni sulla pagina di fatturazione, vedere [La [!DNL Workfront Proof] [!UICONTROL Fatturazione] pagina](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

1. Nel menu a discesa **[!UICONTROL I tuoi account]**, nella parte superiore della pagina (1), scegli l&#39;account Satellite pertinente.

   Viene visualizzata la pagina di fatturazione per l&#39;account Satellite e vengono automaticamente replicati i dati di contatto di fatturazione del tuo account.

   ![Cambia_piano_account_satellite](assets/satellite-account-change-plan-350x156.png)

1. Fare clic sul pulsante **[!UICONTROL Cambia piano]** in alto a destra della pagina. 2)\
   Oppure\
   Aprire il popup facendo clic sul nome del piano corrente o successivo. 3)

1. Aggiorna o esegui il downgrade del piano.

## Aggiunta di utenti all&#39;account Satellite

Dopo aver aggiornato l&#39;account Satellite al piano scelto, è necessario aggiungere gli utenti all&#39;account.

1. Accedere a [!DNL Workfront Proof] come amministratore [!DNL Workfront Proof].
1. Fare clic su **[!UICONTROL Impostazioni account]**.
1. Nel menu a discesa nella parte superiore della pagina, seleziona l’account Satellite pertinente. 1)\
   Viene visualizzata la pagina delle impostazioni dell&#39;account Satellite.
1. Fai clic sul pulsante **[!UICONTROL Nuovo utente]** in alto a destra della pagina. 2)\
   Viene visualizzata la pagina [!DNL New User].

1. Immetti i dettagli dell&#39;utente, quindi fai clic su **[!UICONTROL Salva]**.\
   L’utente riceve una notifica e-mail che gli consente di accedere all’account.

Gli utenti aggiunti all&#39;account Satellite vengono visualizzati come membri nell&#39;elenco dei contatti dell&#39;account hub.

Analogamente, gli utenti nell&#39;account hub vengono visualizzati come membri nei contatti dell&#39;account satellite.

Per visualizzare un elenco completo di tutti gli utenti dell&#39;account Satellite, fare clic sulla scheda **[!UICONTROL Utenti]**.

![SA_New_User.png](assets/sa-new-user-350x156.png)

## Collegamento di account separati esistenti all&#39;account hub

Se in precedenza sono stati creati altri account distinti per i clienti, questi possono essere convertiti in account satellite.

Ci occuperemo di questo problema collegandoli al tuo account [!DNL Workfront Proof] (rendendolo un account hub).

Tutto ciò che devi fare è fornirci i seguenti dettagli:

* Il nome dell&#39;account [!DNL Workfront Proof] e l&#39;indirizzo di posta elettronica utilizzato per configurarlo
* I nomi degli account separati che desideri collegare al tuo account e gli indirizzi e-mail utilizzati per impostare gli account separati.
