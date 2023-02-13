---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: '''Attività di rilascio di Workfront Fusion: Settimana dell''11 gennaio 2021'''
description: Questa pagina descrive tutti i miglioramenti effettuati in Adobe Workfront Fusion la settimana dell’11 gennaio 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 2439e2a7-9404-433a-bd71-a7776042d8a0
hidefromtoc: true
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# Attività di rilascio di Workfront Fusion: settimana 11 gennaio 2021

Questa pagina descrive tutti i miglioramenti effettuati in Adobe Workfront Fusion la settimana dell’11 gennaio 2021.

Per un elenco di tutte le modifiche recenti, vedi [Attività di rilascio di Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Per un elenco delle correzioni di bug recenti in Workfront Fusion, vedi [Aggiornamenti alla manutenzione di Workfront](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) e controlla eventuali aggiornamenti etichettati Workfront Fusion Maintenance Update.

## Connettore e moduli ampliati ora disponibili

È ora possibile utilizzare Workfront Fusion per connettersi all&#39;account Widen. Con i moduli Widen, è possibile:

* Aggiungere risorse a o rimuovere risorse da una raccolta
* Scaricare o caricare file
* Leggere o aggiornare i metadati delle risorse
* Cercare le risorse in base ai criteri specificati
* Recupera un elenco di risorse in una raccolta
* Esegui una chiamata API personalizzata.

Per ulteriori informazioni consulta [Moduli ampliati](../../../workfront-fusion/apps-and-their-modules/widen-modules.md).

## Connettore dati e moduli ora disponibili

È ora possibile utilizzare Workfront Fusion per connettersi all&#39;account Datadog.

Con i moduli Datadog, puoi:

* Punti della cronologia dei post
* Eseguire una chiamata API personalizzata

Per informazioni sui moduli di Datadog, consulta [Moduli Datadog](../../../workfront-fusion/apps-and-their-modules/datadog-modules.md).

## Connettore evento e moduli ora disponibili

È ora possibile utilizzare Workfront Fusion 2.0 per connettersi all&#39;account Cvent.

Con i moduli Cvent, è possibile:

* Creare una richiesta di riunione
* Leggi record quali contatti, eventi o invitati
* Elencare record in base ai criteri specificati
* Registra o aggiungi gli invitati a eventi specifici
* Aggiorna o elimina contatti
* Effettuare una chiamata API personalizzata

Per informazioni sui moduli Cvent disponibili, vedi [Moduli di cvent](../../../workfront-fusion/apps-and-their-modules/cvent-modules.md).

## Connettore e moduli di Microsoft Dynamics 365 ora disponibili

È ora possibile utilizzare Workfront Fusion 2.0 per connettersi all’account Microsoft Dynamics 365. Con i moduli Microsoft Dynamics 365 puoi:

* Attiva uno scenario in cui i record vengono aggiunti o aggiornati in Microsoft Dynamics 365
* Creare, leggere, aggiornare o eliminare un record Microsoft Dynamics 365
* Eseguire una chiamata API personalizzata

Per informazioni sui moduli Microsoft Dynamics 365 disponibili, consulta [Moduli di Microsoft Dynamics 365](../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

## Connettore e moduli DocuSign ora disponibili

È ora possibile utilizzare Workfront Fusion 2.0 per connettersi all&#39;account DOCUSign. Con i moduli Docusign, puoi:

* Attiva uno scenario in cui un involucro cambia il suo stato
* Creare una busta
* Leggere, inviare o aggiungere un destinatario a una busta esistente
* Aggiungere o modificare campi personalizzati nei documenti
* Scarica un documento come file
* Caricare un file in un inviluppo
* Eseguire una chiamata API personalizzata

Per ulteriori informazioni, consulta [Moduli DocuSign](../../../workfront-fusion/apps-and-their-modules/docusign-modules.md).

## Cerca nella cronologia di esecuzione dello scenario

Abbiamo semplificato l’individuazione di informazioni specifiche dalle esecuzioni precedenti degli scenari. La nuova ricerca full text di Fusion consente di cercare nella cronologia di esecuzione i dati contenuti in un bundle. Ad esempio, per identificare l&#39;esecuzione creata per un&#39;attività specifica, è possibile utilizzare la ricerca full text per cercare tale ID attività.

Precedentemente, per trovare informazioni di esecuzione specifiche era necessario visualizzare ciascuna esecuzione singolarmente.

Per ulteriori informazioni, consulta [Visualizzare la cronologia di esecuzione di uno scenario in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Aggiornamenti a Fusion 2.0 Data Store

Per semplificare la personalizzazione degli archivi dati, sono state aggiunte alcune nuove funzionalità. Ora, quando visualizzi un archivio dati, puoi:

* Trascinare per riordinare le colonne
* Modificare una singola cella
* Aggiungi più righe

Per ulteriori informazioni sugli archivi dati, vedi [Moduli di archiviazione dati](../../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## Effettuare una richiesta di autorizzazione della chiave API tramite il connettore HTTP

Per aumentare la flessibilità nelle modalità di accesso alle API, abbiamo aggiunto un nuovo modulo al connettore HTTP. Ora è possibile utilizzare il connettore HTTP per effettuare una richiesta quando il servizio Web a cui si accede richiede l’utilizzo di una chiave API.

Per ulteriori informazioni, consulta [Moduli HTTP](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

## Nuove funzioni disponibili nel pannello di mappatura

Per facilitare la personalizzazione e la semplificazione delle formule nei moduli, sono state aggiunte alcune nuove funzioni.

* il

   ```
   omit
   ```

   funzione è una funzione generale che omette le chiavi specificate dell&#39;oggetto e restituisce il resto.
* il

   ```
   pick
   ```

   funzione è una funzione generale che seleziona dall’oggetto solo le chiavi specificate.
* il

   ```
   escapeMarkdown
   ```

   è una funzione stringa che evita tutti i tag Markdown presenti in un testo.

Per ulteriori informazioni sulle funzioni di omettere e selezionare, vedi [Funzioni generali in Adobe Workfront Fusion](../../../workfront-fusion/functions/general-functions.md).

Per ulteriori informazioni sulla funzione escapeMarkdown, consulta [Funzioni stringa in Adobe Workfront Fusion](../../../workfront-fusion/functions/string-functions.md).
