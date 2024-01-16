---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: Gestire i ruoli bozza in [!DNL Workfront Proof]
description: I ruoli di bozza ti consentono di concedere autorizzazioni agli utenti limitati dal profilo di autorizzazione configurato nel loro profilo utente.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 6e24b9c717ecedd6efbdf62ec01e53ac98079cfe
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 0%

---

# Gestire i ruoli bozza in [!DNL Workfront Proof]

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità del prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Bozza](../../../review-and-approve-work/proofing/proofing.md).

I ruoli di bozza ti consentono di concedere autorizzazioni agli utenti limitati dal profilo di autorizzazione configurato nel loro profilo utente. (Per ulteriori informazioni sui profili di autorizzazione, consulta [Profili delle autorizzazioni di bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

I ruoli della bozza sono diversi dai profili dell’account. Il profilo dell’account si riferisce al livello di autorizzazione complessivo disponibile nel tuo account e influirà sui diritti di cui disponi su tutte le bozze nel tuo account, anche quelle che non sono state esplicitamente condivise con te.

Per ulteriori informazioni, consulta [Profili delle autorizzazioni di bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Informazioni sui ruoli delle bozze

Al momento in cui l’utente viene invitato a rivedere la bozza, vengono concessi agli utenti i seguenti ruoli di bozza per una singola bozza:

* [Sola lettura](#read-only)
* [Revisore](#reviewer)
* [Approvatore](#approver)
* [Revisore e Approvatore](#reviewer-approver)
* [Autore](#author)
* [Moderatore](#moderator)

Il ruolo bozza definisce le azioni che un revisore può intraprendere in relazione a tale bozza specifica.

Ad esempio, se sei un revisore, ti viene chiesto di rivedere la bozza aggiungendo markup e commenti. Se sei un revisore e un approvatore, ti viene chiesto di rivedere e anche di prendere una decisione sulla bozza.

Alcuni ruoli bozza assegnano ai revisori i diritti di modifica sulla bozza (anche se il loro profilo account non lo prevede) e consentono di utilizzare alcune funzioni aggiuntive, come l’aggiunta di azioni sui commenti, la creazione di nuove versioni e l’aggiunta di più revisori alla bozza.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Utilizzare le azioni sui commenti della bozza](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [Condividere una bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### Sola lettura

{#read-only}

![cleaner.png](assets/cleaner.png) Può visualizzare una bozza

![no.png](assets/no.png) Impossibile aggiungere markup

![no.png](assets/no.png) Impossibile aggiungere commenti

![no.png](assets/no.png) Impossibile prendere una decisione

![no.png](assets/no.png) Impossibile eliminare i commenti aggiunti da altri

![no.png](assets/no.png) Non dispone dei diritti di modifica sulla bozza

>[!NOTE]
>
>Se una cartella è condivisa con un utente di [!DNL Workfront Proof], gli verranno automaticamente assegnati diritti di sola lettura per tutti gli elementi esistenti e aggiunti successivamente nella cartella.

Per ulteriori informazioni, consulta [Condividere cartelle in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### Revisore {#reviewer}

![cleaner.png](assets/cleaner.png) Può visualizzare una bozza

![cleaner.png](assets/cleaner.png) Può aggiungere markup

![cleaner.png](assets/cleaner.png) Può aggiungere commenti

![[!DNL cleaner].png](assets/cleaner.png) Può modificare i propri commenti in assenza di risposte

![no.png](assets/no.png) Impossibile prendere una decisione

![no.png](assets/no.png) Impossibile modificare o eliminare i commenti aggiunti da altri utenti

![no.png](assets/no.png) Non dispone dei diritti di modifica sulla bozza

### Approvatore {#approver}

![cleaner.png](assets/cleaner.png) Può visualizzare una bozza

![cleaner.png](assets/cleaner.png) Può prendere una decisione

![no.png](assets/no.png) Impossibile aggiungere markup

![no.png](assets/no.png) Impossibile aggiungere commenti

![no.png](assets/no.png) Impossibile modificare o eliminare i commenti aggiunti da altri utenti

![no.png](assets/no.png) Non dispone dei diritti di modifica sulla bozza

### Revisore e Approvatore {#reviewer-approver}

![cleaner.png](assets/cleaner.png) Può visualizzare una bozza

![cleaner.png](assets/cleaner.png) Può aggiungere markup

![cleaner.png](assets/cleaner.png) Può aggiungere commenti

![[!DNL cleaner].png](assets/cleaner.png) Può modificare i propri commenti in assenza di risposte

![cleaner.png](assets/cleaner.png) Può prendere una decisione

![no.png](assets/no.png) Impossibile modificare o eliminare i commenti aggiunti da altri utenti

![no.png](assets/no.png) Non dispone dei diritti di modifica sulla bozza

### Autore {#author}

![cleaner.png](assets/cleaner.png) Può aggiungere markup

![cleaner.png](assets/cleaner.png) Può aggiungere commenti

![[!DNL cleaner].png](assets/cleaner.png) Può modificare i propri commenti in assenza di risposte

![cleaner.png](assets/cleaner.png) Può prendere una decisione

![cleaner.png](assets/cleaner.png) Può inviare nuove versioni

![cleaner.png](assets/cleaner.png) Può creare una copia della bozza

![cleaner.png](assets/cleaner.png) Può condividere la bozza con altre persone

![cleaner.png](assets/cleaner.png) Può applicare azioni ai commenti

![cleaner.png](assets/cleaner.png) Può risolvere i commenti

![no.png](assets/no.png) Impossibile modificare o eliminare i commenti aggiunti da altri utenti

>[!NOTE]
>
>Questo ruolo può essere assegnato solo agli utenti di [!DNL Workfront Proof].

### Moderatore {#moderator}

![cleaner.png](assets/cleaner.png) Può aggiungere markup

![cleaner.png](assets/cleaner.png) Può aggiungere commenti

![[!DNL cleaner].png](assets/cleaner.png) Può modificare i propri commenti in assenza di risposte

![cleaner.png](assets/cleaner.png) Può prendere una decisione

![cleaner.png](assets/cleaner.png) Può inviare nuove versioni

![cleaner.png](assets/cleaner.png) Può aggiungere nuovi revisori

![cleaner.png](assets/cleaner.png) Può applicare azioni ai commenti

![cleaner.png](assets/cleaner.png) Può risolvere i commenti

![cleaner.png](assets/cleaner.png) È possibile eliminare i commenti e le risposte sulla bozza (create da se stessi o da altri)

* Se si elimina il primo commento in un thread di commenti, verrà eliminato l&#39;intero thread
* Se si eliminano le risposte nel thread di commenti, verrà eliminata solo la risposta

![no.png](assets/no.png) Impossibile modificare i commenti aggiunti da altri

Questo ruolo consente all’utente di gestire e moderare i commenti della bozza, offrendo l’opportunità di mantenere solo i commenti rilevanti sulla bozza e di rimuovere i commenti non rilevanti.

>[!NOTE]
>
>Questo ruolo può essere assegnato solo agli utenti di [!DNL Workfront Proof].

## Assegnazione di ruoli bozza

È possibile assegnare ruoli di bozza durante la creazione di nuove bozze, la creazione di nuove versioni di bozze esistenti o su bozze esistenti.

### Nuove bozze {#new-proofs}

I ruoli delle bozze possono essere assegnati ai revisori sulla [!UICONTROL Nuova bozza] durante il processo di creazione della bozza (1).

![Proof_roles_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### Nuove versioni {#new-versions}

Quando si crea una nuova versione di una bozza, vengono visualizzati automaticamente i revisori della versione precedente (con lo stesso ruolo della versione precedente).

Puoi modificare i ruoli della bozza applicati ai revisori durante la creazione della nuova versione (1).

![Proof_roles_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### Bozze esistenti {#existing-proofs}

Se desideri modificare il ruolo di una persona su una bozza esistente, puoi farlo su [!UICONTROL Dettagli bozza] pagina modificando in linea il loro ruolo nella sezione flusso di lavoro (1).

![Proof_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## Controllo dei ruoli nel visualizzatore bozze

Puoi controllare il ruolo di un revisore direttamente dal Visualizzatore bozze (1) e modificarlo (2), se necessario.

![Proof_roles_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## Ruoli bozza predefiniti

Puoi impostare il tuo ruolo di bozza predefinito su [!DNL Proofing Defaults] nelle impostazioni personali. Ciò significa che quando si viene aggiunti a una bozza, il ruolo di bozza predefinito viene popolato automaticamente. Tieni presente che questo ruolo può essere modificato a livello di bozza da un utente con diritti di modifica su una bozza.

>[!NOTE]
>
>Solo gli utenti con i profili Amministratore o Amministratore fatturazione possono modificare le impostazioni predefinite di verifica per altri utenti nel proprio account.

Per ulteriori informazioni, consulta [Impostazioni personali in [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## Creatori e proprietari

Creatori e proprietari dispongono di diritti di modifica completi sulla bozza.

### Creatori {#creators}

Il creatore della bozza è la persona che carica la bozza nella prima istanza. Il creatore della bozza verrà visualizzato automaticamente nell’elenco persone per la bozza (nel suo ruolo predefinito).

Il giorno [!UICONTROL Nuova bozza] pagina è possibile assegnare un ruolo di bozza diverso al creatore della bozza (diverso dal ruolo predefinito).

Impossibile modificare o rimuovere da una bozza il creatore della bozza.

### Proprietari {#owners}

Per impostazione predefinita, il Creatore è anche il Proprietario della bozza; tuttavia, il Creatore può rendere qualcun altro il Proprietario della bozza durante la creazione iniziale della bozza (sulla [!UICONTROL Nuova bozza] page).

Per cambiare il proprietario nella pagina Nuova bozza:

1. Fare clic sul collegamento di modifica visualizzato accanto al nome del creatore.
1. Seleziona il nuovo Proprietario dal menu a discesa. 2)

![Proof_roles_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

Una volta creata la bozza, è ancora possibile cambiare il proprietario. Chiunque disponga dei diritti di modifica sulla bozza sarà in grado di cambiarne la proprietà a un altro utente tramite [!UICONTROL Dettagli bozza] (vedi sotto).

La possibilità di cambiare il proprietario di una bozza è particolarmente utile dal punto di vista della gestione del flusso di lavoro. Consente alla persona responsabile del progetto di acquisire la proprietà delle bozze, fornendo i diritti di modifica sulle bozze e la possibilità di visualizzarle in [!UICONTROL Le mie bozze] visualizzazione.

Per cambiare il proprietario della bozza tramite [!UICONTROL Dettagli bozza] pagina:

* Fare clic sul menu Azioni accanto al nome della persona che si desidera impostare come Proprietario.
* Seleziona [!UICONTROL **Rendi proprietario**] dal menu a discesa.
* In alternativa, è possibile fare clic su nella [!UICONTROL **Proprietario**] accanto all’immagine della bozza e scegli il nuovo Proprietario dall’elenco a discesa visualizzato.

Al termine dell’operazione, accanto al nome della persona viene visualizzata la parola &quot;Proprietario&quot;.

>[!NOTE]
>
>Solo un utente dello stesso account o un account partner può essere reso proprietario di una bozza. Un utente in un account partner può diventare proprietario di una bozza solo quando:
>
>* Esiste una relazione partner esistente impostata tra gli account. Per ulteriori informazioni, consulta [Account partner in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* Non sono presenti campi personalizzati nel [!UICONTROL Nuova bozza] pagina.
>* La bozza non è stata assegnata a una cartella.
>* Nessun tag applicato alla bozza.

Per delegare temporaneamente la proprietà della bozza in [!DNL Workfront Proof], vedi [Designazione di proprietari bozza temporanei in [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
