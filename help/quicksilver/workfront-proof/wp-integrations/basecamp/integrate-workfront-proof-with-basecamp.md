---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Integra [!DNL Workfront Proof] con [!DNL Basecamp]
description: Se utilizzi  [!DNL Basecamp]  per la gestione dei progetti, puoi offrire al team di progetto strumenti di revisione e approvazione più completi utilizzando  [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Integra [!DNL Workfront Proof] con [!DNL Basecamp]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Se utilizzi [!DNL Basecamp] per la gestione dei progetti, puoi offrire al team di progetto strumenti di revisione e approvazione più completi tramite [!DNL Workfront Proof].

## Informazioni sull&#39;integrazione di [!DNL Basecamp] con [!DNL Workfront]

L&#39;integrazione con [!DNL Basecamp] consente agli utenti di visualizzare, esaminare e approvare le bozze in [!DNL Basecamp]. Gli utenti possono inviare bozze al tuo account [!DNL Workfront Proof] e collegarli al progetto [!DNL Basecamp]. I revisori possono aggiungere commenti e prendere decisioni tramite [!DNL Basecamp], utilizzando la mini bozza incorporata nel messaggio Basecamp.

Se integrato con [!DNL Workfront Proof], [!DNL Basecamp] dispone delle seguenti funzionalità di verifica:

* Gli utenti possono rivedere e approvare le bozze entro [!DNL Basecamp Classic].
* Gli utenti dispongono di strumenti di revisione prontamente disponibili.
* I team di revisione del progetto ricevono un messaggio in [!DNL Basecamp] con una mini bozza per la revisione e l&#39;approvazione.
* Gli utenti possono passare a una bozza a pagina intera per la revisione e l’approvazione.
* Gli utenti possono aggiungere commenti e markup alle bozze mini e full-size.

  >[!NOTE]
  >
  >Una volta risposto, un commento non può essere modificato o eliminato.

* I revisori possono rispondere alle marcature e effettuate da altri revisori.
* Gli utenti vengono avvisati quando è disponibile una nuova versione della bozza.
* Gli utenti che non sono [!DNL Workfront Proof] utenti possono lavorare su una bozza in [!DNL Basecamp].

L&#39;integrazione di [!DNL Workfront Proof] con [!DNL Basecamp] deve essere impostata su due livelli:

* Configura [!DNL Basecamp] in [Impostazioni account:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) In questo modo viene abilitata l&#39;integrazione Basecamp per l&#39;intera organizzazione. Per ulteriori informazioni, vedere [Abilitazione dell&#39;integrazione Basecamp con [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* Configura [!DNL Basecamp] in [Impostazioni personali](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): consente ai creatori e ai proprietari di bozze di connettersi al proprio account Basecamp personale e di autorizzare l&#39;accesso a [!DNL Workfront Proof]. Per ulteriori informazioni, vedere [Configurazione delle impostazioni personali](#configuring-personal-settings).

È possibile integrare [!DNL Workfront] con [!DNL Basecamp] o [!DNL Basecamp Classic]. Ogni versione di [!DNL Basecamp] utilizza un&#39;API diversa e richiede pertanto procedure di configurazione diverse.

Per informazioni sulla configurazione di [!DNL Basecamp Classic], vedere [Integrazione [!DNL Workfront Proof] con [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Abilitazione dell&#39;integrazione di [!DNL Basecamp] con [!DNL Workfront Proof]

In qualità di [profili di autorizzazioni bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) o [profili di autorizzazioni bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), puoi impostare l&#39;integrazione [!DNL Basecamp] per l&#39;intero account nelle [impostazioni account](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. In [!UICONTROL Basecamp], raccogliere le informazioni seguenti:

   * L&#39;URL del tuo account [!DNL Basecamp]
   * URL trovato nella sezione &quot;[!UICONTROL Informazioni personali]&quot;

1. Disconnettersi da [!DNL Basecamp].
1. Fai clic su **[!UICONTROL Impostazioni account]** nell&#39;angolo superiore destro.
1. Fai clic sulla scheda **[!UICONTROL Integrazioni]**.
1. Nella sezione **[!UICONTROL [!DNL Basecamp]]**, a destra dell&#39;integrazione **[!UICONTROL [!DNL Basecamp]]**, fare clic su **[!UICONTROL Abilita]**.

1. Accanto alla **[!UICONTROL [!DNL Basecamp]versione]**, verifica che la **[!UICONTROL versione classica]** sia la versione con cui stai effettuando l&#39;integrazione.

1. (Condizionale) Se non viene visualizzato alcun URL [!DNL Basecamp], fare clic su **[!UICONTROL Modifica]**, digitare l&#39;URL per l&#39;account [!DNL Basecamp], senza includere &quot;http://&quot;, quindi fare clic su **[!UICONTROL Salva]**.

1. Nell&#39;angolo superiore destro della finestra fare clic su **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni personali]**.

1. Fai clic sulla scheda **[!UICONTROL Integrazioni]**.
1. In **[!DNL Basecamp]**, a destra di **[!UICONTROL Integrazione Basecamp]**, fare clic su **[!UICONTROL Abilita]**.

1. Nelle opzioni visualizzate, a destra di **[!UICONTROL [!DNL Basecamp]Token API]**, fai clic su **[!UICONTROL Modifica]**.

1. Nella casella visualizzata digitare l&#39;URL trovato nella sezione &quot;[!UICONTROL Informazioni personali]&quot; di [!DNL Basecamp], quindi fare clic su **[!UICONTROL Salva]**.\
   Dopo aver integrato [!DNL Workfront Proof] con [!DNL Basecamp], gli utenti possono configurare le proprie impostazioni personali. Per informazioni sulla configurazione delle impostazioni personali, vedere [Configurazione delle impostazioni personali](#configuring-personal-settings)

1. Se non riesci ad abilitare l&#39;integrazione di [!DNL Basecamp], l&#39;ID dell&#39;account [!DNL Workfront Proof] potrebbe non essere uguale all&#39;ID dell&#39;account utilizzato in [!DNL Basecamp].
1. Dopo aver integrato [!DNL Workfront Proof] con [!DNL Basecamp], gli utenti possono configurare le proprie impostazioni personali. Per informazioni sulla configurazione delle impostazioni personali, vedere [Configurazione delle impostazioni personali](#configuring-personal-settings).

## Configurazione delle impostazioni personali

Dopo aver configurato le [impostazioni account](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) per l&#39;organizzazione, ogni autore che crea/invia bozze deve impostare le [impostazioni personali.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Vai a **[!UICONTROL Impostazioni personali**&#x200B;**]**.

1. Apri la scheda **[!UICONTROL Integrazioni]** (1).
1. Per abilitare l&#39;integrazione di [!DNL Basecamp], fare clic su **[!UICONTROL Abilita]** (2).
1. Fai clic su **[!UICONTROL Connetti al tuo account [!DNL Basecamp]]** (3).\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. Accedi al tuo account [!DNL Basecamp] (1).\
   ![Pagina_accesso_base.png](assets/basecamp-login-page-350x107.png)

1. Fai clic su **[!UICONTROL Sì, consento l&#39;accesso]** per autorizzare l&#39;accesso [!DNL Workfront Proof] al tuo account (2).\
   ![Pagina_autorizzazione_base](assets/basecamp-authorization-page-350x173.png)

1. (Facoltativo) Quando l&#39;integrazione personale è attiva (3), è possibile passare facilmente da un account all&#39;altro [!DNL Basecamp].

   1. Fare clic su **[!UICONTROL Cambia account [!DNL Basecamp]]** (4).\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      L&#39;account [!UICONTROL Switch Basecamp] consente di accedere alla pagina [!UICONTROL Impostazioni personali], in cui è possibile scegliere gli account [!DNL Basecamp] che si desidera integrare con l&#39;account [!DNL Workfront Proof].

   1. Fai clic su **[!UICONTROL Reintegra con[!DNL Basecamp]]** (5) prima di scegliere l&#39;account [!DNL Basecamp]\

      In questo modo viene aggiornata la pagina [!UICONTROL Impostazioni personali] e viene visualizzato l&#39;elenco aggiornato degli account [!DNL Basecamp].

   1. Fai clic su **[!UICONTROL Integra con questo account]** per connetterlo a [!DNL Workfront Proof].\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      È ora possibile aggiungere bozze a [!DNL Basecamp] progetti.
