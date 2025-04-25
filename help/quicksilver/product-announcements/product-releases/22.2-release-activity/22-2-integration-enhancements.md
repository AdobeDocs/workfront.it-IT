---
title: 22.2 Miglioramenti all’integrazione
description: 22.2 Miglioramenti all’integrazione
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 22.2 Miglioramenti all’integrazione

Questa pagina descrive tutti i miglioramenti all’integrazione apportati con la versione 22.2 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 4 aprile 2022.

Per un elenco di tutte le modifiche disponibili con la versione 22.2, vedere [Panoramica sulla versione 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## È ora disponibile l’integrazione di Adobe Workfront con Anaplan

Per offrirti maggiore flessibilità e insight negli aspetti finanziari dei tuoi progetti Workfront, Workfront ora può integrarsi con il tuo account Anaplan. Collegando oggetti Workfront a oggetti Anaplan, è possibile aggiornare automaticamente le informazioni tra i due account, assicurandosi che le informazioni in entrambi siano aggiornate e identiche. Puoi anche attivare processi automatizzati in Anaplan in base alle azioni in Workfront (o viceversa).

Ad esempio, puoi creare una campagna in Anaplan, quindi un progetto o un programma Workfront collegato alla campagna. Tutti i costi tracciati in Workfront possono quindi essere caricati di nuovo su Anaplan per rivedere le prestazioni della campagna.

Altri flussi di lavoro per i quali si può considerare l’utilizzo dell’integrazione da Workfront ad Anaplan includono:

* Creazione di richieste di budget Anaplan da nuovi progetti Workfront
* Creazione di progetti Workfront da nuove voci di elenco Anaplan
* Avvio delle richieste dei fornitori Anaplan dai progetti Workfront

Per ulteriori informazioni, vedere [Adobe Workfront con Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Aggiornamenti dei connettori avanzati di Workfront per Experience Manager

Il connettore avanzato Workfront per Experience Manager ora include i seguenti aggiornamenti:

* Ora puoi creare cartelle collegate tra Adobe Workfront e Adobe Experience Manager Assets as a Cloud Service anche in presenza di più configurazioni di cartelle collegate a un progetto.
* È stato aggiunto il supporto per l’impaginazione dell’abbonamento agli eventi
* È stato aggiunto il supporto per AEM 6.4.x
* È stato aggiunto il supporto per ambienti proxy
* Diverse correzioni di bug in base al feedback ricevuto da partner e clienti

Per ulteriori informazioni, consulta [Panoramica del connettore avanzato di Workfront per Experience Manager](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>L’implementazione e la configurazione di questo connettore richiedono un partner certificato. Per ulteriori informazioni, vedere [Installare il connettore avanzato di Workfront per Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install).

## Le integrazioni Adobe Creative Cloud ora utilizzano OAuth2

Per una maggiore sicurezza e per rendere più coerente l’esperienza tra le diverse integrazioni, abbiamo aggiornato le integrazioni Adobe Creative Cloud per l’utilizzo dell’autenticazione OAuth2, una modalità standard del settore per l’autenticazione degli utenti. Ora, quando gli utenti effettuano l’accesso, possono visualizzare le azioni e le aree specifiche a cui le integrazioni hanno accesso e consentire l’accesso. In seguito, non sarà necessario effettuare l&#39;accesso con la stessa frequenza.

Per ulteriori informazioni, vedere [Utilizzare l&#39;estensione Workfront per Illustrator e InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## Vedi i dettagli del segreto client per le integrazioni OAuth2 o JWT personalizzate

Per garantire trasparenza nell’utilizzo delle integrazioni personalizzate OAuth2 e JWT, ti abbiamo consentito di visualizzare i dettagli dei segreti client utilizzati dalle integrazioni. Ora puoi vedere le date in cui è stato creato e utilizzato per l’ultima volta il segreto client. Puoi anche aggiungere e visualizzare le tue note sul segreto client.

In precedenza, questi dettagli non erano disponibili.

Per ulteriori informazioni sui segreti client nelle integrazioni personalizzate OAuth2 o JWT, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Vedi il tipo di autenticazione nell’elenco delle applicazioni OAuth2 personalizzate

Ora, quando visualizzi l’elenco delle applicazioni OAuth2 personalizzate nell’organizzazione, puoi vedere se ogni applicazione utilizza l’autenticazione utente o l’autenticazione server.

In precedenza, era possibile visualizzare queste informazioni solo andando nelle opzioni di modifica di ogni applicazione.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Impostare la scadenza per i token di aggiornamento nelle integrazioni OAuth2 personalizzate

Per controllare meglio l’accesso e la sicurezza delle integrazioni OAuth2 personalizzate, ora puoi personalizzare la durata dei token di aggiornamento. Dopo la scadenza del token di aggiornamento di un utente, quest’ultimo dovrà accedere nuovamente all’integrazione.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Usa chiavi pubbliche e private nelle integrazioni OAuth2 personalizzate per le app server-to-server

È ora possibile configurare le applicazioni OAuth2 server-to-server nelle integrazioni personalizzate. Configurando le chiavi pubbliche e private, puoi consentire a Workfront di comunicare con un’altra applicazione senza utilizzare le credenziali di accesso.

In precedenza, tutte le autenticazioni nelle applicazioni OAuth2 personalizzate utilizzavano le credenziali di accesso dell&#39;utente.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## L’integrazione di Google Google Workspace ora utilizza OAuth2

Per una maggiore sicurezza e per rendere più coerente l’esperienza tra le diverse integrazioni, abbiamo aggiornato l’integrazione Google Google Workspace per utilizzare l’autenticazione OAuth2, un modo standard del settore per autenticare gli utenti. Ora, quando gli utenti effettuano l’accesso, possono visualizzare le azioni e le aree specifiche a cui le integrazioni hanno accesso e consentire l’accesso. In seguito, non sarà necessario effettuare l&#39;accesso con la stessa frequenza.

Per ulteriori informazioni, vedere [Accesso e disconnessione da Adobe Workfront per Google Workspace](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
