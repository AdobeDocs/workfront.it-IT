---
title: Miglioramenti dell’integrazione 22.2
description: Miglioramenti dell’integrazione 22.2
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Miglioramenti dell’integrazione 22.2

Questa pagina descrive tutti i miglioramenti all&#39;integrazione apportati con la versione 22.2 all&#39;ambiente Preview. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 4 aprile 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.2, vedi [Panoramica sulla versione 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## È ora disponibile l’integrazione Adobe Workfront con Anaplan

Per offrirti una maggiore flessibilità e una migliore comprensione degli aspetti finanziari dei tuoi progetti Workfront, Workfront può ora integrarsi con il tuo account Anaplan. Collegando gli oggetti Workfront agli oggetti Anaplan, è possibile aggiornare automaticamente le informazioni tra i due account, garantendo che le informazioni in entrambi siano aggiornate e identiche. Puoi anche attivare i processi automatizzati in Anaplan in base alle azioni in Workfront (o viceversa).

Ad esempio, puoi creare una campagna in Anaplan, quindi creare un progetto o un programma Workfront collegato alla campagna. Eventuali costi tracciati in Workfront possono quindi essere caricati nuovamente su Anaplan per esaminare le prestazioni della campagna.

Altri flussi di lavoro che puoi considerare come utilizzare l’integrazione tra Workfront e Anaplan per:

* Creazione di richieste di budget Anaplan da nuovi progetti Workfront
* Creazione di progetti Workfront da nuovi elementi di elenco Anaplan
* Avvio di richieste di fornitori Anaplan da progetti Workfront

Per ulteriori informazioni, consulta [Adobe Workfront con Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Workfront per Experience Manager aggiornamenti avanzati dei connettori

Workfront, ad Experience Manager, include ora i seguenti aggiornamenti:

* È ora possibile creare cartelle collegate tra Adobe Workfront e Adobe Experience Manager Assets as a Cloud Service anche se sono presenti più configurazioni di cartelle collegate al progetto.
* È stato aggiunto il supporto per l’impaginazione dell’abbonamento a un evento
* È stato aggiunto il supporto per AEM 6.4.x
* È stato aggiunto il supporto per gli ambienti proxy
* Diverse correzioni di bug in base al feedback di partner e clienti

Per ulteriori informazioni, consulta [Panoramica del connettore avanzato Workfront per Experience Manager](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>La distribuzione e la configurazione di questo connettore richiede un partner certificato. Vedi [Installazione di Workfront per un connettore avanzato Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=en#) per ulteriori informazioni.

## Le integrazioni Adobe Creative Cloud ora utilizzano OAuth2

Per una maggiore sicurezza e per fare un’esperienza più coerente tra le integrazioni, abbiamo aggiornato le integrazioni Adobe Creative Cloud per utilizzare l’autenticazione OAuth2, un metodo standard di settore per l’autenticazione degli utenti. Ora, quando gli utenti effettuano l’accesso, possono visualizzare le azioni e le aree specifiche a cui le integrazioni hanno accesso e consentire l’accesso. In seguito, non è necessario effettuare l’accesso con la stessa frequenza.

Per ulteriori informazioni, consulta [Utilizzare l’estensione Workfront per Illustrator e InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## Vedi i dettagli del segreto client per le integrazioni personalizzate OAuth2 o JWT

Per garantire la trasparenza nell’utilizzo delle integrazioni personalizzate OAuth2 e JWT, abbiamo reso possibile la visualizzazione dei dettagli dei Segreti client utilizzati dalle integrazioni. Ora puoi vedere le date di creazione e dell’ultimo utilizzo del Segreto client. È inoltre possibile aggiungere e visualizzare le proprie note sul Segreto client.

In precedenza, questi dettagli non erano disponibili.

Per ulteriori informazioni sui segreti client nelle integrazioni personalizzate OAuth2 o JWT, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Vedi il tipo di autenticazione nell’elenco delle applicazioni OAuth2 personalizzate

Ora, quando visualizzi l’elenco delle applicazioni OAuth2 personalizzate nella tua organizzazione, puoi vedere se ogni applicazione utilizza l’autenticazione utente o l’autenticazione server.

In precedenza, era possibile visualizzare queste informazioni solo andando nelle opzioni di modifica su ogni applicazione.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Imposta la scadenza per i token di aggiornamento nelle integrazioni personalizzate OAuth2

Per controllare meglio l’accesso e la sicurezza per le integrazioni OAuth2 personalizzate, ora puoi personalizzare la durata dei token di aggiornamento. Dopo la scadenza del token di aggiornamento di un utente, dovrà accedere nuovamente all’integrazione.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Utilizza le chiavi pubbliche e private nelle integrazioni personalizzate OAuth2 per le app da server a server

È ora possibile configurare le applicazioni OAuth2 server-to-server nelle integrazioni personalizzate. Impostando le chiavi pubblica e privata, puoi consentire a Workfront di comunicare con un’altra applicazione senza utilizzare le credenziali di accesso.

In precedenza, tutte le autenticazioni nelle applicazioni OAuth2 personalizzate utilizzavano le credenziali di accesso dell’utente.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## L’integrazione di Google G Suite ora utilizza OAuth2

Per una maggiore sicurezza e per fare un’esperienza più coerente tra le integrazioni, abbiamo aggiornato l’integrazione di Google G Suite per utilizzare l’autenticazione OAuth2, un metodo standard di settore per l’autenticazione degli utenti. Ora, quando gli utenti effettuano l’accesso, possono visualizzare le azioni e le aree specifiche a cui le integrazioni hanno accesso e consentire l’accesso. In seguito, non è necessario effettuare l’accesso con la stessa frequenza.

Per ulteriori informazioni, consulta [Accesso e uscita da Adobe Workfront per G Suite](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
