---
title: aggiornamenti del progetto durante l’intervallo di tempo previsto per la versione 22.3
description: aggiornamenti del progetto durante l’intervallo di tempo previsto per la versione 22.3
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 0fea13b0a1d8f14c2d601e0ed0a8d15684a3c4d7
workflow-type: tm+mt
source-wordcount: '1549'
ht-degree: 0%

---

# 22.3 Miglioramenti al progetto

Questa pagina descrive tutti i miglioramenti apportati a Project con la versione 22.3 nell’ambiente di anteprima. Questi miglioramenti sono stati resi disponibili nell&#39;ambiente di produzione la settimana dell&#39;11 luglio 2022. Per un elenco di tutte le modifiche disponibili con la versione 22.3, vedi [Panoramica sulla versione 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Delega di lavoro fuori sede

Ora puoi delegare temporaneamente le attività e i problemi assegnati ad altri utenti quando intendi uscire dall’ufficio per un breve periodo di tempo. Questo assicura che la vostra assenza non diventi un blocco stradale per il lavoro in corso.

Prima di questo miglioramento, era possibile delegare solo le approvazioni.

Di seguito sono riportate alcune delle funzioni aggiunte con questo aggiornamento:

* Un&#39;impostazione nell&#39;area Preferenze attività e problemi di Configurazione per l&#39;amministratore di sistema o di gruppo per abilitare la delega nell&#39;ambiente.

* Una nuova opzione per &quot;Delega attività e problemi&quot; nell&#39;area Home per gli utenti con una licenza di revisione o superiore per delegare i loro elementi di lavoro.

* Indicazione nella home e nell&#39;area Assegnazioni delle attività e delle intestazioni di emissione che gli elementi sono delegati ad altri.

* Notifiche di eventi nell’area Configurazione e notifiche e-mail nel profilo utente per controllare le notifiche e-mail sul lavoro delegato


>[!NOTE]
>
>Solo gli utenti con una licenza di revisione o superiore possono delegare il loro lavoro ad altri. Il lavoro può essere delegato a qualsiasi utente, indipendentemente dal suo livello di accesso. Gli utenti delegati ricevono le stesse autorizzazioni degli assegnatari sugli elementi delegati. Se queste autorizzazioni sono inferiori alla configurazione del livello di accesso di un utente, agli utenti delegati potrebbe essere impedito di eseguire alcune delle attività sulle attività e sui problemi ad essi delegati.


Per ulteriori informazioni, consulta [Panoramica sull’attività e sul problema delegato](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## Nuova esperienza durante la conversione di un problema in un’attività

Per rendere coerente l’utilizzo di Workfront con la nuova esperienza Workfront, abbiamo riprogettato l’interfaccia per convertire un problema in un’attività.

Questo aggiornamento include:

* Interfaccia utente aggiornata che corrisponde al resto della nuova esperienza Workfront.

* Accesso per convertire un problema in attività da un elenco o da un report.

* I moduli personalizzati predefiniti definiti nell’area Impostazioni attività del progetto di destinazione aggiunto alla nuova attività.


Per ulteriori informazioni, consulta [Convertire un problema in un’attività in Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Nuova esperienza durante la conversione di un problema in un progetto senza modello

Per rendere coerente l’utilizzo di Workfront con la nuova esperienza Workfront, abbiamo riprogettato l’interfaccia per convertire un problema in un progetto senza utilizzare un modello.

Oltre a un’interfaccia utente aggiornata che corrisponde al resto della nuova esperienza Workfront, è stata aggiunta la possibilità di convertire un problema in progetti vuoti da un elenco o da un rapporto.

Per ulteriori informazioni, consulta [Convertire un problema in un progetto in Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Assegnazione di tag avanzati nel flusso di aggiornamento

È stato migliorato l’assegnazione di tag agli utenti nel flusso di aggiornamento quando si crea un nuovo aggiornamento o si risponde a uno esistente. Ora, quando taggi un utente per includerli in un aggiornamento, oltre al loro nome e al loro avatar, mostriamo anche il loro Ruolo primario e la loro e-mail. Questo aiuta a distinguere tra più utenti con nomi simili o identici.

Per ulteriori informazioni, consulta [Assegnare tag agli altri utenti in caso di aggiornamenti](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Nuova sintassi per i calcoli nei campi personalizzati

Per preparare miglioramenti futuri che consentiranno di aggiungere calcoli ai moduli personalizzati, è stata standardizzata la sintassi dei campi di riferimento aggiunti a un calcolo. È facile utilizzare questa nuova sintassi perché il sistema la immette automaticamente quando inizi a digitare il nome di un campo e quindi a selezionarlo.

Per ulteriori informazioni, consulta la sezione &quot;Generare il calcolo per il campo personalizzato calcolato&quot; nella sezione [articolo Aggiungere dati calcolati a un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Conserva informazioni precise quando due utenti con un ruolo comune sono coinvolti in un processo di approvazione

Per garantire la precisione dei dati per l&#39;approvazione del lavoro, abbiamo apportato una modifica nel modo in cui le informazioni di approvazione vengono registrate su un elemento quando un processo di approvazione a più ruoli è associato all&#39;elemento.

Alcuni processi di approvazione richiedono l’approvazione di due ruoli diversi e due approvatori diversi potrebbero avere uno di questi ruoli in comune. Ora, una volta prese le decisioni di approvazione, Workfront registra ogni approvatore e il rispettivo ruolo associato al processo di approvazione.

Prima di questa modifica, entrambe le approvazioni venivano registrate per il secondo utente perché condividevano uno dei ruoli di approvazione con il primo approvatore. In questo caso, il secondo approvatore sovrascriveva le informazioni del primo approvatore.

Per ulteriori informazioni sui processi di approvazione in Workfront, consulta [Panoramica del processo di approvazione](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Le ore di allocazione non verranno più rimosse quando si apportano modifiche alle assegnazioni

>[!NOTE]
>
>Questa funzione era originariamente prevista per la versione 22.2. È stato rilasciato in produzione il 21 aprile 2022.


Per garantire l&#39;accuratezza dei dati, è stata apportata una modifica per mantenere le ore di allocazione e per mantenere invariata l&#39;ora pianificata delle attività quando si apportano modifiche alle assegnazioni dell&#39;attività.

Sono state apportate le seguenti modifiche alle attività con un tipo di durata semplice:

* Le ore pianificate vengono mantenute quando si rimuovono tutti gli assegnatari.

* Le allocazioni di assegnazione individuali vengono mantenute quando si sostituiscono utenti e ruoli.

* Le allocazioni di assegnazione individuali vengono mantenute sul ruolo durante la rimozione dell&#39;utente. (Rimosso dal rilascio. Ora, l&#39;ora pianificata sarà impostata su 0 dopo aver rimosso tutti gli assegnatari.)


Per ulteriori informazioni sulle ore pianificate, vedi [Panoramica sull’orario pianificato](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Miglioramenti alle bacheche

I seguenti miglioramenti sono stati aggiunti alle bacheche Adobe Workfront:

* Opzioni filtro: ora è possibile filtrare per data di scadenza o stato su una bacheca. Il filtro è stato aggiornato anche con sezioni comprimibili per separare le opzioni.

* Scheda archivio: ora potete archiviare una bacheca mentre vi trovate nella bacheca, invece di dover passare alla dashboard delle bacheche.

* Aggiunta di un team a una bacheca: quando cercate i membri, potete aggiungere un intero team. La scelta di un team aggiunge tutti i membri del team alla bacheca.

* Zone di rilascio nelle colonne : quando si trascina e si rilascia una scheda da una colonna di una bacheca a un’altra, ora viene visualizzata una &quot;zona di rilascio&quot; grigia in cui verrà posizionata la scheda. In precedenza non esisteva un indicatore visivo del posizionamento della scheda.

* Schede collegate: è ora possibile aggiungere schede collegate alle attività e ai problemi di Workfront. L’aggiornamento del nome, della descrizione o dell’assegnatario nella scheda o nell’attività comporta l’aggiornamento degli stessi campi nell’altra posizione.

* Campo di stato su tutte le schede - Un campo Stato e un pulsante Contrassegna completato sono stati aggiunti alle schede ad hoc e collegate. Quando fai clic su Contrassegna completato, lo stato diventa automaticamente Completo.

* Converti scheda ad hoc in scheda connessa - È ora possibile convertire una scheda ad hoc in una scheda connessa dai dettagli della scheda.

* Scollega scheda connessa - La disconnessione di una scheda connessa interrompe la connessione con l&#39;oggetto Workfront. La scheda rimane come una scheda ad hoc sulla bacheca e l&#39;oggetto Workfront non viene interessato.

* Mappatura dello stato nelle colonne : le nuove impostazioni di colonna e i nuovi criteri consentono di definire lo stato, l’assegnatario o il tag applicato alle schede spostate in quella colonna. Inoltre, i nomi di colonna predefiniti in una nuova bacheca sono stati modificati in Colonna 1, Colonna 2 e Colonna 3.

* Indicatore di aggiornamento del campo : ora viene visualizzato un indicatore quando salvi una scheda per confermare che gli aggiornamenti sono stati salvati.


Per ulteriori informazioni, consulta [Guida introduttiva alle bacheche in Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Condividere le cartelle solo nei primi cinque livelli di una gerarchia di cartelle

Per garantire le migliori prestazioni agli utenti che condividono le cartelle, al momento la condivisione è limitata ai primi cinque livelli della gerarchia delle cartelle su un oggetto.

Ogni cartella al sesto livello o inferiore eredita le configurazioni di condivisione dalla cartella direttamente sopra di essa.

Per ulteriori informazioni sulla condivisione delle cartelle, vedi [Condivisione di una cartella di documenti di primo livello](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Campagne Workfront (Beta) - un nuovo modo per gestire il tuo lavoro

>[!NOTE]
>
>Questa funzione verrà rimossa da Anteprima il 9 gennaio 2023. Per ulteriori informazioni, consulta la sezione [23.1 Panoramica sulla versione](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>Questa funzione non sarà inclusa nella versione 22.3 Production. Sarà rilasciato a Production con una versione futura.


>[!NOTE]
>
>Questa funzionalità è disponibile solo come versione beta ed è attualmente in fase di costruzione. Continueremo ad aggiungere funzionalità per il flusso di lavoro Campaign con versioni future. La partecipazione al programma beta per le campagne Workfront è facoltativa.

Stiamo introducendo un nuovo oggetto in Adobe Workfront che ha il potenziale per cambiare il modo in cui gestisci il lavoro.

Campagne Workfront consente di organizzare progetti da portafogli e programmi diversi in un nuovo contenitore di lavoro. Questo nuovo contenitore si evolverà nelle versioni future per includere tutti gli oggetti di lavoro attualmente gestiti in silos separati.

Le seguenti funzionalità sono incluse in questa versione:

* Un nuovo oggetto Workfront denominato Campaign

* Nuova area Campagne (Beta) nel menu principale

* Elenco delle campagne nell’area Campagne

* Pagina dei dettagli di una campagna che visualizza informazioni aggiuntive su una campagna

* Possibilità di aggiungere progetti a una campagna

* Possibilità di modificare le informazioni su una campagna

* Possibilità di rinominare l’oggetto Campaign dal modello di layout

   Gli amministratori di sistema e di gruppo di Workfront possono aggiungere l’area Campagne (Beta) nel menu principale di un modello di layout. Questo lo rende disponibile per tutti gli utenti assegnati al modello. Una volta disponibile, chiunque in Workfront può creare una campagna.




