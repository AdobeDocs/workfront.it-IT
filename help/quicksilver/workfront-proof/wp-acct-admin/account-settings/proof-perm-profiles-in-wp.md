---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Profili delle autorizzazioni di bozza in Workfront Proof
description: In qualità di amministratore di Workfront o di Workfront Proof, puoi assegnare un profilo di autorizzazioni bozza a un utente per specificare le funzionalità di bozza che quest’ultimo disporrà per tutte le bozze presenti nel sistema. Per informazioni sulla configurazione del profilo di autorizzazione di una bozza di un utente, consulta Configurare il profilo di autorizzazione di una bozza di un utente in Workfront Proof.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '1764'
ht-degree: 0%

---

# Profili delle autorizzazioni di bozza in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

In qualità di amministratore [!DNL Workfront] o di amministratore [!DNL Workfront Proof], puoi assegnare un profilo di autorizzazioni di bozza a un utente per specificare le funzionalità di bozza che l&#39;utente disporrà per tutte le bozze nel sistema. Per informazioni sulla configurazione del profilo di autorizzazione di una bozza di un utente, vedere [Configurare il profilo di autorizzazione di una bozza di un utente in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>È inoltre possibile effettuare le seguenti operazioni:
>
>* Concedi agli utenti ruoli specifici per le singole bozze. Per ulteriori informazioni sui ruoli bozza, vedere [Gestione dei ruoli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* Crea profili personalizzati per gli utenti dell’organizzazione. Per ulteriori informazioni, vedere [Configurare profili personalizzati in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>

Nella tabella seguente vengono visualizzate le autorizzazioni disponibili per ogni profilo Autorizzazioni bozza.

| **Elementi propri** |  |  |  |  | **Elementi di altri utenti** |  |  | **Amministratore** | **Fatturazione** |
|---|---|---|---|---|---|---|---|---|---|
|   | **Aggiungi** | **Visualizza** | **Modifica** | **Elimina** | **Visualizza** | **Modifica** | **Elimina** | **Modifica ed Elimina** | **Modifica** |
| Amministratore fatturazione | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |
| Amministratore | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |
| Supervisore | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |
| Manager | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |   |   |   |
| Osservatore |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |
| Visitatore |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style="table-layout:auto"}

Considera quanto segue su ruoli e autorizzazioni:

* Le autorizzazioni di profilo assegnate si riferiscono solo agli utenti e agli elementi nel tuo account. L&#39;eccezione è nel caso degli account satellite, in cui l&#39;amministratore e l&#39;amministratore di fatturazione per gli account principali (hub) possono accedere e gestire le impostazioni e la fatturazione di tali account a livello dell&#39;account hub.
* Gli amministratori di fatturazione e gli amministratori possono eliminare gli utenti. Questa operazione può essere eseguita solo nelle impostazioni dell’account.
* Quando gli amministratori di fatturazione e gli amministratori visualizzano le bozze di proprietà di altri utenti nel loro account, le visualizzano con il ruolo di revisore.
* Utilizzando il ruolo Sola lettura, gli amministratori di fatturazione e gli amministratori possono accedere alle bozze nelle cartelle condivise con loro o nelle cartelle da loro create.

Le sezioni seguenti descrivono ogni profilo e le autorizzazioni associate al profilo in una configurazione standard di [!DNL Workfront Proof]:

* [Amministratore fatturazione](#billing-administrator)
* [Amministratore](#administrator)
* [Supervisore](#supervisor)
* [Manager](#manager)
* [Osservatore](#observer)
* [Visitatore](#visitor)
* [Ospite](#guest)

## Amministratore fatturazione {#billing-administrator}

Gli amministratori fatturazione hanno accesso alle [impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] Pagina fatturazione](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e dispongono delle seguenti autorizzazioni:

![](assets/cleaner2.png)Può generare bozze, caricare file e creare cartelle. Per ulteriori informazioni, vedere [Generare bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Caricare file e contenuti Web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) e [Creare cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)È possibile visualizzare, modificare ed eliminare le proprie bozze e i propri file creati.

![](assets/cleaner2.png)È possibile visualizzare, modificare ed eliminare bozze e file creati da tutti gli utenti dell&#39;organizzazione.

![](assets/cleaner2.png)È possibile eliminare le cartelle pubbliche di altri utenti. Per ulteriori informazioni, vedere [Gestione cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Dispone dei diritti di modifica per tutte le bozze create nell&#39;account.

![](assets/cleaner2.png) può essere impostato come proprietario di Dropzone. Per ulteriori informazioni, vedere [Configurare la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)È possibile accedere alla pagina di fatturazione e modificare i dettagli di fatturazione. Per ulteriori informazioni, vedere [Pagina fatturazione [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![](assets/cleaner2.png)È possibile accedere alla pagina Impostazioni account e modificare i dettagli dell&#39;account. Per ulteriori informazioni, vedere [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Svuotare il cestino. Per ulteriori informazioni, vedere [Ripristina e svuota il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)È possibile aggiungere, modificare ed eliminare utenti.

![](assets/cleaner2.png)È possibile creare gruppi e aggiungere nuovi contatti.

![](assets/cleaner2.png)È possibile eliminare i contatti.

![](assets/cleaner2.png)È possibile modificare le bozze se non sono presenti risposte.

![](assets/no2.png)Impossibile modificare le risposte alle bozze.

![](assets/no2.png)Impossibile eliminare le cartelle private di altri utenti. Per ulteriori informazioni, vedere [Gestione cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

Per informazioni sulle impostazioni account, vedere [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

Per informazioni sulla fatturazione, vedere [The [!DNL Workfront Proof] Billing Page](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Amministratore {#administrator}

Gli amministratori hanno accesso a [Impostazioni account](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)e dispongono delle seguenti autorizzazioni:

![](assets/cleaner2.png)È possibile creare bozze, caricare file e creare cartelle. Per ulteriori informazioni, vedere [Generare bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Caricare file e contenuti Web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) e [Creare cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)È possibile visualizzare, modificare ed eliminare le bozze e i file creati.

![](assets/cleaner2.png)È possibile visualizzare, modificare ed eliminare bozze e file creati da tutti gli utenti dell&#39;organizzazione.

![](assets/cleaner2.png)È possibile eliminare le cartelle pubbliche di altri utenti. Per ulteriori informazioni, vedere [Gestione cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Dispone dei diritti di modifica per tutte le bozze create nell&#39;account.

![](assets/cleaner2.png) può essere impostato come proprietario di Dropzone. Per ulteriori informazioni, vedere [Configurare la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)È possibile accedere alla pagina Impostazioni account e modificare i dettagli dell&#39;account. Per ulteriori informazioni, vedere [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Svuotare il cestino. Per ulteriori informazioni, vedere [Ripristina e svuota il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)È possibile aggiungere, modificare ed eliminare utenti.

![](assets/cleaner2.png)È possibile creare gruppi e aggiungere nuovi contatti.

![](assets/cleaner2.png)È possibile eliminare i contatti.

![](assets/cleaner2.png)È possibile modificare le bozze se non sono presenti risposte.

![](assets/no2.png)Impossibile modificare le risposte alle bozze.

![](assets/no2.png)Impossibile eliminare le cartelle private di altri utenti. Per ulteriori informazioni, vedere [Gestione cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Impossibile accedere alla pagina Fatturazione o modificare i dettagli di fatturazione. Per ulteriori informazioni, vedere [Pagina fatturazione [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Supervisore {#supervisor}

I supervisori dispongono delle seguenti autorizzazioni:

![](assets/cleaner2.png)È possibile creare bozze, caricare file e creare cartelle. Per ulteriori informazioni, vedere [Generare bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Caricare file e contenuti Web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) e [Creare cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)È possibile visualizzare, modificare ed eliminare le proprie bozze e i file creati.

![](assets/cleaner2.png)È possibile visualizzare, modificare ed eliminare bozze e file creati da tutti gli utenti dell&#39;organizzazione.

![](assets/cleaner2.png)È possibile eliminare le cartelle pubbliche di altri utenti. Per ulteriori informazioni, vedere [Gestione cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Dispone dei diritti di modifica per tutte le bozze create nell&#39;account.

![](assets/cleaner2.png) può essere impostato come proprietario di Dropzone. Per ulteriori informazioni, vedere [Configurare la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)È possibile creare gruppi e aggiungere nuovi contatti.

![](assets/cleaner2.png)È possibile eliminare i contatti.

![](assets/cleaner2.png)È possibile modificare le bozze se non sono presenti risposte.

![](assets/no2.png)Impossibile modificare le risposte alle bozze.

![](assets/no2.png)Impossibile eliminare le cartelle private di altri utenti. Per ulteriori informazioni, vedere [Cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![](assets/no2.png)Impossibile accedere alla pagina Fatturazione o alle impostazioni dell&#39;account. Per ulteriori informazioni, vedere [Pagina fatturazione [!DNL Workfront Proof] e [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)

![](assets/no2.png)Impossibile aggiungere, modificare o eliminare utenti.

![](assets/no2.png)Impossibile svuotare il cestino. Per ulteriori informazioni, vedere [Ripristina e svuota il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### Manager {#manager}

I manager dispongono delle seguenti autorizzazioni:

![](assets/cleaner2.png)È possibile creare bozze, caricare file e creare cartelle. Per ulteriori informazioni, vedere [Generare bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Caricare file e contenuti Web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) e [Creare cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)È possibile visualizzare, modificare ed eliminare le proprie bozze e i propri file.

![](assets/cleaner2.png)Consente di visualizzare, esaminare e approvare le bozze di altri utenti condivisi in modo esplicito con loro (diritti di sola lettura per tutti gli elementi di una cartella condivisa). Per ulteriori informazioni, vedere [Gestione dei ruoli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)È possibile creare gruppi e aggiungere un nuovo contatto.

![](assets/no2.png)Impossibile visualizzare, modificare o eliminare bozze e file creati da altri utenti dell&#39;organizzazione.

![](assets/no2.png)Impossibile modificare bozze o risposte.

![](assets/no2.png)Impossibile eliminare le cartelle private di altri utenti. Per ulteriori informazioni, vedere [Gestione cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Impossibile eliminare le cartelle pubbliche di altri utenti. Per ulteriori informazioni, vedere [Gestione cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Impossibile accedere alla pagina Fatturazione o alle impostazioni dell&#39;account. Per ulteriori informazioni, vedere [Pagina fatturazione [!DNL Workfront Proof] e [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)

![](assets/no2.png)Impossibile impostare come proprietario di Dropzone. Per ulteriori informazioni, vedere [Configurare la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Impossibile svuotare il cestino. Per ulteriori informazioni, vedere [Ripristina e svuota il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Impossibile aggiungere, modificare o eliminare utenti.

![](assets/no2.png)Impossibile eliminare i contatti.

### Osservatore {#observer}

Gli osservatori dispongono delle seguenti autorizzazioni:

![](assets/cleaner2.png)Consente di visualizzare, esaminare e approvare le bozze di altri utenti che sono esplicitamente condivisi con loro (diritti di sola lettura per tutto ciò che si trova in una cartella condivisa). Per ulteriori informazioni, vedere [Gestione dei ruoli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Può visualizzare i file condivisi in modo esplicito con loro.

![](assets/cleaner2.png) può visualizzare contatti e gruppi

![](assets/no2.png)Impossibile creare bozze, caricare file e creare cartelle. Per ulteriori informazioni, vedere [Caricare file e contenuto Web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Impossibile visualizzare, modificare o eliminare bozze e file creati da altri utenti dell&#39;organizzazione.

![](assets/no2.png)Impossibile modificare bozze o risposte.

![](assets/no2.png)Impossibile eliminare gli elementi creati nell&#39;organizzazione.

![](assets/no2.png)Impossibile accedere alla pagina Fatturazione o alle impostazioni dell&#39;account. Per ulteriori informazioni, vedere [Pagina fatturazione [!DNL Workfront Proof] e [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)

![](assets/no2.png)Impossibile impostare come proprietario di Dropzone. Per ulteriori informazioni, vedere [Configurare la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Impossibile svuotare il cestino. Per ulteriori informazioni, vedere [Ripristina e svuota il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Impossibile aggiungere, modificare o eliminare utenti.

![](assets/no2.png)Impossibile creare gruppi o aggiungere nuovi contatti.

![](assets/no2.png)Impossibile eliminare i contatti.

>[!NOTE]
>
>I menu e le funzioni disponibili agli osservatori sono limitati.
>
>* Gli osservatori non vedono il menu Intestazione o il menu Nuovo verde nel loro dashboard
>* Gli osservatori non vedono i seguenti collegamenti nelle loro Impostazioni: Impostazioni account, Fatturazione
>

### Visitatore {#visitor}

I visitatori dispongono delle seguenti autorizzazioni:

![](assets/cleaner2.png)Consente di visualizzare, esaminare e approvare le bozze di altri utenti condivisi in modo esplicito con loro (diritti di sola lettura per tutti gli elementi di una cartella condivisa). Per ulteriori informazioni, vedere [Gestione dei ruoli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Può visualizzare i file condivisi in modo esplicito con loro.

![](assets/no2.png) Impossibile visualizzare contatti e gruppi

![](assets/no2.png)Impossibile creare bozze, caricare file e creare cartelle. Per ulteriori informazioni, vedere [Caricare file e contenuto Web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Impossibile visualizzare, modificare o eliminare bozze e file creati da altri utenti dell&#39;organizzazione.

![](assets/no2.png)Impossibile modificare bozze o risposte.

![](assets/no2.png)Impossibile eliminare gli elementi creati nell&#39;organizzazione.

![](assets/no2.png)Impossibile accedere alla pagina Fatturazione o alle impostazioni dell&#39;account. Per ulteriori informazioni, vedere [Pagina fatturazione [!DNL Workfront Proof] e [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)

![](assets/no2.png)Impossibile impostare come proprietario di Dropzone. Per ulteriori informazioni, vedere [Configurare la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Impossibile svuotare il cestino. Per ulteriori informazioni, vedere [Ripristina e svuota il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Impossibile aggiungere, modificare o eliminare utenti.

![](assets/no2.png)Impossibile creare gruppi o aggiungere nuovi contatti.

![](assets/no2.png)Impossibile eliminare i contatti.

>[!NOTE]
>
>I menu e le funzioni disponibili per i visitatori sono limitati.
>
>* I visitatori non visualizzano il menu Intestazione o il menu Nuovo verde nel loro dashboard
>* I visitatori non visualizzano i seguenti collegamenti nelle loro Impostazioni: Impostazioni account, Fatturazione
>

### Ospite {#guest}

Il profilo Guest viene utilizzato per consentire l’accesso alle bozze ai revisori che non dispongono di un proprio account Workfront Proof. Gli ospiti possono accedere alle bozze condivise con loro direttamente tramite le loro notifiche e-mail personali.

![](assets/cleaner2.png)Può visualizzare, esaminare e approvare le bozze condivise in modo esplicito con loro.

![](assets/cleaner2.png)Può visualizzare i file condivisi in modo esplicito con loro.

![](assets/no2.png)Impossibile accedere al dashboard.

![](assets/no2.png)Impossibile condividere le cartelle con le cartelle. Per ulteriori informazioni, vedere [Gestione cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Impossibile aggiungere come autori o moderatori alle bozze. Per ulteriori informazioni, vedere [Gestione dei ruoli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>Gli ospiti non sono utenti di Workfront Proof, pertanto non possono visualizzare tutte le bozze condivise con loro nella propria dashboard.

## Modificare il profilo di autorizzazione di una bozza di un utente

Gli amministratori e gli amministratori di fatturazione possono modificare i profili delle autorizzazioni di tutti gli utenti dell’account.

1. Per trovare l&#39;utente da modificare, eseguire una delle operazioni seguenti:

   * Passa a **[!UICONTROL Impostazioni account]**, quindi fai clic sulla scheda **[!UICONTROL Utenti]**.

   * Passare alla pagina **[!UICONTROL Contatti]**.

1. Fai clic sul nome dell’utente di cui desideri modificare le autorizzazioni. ![](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. Fare clic sul menu a discesa **[!UICONTROL Profilo autorizzazioni]** e selezionare un nuovo profilo di autorizzazione. :

   ![Schermata_2018-03-30_14-18-03.png](assets/screenshot-2018-03-30-14-18-03a.png)

   I profili di autorizzazione sono Amministratore, Supervisore, Manager e Osservatore.

1. Fai clic in un punto qualsiasi al di fuori del menu per salvare.

>[!NOTE]
>
>Gli amministratori non possono assegnare il profilo Amministratore fatturazione. L’elenco delle modifiche apportate al profilo è disponibile nei seguenti registri:
>
>* Registri attività account
>* Il registro del profilo dell’utente (accessibile solo a tale utente)
>

Per ulteriori informazioni sui registri attività, vedere [Informazioni su [!DNL Workfront Proof] Activity Audit Trail](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
