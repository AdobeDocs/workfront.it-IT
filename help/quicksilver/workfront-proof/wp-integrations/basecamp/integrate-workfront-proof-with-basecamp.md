---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Integrare [!DNL Workfront Proof] con [!DNL Basecamp]
description: Se utilizzi [!DNL Basecamp] per la gestione dei progetti puoi offrire al team di progetto strumenti di revisione e approvazione più avanzati utilizzando [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 0%

---

# Integrare [!DNL Workfront Proof] con [!DNL Basecamp]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Se utilizzi [!DNL Basecamp] per la gestione dei progetti puoi offrire al team di progetto strumenti di revisione e approvazione più avanzati utilizzando [!DNL Workfront Proof].

## Informazioni sulla [!DNL Basecamp] Integrazione con [!DNL Workfront]

Integrazione con [!DNL Basecamp] consente agli utenti di visualizzare, rivedere e approvare le bozze all’interno di [!DNL Basecamp]. Gli utenti possono inviare le bozze al tuo [!DNL Workfront Proof] e collegali al tuo [!DNL Basecamp] progetto. I revisori possono commentare e prendere decisioni tramite [!DNL Basecamp], utilizzando la prova mini incorporata nel messaggio Basecamp.

Quando integrato con [!DNL Workfront Proof], [!DNL Basecamp] dispone della seguente funzionalità di correzione:

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

* Configura [!DNL Basecamp] in [Impostazioni account:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Questo consente l’integrazione di Basecamp per l’intera organizzazione. Per ulteriori informazioni, consulta [Abilitazione dell’integrazione di base con [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* Configura [!DNL Basecamp] in [Impostazioni personali](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Questo consente ai creatori e proprietari di prove di connettersi al loro account Basecamp personale e di autorizzare [!DNL Workfront Proof] accesso. Per ulteriori informazioni, consulta [Configurazione delle impostazioni personali](#configuring-personal-settings).

È possibile integrare [!DNL Workfront] con [!DNL Basecamp] o [!DNL Basecamp Classic]. Ogni versione di [!DNL Basecamp] utilizza un’API diversa e richiede pertanto procedure di configurazione diverse.

Per informazioni sulla configurazione [!DNL Basecamp Classic], vedi [Integrazione [!DNL Workfront Proof] con [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Abilitazione della [!DNL Basecamp] Integrazione con [!DNL Workfront Proof]

Come [Profili delle autorizzazioni di prova in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) o [Profili delle autorizzazioni di prova in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), puoi impostare [!DNL Basecamp] integrazione per l’intero account nel [Impostazioni account](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. In [!UICONTROL Basecamp], raccoglie le seguenti informazioni:

   * L’URL per la [!DNL Basecamp] account
   * L&#39;URL si trova in &quot;[!UICONTROL Informazioni personali]&quot; sezione

1. Esci [!DNL Basecamp].
1. Fai clic su **[!UICONTROL Impostazioni account]** nell&#39;angolo in alto a destra.
1. Fai clic sul pulsante **[!UICONTROL Integrazioni]** scheda .
1. In **[!UICONTROL [!DNL Basecamp]]** a destra di **[!UICONTROL [!DNL Basecamp]integrazione]**, fai clic su **[!UICONTROL Abilita]**.

1. Accanto a **[!UICONTROL [!DNL Basecamp]version]**, verifica la **[!UICONTROL Versione classica]** è la versione con cui si esegue l&#39;integrazione.

1. (Condizionale) Se no [!DNL Basecamp] Viene visualizzato l’URL, fai clic su **[!UICONTROL Modifica]**, digita l’URL per la [!DNL Basecamp] account, senza includere &quot;http://&quot;, quindi fai clic su **[!UICONTROL Salva]**.

1. Nell&#39;angolo superiore destro della finestra, fai clic su **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni personali]**.

1. Fai clic sul pulsante **[!UICONTROL Integrazioni]** scheda .
1. Sotto **[!DNL Basecamp]** al diritto di **[!UICONTROL Integrazione basecamp]**, fai clic su **[!UICONTROL Abilita]**.

1. Nelle opzioni visualizzate, a destra di **[!UICONTROL [!DNL Basecamp]Token API]**, fai clic su **[!UICONTROL Modifica]**.

1. Nella casella visualizzata, digita l’URL trovato nella colonna &quot;[!UICONTROL Informazioni personali]&quot; sezione in [!DNL Basecamp], quindi fai clic su **[!UICONTROL Salva]**.\
   Una volta integrati [!DNL Workfront Proof] con [!DNL Basecamp], gli utenti possono configurare le proprie impostazioni personali. Per informazioni sulla configurazione delle impostazioni personali, vedi [Configurazione delle impostazioni personali](#configuring-personal-settings)

1. Se non è possibile attivare [!DNL Basecamp] integrazione, [!DNL Workfront Proof] l&#39;ID account potrebbe non essere lo stesso dell&#39;ID account utilizzato in [!DNL Basecamp].
1. Una volta integrati [!DNL Workfront Proof] con [!DNL Basecamp], gli utenti possono configurare le proprie impostazioni personali. Per informazioni sulla configurazione delle impostazioni personali, vedi [Configurazione delle impostazioni personali](#configuring-personal-settings).

## Configurazione delle impostazioni personali

Dopo aver impostato [Impostazioni account](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) per la tua organizzazione, ogni autore che crea/invia bozze deve impostare le proprie  [impostazioni personali.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Vai a **[!UICONTROL Impostazioni personali** &#x200B;**x]**.

1. Apri **[!UICONTROL Integrazioni]** scheda (1).
1. Per abilitare [!DNL Basecamp] integrazione, fai clic su **[!UICONTROL Abilita]** (2)
1. Fai clic su **[!UICONTROL Collegati al tuo [!DNL Basecamp] account]** (3)\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. Accedi al tuo [!DNL Basecamp] conto (1).\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. Fai clic su **[!UICONTROL Sì, permetterò l&#39;accesso]** autorizzare [!DNL Workfront Proof] accesso al tuo account (2).\
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. (Facoltativo) Quando l&#39;integrazione personale è attiva (3), puoi facilmente passare da un&#39;integrazione all&#39;altra [!DNL Basecamp] conti.

   1. Clic **[!UICONTROL Interruttore [!DNL Basecamp] account]** (4).\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      La [!UICONTROL Cambia account base] ti porta al [!UICONTROL Impostazioni personali] pagina, in cui è possibile scegliere quale delle [!DNL Basecamp] account da integrare con [!DNL Workfront Proof] conto.

   1. Fai clic su **[!UICONTROL Riintegra con[!DNL Basecamp]]** (5) prima di scegliere il [!DNL Basecamp] account\

      Questo aggiorna la [!UICONTROL Impostazioni personali] e mostra l&#39;elenco più aggiornato di [!DNL Basecamp] conti.

   1. Fai clic su **[!UICONTROL Integrazione con questo account]** per collegarlo a [!DNL Workfront Proof].\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      È ora possibile aggiungere bozze a [!DNL Basecamp] progetti.
