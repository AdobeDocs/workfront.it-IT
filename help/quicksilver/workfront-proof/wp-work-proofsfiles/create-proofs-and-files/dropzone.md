---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: create-proofs-and-files
title: Zona di rilascio
description: Se disponi del piano Enterprise, puoi utilizzare Dropzone per inviare nuove bozze e nuove versioni di bozze al tuo account senza dover accedere al tuo account.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e66142fa-3b0d-4821-9aa5-040c62f00d62
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 0%

---

# Zona di rilascio

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Se disponi del piano Enterprise, puoi utilizzare Dropzone per inviare nuove bozze e nuove versioni di bozze al tuo account senza dover accedere al tuo account.

Quando invii una bozza tramite Dropzone, questa viene visualizzata nella pagina Dropzone nel tuo [!DNL Workfront Proof] conto. Da qui puoi instradarlo nel flusso di lavoro.

## Invio di una nuova bozza tramite l’URL Dropzone

1. Nel browser, passa all’URL univoco di Dropzone , come descritto in [Configura la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. Immetti l&#39;indirizzo e-mail.
1. Fai clic su **[!UICONTROL Selezionare un file]** o **[!UICONTROL Acquisire una pagina web]** e scegli il file o la pagina web da caricare.

1. Immetti il codice di sicurezza, quindi fai clic su **[!UICONTROL Successivo]**.\
   Una barra di avanzamento mostra l’avanzamento del caricamento.\
   Nella schermata successiva, potrai aggiungere i dettagli di bozza.\
   Questa sezione viene visualizzata solo se è stata abilitata nelle impostazioni di Dropzone.

1. Dopo aver compilato i dettagli, fai clic su **[!UICONTROL Successivo]**.
1. Tutti i revisori aggiunti alla bozza riceveranno il proprio messaggio e-mail di notifica solo dopo l’attivazione della bozza (vedi di seguito).
1. Dopo l’invio della bozza a Dropzone, la bozza attraversa i seguenti stati:

   * Quando carichi un file nella zona di rilascio, la bozza viene visualizzata come bozza.
   * Una volta completato l’invio, la bozza viene visualizzata nella zona di rilascio come Inviata.
   * Una volta che la bozza è stata attivata e sbloccata, viene visualizzata nella tua zona di rilascio come attiva.
   * Se la bozza è bloccata, viene visualizzata nella tua zona di rilascio come bloccata.

## Invio di una nuova versione di una bozza esistente tramite l’URL Dropzone

1. Nel browser, passa all’URL univoco di Dropzone , come descritto in [Configura la zona di rilascio in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. Immetti l&#39;indirizzo e-mail.
1. Seleziona la casella di controllo per indicare che stai caricando una nuova versione di una bozza esistente.\
   Per informazioni sulla creazione di una nuova versione di una bozza, consulta .
1. Fai clic su **[!UICONTROL Selezionare un file]** o **[!UICONTROL Acquisire una pagina web]** e scegli il file o la pagina web da caricare.

1. Immetti il codice di sicurezza, quindi fai clic su **[!UICONTROL Successivo]**.\
   Una barra di avanzamento mostra l’avanzamento del caricamento.\
   Workfront Proof invia un’e-mail di convalida.

1. Fai clic sul collegamento nell’e-mail.\
   L’e-mail apre la finestra Dropzone nel browser. Il collegamento nella notifica e-mail è valido per 24 ore.
1. Seleziona la versione precedente della bozza (verranno visualizzate solo le bozze create/inviate).\
   Nella schermata successiva sarà possibile aggiungere i dettagli della bozza.\
   Questa sezione viene visualizzata solo se è stata abilitata nelle impostazioni di Dropzone.

1. Digita i dettagli e fai clic su **[!UICONTROL Successivo]**.

   >[!NOTE]
   >
   >Tutti i revisori aggiunti alla bozza riceveranno il proprio messaggio e-mail di notifica solo dopo l’attivazione della bozza (vedi di seguito).

   Dopo l’invio della bozza a Dropzone, la bozza attraversa i seguenti stati:

   * Quando carichi un file nella zona di rilascio, la bozza viene visualizzata come bozza.
   * Una volta completato l’invio, la bozza viene visualizzata nella zona di rilascio come Inviata.
   * Una volta che la bozza è stata attivata e sbloccata, viene visualizzata nella tua zona di rilascio come attiva.
   * Se la bozza è bloccata, viene visualizzata nella tua zona di rilascio come bloccata.

## Inviare una bozza a Dropzone

>[!NOTE]
>
>L’invio di una bozza alla zona di rilascio non è più supportato.


## Completamento dell’invio

Workfront ti invia (il mittente) un messaggio e-mail di invio completo che ti chiede di confermare se il file è una nuova bozza o una nuova versione. Il collegamento nella notifica e-mail è valido per 24 ore.

1. Fai clic sul collegamento e segui i passaggi indicati sopra, a seconda che si tratti di una nuova bozza o di una nuova versione di una bozza esistente.

## Attivazione della bozza

Il proprietario di Dropzone riceve un messaggio e-mail di notifica per informare che è stata inviata una nuova bozza a Dropzone:

* La bozza viene visualizzata nella pagina Dropzone del tuo account (per accedere alla pagina Dropzone , fai clic sul collegamento nella barra laterale di navigazione a sinistra).
* La bozza è accessibile dal proprietario di Dropzone (o da un utente con almeno un profilo di supervisore). Il proprietario può essere modificato nelle impostazioni di Dropzone (solo un amministratore di fatturazione o un amministratore può farlo).
* Prima che la prova possa essere elaborata, deve essere attivata/sbloccata dal proprietario del Dropzone (un utente con almeno un profilo di supervisore può farlo). Lo stato della bozza viene visualizzato come Inviato fino a quando non è stata attivata/sbloccata.

Per attivare la bozza:

1. Vai al menu a discesa a destra della bozza e fai clic su **[!UICONTROL Attiva]**.
1. Una volta attivata o sbloccata la bozza:

   * Lo stato della bozza diventa Attivo.
   * Tutte le persone aggiunte alla bozza riceveranno un’e-mail di notifica per informare che dispongono di una nuova bozza da esaminare. (Nessun messaggio e-mail viene inviato finché la bozza non è stata attivata o sbloccata.)
   * La prova può essere lavorata come normale
   * Se anche il mittente si aggiunge esplicitamente alla bozza, non riceverà un&#39;e-mail di nuova bozza. Per ulteriori informazioni, consulta [Nuova e-mail a prova di](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

## Gestione della zona di rilascio

La pagina Dropzone facilita la gestione degli invii al tuo Dropzone. La pagina Dropzone include le seguenti opzioni e funzionalità:

* Layout pagina (1)
* Scegliere di includere/escludere le bozze archiviate nella visualizzazione (2)
* Pulsanti di azione (3)
* Ordina (4)
* Filtro (5)
* Menu Azioni bozza (6)
* Annulla archiviazione della bozza (7)
* Riepilogo espandi/comprimi bozza (8)
* Selezionare una bozza (9)

Le opzioni di layout e ordinamento e filtro della pagina sono le stesse di [!DNL Views] elenchi. Vedi [Gestire gli elementi nella pagina Visualizzazioni in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) per ulteriori informazioni.

![New_Dropzone_design_Feb_2013_.jpg](assets/new-dropzone-design--feb-2013--350x224.jpg)
