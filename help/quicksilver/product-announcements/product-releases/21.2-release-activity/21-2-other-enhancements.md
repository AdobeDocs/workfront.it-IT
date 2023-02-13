---
content-type: release-notes
keywords: note, trimestrale, aggiornamento, versione
navigation-topic: 2021-2-release-activity
title: 21.2 Altri miglioramenti
description: Questa pagina descrive tutti gli altri miglioramenti apportati nell’ambiente di anteprima con la versione 21.2. Questi miglioramenti saranno resi disponibili nell'ambiente di produzione la settimana del 10 maggio 2021. Per un elenco di tutte le modifiche disponibili con la versione 21.2, consulta Panoramica sulla versione 21.2.
author: Luke
feature: Product Announcements
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 21.2 Altri miglioramenti

Questa pagina descrive tutti gli altri miglioramenti apportati nell’ambiente di anteprima con la versione 21.2. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione la settimana del 10 maggio 2021. Per un elenco di tutte le modifiche disponibili con la versione 21.2, vedi [Panoramica sulla versione 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Ora siamo ufficialmente Adobe Workfront

Workfront si è ribellato ad Adobe Workfront.

Le aree più importanti all’interno dell’applicazione Adobe Workfront e dei nostri siti web rivolti ai clienti sono state aggiornate. Altre aree verranno presto aggiornate.

**Aree aggiornate**

* Schermata di accesso, navigazione superiore, correzione
* Interfaccia dei modelli di layout, menu principale, Esportazione Forms personalizzata (disponibile solo nella nuova esperienza Adobe Workfront)
* App mobile Workfront (iOS e Android)

Aree in fase di aggiornamento

* App di correzione per desktop e dispositivi mobili
* Esportazioni PDF per elenchi e rapporti
* Icona Favicon nella scheda del browser

**Aree in fase di aggiornamento successiva**

* Notifiche e-mail

## Convalida inserire nell&#39;elenco Consentiti e-mail

>[!NOTE]
>
>Disponibile solo nella nuova esperienza Adobe Workfront.

Se utilizzi l’inserire nell&#39;elenco Consentiti e-mail, gli indirizzi e-mail nuovi e aggiornati dell’utente vengono ora convalidati in base all’inserire nell&#39;elenco Consentiti. Quando aggiungi un nuovo utente o modifichi un utente esistente e immetti un dominio e-mail non presente nell’inserire nell&#39;elenco Consentiti, un messaggio ti notifica che l’utente non riceverà messaggi e-mail. Puoi comunque salvare il profilo utente, ma devi aggiungere il dominio all’inserire nell&#39;elenco Consentiti, in modo che l’utente riceva le e-mail.

Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Nuovo aspetto per le intestazioni degli oggetti

>[!NOTE]
>
>Questa funzione è stata rilasciata nell’ambiente di produzione il 10 marzo 2020.
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Per rafforzare ulteriormente la gerarchia delle informazioni e aiutare gli utenti a comprendere più chiaramente sulla pagina che si trovano, ogni intestazione di oggetto ora ha:

* Icone colorate e più moderne per ogni tipo di oggetto
* Tipo di oggetto elencato sopra il nome dell’oggetto
* Stile di font e dimensioni del testo aggiornati
* Altre modifiche di stile minori

In precedenza, a destra del titolo dell’oggetto non era presente alcuna icona e a destra era visualizzato un badge con il nome dell’oggetto.

Anche le intestazioni di pagina delle aree della nuova esperienza Workfront, ad esempio Analisi avanzate, Gestione risorse e altre, hanno questo aspetto aggiornato.

Per ulteriori informazioni sulle intestazioni dei nuovi oggetti nella nuova esperienza Workfront, consulta [Nuove intestazioni oggetto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## Aggiornamenti delle risposte alla ricerca dello stato degli oggetti

Workfront ora memorizza gli stati degli oggetti in un nuovo modo.

Queste modifiche non influiscono sul modo in cui vengono effettuate le richieste di ricerca dello stato. Tuttavia, le richieste API contenenti una ricerca per lo stato di un oggetto restituiranno un elenco incompleto degli stati del gruppo.

Per ulteriori informazioni, consulta [Modifiche API di base: Risposte alla ricerca dello stato](../../../wf-api/api/api-changes-search.md) .

## Payload dell’abbonamento a un evento aggiornato per includere tutti i campi che terminano con l’ID

Tutti i payload di abbonamento all’evento ora contengono ogni campo che termina con &quot;ID&quot;.

È importante notare che ogni oggetto ha un proprio set univoco di campi associati, che include un set univoco di campi associati che terminano con ID. Ciò significa che mentre ogni payload contiene tutti i campi associati all’oggetto che terminano con ID, ogni oggetto ha un diverso set di campi che terminano con ID.

## Blueprint beta ora disponibile in anteprima

>[!NOTE]
>
>Questa funzionalità sarà generalmente disponibile nell’ambiente di produzione solo dopo la versione 21.3 di quest’anno. Disponibile solo nella nuova esperienza Adobe Workfront.

Blueprint fornisce elementi di base per aiutarti a creare un sistema di gestione del lavoro che cresce con te. Gli amministratori di sistema possono sfogliare il catalogo delle blueprint e installare modelli di progetto pronti all’uso.

Per ulteriori informazioni, consulta [Blueprint](../../../administration-and-setup/blueprints/blueprints.md).
