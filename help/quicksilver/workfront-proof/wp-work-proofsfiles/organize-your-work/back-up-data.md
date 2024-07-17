---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Esegui backup dei dati  [!DNL Workfront Proof]
description: Puoi richiedere un backup di tutti i tuoi dati in [!DNL Workfront Proof] utilizzando la funzione di backup.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 3b831bb5-2d03-4d7e-ad1f-54ae95f05ccd
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# Backup Dei Dati Di [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

## Introduzione ai backup

È possibile richiedere un backup di tutti i dati in [!DNL Workfront Proof] utilizzando la funzione di backup.

Il backup viene consegnato come file .zip. Include un’esportazione XML di tutti i dati (inclusi commenti e risposte per tutte le versioni di tutte le bozze); tuttavia, non include i file originali caricati come bozze.

Ogni file zip di backup creato per il download ha un nome file univoco, ad esempio:

9789_05_05_2011_61703.zip

Il nome del file in questo esempio fornisce le seguenti informazioni:

* 9789 è l&#39;identificatore dell&#39;account [!DNL Workfront Proof]
* 05_05_2011 è la data di creazione, il 5 maggio 2011
* 61703 è un numero assegnato casualmente dal sistema

Questa convenzione di denominazione consente di memorizzare facilmente tutti i file .zip di backup in un&#39;unica posizione sul computer e di sapere esattamente quando ogni backup è stato creato per te.

La funzione [!UICONTROL Backup] consente di decidere come utilizzare le risorse:

* Consente di liberare spazio di archiviazione senza perdere le bozze attive o archiviate. È possibile richiedere un backup, eliminare le bozze, quindi svuotare [Ripristina e Svuotare il cestino in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).
* Consente di accedere a tutti i file caricati originariamente in [!DNL Workfront] Proof. Puoi scaricarli utilizzando la funzione [!UICONTROL scarica file originale] prima di eliminare le bozze.

>[!NOTE]
>
>Quando si utilizzano i backup, tenere presente quanto segue:
>
>* I backup sono disponibili su piani aziendali e illimitati. Contatta il nostro [team vendite](mailto:sales@proofhq.com) per un preventivo.
>* Il tipo di codifica dei dati è impostato su UTF-8 per impostazione predefinita. Si consiglia questa impostazione. Si tratta del tipo di codifica più comunemente utilizzato dalle applicazioni Internet.
>* È possibile richiedere un solo [!DNL backup] alla volta. Durante l&#39;elaborazione del file zip di backup, il collegamento Richiedi nuovo backup nella scheda Backup non viene visualizzato e il messaggio visualizzato rimane invariato. Per informazioni sulla richiesta di un backup, vedere [Richiedere un nuovo backup dei dati in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/request-new-data-backup-in-wp.md).
>



## Backup dei dati

1. Fare clic su **[!UICONTROL Impostazioni account]** nell&#39;angolo superiore destro dell&#39;interfaccia [!DNL Workfront Proof]. 1)
1. Fare clic sulla scheda **[!UICONTROL Backup]**. 2)
1. Fai clic sul collegamento **[!UICONTROL Richiedi nuovo backup]** (3)

Quando il backup è pronto, si verifica quanto segue:

* Ricevi un&#39;e-mail da [!DNL Workfront Proof] con la notifica di questo (il backup di [!DNL Workfront Proof] è pronto). L’e-mail contiene un collegamento per il download dei dati di backup.
* Nella scheda Backup di [Impostazioni account](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) viene visualizzato un collegamento di download per i dati di backup.
* Il collegamento Richiedi nuovo backup (3) viene nuovamente visualizzato nella scheda Backup

I dati saranno pronti per essere scaricati come file zip. Puoi scaricare il file .zip di backup dall&#39;e-mail di notifica o dalle [!UICONTROL impostazioni account], come descritto nelle sezioni seguenti:

* [Download del file .zip di backup dalla notifica e-mail](#downloading-your-backup-zip-file-from-your-email-notification)
* [Download del file .zip di backup dalle impostazioni dell’account](#downloading-your-backup-zip-file-from-the-account-settings)

![Request_Backup.png](assets/request-backup-350x167.png)

## Download del file .zip di backup dalla notifica e-mail {#downloading-your-backup-zip-file-from-your-email-notification}

Quando il file zip di backup è pronto per il download, si riceve un&#39;e-mail da [!DNL Workfront Proof] con l&#39;oggetto &#39;Il backup di [!DNL Workfront Proof] è pronto.&#39;

Per scaricare il file .zip di backup dall’e-mail:

1. Fai clic sul collegamento di download nell’e-mail.\
   ![Posta_backup.png](assets/backup-mail-350x120.png)\
   Se non si è al momento connessi a [!DNL Workfront Proof], viene visualizzata una nuova finestra del browser e viene visualizzata la pagina di accesso.

## Download del file .zip di backup dalle impostazioni dell’account {#downloading-your-backup-zip-file-from-the-account-settings}

Quando il file .zip di backup è pronto per il download, la scheda [!UICONTROL Backup] lo indica visualizzando un collegamento per il download. Inoltre, viene nuovamente visualizzato il collegamento [!UICONTROL Richiedi nuovo backup].

1. Fare clic su **[!UICONTROL Impostazioni account]** nell&#39;angolo superiore destro dell&#39;interfaccia [!DNL Workfront Proof]. 1)
1. Fare clic sulla scheda **[!UICONTROL Backup]**. 2)\
   Se nessun utente dell&#39;account ha richiesto backup, la scheda [!UICONTROL Backup] indica che non sono presenti backup. Se un utente ha richiesto un backup, nella scheda viene visualizzata la data di creazione e il collegamento per il download dell’ultimo backup.

1. Fai clic sul collegamento **[!UICONTROL Scarica backup]**. 3)\
   ![Download_Backup.png](assets/download-backup-350x167.png) Viene visualizzata una schermata di download dei file in cui viene richiesto se si desidera aprire o salvare il file di download.

1. Fai clic su **[!UICONTROL Salva]**, quindi seleziona il percorso nel computer in cui desideri salvare il file .zip di backup.\
   Il messaggio che identifica la data del backup più recente rimane visualizzato nella parte inferiore della pagina [!UICONTROL Backup] fino alla successiva richiesta di backup. Il collegamento Scarica backup si applica all&#39;ultimo backup. Ogni volta che viene visualizzato il collegamento [!UICONTROL Richiedi nuovo backup], è possibile fare clic su di esso per richiedere un altro backup.

## Informazioni sui file nel file zip di backup

Il file .zip di backup contiene sette file CSV (valori separati da virgole o delimitati da virgole) che includono informazioni dalle bozze attive e archiviate fino al momento del backup dei dati:

* comments.csv - include commenti sulle bozze
* comment_reply.csv - include le risposte ai commenti sulle bozze organization.csv - include l’identificatore numerico e il nome della tua organizzazione (il tuo account)
* contacts.csv - include l&#39;identificatore numerico, il nome e l&#39;organizzazione per ogni contatto
* files.csv - include informazioni dalla pagina Dettagli bozza o Dettagli file sulle bozze o sui file caricati in [!DNL Workfront Proof]
* recipients.csv: include l&#39;identificatore numerico, il ruolo e le decisioni di ogni persona specificata come revisore, revisore e approvatore, ecc., quando le bozze vengono caricate per la revisione il [!DNL Workfront Proof]
* users.csv - include identificatori numerici e nomi di tutti gli utenti nell’account

Puoi estrarre questi file dal file .zip di backup con qualsiasi utilità zip utilizzata, quindi memorizzarli nel percorso desiderato sul computer. Dopo aver salvato il file zip ed estratto i singoli file CSV, puoi manipolare le informazioni come desideri per la conservazione dei record interni.

Ogni file .zip di backup creato su richiesta ha un nome distinto che include la data di creazione del backup, ma i file CSV inclusi in ciascun file .zip di backup hanno sempre gli stessi nomi. È possibile utilizzare uno dei metodi seguenti per garantire che i file di backup siano distinti l&#39;uno dall&#39;altro:

* Crea una nuova cartella per ogni file zip di backup e i file CSV estratti.
* Rinomina ogni singolo file CSV per includere la data di backup quando lo estrai dal file zip.

>[!NOTE]
>
>Se [!DNL Microsoft Excel] è installato nel computer, l&#39;utility di estrazione potrebbe elencare il tipo di file per i singoli file CSV come [!DNL Microsoft Office Excel] file con valori separati da virgola. È possibile aprire un file CSV estratto utilizzando [!DNL Excel] e salvare il file come cartella di lavoro [!DNL Excel] (&#42;.xlsx) o come altro tipo di file.
