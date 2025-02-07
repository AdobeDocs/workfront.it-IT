---
content-type: release-notes
keywords: note,trimestrale,aggiornamento,rilascio
navigation-topic: 2021-2-release-activity
title: 21.2 Altri miglioramenti
description: Questa pagina descrive tutti gli altri miglioramenti apportati con la versione 21.2 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 10 maggio 2021. Per un elenco di tutte le modifiche disponibili con la versione 21.2, consulta Panoramica sulla versione 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 21.2 Altri miglioramenti

Questa pagina descrive tutti gli altri miglioramenti apportati con la versione 21.2 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 10 maggio 2021. Per un elenco di tutte le modifiche disponibili con la versione 21.2, consulta la [panoramica sulla versione 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Ora siamo ufficialmente Adobe Workfront

Workfront è stato rinominato in Adobe Workfront.

Sono state aggiornate le aree più importanti dell’applicazione Adobe Workfront e dei siti web rivolti ai clienti. Altre aree verranno aggiornate a breve.

**Aree aggiornate**

* Schermata di accesso, navigazione superiore, verifica
* Interfaccia utente modelli di layout, menu principale, esportazione personalizzata Forms (disponibile solo nella nuova esperienza Adobe Workfront)
* App mobile Workfront (iOS e Android)

Aree che verranno aggiornate a breve

* App di correzione per desktop e dispositivi mobili
* Esportazioni PDF per elenchi e report
* Icona Favicon nella scheda del browser

**Aree che si aggiornano più tardi**

* Notifiche e-mail

## Convalida del inserisco nell&#39;elenco Consentiti di posta elettronica di

>[!NOTE]
>
>Disponibile solo nella nuova esperienza Adobe Workfront.

Se utilizzi il inserisco nell&#39;elenco Consentiti di e-mail, gli indirizzi e-mail nuovi e aggiornati dell’utente vengono ora convalidati in base al inserisco nell&#39;elenco Consentiti di. Quando aggiungi un nuovo utente o ne modifichi uno esistente e immetti un dominio e-mail che non si trova nel elenco Consentiti, viene visualizzato un messaggio per informare che l’utente non riceverà messaggi e-mail. Puoi comunque salvare il profilo utente, ma devi aggiungere il dominio al inserisco nell&#39;elenco Consentiti di in modo che l’utente riceva le e-mail.

Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Nuovo aspetto per le intestazioni oggetto

>[!NOTE]
>
>Questa funzione è stata rilasciata nell’ambiente di produzione il 10 marzo 2020.
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Per rafforzare ulteriormente la gerarchia delle informazioni e aiutare gli utenti a comprendere più chiaramente su quale pagina si trovano, ogni intestazione dell’oggetto ora dispone di:

* Icone colorate e più moderne per ciascun tipo di oggetto
* Il tipo di oggetto elencato sopra il nome dell&#39;oggetto
* Stile font e dimensione testo aggiornati
* Altre modifiche minori allo stile

In precedenza non esisteva alcuna icona e a destra del titolo dell’oggetto appariva un badge con il nome dell’oggetto.

Anche le intestazioni di pagina delle aree della nuova esperienza Workfront, come Analisi avanzate, Gestione risorse e altre, hanno questo aspetto aggiornato.

Per ulteriori informazioni sulle nuove intestazioni oggetto nella nuova esperienza Workfront, vedi [Nuove intestazioni oggetto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![Intestazione oggetto](assets/product-announcement-object-header-350x179.png)

## Aggiornamenti alle risposte alla ricerca dello stato dell&#39;oggetto

Workfront ora memorizza gli stati degli oggetti in un nuovo modo.

Queste modifiche non influiscono sul modo in cui vengono effettuate le richieste di ricerca dello stato. Tuttavia, le richieste API contenenti una ricerca dello stato dell’oggetto restituiranno un elenco incompleto degli stati del gruppo.

Per ulteriori informazioni, consulta [Modifiche API di base: risposte alla ricerca di stato](../../../wf-api/api/api-changes-search.md) .

## Payload di abbonamento agli eventi aggiornati per includere tutti i campi che terminano con ID

Tutti i payload di abbonamento agli eventi ora contengono ogni campo che termina con &quot;ID&quot;.

È importante notare che ogni oggetto ha il proprio set univoco di campi associati, che include un set univoco di campi associati che terminano con ID. Ciò significa che mentre ogni payload contiene tutti i campi associati all’oggetto che terminano con ID, ogni oggetto ha un diverso set di campi che terminano con ID.

## La versione beta dei blueprint è ora disponibile in Anteprima

>[!NOTE]
>
>Questa funzionalità non sarà generalmente disponibile nell’ambiente di produzione fino alla versione 21.3, più avanti nell’anno. Disponibile solo nella nuova esperienza Adobe Workfront.

Blueprint fornisce elementi di base per aiutarti a creare un sistema di gestione del lavoro che cresce con te. Gli amministratori di sistema possono sfogliare il catalogo dei blueprint e installare modelli di progetto pronti all’uso.

Per ulteriori informazioni, vedere [Blueprint](../../../administration-and-setup/blueprints/blueprints.md).
