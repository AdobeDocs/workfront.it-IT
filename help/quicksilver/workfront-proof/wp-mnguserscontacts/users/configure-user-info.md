---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Configura informazioni utente tramite  [!DNL Workfront Proof]
description: Configura informazioni utente tramite  [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Configura informazioni utente tramite [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

1. Inizia a creare o modificare un utente come descritto in [Crea utenti utilizzando [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Specifica le seguenti informazioni:

   * Nella sezione **[!UICONTROL Dati personali]**:

      * **Indirizzo e-mail:** indirizzo e-mail dell&#39;utente.
      * **Nome:** Nome dell&#39;utente.
      * **Cognome:** Cognome dell&#39;utente.
      * **Posizione:** la posizione dell&#39;utente nell&#39;azienda.
      * **Profilo di autorizzazione:** le autorizzazioni dell&#39;utente sull&#39;account di bozza.
      * **Lingua:** lingua principale dell&#39;utente.
      * **Fuso orario:** Selezionare il fuso orario dell&#39;utente.
      * **Formato data:** Selezionare il formato data preferito dall&#39;utente.
      * **Consenso - E-mail prodotto e marketing:** Seleziona se dare il consenso dell&#39;utente per le e-mail prodotto e marketing.
      * **Solo API:** consente all&#39;utente di accedere solo tramite l&#39;API.

   * Nella sezione **[!UICONTROL Dettagli utente]** digitare le informazioni di contatto dell&#39;utente, ad esempio indirizzo e numero di telefono.
   * Nella sezione **[!UICONTROL Impostazioni bozza predefinite]** configura le impostazioni che influiscono sul modo in cui l&#39;utente crea o lavora le bozze.

      * **Ruolo bozza predefinito:** Selezionare un ruolo bozza predefinito per l&#39;utente. Le opzioni del ruolo sono **[!UICONTROL Sola lettura]**, **[!UICONTROL Revisore]**, **[!UICONTROL Approvatore]**, **[!UICONTROL Revisore e Approvatore]**, **[!UICONTROL Autore]** o **[!UICONTROL Moderatore]**.

        Per ulteriori informazioni sui ruoli bozza, vedere [Gestione dei ruoli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Blocca la bozza quando vengono prese tutte le decisioni:** blocca automaticamente la bozza da ulteriori modifiche dopo che tutte le decisioni sulla bozza sono state prese.
      * **Accesso richiesto. La bozza può essere condivisa solo con altri utenti:** Rende la bozza disponibile solo agli utenti con credenziali di accesso [!DNL Workfront Proof].
      * **È richiesta una sola decisione:** è necessaria una sola decisione per una bozza.
      * **Download del file originale:** Consente all&#39;utente di scaricare il file originale per una bozza. Questa opzione è attivata per impostazione predefinita.

        Per ulteriori informazioni sul download dei file originali, vedere [Scarica file archiviati in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Iscrizione. Gli utenti possono iscriversi alla bozza tramite l&#39;URL pubblico o il codice di incorporamento:** Consente ai revisori esterni all&#39;organizzazione di iscriversi alla bozza tramite l&#39;URL pubblico o il codice di incorporamento.

        Quando questa opzione è selezionata, **Il Sottoscrittore deve fare clic su un collegamento in un&#39;e-mail per accedere a una bozza**. Seleziona questa opzione per richiedere al revisore esterno di fare clic su un collegamento nell’e-mail per accedere alla bozza.
Questa opzione è attivata per impostazione predefinita se è selezionata l&#39;opzione **Condivisione pubblica**.

      * **Ruolo predefinito per i nuovi revisori ospiti:** Seleziona un ruolo di bozza predefinito per i revisori ospiti. Le opzioni sono le stesse del **Ruolo bozza predefinito**, ad eccezione di Moderatore e Autore.

   * Nella sezione **[!UICONTROL Impostazioni predefinite avvisi e-mail]**:

      * **Avviso e-mail predefinito:** Seleziona la frequenza con cui l&#39;utente riceve gli aggiornamenti e-mail. Seleziona **Tutte le attività, Risposte ai commenti, Decisioni, Decisione finale, Riepilogo orario, Riepilogo giornaliero,** o **Disabilitato**.

        Per ulteriori informazioni sulle opzioni predefinite per gli avvisi e-mail, vedere [Configurare le impostazioni per le notifiche e-mail in [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Avviso e-mail predefinito per i nuovi revisori ospiti:** Seleziona la frequenza con cui i revisori ospiti ricevono gli aggiornamenti e-mail. Le opzioni sono le stesse di quelle per **Avviso e-mail predefinito.**

      * **Invia una conferma e-mail quando le bozze sono pronte:** Seleziona questa opzione per inviare automaticamente un&#39;e-mail di conferma all&#39;utente quando le bozze sono pronte.
      * **Formato delle e-mail inviate all&#39;utente:** Selezionare **[!UICONTROL HTML]** o **[!UICONTROL Testo normale]** come formato predefinito per le e-mail inviate all&#39;utente.

   * Nella sezione **[!UICONTROL Impostazioni messaggi personalizzati]**: Crea le impostazioni per i modelli di bozza.

     Per ulteriori informazioni sui modelli, consulta:

      * **Modello oggetto bozza:** Creare un modello per un oggetto bozza.
      * **Modello di messaggio bozza:** Creare un modello per un messaggio bozza e il relativo formato.
