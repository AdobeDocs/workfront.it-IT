---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Configurare le informazioni utente tramite [!DNL Workfront Proof]
description: Configurare le informazioni utente tramite [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Configurare le informazioni utente tramite [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità del prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Bozza](../../../review-and-approve-work/proofing/proofing.md).

1. Iniziare a creare o modificare un utente come descritto in [Crea utenti tramite [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Specifica le seguenti informazioni:

   * In **[!UICONTROL Dati personali]** sezione:

      * **Indirizzo e-mail:** Indirizzo e-mail dell’utente.
      * **Nome:** Nome dell’utente.
      * **Cognome** Cognome dell’utente.
      * **Posizione:** La posizione dell’utente nell’azienda.
      * **Profilo di autorizzazione:** Autorizzazioni dell’utente sull’account della bozza.
      * **Lingua:** La lingua principale dell’utente.
      * **Fuso orario:** Seleziona il fuso orario dell’utente.
      * **Formato data:** Seleziona il formato data preferito dall’utente.
      * **Consenso - E-mail relative a prodotti e marketing:** Seleziona se dare il consenso dell&#39;utente per le e-mail di prodotto e marketing.
      * **Solo API:** Consente all’utente di accedere solo tramite l’API.

   * In **[!UICONTROL Dettagli utente]** digitare le informazioni di contatto dell&#39;utente, ad esempio indirizzo e numero di telefono.
   * In **[!UICONTROL Impostazioni bozza predefinite]** , configura le impostazioni che influiscono sul modo in cui l’utente crea o lavora le bozze.

      * **Ruolo bozza predefinito:** Seleziona un ruolo di bozza predefinito per l’utente. Le opzioni del ruolo sono **[!UICONTROL Sola lettura]**, **[!UICONTROL Revisore]**, **[!UICONTROL Approvatore]**, **[!UICONTROL Revisore e Approvatore]**, **[!UICONTROL Autore]**, o **[!UICONTROL Moderatore]**.

        Per ulteriori informazioni sui ruoli delle bozze, consulta [Gestire i ruoli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Blocca la bozza quando vengono prese tutte le decisioni:** Blocca automaticamente la bozza da ulteriori modifiche dopo aver preso tutte le decisioni sulla bozza.
      * **Accesso richiesto. La bozza può essere condivisa solo con altri utenti:** Rende la bozza disponibile solo agli utenti con [!DNL Workfront Proof] credenziali di accesso.
      * **È necessaria una sola decisione:** Richiede una sola decisione su una bozza.
      * **Download del file originale:** Consente all’utente di scaricare il file originale per una bozza. Questa opzione è attivata per impostazione predefinita.

        Per ulteriori informazioni sul download dei file originali, vedere [Scarica i file memorizzati in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Iscrizione. Gli utenti possono iscriversi alla bozza tramite l’URL pubblico o il codice di incorporamento:** Consente ai revisori esterni all’organizzazione di registrarsi per la bozza tramite l’URL pubblico o il codice di incorporamento.

        Quando questa opzione è selezionata, **Per accedere a una bozza, l’utente deve fare clic su un collegamento in un’e-mail** è disponibile anche. Seleziona questa opzione per richiedere al revisore esterno di fare clic su un collegamento nell’e-mail per accedere alla bozza.
Questa opzione è attivata per impostazione predefinita se **Condivisione pubblica** è selezionata.

      * **Ruolo predefinito per i nuovi revisori ospiti:** Seleziona un ruolo di bozza predefinito per i revisori ospiti. Le opzioni sono le stesse di quelle **Ruolo bozza predefinito**, ad eccezione di Moderatore e Autore.

   * In **[!UICONTROL Impostazioni predefinite degli avvisi e-mail]** sezione:

      * **Avviso e-mail predefinito:** Seleziona la frequenza con cui l’utente riceve gli aggiornamenti e-mail. Seleziona **Tutte le attività, Risposte ai commenti, Decisioni, Decisione finale, Riepilogo orario, Riepilogo giornaliero,** o **Disabilitato**.

        Per ulteriori informazioni sulle opzioni predefinite per gli avvisi e-mail, consulta [Configurare le impostazioni delle notifiche e-mail in [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Avviso e-mail predefinito per i nuovi revisori ospiti:** Seleziona la frequenza con cui i revisori guest ricevono gli aggiornamenti e-mail. Le opzioni sono le stesse di **Avviso e-mail predefinito.**

      * **Invia una conferma e-mail quando le bozze sono pronte:** Seleziona questa opzione per inviare automaticamente un’e-mail di conferma all’utente quando le bozze sono pronte.
      * **Formato delle e-mail inviate all&#39;utente:** Seleziona **[!UICONTROL HTML]** o **[!UICONTROL Testo normale]** come formato predefinito per le e-mail inviate all’utente.

   * In **[!UICONTROL Impostazioni messaggi personalizzate]** sezione: Creare le impostazioni per i modelli di bozza.

     Per ulteriori informazioni sui modelli, consulta:

      * **Modello oggetto bozza:** Crea un modello per un oggetto bozza.
      * **Modello di messaggio bozza:** Crea un modello per un messaggio bozza e il relativo formato.
