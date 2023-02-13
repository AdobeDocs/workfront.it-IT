---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: Domande frequenti - Creazione e condivisione di bozze e file
description: Una bozza è un file statico, audio o video che può essere rivisto nel visualizzatore di correzione. I revisori aggiunti a una bozza dispongono di un set di strumenti a loro disposizione per commentare e prendere decisioni sulla bozza.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb0eb160-4bcf-4bc1-ad13-df19f692bef6
source-git-commit: d5ffd576fcedf9b10dce5e5d5bd9245dd7f67ef8
workflow-type: tm+mt
source-wordcount: '1365'
ht-degree: 0%

---

# Domande frequenti - Creazione e condivisione di bozze e file

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

## Qual è una prova?

### Risposta

Una bozza è un file statico, audio o video che può essere rivisto nel visualizzatore di correzione. I revisori aggiunti a una bozza dispongono di un set di strumenti a loro disposizione per commentare e prendere decisioni sulla bozza.

## Quali tipi di file sono supportati?

### Risposta

Le bozze possono essere create da file statici, audio e video. Non puoi caricare file di dimensioni superiori a 4 GB. [!DNL Workfront] supporta più di 150 tipi di file (vedi [Panoramica sui tipi di file di correzione supportati e sui limiti di dimensione](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md) per un elenco completo).

## Qual è la differenza tra una bozza e un file?

### Risposta

Quando carichi un file in [!DNL Workfront Proof], il sistema memorizza il file nel [!DNL Workfront Proof] conto. Quando lo condividi, [!DNL Workfront Proof] invia un messaggio e-mail ai destinatari con un collegamento che possono fare clic per scaricare il file. Puoi condividere qualsiasi tipo di file.

Quando crei una bozza da un file caricato in [!DNL Workfront Proof], puoi rendere il file disponibile per la revisione nel visualizzatore di correzione. I revisori ricevono un’e-mail con un collegamento alla bozza. Quando aprono la bozza, visualizzano l’immagine della bozza, possono aggiungere commenti e prendere decisioni al riguardo. Puoi creare bozze utilizzando i file dell’elenco dei tipi di file supportati. Puoi anche creare bozze utilizzando gli URL per siti web e altri contenuti web.

Per un elenco completo dei tipi di file supportati, vedi [Panoramica sui tipi di file di correzione supportati e sui limiti di dimensione](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

## Come si crea una bozza?

### Risposta

Puoi creare bozze da file statici, file audio, file video e URL (vedi ).

Per creare una bozza nell’account, devi essere un utente con il profilo di autorizzazione appropriato (consulta [[!UICONTROL Profili delle autorizzazioni di prova] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

Se carichi più file contemporaneamente, puoi creare più bozze da inviare allo stesso gruppo di revisori utilizzando un’e-mail. Se la tua organizzazione dispone di un [!UICONTROL Enterprise] o [!UICONTROL Senza limiti] è possibile combinare i file in una singola bozza (consulta [Creare una bozza a più pagine](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)).

## Cosa sono i ruoli di bozza e gli avvisi e-mail?

### Risposta

I ruoli di bozza definiscono le azioni che un revisore deve intraprendere su una bozza. È possibile utilizzare opzioni di ruolo diverse per i revisori quando si crea una bozza, a seconda che si desideri che possano creare commenti, prendere decisioni e così via. Per ulteriori informazioni, consulta [Gestisci ruoli di bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

Gli avvisi e-mail aggiornano i revisori sui progressi di una bozza (sono diversi dalle nuove notifiche di bozza e di bozza). È possibile selezionare diverse opzioni per diversi revisori, a seconda del ruolo di ciascun revisore sulla bozza. Per ulteriori informazioni, consulta [Crea una bozza avanzata con un [!UICONTROL Flusso di lavoro automatizzato]](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Posso creare una bozza da più file?

### Risposta

La combinazione di più file in un’unica bozza è una funzione disponibile in [!UICONTROL Enterprise] e [!UICONTROL Senza limiti] piani di edizione. Questa opzione è possibile solo per i file statici, non per i file video. Per ulteriori informazioni, consulta  [Creare una bozza a più pagine](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Posso creare bozze dagli URL?

### Risposta

Sì, è possibile creare bozze da siti web e altri contenuti web. Quando aggiungi un URL per creare una bozza, puoi specificare se desideri una bozza statica o interattiva:

* In una bozza interattiva, i revisori possono navigare e interagire come di consueto con il sito web o altri contenuti web, ad esempio annunci in streaming video o audio, [!DNL Flash] elementi in un annuncio, animazioni HTML e banner interattivi. Per ulteriori informazioni, consulta [Creare una bozza per il contenuto interattivo in un file ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).
* Per una prova statica, [!DNL Workfront] esegue una serie di schermate delle pagine e delle sottopagine specificate. I collegamenti ipertestuali sono attivi nella bozza, quindi puoi verificare se portano o meno alla destinazione corretta. Per ulteriori informazioni, consulta [Creare una bozza statica per un sito web o altro contenuto web](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-static-proof-website-other-web-content.md).

Puoi aggiungere più URL contemporaneamente se li separi con uno spazio. La combinazione è disponibile solo in [!UICONTROL Enterprise] e [!UICONTROL Senza limiti] piani di edizione.

## Le persone che non dispongono di un accesso possono creare delle bozze nel mio account?

### Risposta

Per creare le bozze direttamente in una [!DNL Workfront Proof] conto.

## Cosa significa condividere una bozza?

### Risposta

La condivisione di una bozza consente ai revisori di accedervi in modo che possano aggiungere commenti e contrassegni e prendere decisioni al riguardo. I revisori degli ospiti accedono alle bozze dalla notifica e-mail che ricevono. Revisori con i propri [!DNL Workfront Proof] l&#39;account può accedere alle bozze [!UICONTROL Dashboard].

## Come posso condividere una prova?

### Risposta

Quando crei una bozza, puoi aggiungere revisori nel [!UICONTROL Flusso di lavoro] della sezione [!UICONTROL Nuova bozza] pagina. Quando la prova è pronta, [!DNL Workfront Proof] invia un’e-mail ai revisori contenente un collegamento alla bozza.

Se disponi di diritti sufficienti su una bozza, puoi utilizzare il visualizzatore di correzione, il tuo [!UICONTROL Dashboard]o una delle viste elenco per aggiungere revisori a una bozza esistente (consulta [Condividi una bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) and [Manage Items on the [!UICONTROL Views] Ingresso pagina [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

L’aggiunta di revisori è il modo più comune per condividere le bozze. Per scoprire altre opzioni disponibili, consulta:

* [Condividere collegamenti a bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof-links.md)
* [Condividi l’URL pubblico in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md)
* [Iscriviti a una bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)
* [Crea una prova Mini in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/create-mini-proof.md)

## È necessario essere un utente per esaminare una bozza?

### Risposta

No. Recensori ospiti (persone senza [!DNL Workfront Proof] credenziali di accesso) può accedere a una bozza dalla notifica e-mail di prova che ricevono. Puoi condividere una prova con tutti gli ospiti che desideri.

È possibile limitare la condivisione di bozze alle persone con [!DNL Workfront Proof] credenziali di accesso. Questo aggiunge un altro livello di sicurezza alle bozze. Per una maggiore sicurezza, gli amministratori di sistema di [!UICONTROL Enterprise] e [!UICONTROL Senza limiti] i piani possono configurare questo requisito per tutte le bozze create nell’organizzazione.

Per ulteriori informazioni sulla richiesta di accesso, consulta [Prova di sicurezza in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/proof-security-in-workfront-proof.md).

Se l&#39;organizzazione richiede ai revisori di firmare le bozze elettronicamente, il che richiede l&#39;accesso [!DNL Workfront Proof], gli utenti possono condividere le bozze solo con gli utenti registrati. Disponibile il [!UICONTROL Enterprise] e [!UICONTROL Senza limiti] piani di edizione. Per ulteriori informazioni, consulta [Informazioni sulle firme elettroniche in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md).

## Posso impostare una scadenza per i miei revisori?

### Risposta

Quando crei la bozza, puoi impostare una scadenza per una nuova bozza o una nuova versione di prova. Lo fai nel [!UICONTROL Flusso di lavoro] della sezione [!UICONTROL Nuova bozza] pagina. Se utilizzi [!UICONTROL Flusso di lavoro automatizzato], puoi impostare una scadenza diversa per ogni fase della revisione.

È inoltre possibile impostare o aggiornare una scadenza per una bozza esistente utilizzando [!UICONTROL Dettagli bozza] pagina. Per ulteriori informazioni, consulta [Gestisci dettagli bozza in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

## Come posso creare una nuova versione della bozza?

### Risposta

I revisori spesso richiedono modifiche nei loro commenti su una bozza e desiderano vedere una nuova versione della bozza. Puoi creare nuove versioni di una bozza. [!DNL Workfront Proof] ricorda le impostazioni della bozza della versione precedente. È comunque possibile modificare queste impostazioni se è necessario eseguire un&#39;operazione come l&#39;aggiunta o la rimozione di revisori per la bozza.

Devi condividere ogni versione con i revisori specifici che devono visualizzarla. Ad esempio, se condividi solo la versione 3 con un revisore, tale persona non può vedere le versioni 1 e 2. I supervisori e gli amministratori nel tuo account sovrascrivono tutti i progetti nell’account, in modo che possano vedere e modificare tutte le versioni della bozza.

Per ulteriori informazioni, consulta .

## Posso condividere file utilizzando [!DNL Workfront Proof]?

### Risposta

Sì. Se desideri condividere qualcosa con altre persone, ma non è necessario che le visualizzino come bozza (o se si tratta di un tipo di file non supportato da [!DNL Workfront Proof]), puoi caricarla come file nella tua [!DNL Workfront Proof] conto. Come per le bozze, puoi organizzare i file in cartelle, assegnare tag ai file e aggiungere un messaggio personalizzato all’e-mail di notifica quando condividi il file. Per ulteriori informazioni, consulta [Caricare file e contenuti web in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

Quando i destinatari ricevono la notifica e-mail relativa a un file che stai condividendo, possono scaricare il file facendo clic sul collegamento presente nella notifica.

[!DNL Workfront Proof] gli utenti possono convertire i file in bozze dopo averli salvati nel loro account.

<!--Is there a limit-->
