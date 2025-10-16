---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Configura la sezione  [!DNL Adobe Workfront]  per  [!DNL Salesforce]  utenti
description: Dopo aver installato  [!DNL Adobe Workfront] per Salesforce come amministratore [!DNL Workfront] puoi renderla disponibile agli utenti aggiungendola in una nuova sezione ai layout di pagina Opportunità e Account in Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 1%

---

# Configura la sezione [!DNL Adobe Workfront] per [!DNL Salesforce] utenti

>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Come parte di questo processo di transizione, l&#39;integrazione di Workfront for Salesforce non sarà disponibile dopo il **28 febbraio 2026**.
>
>È consigliabile utilizzare l’automazione e l’integrazione di Workfront per le esigenze di integrazione della tua organizzazione con Salesforce.
>
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Salesforce, vedere [Moduli Salesforce](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Dopo aver installato [!DNL Adobe Workfront] per [!DNL Salesforce] come amministratore [!DNL Workfront], puoi renderla disponibile agli utenti aggiungendola in una nuova sezione alle loro [!UICONTROL opportunità] e [!UICONTROL account]
layout di pagina in [!UICONTROL Salesforce].

Per informazioni sull&#39;installazione di [!DNL Workfront for Salesforce], vedere [Installa [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Affinché gli utenti dispongano di [!DNL Workfront] nei framework [!DNL Classic] e [!DNL Lightning Experience], è necessario aggiungere le pagine [!DNL WorkfrontOpportunities] e [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] ai layout di pagina [!UICONTROL Opportunity] e [!UICONTROL Accounts], rispettivamente.



## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Piano</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

* È necessaria un&#39;istanza [!DNL Salesforce] con accesso a un account amministratore di sistema.
* È necessaria un&#39;istanza [!DNL Workfront] con accesso a un account amministratore di sistema.

## Configura la sezione [!DNL Workfront] nel framework [!DNL Salesforce Classic]

1. Accedere a [!DNL Salesforce] come amministratore Workfront.
1. Fare clic su **[!UICONTROL Configurazione].**
1. Nella sezione **[!UICONTROL Build]** espandere **[!UICONTROL Personalizza].**

1. Espandi **[!UICONTROL Opportunità]**, quindi fai clic su **[!UICONTROL Layout di pagina]** per aggiungere la sezione [!DNL Workfront] a un&#39;opportunità.

   Oppure

   Espandi **[!UICONTROL Account]**, quindi fai clic su **[!UICONTROL Layout di pagina]** per aggiungere la sezione [!DNL Workfront] a un account
.

1. Fai clic su **[!UICONTROL Modifica]** in un layout esistente.

   Oppure

   Fai clic su **[!UICONTROL Nuovo]** per aggiungere un nuovo layout.

1. (Facoltativo) Trascina il componente **[!UICONTROL Sezione]** nel layout e rilascialo nella posizione desiderata.\

1. (Facoltativo) Specificate un nome per la nuova sezione.

   È consigliabile denominare questa sezione **[!DNL Workfront]**.

1. (Facoltativo) Specifica il **[!UICONTROL Layout]** e il **[!UICONTROL Ordine dei tasti di tabulazione]** desiderati per la nuova sezione.

   È consigliabile selezionare il layout **[!UICONTROL 1-Colonna]** per la sezione [!DNL Workfront].

1. Fai clic su **[!UICONTROL OK]**.
1. Nell&#39;area **[!UICONTROL Layout]**, fare clic su **[!UICONTROL Pagine Visualforce].**

1. Trascina e rilascia il componente **[!UICONTROL WorkfrontOpportunities]** nella nuova sezione del layout **[!UICONTROL Opportunities]**.

   Oppure

   Trascina e rilascia il componente **[!UICONTROL WorkfrontAccounts]** nella nuova sezione nel layout **[!UICONTROL Account]**.\

1. Fai clic sull&#39;icona **[!UICONTROL Proprietà]** in alto a destra del componente appena aggiunto.\

1. Per ottenere una visualizzazione ottimale, specificare le proprietà seguenti per la pagina [!DNL Workfront Visualforce]:

   * **[!UICONTROL Larghezza (in pixel o %)]**: 100%
   * **[!UICONTROL Altezza (in pixel)]**: 600
   * Selezionare **[!UICONTROL Mostra barre di scorrimento]**.

1. Fai clic su **[!UICONTROL OK]**.
1. Fai clic su **[!UICONTROL Salva]** per salvare il layout.

   Tutti gli utenti a cui è stato assegnato questo layout possono ora visualizzare la sezione [!DNL Workfront] nei loro oggetti [!UICONTROL Opportunities] o [!UICONTROL Accounts].

   Gli utenti visualizzano una schermata di accesso di [!DNL Workfront] nella sezione [!DNL Workfront]. Se non dispongono di un account [!DNL Workfront], è possibile comprimere la sezione, ma non rimuoverla dal layout.

## Configura la sezione [!DNL Workfront] nel framework [!DNL Salesforce Lightning Experience]

È possibile aggiungere la sezione [!DNL Workfront] al layout di un [!DNL Salesforce] [!UICONTROL opportunità] o di un account
nel framework [!DNL Salesforce Lightning Experience] accedendo all&#39;area [!UICONTROL Setup] o da un account
o [!UICONTROL oggetto Opportunity].

* [Configura la sezione  [!DNL Workfront]  al livello [!UICONTROL Configurazione]](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configura la sezione  [!DNL Workfront]  a livello di opportunità o account](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configura la sezione [!DNL Workfront] al livello [!UICONTROL Configurazione] {#configure-the-workfront-section-at-the-setup-level}

1. Accedere a [!DNL Salesforce] come amministratore di sistema.
1. Fai clic sull&#39;icona **[!UICONTROL Configurazione]**, quindi fai clic su **[!UICONTROL Configurazione]**.

1. Espandere **[!UICONTROL Oggetto e campi]**, quindi fare clic su **[!UICONTROL Gestione oggetti]**.

1. Fai clic su **[!UICONTROL Opportunità]** per personalizzare il layout di un&#39;opportunità.

   Oppure

   Fai clic su **[!UICONTROL Account]** per personalizzare il layout di un account.

1. Fare clic su **[!UICONTROL Layout di pagina]**.
1. Fare clic sul nome di un layout di pagina esistente per modificarlo.

   Oppure

   Fai clic su **[!UICONTROL Nuovo]** per creare un nuovo layout di pagina.

1. Continua con [Configura la  [!DNL Workfront] sezione a livello di opportunità o account](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) di seguito.

### Configura la sezione [!DNL Workfront] a livello di opportunità o account {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Accedere a [!DNL Salesforce] come amministratore di sistema.
1. Vai a un **[!UICONTROL opportunità]** o **[!UICONTROL account]**.

1. Fai clic sull&#39;icona **[!UICONTROL Configurazione]**, quindi fai clic su **[!UICONTROL Modifica pagina]**.

1. Espandi la sezione **[!UICONTROL Gestione personalizzata]**.
1. Trascina e rilascia il componente **[!DNL Workfront]** nell&#39;opportunità [!UICONTROL o nell&#39;account]
pagina.

   È consigliabile utilizzare l&#39;intera larghezza della pagina per la sezione [!DNL Workfront] anziché una delle colonne del layout.

1. Fai clic su **[!UICONTROL Salva]**.

   Tutti gli utenti a cui è stato assegnato questo layout possono ora visualizzare la sezione [!DNL Workfront] nei loro oggetti [!UICONTROL Opportunities] o [!UICONTROL Accounts].

   >[!NOTE]
   >
   >Gli utenti visualizzano una schermata di accesso di [!DNL Workfront] nella sezione [!DNL Workfront]. Se non dispongono di un account [!DNL Workfront], è possibile comprimere la sezione, ma non rimuoverla dal layout. Gli utenti possono accedere utilizzando il metodo di autenticazione che hai attivato: Autenticazione avanzata o l’URL SAML (Security Assertion Markup Language).

