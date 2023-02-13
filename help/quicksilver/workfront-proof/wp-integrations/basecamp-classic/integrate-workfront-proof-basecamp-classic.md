---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Integrare [!DNL Workfront Proof] con Basecamp Classic
description: Se utilizzi [!DNL Basecamp] per la gestione dei progetti puoi offrire al team di progetto strumenti di revisione e approvazione più avanzati utilizzando [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Integrare [!DNL Workfront Proof] con [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Se utilizzi [!DNL Basecamp] per la gestione dei progetti puoi offrire al team di progetto strumenti di revisione e approvazione più avanzati utilizzando [!DNL Workfront Proof].

## Informazioni sulla [!DNL Basecamp] Integrazione con [!DNL Workfront]

Integrazione con [!DNL Basecamp] consente agli utenti di visualizzare, rivedere e approvare le bozze all’interno di [!DNL Basecamp]. Gli utenti possono inviare le bozze al tuo [!DNL Workfront Proof] e collegali al tuo [!DNL Basecamp] progetto. I revisori possono e possono [Prendere una decisione su una bozza nel visualizzatore di correzione](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) tramite [!DNL Basecamp], utilizzando la prova mini incorporata nel messaggio Basecamp.

Quando integrato con [!DNL Workfront Proof], [!DNL Basecamp] consente agli utenti di effettuare le seguenti operazioni con le bozze:

* Gli utenti possono rivedere e approvare le bozze in [!DNL Basecamp Classic].
* Gli utenti dispongono di strumenti di revisione immediatamente disponibili.
* I team di revisione dei progetti ricevono un messaggio in [!DNL Basecamp] con una mini prova per la revisione e l&#39;approvazione.
* Gli utenti possono passare a una bozza a pagina intera per la revisione e l’approvazione.
* Gli utenti possono aggiungere commenti e annotazioni sia alle bozze mini che a quelle complete.

   >[!NOTE]
   >
   >Una volta risposto a un commento, non è possibile modificarlo o eliminarlo.

* I revisori possono rispondere alle marcature e effettuate da altri revisori.
* Gli utenti vengono avvisati quando è disponibile una nuova versione della bozza.
* Utenti che non sono [!DNL Workfront Proof] gli utenti possono lavorare su una bozza in [!DNL Basecamp].

L&#39;integrazione di [!DNL Workfront Proof] con [!DNL Basecamp] deve essere impostato su due livelli:

* Configura [!DNL Basecamp] in [Impostazioni account:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Questo consente l’integrazione di Basecamp per l’intera organizzazione.
* Per ulteriori informazioni, consulta [Abilitazione della [!DNL Basecamp] Integrazione con [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* Configura [!DNL Basecamp] in [Impostazioni personali](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Questo consente ai creatori e proprietari di prove di connettersi al proprio personale [!DNL Basecamp] e autorizzare [!DNL Workfront Proof] accesso. Per ulteriori informazioni, consulta [Configurazione delle impostazioni personali](#configuring-personal-settings).

È possibile integrare [!DNL Workfront] con [!DNL Basecamp] o [!DNL Basecamp Classic]. Ogni versione di [!DNL Basecamp] utilizza un’API diversa e richiede pertanto procedure di configurazione diverse.

Per informazioni sulla configurazione [!DNL Basecamp Classic], vedi [Abilitazione della [!DNL Basecamp] Integrazione con [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) in questo articolo.

Per informazioni sulla configurazione [!DNL Basecamp], vedi [Integrare [!DNL Workfront Proof] con [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## Abilitazione della [!DNL Basecamp] Integrazione con [!DNL Workfront Proof]

Come [Profili delle autorizzazioni di prova in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) o [Profili delle autorizzazioni di prova in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), puoi impostare l’integrazione di Basecamp per l’intero account nel tuo [Impostazioni account](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Vai a [Impostazioni account.](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. Apri **[!UICONTROL Integrazioni]** scheda (1).
1. Per abilitare l’integrazione di Basecamp, fai clic su **[!UICONTROL Abilita]** (2)
1. Verifica che [!DNL Basecamp Classic] è la versione con cui si esegue l’integrazione (3).
1. (Condizionale) Se no [!DNL Basecamp] Viene visualizzato l’URL (4), fai clic su **[!UICONTROL Modifica]** e immetti l&#39;URL per il tuo [!DNL Basecamp] account (senza http://).
1. Fai clic su **[!UICONTROL Salva]** (5)\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. (Facoltativo) Controlla il tuo [!DNL Basecamp] URL nel browser dopo l&#39;accesso al [!DNL Basecamp Classic] conto (6).

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   Una volta integrati [!DNL Workfront Proof] con [!DNL Basecamp], gli utenti possono configurare le proprie impostazioni personali. Per informazioni sulla configurazione delle impostazioni personali, vedi [Configurazione delle impostazioni personali](#configuring-personal-settings).

   Se non è possibile attivare [!DNL Basecamp] integrazione, [!DNL Workfront Proof] l&#39;ID account potrebbe non essere lo stesso dell&#39;ID account utilizzato in [!DNL Basecamp].

## Configurazione delle impostazioni personali

Dopo aver impostato [Impostazioni account](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) per la tua organizzazione, ogni autore che crea/invia bozze deve impostare le proprie  [impostazioni personali.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>Il completamento di questi passaggi è più semplice se disponi dei [!DNL Basecamp] si apre in una finestra del browser e la [!DNL Workfront Proof] si apre in un&#39;altra finestra.

* [Recupero [!DNL Basecamp] Token API](#retrieving-your-basecamp-api-token)
* [Aggiunta di [!DNL Basecamp] Token API per le impostazioni personali](#adding-your-basecamp-api-token-to-your-personal-settings)

### Recupero [!DNL Basecamp] Token API

Completare l&#39;integrazione a livello individuale in [!DNL Workfront Proof], gli utenti devono disporre del proprio token di autenticazione individuale per [!DNL Basecamp] API.

Per recuperare [!DNL Basecamp] Token API:

1. Accedi al tuo [!DNL Basecamp] conto.
1. Fai clic su **[!UICONTROL Informazioni personali]** (1) nell&#39;angolo superiore destro dello schermo.\
   La [!UICONTROL Informazioni personali] viene visualizzata la pagina .\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. In [!UICONTROL Token di autenticazione] sezione, fai clic su **[!UICONTROL Mostra i token]** (2) per visualizzare i token di autenticazione personali.
1. Seleziona la **[!UICONTROL Token per i lettori di feed]** o **[!UICONTROL API di base]** (3), quindi copia il token negli Appunti.

1. Incolla [!DNL Basecamp] Token API nel [!UICONTROL Token per i lettori di feed] o [!UICONTROL API di base] scatola.\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### Aggiunta di [!DNL Basecamp] Token API per le impostazioni personali

Per incollare [!DNL Basecamp] Token API nel tuo [!DNL Workfront Proof] [Impostazioni personali](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):

1. Vai a [[!UICONTROL Integrazioni] - Configurazione utente](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) nel tuo [Impostazioni personali](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1)\
   Un amministratore deve prima abilitare [!DNL Basecamp Classic] integrazione per abilitare le impostazioni personali. Per informazioni sulla configurazione dell’integrazione, consulta [Abilitazione della [!DNL Basecamp] Integrazione con [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) in questo articolo.

1. In [!DNL Basecamp] Token API (2), incolla il token appena copiato dal tuo [!DNL Basecamp] [!UICONTROL Informazioni personali] nel campo (3).\
   Per informazioni sulla copia del [!DNL Basecamp] Token API, vedi [Recupero [!DNL Basecamp] Token API](#retrieving-your-basecamp-api-token) in questo articolo.

1. Fai clic su **[!UICONTROL Salva]** (4)

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

Le [!DNL Workfront Proof] [Impostazioni personali](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) sono ora integrati con i [!DNL Basecamp Classic] conto.
