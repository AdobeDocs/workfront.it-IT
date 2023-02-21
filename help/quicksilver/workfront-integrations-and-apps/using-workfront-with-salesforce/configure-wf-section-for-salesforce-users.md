---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Configura le [!DNL Adobe Workfront] sezione per [!DNL Salesforce] utenti
description: Dopo l'installazione [!DNL Adobe Workfront] per Salesforce come [!DNL Workfront] amministratore, puoi renderlo disponibile agli utenti aggiungendolo in una nuova sezione ai layout della pagina Opportunità e account di Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 1%

---

# Configura le [!DNL Adobe Workfront] sezione per [!DNL Salesforce] utenti

A [!UICONTROL Pro] [!DNL Workfront] Per utilizzare questa funzione è necessario pianificare. Per ulteriori informazioni sui vari piani disponibili, vedi [[!DNL Workfront] Piani.](https://www.workfront.com/plans)

Dopo l&#39;installazione [!DNL Adobe Workfront] per [!DNL Salesforce] come [!DNL Workfront] amministratore, puoi renderlo disponibile agli utenti aggiungendolo in una nuova sezione al loro [!UICONTROL Opportunità] e [!UICONTROL Account]
layout di pagina in [!UICONTROL Salesforce].

Per informazioni sull’installazione [!DNL Workfront for Salesforce], vedi [Installa [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Per gli utenti [!DNL Workfront] disponibili in entrambi i [!DNL Classic] e [!DNL Lightning Experience] framework, devi aggiungere [!DNL WorkfrontOpportunities] e [!DNL WorkfrontAccounts] [!UICONTROL Effetto visivo] alle pagine [!UICONTROL Opportunità] e [!UICONTROL Account] layout di pagina, rispettivamente.

## Requisiti di accesso

Per utilizzare la funzionalità descritta in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Prerequisiti

* Devi avere un [!DNL Salesforce] istanza con accesso a un account amministratore di sistema.
* Devi avere un [!DNL Workfront] istanza con accesso a un account amministratore di sistema.

## Configura le [!DNL Workfront] nella sezione [!DNL Salesforce Classic] quadro

1. Accedi a [!DNL Salesforce] come amministratore Workfront.
1. Fai clic su **[!UICONTROL Configurazione].**
1. In **[!UICONTROL Crea]** sezione, espandi **[!UICONTROL Personalizza].**

1. Espandi **[!UICONTROL Opportunità]**, quindi fai clic su **[!UICONTROL Layout di pagina]** per aggiungere [!DNL Workfront] a un&#39;opportunità.

   Oppure

   Espandi **[!UICONTROL Account]**, quindi fai clic su **[!UICONTROL Layout di pagina]** per aggiungere [!DNL Workfront] a un account .

1. Fai clic su **[!UICONTROL Modifica]** su un layout esistente.

   Oppure

   Fai clic su **[!UICONTROL Nuovo]** per aggiungere un nuovo layout.

1. (Facoltativo) Trascina il **[!UICONTROL Sezione]** al layout e rilasciarlo nella posizione desiderata.\

1. (Facoltativo) Specifica un nome per la nuova sezione.

   Ti consigliamo di assegnare un nome a questa sezione **[!DNL Workfront]**.

1. (Facoltativo) Specifica la **[!UICONTROL Layout]** e **[!UICONTROL Ordine dei tasti di tabulazione]** per la nuova sezione.

   È consigliabile selezionare **[!UICONTROL 1 colonna]** layout per [!DNL Workfront] sezione .

1. Fai clic su **[!UICONTROL OK]**.
1. In **[!UICONTROL Layout]** area, fai clic su **[!UICONTROL Pagine della visualizzazione].**

1. Trascina e rilascia la **[!UICONTROL Opportunità di lavoro]** nella nuova sezione **[!UICONTROL Opportunità]** Layout.

   Oppure

   Trascina e rilascia la **[!UICONTROL Account di lavoro]** nella nuova sezione  **[!UICONTROL Account]** Layout.\

1. Fai clic sul pulsante **[!UICONTROL Proprietà]** in alto a destra del componente appena aggiunto.\

1. Per ottenere una visualizzazione ottimale, specifica le seguenti proprietà per [!DNL Workfront Visualforce] pagina:

   * **[!UICONTROL Larghezza (in pixel o %)]**: 100%
   * **[!UICONTROL Altezza (in pixel)]**: 600
   * Seleziona **[!UICONTROL Mostra barre di scorrimento]**.

1. Fai clic su **[!UICONTROL OK]**.
1. Fai clic su **[!UICONTROL Salva]** per salvare il layout.

   Tutti gli utenti a cui è stato assegnato questo layout possono ora visualizzare il [!DNL Workfront] sezione [!UICONTROL Opportunità] o [!UICONTROL Account] oggetti.

   Gli utenti visualizzano un [!DNL Workfront] schermata di accesso [!DNL Workfront] sezione . Se non hanno un [!DNL Workfront] possono comprimere la sezione, ma non rimuoverla dal layout.

## Configura le [!DNL Workfront] nella sezione [!DNL Salesforce Lightning Experience] quadro

Puoi aggiungere la [!DNL Workfront] al layout di un [!DNL Salesforce] [!UICONTROL Opportunità] o Account nel [!DNL Salesforce Lightning Experience] o mediante l&#39;accesso al [!UICONTROL Configurazione] o da un account o [!UICONTROL Opportunità] oggetto.

* [Configura le [!DNL Workfront] nella sezione [!UICONTROL Configurazione] livello](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configura le [!DNL Workfront] Sezione a livello di opportunità o account](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configura le [!DNL Workfront] nella sezione [!UICONTROL Configurazione] livello {#configure-the-workfront-section-at-the-setup-level}

1. Accedi a [!DNL Salesforce] come amministratore di sistema.
1. Fai clic sul pulsante **[!UICONTROL Configurazione]** icona, quindi fai clic su **[!UICONTROL Configurazione]**.

1. Espandi **[!UICONTROL Oggetto e campi]**, quindi fai clic su **[!UICONTROL Gestione oggetti]**.

1. Fai clic su **[!UICONTROL Opportunità]** personalizzare il layout di un&#39;opportunità.

   Oppure

   Fai clic su **[!UICONTROL Account]** personalizzare il layout di un account.

1. Fai clic su **[!UICONTROL Layout di pagina]**.
1. Fare clic sul nome di un layout di pagina esistente per modificarlo.

   Oppure

   Fai clic su **[!UICONTROL Nuovo]** per creare un nuovo layout di pagina.

1. Continua con [Configura le [!DNL Workfront] Sezione a livello di opportunità o account](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) sotto.

### Configura le [!DNL Workfront] Sezione a livello di opportunità o account {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Accedi a [!DNL Salesforce] come amministratore di sistema.
1. Vai a un **[!UICONTROL Opportunità]** o **[!UICONTROL Account]**.

1. Fai clic sul pulsante **[!UICONTROL Configurazione]** icona, quindi fai clic su **[!UICONTROL Modifica pagina]**.\

1. Espandi la **[!UICONTROL Personalizzato]** sezione .
1. Trascina e rilascia la **[!DNL Workfront]** componente [!UICONTROL Opportunità] o alla pagina Account.

   È consigliabile utilizzare l’intera larghezza della pagina per [!DNL Workfront] anziché una delle colonne del layout.

1. Fai clic su **[!UICONTROL Salva]**.

   Tutti gli utenti a cui è stato assegnato questo layout possono ora visualizzare il [!DNL Workfront] sezione [!UICONTROL Opportunità] o [!UICONTROL Account] oggetti.

   >[!NOTE]
   >
   >Gli utenti visualizzano un [!DNL Workfront] schermata di accesso [!DNL Workfront] sezione . Se non hanno un [!DNL Workfront] possono comprimere la sezione, ma non rimuoverla dal layout. Gli utenti possono accedere utilizzando il metodo di autenticazione abilitato: Autenticazione avanzata o URL SAML (Security Assertion Markup Language).

