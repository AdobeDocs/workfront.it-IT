---
title: Aggiorna i metadati SAML 2.0 nel tuo IDP quando utilizzi l'autenticazione avanzata
description: In qualità di amministratore di Adobe Workfront, puoi integrare Workfront single sign-on (SSO) con qualsiasi provider di identità che supporti il protocollo SAML (Security Assertion Markup Language) 2.0.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: b6fc4775953e47a1b9d84d7537a6d9f5d35b1f2c
workflow-type: tm+mt
source-wordcount: '935'
ht-degree: 0%

---

# Aggiorna i metadati SAML 2.0 nel tuo IDP quando utilizzi l&#39;autenticazione avanzata

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

In qualità di amministratore di Adobe Workfront, puoi integrare Workfront single sign-on (SSO) con qualsiasi provider di identità che supporti il protocollo SAML (Security Assertion Markup Language) 2.0.

Le sezioni seguenti descrivono il processo di integrazione quando l’account Workfront è stato aggiornato all’esperienza di autenticazione avanzata (non ancora disponibile per tutte le organizzazioni). Per ulteriori informazioni sull’esperienza di autenticazione avanzata, consulta [Panoramica sull’autenticazione migliorata](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Per informazioni sulla configurazione di SAML prima della migrazione all’esperienza di autenticazione avanzata, consulta [Aggiornare i metadati SAML 2.0 nel provider di identità](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


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

## Utilizza Okta come provider di identità

Okta è un esempio di provider di identità che supporta SAML 2.0. Questa sezione descrive come utilizzare Okta come provider di identità. Passaggi simili sarebbero necessari per configurare un altro provider di identità che supporti SAML 2.0.

>[!NOTE]
>
>Gli utenti vengono mappati in base al loro indirizzo e-mail. Per accedere a Workfront utilizzando Okta, devi avere un utente con lo stesso indirizzo e-mail (senza distinzione tra maiuscole e minuscole) creato nel tuo cliente Workfront.

Completa le sezioni seguenti per configurare Okta come provider di identità in Workfront.

* [Creare un’app Workfront in Okta](#create-a-workfront-app-in-okta)
* [Aggiungi la tua istanza Okta come provider di identità in Workfront](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Creare un’app Workfront in Okta {#create-a-workfront-app-in-okta}

1. Accedi al tuo ambiente Okta.
1. Assicurati che **Interfaccia classica** nell&#39;angolo superiore sinistro dell&#39;interfaccia Okta.
1. Nel menu , fai clic su **Applicazioni** > **Applicazioni**.

1. Fai clic su **Aggiungi applicazione**, quindi fai clic su **Crea nuova app**.

1. In **Finestra di dialogo Crea nuova integrazione applicazione** casella, seleziona **SAML 2.0**, quindi fai clic su **Crea**.

1. Specifica un nome per l’app Workfront, quindi fai clic su **Successivo**.
1. Nella pagina Impostazioni SAML visualizzata, individuare le informazioni necessarie per la pagina Impostazioni SAML:

   1. Senza uscire dalla scheda del browser in cui viene visualizzata l&#39;interfaccia Okta, apri una scheda o una finestra del browser separata.
   1. Specifica il seguente URL nel browser:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. Nel file XML risultante, identificare i valori per **entityID** e **Posizione**.

      ![sso-okta.png](assets/sso-okta.png)

   1. Copia il valore dal **entityID** agli Appunti del sistema. Non chiudere questa scheda del browser.

1. Torna alla pagina Impostazioni SAML aperta nel passaggio 6.
1. Incolla il valore dal **entityID** nel campo **URI pubblico (ID entità SP)** campo .

1. Nel file XML nell’altra scheda del browser, copia il valore dal **Posizione** campo .
1. Incolla il valore dal **Posizione** nel campo **Single sign-on** **URL** campo .

1. Scorri fino a **Dichiarazioni degli attributi (facoltativo)** sezione .
1. In **Nome** campo , specifica **email**.

1. In **Valore** campo , specifica **user.email**.

1. (Facoltativo) Aggiungi eventuali valori avanzati.
1. Fai clic su **Successivo**.
1. Seleziona, **Sono un cliente Okta che aggiunge un’app interna**, quindi fai clic su **Fine**.

### Aggiungi la tua istanza Okta come provider di identità in Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Questa procedura fornisce informazioni essenziali per configurare Okta come provider di identità in Workfront. Per ulteriori informazioni su altre mappature o opzioni di configurazione, consulta [Configurare Adobe Workfront con SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Scarica i metadati del provider di identità per la tua istanza Okta:

   1. Accedi al tuo ambiente Okta.
   1. Assicurati che **Interfaccia classica** nell&#39;angolo superiore sinistro dell&#39;interfaccia Okta.
   1. Nel menu , fai clic su **Applicazioni** > **Applicazioni**.

   1. Fai clic sull’app Workfront creata, come descritto nella sezione , [Creare un’app Workfront in Okta](#create-a-workfront-app-in-okta)
   1. Sulla **Accedi** scheda , fai clic su **Metadati del provider di identità**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      I metadati vengono aperti come XML in una nuova scheda del browser.

   1. Copia l’URL visualizzato nel campo URL del browser.

1. Accedi a Workfront come amministratore Workfront.
1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Sistema** > **Single Sign-On (SSO)**.

1. (Condizionale) Se vengono visualizzate due schede, fai clic sul pulsante **Nuovi provider SSO** scheda .

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >Non eliminare le impostazioni di configurazione SSO esistenti nel **Provider SSO corrente** finché il tuo account non viene aggiornato all’esperienza di autenticazione avanzata e la nuova configurazione SSO non funziona completamente.

1. Fai clic su **Nuovo provider SSO**.
1. Specifica un nome, ad esempio Okta IDP, quindi specifica una descrizione.
1. In **Compilare campi da metadati del provider di identità** incolla l’URL copiato al passaggio 1 nel **URL metadati** campo .\
   In alternativa, puoi fare clic su **Scegli file** per caricare un file .xml, ma ti consigliamo di incollare l’URL.

1. In **Attributi utente mappa** nella sezione **Attributo directory** campo, tipo **email**. (**Indirizzo e-mail** è già popolato in **Attributo utente Workfront** campo .)

1. (Facoltativo) Abilita **Crea provider SSO predefinito** per inviare utenti non autenticati alla schermata di accesso del provider di identità anziché alla schermata di accesso di Workfront per l’autenticazione. È consigliabile abilitare questa opzione solo se tutti gli utenti del sistema accedono a Workfront tramite il provider di identità.
1. Seleziona la **Abilita** casella di controllo. Prima di eseguire questa operazione, assicurati che gli utenti del tuo sistema siano a conoscenza della nuova esperienza di accesso per assicurarti di non perdere l’accesso al sistema Workfront.
1. Fai clic su **Prova connessione**.\
   Dovresti visualizzare un messaggio che indica che la connessione è riuscita.

1. Fai clic su **Salva**.

## Utilizzo di altri provider di identità

Quando utilizzi provider di identità diversi da Okta (ad esempio Ping o Centrify), devi ricaricare i metadati Workfront nel provider di identità.
