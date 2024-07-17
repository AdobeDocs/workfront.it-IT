---
title: Aggiornamento dei metadati SAML 2.0 nell’IDP quando si utilizza l’autenticazione avanzata
description: In qualità di amministratore di Adobe Workfront, puoi integrare Workfront Single Sign-On (SSO) con qualsiasi provider di identità che supporti il protocollo SAML (Security Assertion Markup Language) 2.0.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# Aggiornamento dei metadati SAML 2.0 nell’IDP quando si utilizza l’autenticazione avanzata

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

In qualità di amministratore di Adobe Workfront, puoi integrare Workfront Single Sign-On (SSO) con qualsiasi provider di identità che supporti il protocollo SAML (Security Assertion Markup Language) 2.0.

Le sezioni seguenti descrivono il processo di integrazione quando l’account Workfront è stato aggiornato all’esperienza di autenticazione avanzata (non ancora disponibile per tutte le organizzazioni). Per ulteriori informazioni sull&#39;autenticazione avanzata, vedere [Panoramica sull&#39;autenticazione avanzata](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Per informazioni sulla configurazione di SAML prima della migrazione all&#39;esperienza di autenticazione avanzata, vedere [Aggiornare i metadati SAML 2.0 nel provider di identità](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


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

## Utilizza Okta come provider di identità

Okta è un esempio di provider di identità che supporta SAML 2.0. Questa sezione descrive come utilizzare Okta come provider di identità. Passaggi simili sono necessari quando si configura un altro provider di identità che supporta SAML 2.0.

>[!NOTE]
>
>Gli utenti vengono mappati in base al loro indirizzo e-mail. Per accedere a Workfront utilizzando Okta, devi avere un utente con lo stesso indirizzo e-mail (senza distinzione tra maiuscole e minuscole) creato nel cliente Workfront.

Completa le sezioni seguenti per configurare Okta come provider di identità in Workfront.

* [Crea un&#39;app Workfront in Okta](#create-a-workfront-app-in-okta)
* [Aggiungere l’istanza Okta come provider di identità in Workfront](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Creare un’app Workfront in Okta {#create-a-workfront-app-in-okta}

1. Accedi all’ambiente Okta.
1. Verificare che **Interfaccia classica** sia selezionata nell&#39;angolo superiore sinistro dell&#39;interfaccia Okta.
1. Nel menu, fai clic su **Applicazioni** > **Applicazioni**.

1. Fai clic su **Aggiungi applicazione**, quindi su **Crea nuova app**.

1. Nella casella **Crea nuova integrazione applicazione**, selezionare **SAML 2.0**, quindi fare clic su **Crea**.

1. Specifica un nome per l&#39;app Workfront, quindi fai clic su **Avanti**.
1. Nella pagina Impostazioni SAML visualizzata, individuare le informazioni necessarie per la pagina Impostazioni SAML:

   1. Senza uscire dalla scheda del browser in cui è visualizzata l’interfaccia Okta, apri una scheda o una finestra del browser separata.
   1. Specifica il seguente URL nel browser:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. Nel file XML risultante, identificare i valori per **entityID** e **Location**.

      ![sso-okta.png](assets/sso-okta.png)

   1. Copia il valore dal campo **entityID** negli Appunti di sistema. Non chiudere questa scheda del browser.

1. Torna alla pagina Impostazioni SAML aperta al passaggio 6.
1. Incolla il valore dal campo **entityID** nel campo **Audience URI (ID entità SP)**.

1. Nel file XML nell&#39;altra scheda del browser, copia il valore dal campo **Posizione**.
1. Incolla il valore dal campo **Posizione** nel campo **Single Sign-on** **URL**.

1. Scorri fino alla sezione **Istruzioni attributo (facoltativo)**.
1. Nel campo **Name**, specifica **email**.

1. Nel campo **Valore**, specifica **user.email**.

1. (Facoltativo) Aggiungi eventuali valori avanzati.
1. Fai clic su **Avanti**.
1. Seleziona, **Sono un cliente Okta che aggiunge un&#39;app interna**, quindi fai clic su **Fine**.

### Aggiungere l’istanza Okta come provider di identità in Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Questa procedura fornisce informazioni essenziali per configurare Okta come provider di identità in Workfront. Per ulteriori informazioni su altre mappature o opzioni di configurazione, vedere [Configurare Adobe Workfront con SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Scarica i metadati del provider di identità per l’istanza Okta:

   1. Accedi all’ambiente Okta.
   1. Verificare che **Interfaccia classica** sia selezionata nell&#39;angolo superiore sinistro dell&#39;interfaccia Okta.
   1. Nel menu, fai clic su **Applicazioni** > **Applicazioni**.

   1. Fai clic sull&#39;app Workfront creata, come descritto nella sezione [Creare un&#39;app Workfront in Okta](#create-a-workfront-app-in-okta)
   1. Nella scheda **Accedi**, fai clic su **Metadati provider di identità**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      I metadati vengono aperti come XML in una nuova scheda del browser.

   1. Copia l’URL visualizzato nel campo URL del browser.

1. Accedi a Workfront come amministratore Workfront.
1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fare clic su **Sistema** > **Single Sign-On (SSO)**.

1. (Condizionale) Se sono presenti due schede, fare clic sulla scheda **Nuovi provider SSO**.

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >Non eliminare le impostazioni di configurazione SSO esistenti nella scheda **Provider SSO corrente** finché l&#39;account non viene aggiornato all&#39;esperienza di autenticazione avanzata e la nuova configurazione SSO non è completamente funzionante.

1. Fare clic su **Nuovo provider SSO**.
1. Specifica un nome, ad esempio Okta IDP, quindi specifica una descrizione.
1. Nella sezione **Popolare i campi dai metadati del provider di identità**, incolla l&#39;URL copiato nel passaggio 1 nel campo **URL metadati**.\
   In alternativa, è possibile fare clic su **Scegli file** per caricare un file con estensione xml, ma si consiglia di incollare l&#39;URL.

1. Nella sezione **Mappa attributi utente**, nel campo **Attributo directory**, digitare **e-mail**. (**Indirizzo e-mail** è già popolato nel campo **Attributo utente Workfront**.)

1. (Facoltativo) Abilitare **Rendi provider SSO predefinito** per inviare utenti non autenticati alla schermata di accesso del provider di identità anziché alla schermata di accesso di Workfront per l&#39;autenticazione. È consigliabile abilitare questa opzione solo se tutti gli utenti del sistema accedono a Workfront tramite il provider di identità.
1. Selezionare la casella di controllo **Abilita**. Prima di procedere, accertati che gli utenti del tuo sistema siano a conoscenza della nuova esperienza di accesso per evitare di perdere l’accesso al sistema Workfront.
1. Fare clic su **Verifica connessione**.\
   Dovresti visualizzare un messaggio che ti informa che la connessione è riuscita.

1. Fai clic su **Salva**.

## Utilizzo di altri provider di identità

Quando utilizzi provider di identità diversi da Okta (ad esempio Ping o Centrify), devi ricaricare i metadati di Workfront nel provider di identità.
