---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
title: La [!DNL Workfront] Pagina di fatturazione delle prove
description: Per accedere al [!UICONTROL Fatturazione] aprire il menu Impostazioni in alto a destra dello schermo e scegliere Fatturazione dal menu a discesa.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f3828671-e950-4649-9f6d-881101100a96
source-git-commit: 1312e3d5256f28ca0197c73a6c06016d6d7c7e2a
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# La [!DNL Workfront Proof] Pagina di fatturazione

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

## Pagina di fatturazione

Per accedere al [!UICONTROL Fatturazione] aprire **[!UICONTROL Impostazioni]** in alto a destra dello schermo e scegli **[!UICONTROL Fatturazione]** nel menu a discesa .

La [!UICONTROL Fatturazione] La pagina contiene quanto segue:

* Nome account (1)
* Elenco degli account (ad esempio se si dispone di account Satellite)(2)
* Piano di modifica (3)
* Modificare i dati di pagamento (4)
* Nuovo conto satellitare (5)
* Chiudi conto (6)
* Informazioni sul piano attuale (7)
* Contatto di fatturazione e indirizzo (8)
* Statistiche di utilizzo (9)
* Storico di fatturazione (10)
* Attività di fatturazione (11)

   ![Billing_page.jpg](assets/billing-page-350x315.jpg)

## [!UICONTROL Piano corrente]

Questa sezione (7) mostra i dettagli del piano corrente, compresi i seguenti elementi:

* Nome del piano
* Metodo di pagamento corrente
* Date di inizio e fine del piano corrente
* Tipo di piano successivo
* Metodo di pagamento del piano successivo

   Per ulteriori informazioni, consulta [Scegliere il metodo di pagamento in [!DNL Workfront Proof]](../../../workfront-proof/wp-billingsettings/manage-your-billing/choose-payment-method-in-wp.md).

## [!UICONTROL Contatto di fatturazione e indirizzo]

Questa sezione (8) mostra il contatto di fatturazione principale e i dettagli dell&#39;indirizzo del tuo account.

Il contatto Fatturazione può essere selezionato solo dagli utenti impostati come Amministratori fatturazione sul tuo account. Negli account Satellite, solo gli amministratori di fatturazione dell&#39;account principale possono essere impostati in questo campo.

![Billing_Contact.png](assets/billing-contact-350x137.png)

>[!NOTE]
>
> È possibile avere più amministratori di fatturazione sul tuo account, ma solo uno di essi, selezionati nella [!UICONTROL Contatto di fatturazione] riceverà tutte le notifiche di fatturazione e gli avvisi sull&#39;utilizzo dell&#39;account.

Questo include le seguenti e-mail di notifica:

* Uso della bozza
* Fatture
* Downgrade
* Avviso di sospensione pagamento/conto in ritardo
* Errore carta di credito

   ![Billin_CC.png](assets/billin-cc-350x103.png)

La [!UICONTROL Fatturazione CC] consente inoltre di aggiungere un indirizzo e-mail da copiare su tutte le e-mail relative alla fatturazione. Fai clic sul campo per attivare la modifica incline e inserisci un indirizzo e-mail a tua scelta (può essere anche l’indirizzo e-mail di un utente esistente).

## [!UICONTROL Indirizzo di fatturazione]

Questa sezione utilizza la modifica in linea, quindi fai clic sui campi per immettere o modificare il testo.

>[!NOTE]
>
> Inseriamo questo indirizzo nelle fatture di abbonamento in modo che questi dati siano sempre aggiornati.

![Billing_Address.png](assets/billing-address-350x199.png)

## [!UICONTROL Statistiche di utilizzo]

Questa sezione mostra le statistiche di utilizzo del tuo account nel periodo di fatturazione corrente, tra cui:

* Archiviazione utilizzata
* Prove utilizzate
* Limite utenti utilizzato

![Usage_Statistics.png](assets/usage-statistics-350x51.png)

### [!UICONTROL Avvisi di utilizzo]

La [[!UICONTROL Profili delle autorizzazioni di prova] in [!DNL Workfront] Prova](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) impostato come Contatto di fatturazione (1) sul tuo account verrà notificato via e-mail quando il tuo account raggiunge:

* 75% e quindi 98% della capacità di storage
* 75% e poi 100% del limite di prova

![Billing_Contact__1_.png](assets/billing-contact--1--350x74.png)

Una volta raggiunte le bozze o i limiti di archiviazione, vedrai anche gli avvisi nella parte superiore della [!UICONTROL Fatturazione] pagina:

* Limite di bozze raggiunto

   ![Proofs_limit_reach.png](assets/proofs-limit-reached-350x65.png)

* Limite di archiviazione raggiunto

![Storage_limit_reach.png](assets/storage-limit-reached-350x65.png)

>[!NOTE]
>
>Il conteggio delle prove viene utilizzato quando le bozze vengono create nel tuo account e non può essere ripristinato rimuovendo le bozze.

È possibile liberare spazio di archiviazione eliminando le bozze e i file e svuotando il [!UICONTROL Cestino] successivamente.

Ricorda che se hai bisogno di più prove, archiviazione o utenti, puoi aggiornare il tuo account in qualsiasi momento; e ha effetto immediato.

## [!UICONTROL Cronologia fatturazione]

Questa sezione mostra l’attività per tutti i periodi di fatturazione recenti. È inoltre possibile scaricare le fatture da questa sezione.

Per ulteriori informazioni, consulta &quot; [Download del [!DNL Workfront Proof] Fattura](../../../workfront-proof/wp-billingsettings/manage-your-billing/download-wp-invoice.md).&quot;

## [!UICONTROL Attività di fatturazione]

Questa sezione mostra le modifiche recenti apportate alla configurazione di fatturazione, ad esempio abbonamenti, aggiornamenti, downgrade e rinnovi [!DNL Workfront Proof] Pianifica.

Se si modifica il piano in uno con un limite utente inferiore (1), gli utenti che superano il nuovo limite verranno disattivati automaticamente all&#39;avvio del nuovo piano. Questa attività verrà anche acquisita nei registri account (2).

![Billing_Downgrade_log.png](assets/billing-downgrade-log-350x45.png)

![Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)
