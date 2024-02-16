---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Miglioramenti al progetto 2020.1
description: Questa pagina descrive tutti i miglioramenti apportati ai progetti con la versione 2020.1. Questi miglioramenti sono attualmente disponibili nell’ambiente di anteprima e saranno disponibili nell’ambiente di produzione a fine marzo o all’inizio di aprile 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Miglioramenti al progetto 2020.1

Questa pagina descrive tutti i miglioramenti apportati ai progetti con la versione 2020.1. Questi miglioramenti sono attualmente disponibili nell’ambiente di anteprima e saranno disponibili nell’ambiente di produzione a fine marzo o all’inizio di aprile 2020.

Per un elenco di tutte le modifiche disponibili con la versione 2020.1, consulta [Panoramica sulla versione 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Visualizzare più facilmente chi è taggato in un aggiornamento

Ora è più facile vedere quali utenti vengono taggati in un aggiornamento. Il nome degli utenti taggati viene visualizzato in blu e si collega al profilo utente.

Gli utenti taggati sono elencati anche nella casella dei commenti.

Prima di questo miglioramento, gli utenti ai quali erano stati assegnati dei tag non venivano visualizzati nella casella Notify (Notifica).

Per ulteriori informazioni, consulta [Assegna tag ad altri utenti in caso di aggiornamenti](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Includere e identificare il testo citato in un commento o in una risposta di aggiornamento

Quando si digita un commento, è possibile contrassegnarne una parte come testo citato per distinguerlo dal proprio commento. Utilizza il pulsante Citazione nell’editor di HTML.

Per ulteriori informazioni, consulta [Aggiorna lavoro](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


## Citare un commento precedente in un commento o in una risposta di aggiornamento

Quando inserite un commento in un thread di aggiornamento, potete includere rapidamente nel thread il testo di un commento precedente. Cercare l&#39;opzione Risposta preventivo nel menu Altro accanto al commento che si desidera citare.

Per ulteriori informazioni, consulta [Aggiorna lavoro](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Informazioni aggiuntive sui rischi

Per comprendere meglio i rischi dei progetti, ora puoi vedere chi e quando è stato inserito un rischio e quando è stato aggiornato in un progetto. Puoi accedere a queste informazioni in una visualizzazione dei rischi e tramite l’API Workfront pubblica. Questi campi saranno disponibili con la versione 11 dell’API, rilasciata con la versione 2020.1 di Produzione.

Per informazioni sui rischi in Workfront, consulta [Creare e modificare i rischi nei progetti](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

## Campi aggiuntivi aggiunti alle attività delle baseline e delle baseline

Per comprendere meglio l&#39;avanzamento finanziario dei progetti, è ora possibile includere informazioni aggiuntive sui costi e sui ricavi in un report Previsione o Attività prevista. Le informazioni finanziarie aggiuntive non vengono aggiunte alle previsioni salvate, ma vengono aggiunte per le nuove previsioni.

Per informazioni sui campi finanziari dei progetti e delle attività accessibili dagli oggetti Attività previste e Attività previste, vedere [Finanziamenti del progetto inclusi nelle linee di base del progetto](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## I problemi nello stato &quot;Approvazione in sospeso chiuso&quot; sono considerati incompleti

Il modo in cui Workfront gestisce i problemi con lo stato &quot;Completato-In attesa di approvazione&quot; è stato modificato. Ora, questi problemi vengono percepiti come aperti e il progetto non può essere contrassegnato come completo finché l’approvazione non viene risolta.

Prima di questa modifica, i problemi nello stato &quot;Chiuso-In attesa di approvazione&quot; venivano considerati chiusi.

Tutti i problemi posti nello stato Chiuso - In attesa di approvazione prima di questa modifica si comportano come in precedenza, essendo considerati completati e consentendo il completamento del progetto. Tutti i problemi posizionati in questo stato dopo questa modifica verranno considerati incompleti.

Per informazioni sugli stati dei progetti, vedi [Accedere all’elenco degli stati del progetto di sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

