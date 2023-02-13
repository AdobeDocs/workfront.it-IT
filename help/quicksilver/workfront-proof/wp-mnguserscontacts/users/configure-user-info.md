---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Configurare le informazioni utente tramite [!DNL Workfront Proof]
description: Configurare le informazioni utente tramite [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Configurare le informazioni utente tramite [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

1. Inizia a creare o modificare un utente come descritto in [Crea utenti utilizzando [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Specifica le seguenti informazioni:

   * In **[!UICONTROL Dati personali]** sezione:

      * **Indirizzo e-mail:** L’indirizzo e-mail dell’utente.
      * **Nome:** Nome dell&#39;utente.
      * **Cognome:** Cognome dell&#39;utente.
      * **Posizione:** Posizione dell&#39;utente nell&#39;azienda.
      * **Profilo di autorizzazione:** Le autorizzazioni dell&#39;utente per l&#39;account della bozza.
      * **Lingua:** Lingua principale dell&#39;utente.
      * **Fuso orario:** Seleziona il fuso orario dell’utente.
      * **Formato data:** Seleziona il formato di data preferito dall’utente.
      * **Opt in - E-mail di prodotto e marketing:** Seleziona se l’utente deve effettuare l’accesso per e-mail di prodotto e marketing.
      * **Solo API:** Consente all’utente di accedere solo tramite l’API.
   * In **[!UICONTROL Dettagli utente]** digitare le informazioni di contatto dell&#39;utente, ad esempio l&#39;indirizzo e il numero di telefono.
   * In **[!UICONTROL Impostazioni predefinite della bozza]** configura le impostazioni che influiscono sul modo in cui l’utente crea o lavora sulle bozze.

      * **Ruolo di bozza predefinito:** Selezionare un ruolo di bozza predefinito per l&#39;utente. Le opzioni del ruolo sono **[!UICONTROL Sola lettura]**, **[!UICONTROL Revisore]**, **[!UICONTROL Approvatore]**, **[!UICONTROL Revisore e approvatore]**, **[!UICONTROL Autore]** oppure **[!UICONTROL Moderatore]**.

         Per ulteriori informazioni sui ruoli di bozza, consulta [Gestisci ruoli di bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Blocca la bozza quando vengono prese tutte le decisioni:** Blocca automaticamente la bozza da ulteriori modifiche dopo tutte le decisioni sulla bozza.
      * **Accesso richiesto. La bozza può essere condivisa solo con altri utenti:** Rende la bozza disponibile solo agli utenti con [!DNL Workfront Proof] credenziali di accesso.
      * **È necessaria una sola decisione:** Richiede una sola decisione su una prova.
      * **Download del file originale:** Consente all&#39;utente di scaricare il file originale per una bozza. Questa opzione è attivata per impostazione predefinita.

         Per ulteriori informazioni sul download dei file originali, vedi [Scarica i file memorizzati in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

         <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Iscrizione. Le persone possono registrarsi per la bozza tramite l’URL pubblico o il codice di incorporamento:** Consente ai revisori esterni all’organizzazione di registrarsi per la bozza tramite l’URL pubblico o il codice di incorporamento.

         Quando questa opzione è selezionata, **L’utente iscritto deve fare clic su un collegamento in un messaggio e-mail per accedere a una bozza** è disponibile anche. Seleziona questa opzione per richiedere al revisore esterno di fare clic su un collegamento all’interno dell’e-mail per accedere alla bozza.
Questa opzione è attivata per impostazione predefinita se **Condivisione pubblica** è selezionata.

      * **Ruolo predefinito per i nuovi revisori ospiti:** Seleziona un ruolo di bozza predefinito per i revisori ospiti. Le opzioni sono le stesse di quelle in **Ruolo di bozza predefinito.**
   * In **[!UICONTROL Impostazioni predefinite avvisi e-mail]** sezione:

      * **Avviso e-mail predefinito:** Seleziona la frequenza con cui l’utente riceve gli aggiornamenti e-mail. Seleziona **Tutte le attività, Risposte ai miei commenti, Decisioni, Decisione finale, Riepilogo orario, Riepilogo giornaliero,** o **Disabilitato**.

         Per ulteriori informazioni sulle opzioni di avviso e-mail predefinite, consulta [Configura le impostazioni di notifica e-mail in [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Avviso e-mail predefinito per i nuovi revisori ospiti:** Seleziona la frequenza con cui i revisori ricevono gli aggiornamenti e-mail. Le opzioni sono le stesse di quelle per **Avviso e-mail predefinito.**

      * **Invia una conferma e-mail quando le bozze sono pronte:** Seleziona questa opzione per inviare automaticamente all’utente un messaggio e-mail di conferma quando le bozze sono pronte.
      * **Formato delle e-mail inviate a questo utente:** Seleziona **[!UICONTROL HTML]** o **[!UICONTROL Testo normale]** come formato predefinito per le e-mail inviate all’utente.
   * In **[!UICONTROL Impostazioni dei messaggi personalizzate]** sezione: Crea le impostazioni per i modelli di bozza.

      Per ulteriori informazioni sui modelli, consulta:

      * **Modello del soggetto di prova:** Crea un modello per un soggetto della bozza.
      * **Modello di messaggio di bozza:** Crea un modello per un messaggio di bozza e il relativo formato.
