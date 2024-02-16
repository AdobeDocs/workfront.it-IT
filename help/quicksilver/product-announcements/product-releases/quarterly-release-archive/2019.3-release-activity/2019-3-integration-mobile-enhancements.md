---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: Integrazione 2019.3 e miglioramenti per dispositivi mobili
description: Questa pagina descrive tutte le modifiche e i miglioramenti apportati all’integrazione per dispositivi mobili con la versione 2019.3. È stato reso disponibile nell’ambiente di produzione la settimana del 19 agosto 2019.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Integrazione 2019.3 e miglioramenti per dispositivi mobili

Questa pagina descrive tutte le modifiche e i miglioramenti apportati all’integrazione per dispositivi mobili con la versione 2019.3. È stato reso disponibile nell’ambiente di produzione la settimana del 19 agosto 2019.

Per un elenco di tutte le modifiche apportate in 2019.3, consulta [Panoramica sull’attività della versione 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Supporto degli elementi condivisi nell&#39;integrazione con MS OneDrive

Ora puoi collegare i file e le cartelle di OneDrive condivisi agli oggetti di Workfront. Al contrario, è possibile caricare file in Workfront in cartelle condivise in OneDrive.

Per ulteriori informazioni, consulta le sezioni [Collegare un documento esterno a Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents), [Collega una o più cartelle esterne](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder), e [Aggiornare e collegare un documento da Workfront a un provider cloud esterno](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) nell’articolo [Collegare documenti da applicazioni esterne](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Per informazioni, consulta la sezione [Collegare un documento esterno a Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) nell’articolo [Collegare documenti da applicazioni esterne](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Specifica del dominio richiesta per tutti gli accessi a Workfront

Tutti gli accessi a Workfront ora richiedono all’utente di specificare il dominio, se questo non è già specificato nell’URL di Workfront. La richiesta di queste informazioni aumenta la sicurezza dell’istanza di Workfront. Inoltre, se l’implementazione di Workfront ha più istanze, questo miglioramento consente di aggiungere lo stesso utente a ogni istanza di Workfront all’interno dell’implementazione.

Questa modifica può influire sia sugli accessi utente che sulle integrazioni API:

* **Accessi utente**

  Se il dominio della tua azienda non è incluso nell’URL di Workfront, nella schermata di accesso verrà visualizzato un nuovo campo Dominio oltre ai campi Nome utente e Password.

  Per la maggior parte dei clienti, non è richiesta alcuna modifica perché le informazioni sul dominio sono già incluse nell’URL di Workfront. Ad esempio, &quot;*dominio*.my.workfront.com.&quot;

* **Integrazioni API**

  Se un codice API viene reindirizzato a un indirizzo che non include il nome di dominio, tale codice non funzionerà più.

Per ulteriori informazioni, consulta [Accedere ad Adobe Workfront](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md).

## Convertire attività e problemi in progetti tramite l’app mobile su iOS

Ora è possibile convertire singole attività e problemi in progetti nell’app mobile Workfront su iOS.

## Accedi all’app mobile con impronta digitale o ID volto

A seconda del dispositivo, puoi scegliere di accedere all’app mobile di Workfront utilizzando la tecnologia impronta digitale o face ID. Quando accedi all’app mobile, ti chiederà se desideri effettuare l’accesso con qualsiasi metodo di autenticazione supportato dal telefono.

Per ulteriori informazioni su come gestire questa funzione, consulta [Adobe Workfront per iOS](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) o [Adobe Workfront per Android](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md).

## Nuova impostazione per la disconnessione automatica degli utenti da dispositivi mobili

Per rendere l’app mobile di Workfront più sicura per te e per la tua azienda, gli utenti verranno disconnessi automaticamente dopo 15 giorni di inattività. Gli amministratori di Workfront possono personalizzare questo limite di tempo nell’applicazione Web in Configurazione > Sistema > Preferenze.

Per ulteriori informazioni, consulta [Configurare le preferenze di sicurezza del sistema](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## L&#39;App Mobile Richiede Il Dominio Durante L&#39;Accesso

Per migliorare la sicurezza, l&#39;app mobile di Workfront ora richiede di fornire il dominio se non si accede con credenziali Single Sign-On.

>[!NOTE]
>
>Disponibilità di iOS: 12 giugno 2019
>
>Disponibilità della produzione: 17 giugno 2019

## Eliminare oggetti utilizzando l’app Mobile su iOS

>[!NOTE]
>
>Questa funzione è stata resa disponibile negli app store per iOS la settimana del 19 agosto 2019.

Ora puoi eliminare oggetti come attività, problemi e schede orario nell’app mobile di iOS. Per eliminare l&#39;oggetto è necessario disporre delle autorizzazioni corrette.

## Filtrare per progetti inattivi nell’app mobile

>[!NOTE]
>
>Questa funzione sarà disponibile negli app store sia per iOS che per Android nella settimana del 19 agosto 2019.

Abbiamo aggiunto l’opzione Dead Projects (Progetti inattivi) come filtro nella scheda Projects (Progetti) dell’app Mobile.

## Reimpostare la password utilizzando l’app mobile

Puoi usare l’app Workfront Mobile per reimpostare la password, se l’hai dimenticata. Toccare Password dimenticata? e seguire le istruzioni visualizzate. Non è possibile reimpostare la password SSO nell&#39;app mobile.

## Nuovo look and feel per dispositivi mobili

Abbiamo aggiunto i seguenti miglioramenti per migliorare la tua esperienza nell’app mobile di Workfront.

* I seguenti elementi sono stati spostati dalla barra superiore della pagina Dettagli ad aree più prominenti sullo schermo:

   * L’icona più è ora nell’angolo in basso a sinistra dello schermo
   * Il segno di spunta per iniziare a lavorare su un elemento ora è un pulsante Lavoraci in alto e al centro dello schermo

* Per visualizzare i moduli personalizzati allegati, tocca Mostra altro nella parte inferiore della pagina Dettagli.
* È stato modificato l’aspetto delle pagine utilizzate per inviare attività, problemi e richieste.

