---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Configurare il Single Sign-On per [!DNL Workfront Proof] utenti
description: Se si dispone del piano Select o Premium, è possibile fornire la funzionalità Single Sign-On (SSO) che consente di utilizzare il nome utente e la password dell'organizzazione esistente per accedere al [!DNL Workfront Proof] account.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: 007a603ef1df2a02959d7fb623ac784bf5b9cb80
workflow-type: tm+mt
source-wordcount: '1264'
ht-degree: 0%

---

# Configurare il Single Sign-On per [!DNL Workfront Proof] utenti

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità del prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Bozza](../../../review-and-approve-work/proofing/proofing.md).

Se si dispone del piano Select o Premium, è possibile fornire la funzionalità Single Sign-On (SSO) che consente di utilizzare il nome utente e la password dell&#39;organizzazione esistente per accedere al [!DNL Workfront Proof] account.

Ciò significa che eseguirai l’autenticazione sul tuo sistema di accesso, non su [!DNL Workfront Proof] pagina di accesso.

>[!NOTE]
>
>Devi avere un sottodominio o un dominio personalizzato impostato sul tuo [!DNL Workfront Proof] per abilitare SAML. I sottodomini personalizzati sono liberi di impostare. Consulta [Marchio](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) per ulteriori informazioni.Per ulteriori informazioni sui domini completamente personalizzati, consulta [Marchio [!DNL Workfront Proof] site - advanced](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

## Abilitazione di SSO in [!DNL Workfront Proof]

La funzionalità Single Sign-On può essere attivata sul [!UICONTROL Single sign-on] scheda del [!UICONTROL Impostazioni account], e si applicherà a tutti gli utenti sul tuo [!DNL Workfront Proof] account. Consulta [Impostazioni account](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) per ulteriori informazioni.

## ID entità

In qualità di fornitore di servizi, abbiamo pubblicato il nostro ID entità qui:

[https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq) (dove &quot;yoursubdomain&quot; è il sottodominio del tuo account)

[!DNL Workfront Proof] richiede l’indirizzo e-mail dell’utente come identificatore univoco, che può essere trasmesso come uno dei seguenti attributi:

* urn:mace:dir:attribute-def:emailAddress
* http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress
* http://schemas.xmlsoap.org/claims/EmailAddress
* urn:oid:0.9.2342.19200300.100.1.3.
* http://axschema.org/contact/email
* openid.sreg.email
* mail
* email
* emailAddress

Per configurare l&#39;SSO:

1. Apri **[!UICONTROL Single Sign-On]** (1).
1. Inserisci il **URL SSO** (2).
Collegamento al server SSO (ad esempio, **https://sso.mycompany.com/opensso**).

1. Inserisci il **URL di accesso** 3).
Questo è l’URL che verrà richiamato per reindirizzare gli utenti al provider di identità.

1. Non si tratta di un URL effettivo immesso nel browser, ma di un endpoint che elaborerà le informazioni inviate per presentare la schermata di accesso.

Inserisci il **URL disconnessione** 4).
Questo è l&#39;URL a cui verrai restituito dopo la disconnessione, ad esempio

**https://www.yourcompany.com/services/logout.asp**

1. Inserisci il **Impronta digitale del certificato** (5).
1. L&#39;impronta digitale SHA1 del certificato SAML fornito dal provider di identità SAML.
1. Assicurati di includere le informazioni chiave impostandole sul provider di identità.
1. Switch **SSO** a **[!UICONTROL Abilitato]** 6).
Una volta abilitato l’accesso SSO, tu e altri utenti del tuo account effettuerete l’accesso utilizzando il vostro meccanismo di autenticazione. Ciò significa che quando gli utenti accedono al tuo [!DNL Workfront Proof] schermata di accesso dell’account (ad esempio, **yourcompany.proofhq.com/login**), verrà visualizzata la finestra di trasferimento nella pagina di accesso di autenticazione.

1. (Facoltativo) Abilita **Assegna automaticamente ruoli agli utenti** 7).
Una volta abilitata questa opzione, gli account utente verranno creati automaticamente per le persone che non hanno il proprio [!DNL Workfront Proof] , ma accederà al tuo [!DNL Workfront Proof] utilizzando le credenziali Single Sign-On. Questa azione viene eseguita solo quando il limite utente non è ancora stato raggiunto sul tuo account.

1. Ai nuovi utenti con provisioning vengono assegnate per impostazione predefinita le autorizzazioni del profilo Manager. Per ulteriori informazioni, consulta [Profili delle autorizzazioni di bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

![Enable_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## Abilitazione di SSO per gli account satellite

Quando disponi di account satellite connessi al tuo account hub, puoi amministrarli dal livello dell’account hub.

Single Sign-On è una funzionalità Select e Premium, pertanto è possibile abilitare il Single Sign-On solo sui satelliti inclusi nei piani Select e Premium.

1. Clic **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]** (1)

1. Fai clic sull’account satellite nel menu a discesa (2).
1. Apri **[!UICONTROL Single Sign-On]** (3).
1. Inizia a modificare la configurazione SSO (4).
1. ![Enabling_SSO_Satellite_Account.png](assets/enabling-sso---satellite-account-350x266.png)
Qui sono disponibili due metodi (5) di configurazione:

1. **Ereditato:** SSO con la configurazione ripresa dall&#39;account hub.
Se un utente accede a [!DNL Workfront Proof] tramite **pagina di accesso predefinita** ([https://www.proofhq.com/login](https://www.proofhq.com/login)) ci sarà **due livelli di autorizzazione**: per prima cosa viene richiesto a un utente di accedere utilizzando [!DNL Workfront Proof] accedere ai dati (e-mail e password); l&#39;utente viene quindi trasferito attraverso una finestra SSO alla pagina di accesso SSO.
Pertanto, con il servizio SSO abilitato, si consiglia di accedere tramite il proprio [!DNL Workfront Proof] sottodominio/dominio.

   >[!NOTE]
   >
   >In questo momento, quando Single Sign-On è abilitato sul [!DNL Workfront Proof] account, non potrai accedere all’app iPhone con tali credenziali.

   1. **Manuale** (impostazione predefinita): SSO con una configurazione diversa, ad esempio che punta a un altro provider di identità.

      >[!NOTE]
      >
      >Se l&#39;account satellite eredita la configurazione SSO dall&#39;account hub, la schermata di accesso sarà quella dell&#39;account hub. Quando l’utente dell’account satellite immette i propri dettagli di accesso SSO in questa pagina, verrà reindirizzato all’account satellite.

      ![Enabling_SSO_Satellite_Account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. Clic **[!UICONTROL Salva]** 6).

## Impostazioni SSO ereditate da un account hub

Quando scegli di ereditare le impostazioni dall&#39;account hub, tutti i campi vengono ora compilati con i dati dell&#39;account hub (7) e il Single Sign-On viene automaticamente abilitato/disabilitato(8) come nell&#39;account principale. Inoltre non ci sono più collegamenti di modifica nei campi, in quanto l&#39;intera configurazione SSO per l&#39;account Satellite è ora impostata e gestita dall&#39;account hub.

![Satellite_Account_Inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

Nel tuo account hub (9) il [!UICONTROL Utilizzo SSO] mostra che questa configurazione è utilizzata dagli account satellite (10).\
![Hub_Account_Inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## SSO configurato manualmente

Se è stata scelta la configurazione SSO manuale per un account satellite (1), è necessario immettere manualmente i dati per il Single Sign-On.

1. Clic **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]** (1)

1. Apri **[!UICONTROL Single sign-on]** scheda.
1. Clic **[!UICONTROL Modifica],** compila il campo e fai clic su **[!UICONTROL Salva]** (2).

1. Il giorno **[!UICONTROL SSO]** riga, fai clic su **[!UICONTROL Abilitato]** 3).

![Satellite_Account_Manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## Accesso SSO

1. Clic **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]** (1)

1. Apri **[!UICONTROL Single sign-on]** scheda.
1. Assicurati che il tuo [!DNL Workfront Proof] dominio/sottodominio (1) e che gli utenti accedano al tuo [!DNL Workfront Proof] tramite questo dominio/sottodominio personalizzato.
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
Con il Single Sign-On abilitato, l&#39;URL di accesso del sottodominio (ad esempio, yourcompany.proofhq.com/login) visualizza una schermata di trasferimento (2) che porta direttamente alla pagina di accesso SSO.
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. Se un utente accede a [!DNL Workfront Proof] tramite **pagina di accesso predefinita** ([https://www.proofhq.com/login](https://www.proofhq.com/login)) ci sarà **due livelli di autorizzazione**. Innanzitutto, viene richiesto a un utente di effettuare l’accesso tramite [!DNL Workfront Proof] accedere ai dati (e-mail e password). L&#39;utente viene quindi trasferito tramite una finestra SSO (2) alla pagina di accesso SSO.\
   Pertanto, con il servizio SSO abilitato, si consiglia di accedere tramite il proprio [!DNL Workfront Proof] sottodominio/dominio.

1. Al momento, se l’accesso Single Sign-On è abilitato sul tuo account Workfront Proof, non potrai accedere all’app iPhone con tali credenziali.

## Informazioni sull&#39;aggiunta di un nuovo utente

Quando la funzionalità Single Sign-On è attivata sul [!DNL Workfront Proof] account, i nuovi utenti non riceveranno alcuna e-mail di conferma in quanto i loro account verranno attivati automaticamente e pronti per l’uso.

Dal tuo [!DNL Workfront Proof] pagina di accesso, dopo aver fatto clic su [!UICONTROL Login] , gli utenti vengono reindirizzati alla pagina di accesso SSO e viene richiesto di immettere le credenziali di accesso Single Sign-On.

>[!IMPORTANT]
>
>Gli utenti vengono identificati tramite un indirizzo e-mail durante il processo di autenticazione, il che significa che l’account e-mail utilizzato per l’accesso SSO deve essere l’indirizzo e-mail dell’utente registrato nel tuo account.

## Active Directory Federation Services (ADFS)

Active Directory Federation Services (ADFS) è un [!DNL Microsoft] componente software che può essere installato su sistemi operativi Windows Server per consentire agli utenti l&#39;accesso Single Sign-On a sistemi e applicazioni che si trovano oltre i confini dell&#39;organizzazione. Per ulteriori informazioni, vedere &quot;Active Directory Federation Services&quot; nel sito Web Microsoft Developer Network.

Il [!DNL Workfront Proof] Il sistema supporta SAML 2.0 ed è compatibile solo con ADFS versione 2.0 o successiva.

Consulta [Accesso Single Sign-On [!DNL Workfront Proof]: configurazione ADFS](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md) per istruzioni dettagliate.
