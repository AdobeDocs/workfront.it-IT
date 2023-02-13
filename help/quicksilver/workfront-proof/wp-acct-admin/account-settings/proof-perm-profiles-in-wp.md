---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Profili delle autorizzazioni di prova in Workfront Proof
description: In qualità di amministratore di Workfront o amministratore di Workfront Proof, puoi assegnare un profilo di autorizzazioni di prova a un utente per specificare le funzionalità di correzione che l’utente avrà per tutte le bozze del sistema. Per informazioni sulla configurazione del profilo delle autorizzazioni di prova di un utente, consulta Configurare un profilo delle autorizzazioni di prova di un utente in Workfront Proof .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '1769'
ht-degree: 1%

---

# Profili delle autorizzazioni di prova in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Come [!DNL Workfront] amministratore o [!DNL Workfront Proof] amministratore, puoi assegnare un profilo di autorizzazioni di prova a un utente per specificare le funzionalità di correzione che l’utente avrà per tutte le bozze del sistema. Per informazioni sulla configurazione del profilo di autorizzazione per la bozza di un utente, consulta [Configura il profilo delle autorizzazioni di prova di un utente in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>Puoi anche effettuare le seguenti operazioni:
>
>* Concedi agli utenti ruoli specifici su singole bozze. Per ulteriori informazioni sui ruoli di bozza, consulta [Gestisci ruoli di bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* Crea profili personalizzati per gli utenti della tua organizzazione. Per ulteriori informazioni, consulta [Configurare profili personalizzati in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>


Nella tabella seguente sono visualizzate le autorizzazioni disponibili per ogni profilo di autorizzazioni di prova.

| **Elementi propri** |  |  |  |  | **Altri elementi degli utenti** |  |  | **Amministrazione** | **Fatturazione** |
|---|---|---|---|---|---|---|---|---|---|
|  | **Aggiungi** | **Visualizza** | **Modifica** | **Elimina** | **Visualizza** | **Modifica** | **Elimina** | **Modifica ed Elimina** | **Modifica** |
| Amministratore fatturazione | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |
| Amministrazione | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |
| Supervisore | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |
| Manager | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |   |   |   |
| Osservatore |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |
| Visitatore |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

Considera quanto segue su ruoli e autorizzazioni:

* Le autorizzazioni di profilo assegnate si riferiscono solo agli utenti e agli elementi nel tuo account. L&#39;eccezione è nel caso di account Satellite, dove l&#39;amministratore e l&#39;amministratore di fatturazione per gli account principali (hub) possono accedere e gestire le impostazioni dell&#39;account e la fatturazione di tali account dal livello dell&#39;account hub.
* Gli amministratori di fatturazione e gli amministratori possono eliminare gli utenti. Questa operazione può essere eseguita solo nelle impostazioni account.
* Quando gli amministratori e gli amministratori di fatturazione visualizzano le bozze di proprietà di altri utenti nel proprio account, le visualizzano con il ruolo di un revisore.
* Utilizzando il ruolo di sola lettura, gli amministratori e gli amministratori di fatturazione possono accedere alle bozze nelle cartelle condivise con loro o nelle cartelle create da essi.

Le sezioni seguenti descrivono ogni profilo e le autorizzazioni associate al profilo in uno standard [!DNL Workfront Proof] configurazione:

* [Amministratore fatturazione](#billing-administrator)
* [Amministratore](#administrator)
* [Supervisore](#supervisor)
* [Manager](#manager)
* [Osservatore](#observer)
* [Visitatore](#visitor)
* [Ospite](#guest)

## Amministratore fatturazione {#billing-administrator}

Gli amministratori di fatturazione hanno accesso a [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] Pagina di fatturazione](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)e dispongono delle seguenti autorizzazioni:

![](assets/cleaner2.png)Può generare bozze, caricare file e creare cartelle. Per ulteriori informazioni, consulta [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Caricare file e contenuti web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)e [Crea cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Può visualizzare, modificare ed eliminare le proprie bozze e i propri file creati.

![](assets/cleaner2.png)Può visualizzare, modificare ed eliminare bozze e file creati da tutti gli utenti dell’organizzazione.

![](assets/cleaner2.png)Può eliminare le cartelle pubbliche di altri utenti. Per ulteriori informazioni, consulta [Gestisci cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Dispone dei diritti di modifica su tutte le bozze create nell’account.

![](assets/cleaner2.png)Può essere impostato come proprietario di Dropzone. Per ulteriori informazioni, consulta [Configura la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Può accedere alla pagina di fatturazione e modificare i dettagli di fatturazione. Per ulteriori informazioni, consulta [La [!DNL Workfront Proof] Pagina di fatturazione](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![](assets/cleaner2.png)Può accedere alla pagina Impostazioni account e modificare i dettagli dell&#39;account. Per ulteriori informazioni, consulta [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Posso svuotare la spazzatura. Per ulteriori informazioni, consulta [Ripristina e svuota il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Può aggiungere, modificare ed eliminare utenti.

![](assets/cleaner2.png)Può creare gruppi e aggiungere nuovi contatti.

![](assets/cleaner2.png)Può eliminare i contatti.

![](assets/cleaner2.png)Può modificare le bozze se non sono presenti risposte.

![](assets/no2.png)Impossibile modificare le risposte della bozza.

![](assets/no2.png)Impossibile eliminare le cartelle private di altri utenti. Per ulteriori informazioni, consulta [Gestisci cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

Per informazioni sulle impostazioni dell&#39;account, consulta [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

Per informazioni sulla fatturazione, vedi [La [!DNL Workfront Proof] Pagina di fatturazione](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Amministratore {#administrator}

Gli amministratori hanno accesso a [Impostazioni account](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)e dispongono delle seguenti autorizzazioni:

![](assets/cleaner2.png)Può creare bozze, caricare file e creare cartelle. Per ulteriori informazioni, consulta [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Caricare file e contenuti web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)e [Crea cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Può visualizzare, modificare ed eliminare bozze e file creati.

![](assets/cleaner2.png)Può visualizzare, modificare ed eliminare bozze e file creati da tutti gli utenti dell’organizzazione.

![](assets/cleaner2.png)Può eliminare le cartelle pubbliche di altri utenti. Per ulteriori informazioni, consulta [Gestisci cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Dispone dei diritti di modifica su tutte le bozze create nell’account.

![](assets/cleaner2.png)Può essere impostato come proprietario di Dropzone. Per ulteriori informazioni, consulta [Configura la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Può accedere alla pagina Impostazioni account e modificare i dettagli dell&#39;account. Per ulteriori informazioni, consulta [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Posso svuotare la spazzatura. Per ulteriori informazioni, consulta [Ripristina e svuota il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Può aggiungere, modificare ed eliminare utenti.

![](assets/cleaner2.png)Può creare gruppi e aggiungere nuovi contatti.

![](assets/cleaner2.png)Può eliminare i contatti.

![](assets/cleaner2.png)Può modificare le bozze se non sono presenti risposte.

![](assets/no2.png)Impossibile modificare le risposte della bozza.

![](assets/no2.png)Impossibile eliminare le cartelle private di altri utenti. Per ulteriori informazioni, consulta [Gestisci cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Impossibile accedere alla pagina Fatturazione o modificare i dettagli di fatturazione. Per ulteriori informazioni, consulta [La [!DNL Workfront Proof] Pagina di fatturazione](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Supervisore {#supervisor}

Le autorità di vigilanza dispongono delle seguenti autorizzazioni:

![](assets/cleaner2.png)Può creare bozze, caricare file e creare cartelle. Per ulteriori informazioni, consulta [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Caricare file e contenuti web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)e [Crea cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Può visualizzare, modificare ed eliminare le proprie bozze e i propri file creati.

![](assets/cleaner2.png)Può visualizzare, modificare ed eliminare bozze e file creati da tutti gli utenti dell’organizzazione.

![](assets/cleaner2.png)Può eliminare le cartelle pubbliche di altri utenti. Per ulteriori informazioni, consulta [Gestisci cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Dispone dei diritti di modifica su tutte le bozze create nell’account.

![](assets/cleaner2.png)Può essere impostato come proprietario di Dropzone. Per ulteriori informazioni, consulta [Configura la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Può creare gruppi e aggiungere nuovi contatti.

![](assets/cleaner2.png)Può eliminare i contatti.

![](assets/cleaner2.png)Può modificare le bozze se non sono presenti risposte.

![](assets/no2.png)Impossibile modificare le risposte della bozza.

![](assets/no2.png)Impossibile eliminare le cartelle private di altri utenti. Per ulteriori informazioni, consulta [Cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![](assets/no2.png)Impossibile accedere alla pagina di fatturazione o alle impostazioni dell&#39;account. Per ulteriori informazioni, consulta [La [!DNL Workfront Proof] Pagina di fatturazione](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Impossibile aggiungere, modificare o eliminare utenti.

![](assets/no2.png)Impossibile svuotare il cestino. Per ulteriori informazioni, consulta [Ripristina e svuota il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### Manager {#manager}

I manager dispongono delle seguenti autorizzazioni:

![](assets/cleaner2.png)Può creare bozze, caricare file e creare cartelle. Per ulteriori informazioni, consulta [Genera bozze in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Caricare file e contenuti web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)e [Crea cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Può visualizzare, modificare ed eliminare le proprie bozze e i propri file creati o di proprietà.

![](assets/cleaner2.png)Può visualizzare, esaminare e approvare le bozze di altri utenti che sono esplicitamente condivisi con loro (diritti di sola lettura per tutto ciò che si trova in una cartella condivisa). Per ulteriori informazioni, consulta [Gestisci ruoli di bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Può creare gruppi e aggiungere un nuovo contatto.

![](assets/no2.png)Impossibile visualizzare, modificare o eliminare bozze e file creati da altri utenti dell&#39;organizzazione.

![](assets/no2.png)Impossibile modificare le bozze o le risposte.

![](assets/no2.png)Impossibile eliminare le cartelle private di altri utenti. Per ulteriori informazioni, consulta [Gestisci cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Impossibile eliminare le cartelle pubbliche di altri utenti. Per ulteriori informazioni, consulta [Gestisci cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Impossibile accedere alla pagina di fatturazione o alle impostazioni dell&#39;account. Per ulteriori informazioni, consulta [La [!DNL Workfront Proof] Pagina di fatturazione](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Impossibile impostare come proprietario di Dropzone. Per ulteriori informazioni, consulta [Configura la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Impossibile svuotare il cestino. Per ulteriori informazioni, consulta [Ripristina e svuota il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Impossibile aggiungere, modificare o eliminare utenti.

![](assets/no2.png)Impossibile eliminare i contatti.

### Osservatore {#observer}

Gli osservatori dispongono delle seguenti autorizzazioni:

![](assets/cleaner2.png)Può visualizzare, esaminare e approvare le bozze di altri utenti che sono esplicitamente condivisi con loro (diritti di sola lettura per tutto ciò che si trova in una cartella condivisa). Per ulteriori informazioni, consulta [Gestisci ruoli di bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Può visualizzare i file condivisi in modo esplicito con loro.

![](assets/cleaner2.png) Può visualizzare contatti e gruppi

![](assets/no2.png)Impossibile creare bozze, caricare file e creare cartelle. Per ulteriori informazioni, consulta [Caricare file e contenuti web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Impossibile visualizzare, modificare o eliminare bozze e file creati da altri utenti dell&#39;organizzazione.

![](assets/no2.png)Impossibile modificare le bozze o le risposte.

![](assets/no2.png)Impossibile eliminare gli elementi creati nell&#39;organizzazione.

![](assets/no2.png)Impossibile accedere alla pagina di fatturazione o alle impostazioni dell&#39;account. Per ulteriori informazioni, consulta [La [!DNL Workfront Proof] Pagina di fatturazione](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Impossibile impostare come proprietario di Dropzone. Per ulteriori informazioni, consulta [Configura la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Impossibile svuotare il cestino. Per ulteriori informazioni, consulta [Ripristina e svuota il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Impossibile aggiungere, modificare o eliminare utenti.

![](assets/no2.png)Impossibile creare gruppi o aggiungere nuovi contatti.

![](assets/no2.png)Impossibile eliminare i contatti.

>[!NOTE]
>
>I menu e le funzioni disponibili per gli osservatori sono limitati.
>
>* Gli osservatori non visualizzano il menu Intestazione o il menu Nuovo verde nel dashboard
>* Gli osservatori non vedono i seguenti collegamenti nelle loro impostazioni: Impostazioni account, Fatturazione
>


### Visitatore {#visitor}

I visitatori dispongono delle seguenti autorizzazioni:

![](assets/cleaner2.png)Può visualizzare, esaminare e approvare le bozze di altri utenti che sono esplicitamente condivisi con loro (diritti di sola lettura per tutto ciò che si trova in una cartella condivisa). Per ulteriori informazioni, consulta [Gestisci ruoli di bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Può visualizzare i file condivisi in modo esplicito con loro.

![](assets/no2.png) Impossibile visualizzare contatti e gruppi

![](assets/no2.png)Impossibile creare bozze, caricare file e creare cartelle. Per ulteriori informazioni, consulta [Caricare file e contenuti web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Impossibile visualizzare, modificare o eliminare bozze e file creati da altri utenti dell&#39;organizzazione.

![](assets/no2.png)Impossibile modificare le bozze o le risposte.

![](assets/no2.png)Impossibile eliminare gli elementi creati nell&#39;organizzazione.

![](assets/no2.png)Impossibile accedere alla pagina di fatturazione o alle impostazioni dell&#39;account. Per ulteriori informazioni, consulta [La [!DNL Workfront Proof] Pagina di fatturazione](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) e [Impostazioni account in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Impossibile impostare come proprietario di Dropzone. Per ulteriori informazioni, consulta [Configura la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Impossibile svuotare il cestino. Per ulteriori informazioni, consulta [Ripristina e svuota il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Impossibile aggiungere, modificare o eliminare utenti.

![](assets/no2.png)Impossibile creare gruppi o aggiungere nuovi contatti.

![](assets/no2.png)Impossibile eliminare i contatti.

>[!NOTE]
>
>I menu e le funzioni disponibili per i visitatori sono limitati.
>
>* I visitatori non visualizzano il menu Intestazione o il menu Nuovo verde nel dashboard
>* I visitatori non vedono i seguenti collegamenti nelle loro impostazioni: Impostazioni account, Fatturazione
>


### Ospite {#guest}

Il profilo Guest viene utilizzato per consentire l’accesso alle bozze ai revisori che non dispongono di un proprio account di prova Workfront. Gli ospiti possono accedere alle bozze condivise con loro direttamente tramite le loro notifiche e-mail personali.

![](assets/cleaner2.png)Può visualizzare, rivedere e approvare le bozze condivise in modo esplicito con loro.

![](assets/cleaner2.png)Può visualizzare i file condivisi in modo esplicito con loro.

![](assets/no2.png)Impossibile accedere al dashboard.

![](assets/no2.png)Impossibile condividere con loro cartelle. Per ulteriori informazioni, consulta [Gestisci cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Impossibile aggiungere alle bozze Autori o Moderatori. Per ulteriori informazioni, consulta [Gestisci ruoli di bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>Gli ospiti non sono utenti a prova di Workfront, quindi non possono vedere tutte le bozze condivise con loro nel proprio dashboard.

## Modificare il profilo delle autorizzazioni di prova di un utente

Gli amministratori e gli amministratori di fatturazione possono modificare i profili di autorizzazione di tutti gli utenti dell’account.

1. Per trovare l’utente da modificare, effettua una delle seguenti operazioni:

   * Passa a **[!UICONTROL Impostazioni account]**, quindi fai clic su **[!UICONTROL Utenti]** scheda .

   * Vai a **[!UICONTROL Contatti]** pagina.

1. Fare clic sul nome dell&#39;utente di cui si desidera modificare le autorizzazioni. ![](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. Fai clic sul pulsante **[!UICONTROL Profilo di autorizzazione]** menu a discesa e seleziona un nuovo profilo di autorizzazioni. :

   ![Screenshot_2018-03-30_14-18-03.png](assets/screenshot-2018-03-30-14-18-03a.png)

   I profili di autorizzazione sono Amministratore, Supervisore, Manager e Osservatore.

1. Fai clic in un punto qualsiasi all’esterno del menu per salvare.

>[!NOTE]
>
>Gli amministratori non possono assegnare il profilo Amministratore fatturazione. Puoi trovare un elenco delle modifiche al profilo nei seguenti registri:
>
>* Registri di attività dell’account
>* Registro del profilo dell’utente (accessibile solo a tale utente)
>


Per ulteriori informazioni sui registri attività, consulta [Informazioni sulla [!DNL Workfront Proof] Traccia di audit dell’attività](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
