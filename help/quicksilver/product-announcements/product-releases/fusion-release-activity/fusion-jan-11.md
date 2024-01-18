---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Attività di rilascio di Workfront Fusion: settimana dell’11 gennaio 2021"
description: Questa pagina descrive tutti i miglioramenti apportati ad Adobe Workfront Fusion la settimana dell’11 gennaio 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 2439e2a7-9404-433a-bd71-a7776042d8a0
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Attività di rilascio di Workfront Fusion: settimana dell’11 gennaio 2021

Questa pagina descrive tutti i miglioramenti apportati ad Adobe Workfront Fusion la settimana dell’11 gennaio 2021.

Per un elenco di tutte le modifiche recenti, vedi [Attività di rilascio di Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Per un elenco delle correzioni di bug recenti in Workfront Fusion, vedi [Aggiornamenti di manutenzione per Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) e verificare la presenza di eventuali aggiornamenti etichettati Aggiornamento di manutenzione di Workfront Fusion.

## Connettore e moduli Widen ora disponibili

Ora puoi utilizzare Workfront Fusion per connettersi al tuo account Widen. I moduli Widen consentono di:

* Aggiungere o rimuovere risorse da una raccolta
* Scaricare o caricare i file
* Lettura o aggiornamento dei metadati delle risorse
* Cercare le risorse in base ai criteri specificati
* Recuperare un elenco di risorse in una raccolta
* Esegui una chiamata API personalizzata.

Per ulteriori informazioni, consulta [Amplia moduli](../../../workfront-fusion/apps-and-their-modules/widen-modules.md).

## Connettore e moduli Datadog ora disponibili

È ora possibile utilizzare Workfront Fusion per connettersi all’account Datadog.

Con i moduli Datadog è possibile:

* Pubblica punti serie temporali
* Eseguire una chiamata API personalizzata

Per informazioni sui moduli Datadog, vedi [Moduli Datadog](../../../workfront-fusion/apps-and-their-modules/datadog-modules.md).

## Sono ora disponibili il connettore e i moduli Cvent

È ora possibile utilizzare Workfront Fusion 2.0 per connettersi al proprio account Cvent.

Con i moduli Cvent è possibile:

* Creare una convocazione di riunione
* Lettura di record quali contatti, eventi o invitati
* Elenca i record in base ai criteri specificati
* Registrare o aggiungere invitati a eventi specifici
* Aggiornare o eliminare contatti
* Effettuare una chiamata API personalizzata

Per informazioni sui moduli evento disponibili, vedere [Moduli evento](../../../workfront-fusion/apps-and-their-modules/cvent-modules.md).

## Connettore e moduli Microsoft Dynamics 365 ora disponibili

È ora possibile utilizzare Workfront Fusion 2.0 per connettersi all’account Microsoft Dynamics 365. Con i moduli di Microsoft Dynamics 365 è possibile:

* Attiva uno scenario quando i record vengono aggiunti o aggiornati in Microsoft Dynamics 365
* Creare, leggere, aggiornare o eliminare un record di Microsoft Dynamics 365
* Eseguire una chiamata API personalizzata

Per informazioni sui moduli di Microsoft Dynamics 365 disponibili, vedere [Moduli Microsoft Dynamics 365](../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

## Il connettore e i moduli DocuSign sono ora disponibili

È ora possibile utilizzare Workfront Fusion 2.0 per connettersi al proprio account Docusign. Con i moduli Documentazione è possibile:

* Attiva uno scenario quando un involucro cambia stato
* Creare una busta
* Lettura, invio o aggiunta di un destinatario a una busta esistente
* Aggiungere o modificare campi personalizzati nei documenti
* Scaricare un documento come archiviato
* Caricare un file in una busta
* Eseguire una chiamata API personalizzata

Per ulteriori informazioni, consulta [Moduli DocuSign](../../../workfront-fusion/apps-and-their-modules/docusign-modules.md).

## Cerca nella cronologia di esecuzione dello scenario

È stato semplificato l’individuazione di informazioni specifiche provenienti da esecuzioni di scenari precedenti. La nuova ricerca full-text di Fusion consente di cercare nella cronologia di esecuzione tutti i dati contenuti in un bundle. Ad esempio, per identificare l&#39;esecuzione che ha creato un&#39;attività specifica, è possibile utilizzare la ricerca full-text per cercare l&#39;ID attività.

In precedenza, per trovare informazioni specifiche sull’esecuzione era necessario visualizzare ogni singola esecuzione.

Per ulteriori informazioni, consulta [Visualizzare la cronologia di esecuzione di uno scenario in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Aggiornamenti a Fusion 2.0 Data Store

Per semplificare la personalizzazione degli archivi dati, sono state aggiunte alcune nuove funzionalità. Ora quando visualizzi un archivio dati puoi:

* Trascina per riordinare le colonne
* Modificare una singola cella
* Aggiungere più righe

Per ulteriori informazioni sugli archivi dati, consulta [Moduli archivio dati](../../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## Effettuare una richiesta di autorizzazione della chiave API tramite il connettore HTTP

Per aumentare la flessibilità nelle modalità di accesso alle API, è stato aggiunto un nuovo modulo al connettore HTTP. Ora puoi utilizzare il connettore HTTP per effettuare una richiesta quando il servizio web a cui accedi richiede l’utilizzo di una chiave API.

Per ulteriori informazioni, consulta [Moduli HTTP](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

## Nuove funzioni disponibili nel pannello di mappatura

Sono state aggiunte alcune nuove funzioni che consentono di personalizzare e semplificare le formule nei moduli.

* il

  ```
  omit
  ```

  La funzione è una funzione generale che omette i tasti specificati dell&#39;oggetto e restituisce il resto.
* il

  ```
  pick
  ```

  è una funzione generale che seleziona solo i tasti specificati dall’oggetto.
* il

  ```
  escapeMarkdown
  ```

  La funzione è una funzione stringa che esce da tutti i tag Markdown in un testo.

Per ulteriori informazioni sulle funzioni Ometti e Scegli, consulta [Funzioni generali di Adobe Workfront Fusion](../../../workfront-fusion/functions/general-functions.md).

Per ulteriori informazioni sulla funzione escapeMarkdown, consulta [Funzioni stringa in Adobe Workfront Fusion](../../../workfront-fusion/functions/string-functions.md).
