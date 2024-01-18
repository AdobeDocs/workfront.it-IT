---
title: aggiornamenti del progetto durante l’intervallo di tempo della versione 22.3
description: aggiornamenti del progetto durante l’intervallo di tempo della versione 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

# 22.3 Miglioramenti al progetto

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di anteprima con la versione 22.3 di Project. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana dell’11 luglio 2022. Per un elenco di tutte le modifiche disponibili con la versione 22.3, consulta [Panoramica sulla versione 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Delega fuori sede

Ora è possibile delegare temporaneamente le attività e i problemi assegnati ad altri utenti quando si prevede di uscire dall&#39;ufficio per un breve periodo di tempo. In questo modo l&#39;assenza non sarà un ostacolo al completamento del lavoro.

Prima di questo miglioramento, era possibile delegare solo le approvazioni.

Di seguito sono riportate alcune delle funzioni aggiunte con questo aggiornamento:

* Impostazione nell’area Preferenze attività e problemi di Configura per l’amministratore di sistema o di gruppo per abilitare la delega nell’ambiente.

* Una nuova opzione per &quot;Delega attività e problemi&quot; nell’area Home per gli utenti con una licenza Revisione o superiore per delegare i loro elementi di lavoro.

* Indica nella Home e nell’area Assegnazioni delle intestazioni di attività e problemi che gli elementi sono delegati ad altri.

* Notifiche degli eventi nell’area Configura e notifiche e-mail nel profilo utente per controllare le notifiche e-mail sul lavoro delegato


>[!NOTE]
>
>Solo gli utenti con una licenza Revisione o superiore possono delegare il proprio lavoro ad altri. Il lavoro può essere delegato a qualsiasi utente, indipendentemente dal suo livello di accesso. Gli utenti delegati ricevono le stesse autorizzazioni degli assegnatari per gli elementi delegati. Se queste autorizzazioni sono inferiori alla configurazione del livello di accesso di un utente, agli utenti delegati potrebbe essere impedito di eseguire alcune delle attività sulle attività e sui problemi loro delegati.


Per ulteriori informazioni, consulta [Panoramica sulle attività e sui problemi dei delegati](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## Nuova esperienza durante la conversione di un problema in un’attività

Per rendere l’utilizzo di Workfront coerente con la nuova esperienza Workfront, abbiamo riprogettato l’interfaccia per convertire un problema in un’attività.

Questo aggiornamento include:

* Interfaccia utente aggiornata che corrisponde al resto della nuova esperienza Workfront.

* Accesso per convertire un problema in attività da un elenco o da un report.

* I moduli personalizzati predefiniti definiti nell’area Impostazioni attività del progetto di destinazione aggiunto alla nuova attività.


Per ulteriori informazioni, consulta [Convertire un problema in un’attività in Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Nuova esperienza durante la conversione di un problema in un progetto senza modello

Per rendere il tuo utilizzo di Workfront coerente con la nuova esperienza Workfront, abbiamo riprogettato l’interfaccia per convertire un problema in un progetto senza utilizzare un modello.

Oltre a un’interfaccia utente aggiornata che corrisponde al resto della nuova esperienza Workfront, è stata aggiunta la possibilità di convertire un problema in progetti vuoti da un elenco o da un rapporto.

Per ulteriori informazioni, consulta [Convertire un problema in un progetto in Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Applicazione di tag avanzati nel flusso di aggiornamento

Sono stati migliorati i tag degli utenti nel flusso di aggiornamento quando crei un nuovo aggiornamento o rispondi a uno esistente. Ora, quando si assegna un tag a un utente per includerlo in un aggiornamento, oltre al nome e all’avatar, vengono visualizzati anche il Ruolo principale e l’e-mail. Questo aiuta a distinguere tra più utenti con nomi simili o identici.

Per ulteriori informazioni, consulta [Assegna tag ad altri utenti in caso di aggiornamenti](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Nuova sintassi per i calcoli nei campi personalizzati

Per prepararti ai miglioramenti futuri che ti aiuteranno ad aggiungere calcoli ai moduli personalizzati, abbiamo standardizzato la sintassi per i campi di riferimento che aggiungi a un calcolo. È facile utilizzare questa nuova sintassi perché il sistema la inserisce automaticamente quando si inizia a digitare il nome di un campo e quindi a selezionarlo.

Per ulteriori informazioni, consulta la sezione &quot;Generare il calcolo per il campo personalizzato calcolato&quot; in [articolo Aggiungere dati calcolati a un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Informazioni accurate quando due utenti con un ruolo comune sono coinvolti in un processo di approvazione

Per garantire la precisione dei dati per l&#39;approvazione del lavoro, è stata apportata una modifica alla modalità di registrazione delle informazioni di approvazione su un elemento quando all&#39;elemento è associato un processo di approvazione con più ruoli.

Alcuni processi di approvazione richiedono l’approvazione da due ruoli diversi e due approvatori diversi potrebbero avere uno di questi ruoli in comune. In questo caso, dopo aver preso le decisioni di approvazione, Workfront registra ogni approvatore e il relativo ruolo associato al processo di approvazione.

Prima di questa modifica, entrambe le approvazioni erano registrate per il secondo utente perché condivideva uno dei ruoli di approvazione con il primo approvatore. In questo caso, il secondo approvatore stava sovrascrivendo le informazioni del primo approvatore.

Per ulteriori informazioni sui processi di approvazione in Workfront, consulta [Panoramica del processo di approvazione](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Le ore di allocazione non verranno più rimosse quando si apportano modifiche alle assegnazioni

>[!NOTE]
>
>Questa funzione era stata originariamente pianificata per il rilascio con la versione 22.2. È stato rilasciato in produzione il 21 aprile 2022.


Per garantire la precisione dei dati, è stata apportata una modifica per mantenere le ore di allocazione e le ore pianificate dell&#39;attività invariate quando si apportano modifiche alle assegnazioni dell&#39;attività.

Sono state apportate le seguenti modifiche alle attività con un tipo di durata semplice:

* Le ore pianificate vengono mantenute quando si rimuovono tutti gli assegnatari.

* Le singole allocazioni di assegnazione vengono mantenute durante la sostituzione di utenti e ruoli.

* Le singole allocazioni di assegnazione vengono mantenute nel ruolo quando si rimuove l&#39;utente. (Rimosso dalla versione. Ora, le ore pianificate saranno impostate su 0 dopo la rimozione di tutti gli assegnatari.)


Per ulteriori informazioni sulle ore pianificate, vedi [Panoramica sulle ore pianificate](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Miglioramenti alle schede madri

Sono stati aggiunti i seguenti miglioramenti alle schede madri Adobe Workfront:

* Opzioni di filtro: ora puoi filtrare per data di scadenza o stato su una bacheca. Il filtro è stato aggiornato anche con sezioni comprimibili per separare le opzioni.

* Scheda archivio: ora è possibile archiviare una scheda mentre si è nella scheda, invece di dover passare alla dashboard delle schede.

* Aggiungere un team a una bacheca - Quando si cerca i membri, è possibile aggiungere un intero team. La scelta di un team aggiunge tutti i membri del team alla bacheca.

* Rilascia zone nelle colonne: quando si trascina una scheda da una colonna di bacheca a un’altra, ora viene visualizzata una &quot;zona di rilascio&quot; grigia nel punto in cui verrà posizionata la scheda. In precedenza non esisteva un indicatore visivo del posizionamento della scheda.

* Schede collegate - È ora possibile aggiungere schede connesse ad attività e problemi di Workfront. Se si aggiorna il nome, la descrizione o l’assegnatario nella scheda o nell’attività, verranno aggiornati gli stessi campi nell’altra posizione.

* Campo di stato su tutte le schede: sono stati aggiunti un campo di stato e un pulsante Contrassegna come completato sia alle schede ad hoc che a quelle connesse. Quando si fa clic su Segna come completato, lo stato cambia automaticamente in Completo.

* Converti una scheda ad hoc in una scheda collegata: ora puoi convertire una scheda ad hoc in una scheda collegata dai dettagli della scheda.

* Disconnetti scheda connessa: la disconnessione di una scheda connessa interrompe la connessione con l&#39;oggetto Workfront. La scheda rimane come scheda ad hoc sulla bacheca e l’oggetto Workfront non è interessato.

* Mappatura dello stato nelle colonne: le nuove impostazioni e i nuovi criteri delle colonne consentono di definire uno stato, un assegnatario o un tag applicato alle schede spostate in tale colonna. Inoltre, i nomi delle colonne predefiniti in una nuova bacheca sono stati modificati in Colonna 1, Colonna 2 e Colonna 3.

* Indicatore di aggiornamento del campo: ora quando salvi una scheda viene visualizzato un indicatore che indica che gli aggiornamenti sono stati salvati.


Per ulteriori informazioni, consulta [Introduzione alle bacheche in Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Condividere cartelle solo nei primi cinque livelli di una gerarchia di cartelle

Per garantire le migliori prestazioni agli utenti che condividono cartelle, attualmente la condivisione è limitata ai primi cinque livelli di una gerarchia di cartelle su un oggetto.

Ogni cartella al sesto livello o inferiore eredita le configurazioni di condivisione dalla cartella direttamente al di sopra di essa.

Per ulteriori informazioni sulla condivisione delle cartelle, vedere [Condivisione di una cartella documenti di primo livello](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Campagne Workfront (Beta): un nuovo modo di gestire il tuo lavoro

>[!NOTE]
>
>Questa funzione dovrebbe essere rimossa dall’anteprima il 9 gennaio 2023. Per ulteriori informazioni, vedere [Pagina di panoramica sulla versione 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>Questa funzione non sarà inclusa nella versione di produzione 22.3. Verrà rilasciato in produzione con una versione futura.


>[!NOTE]
>
>Questa funzionalità è disponibile solo come versione beta ed è attualmente in costruzione. Continueremo ad aggiungere funzionalità per il flusso di lavoro di Campaign con le versioni future. La partecipazione al programma beta per le campagne Workfront è volontaria.

Stiamo introducendo un nuovo oggetto in Adobe Workfront che ha il potenziale per cambiare il modo in cui gestisci il lavoro.

Workfront Campaigns consente di organizzare progetti da diversi portfolio e programmi in un nuovo contenitore di lavoro. Questo nuovo contenitore si evolverà nelle versioni future per includere alla fine tutti gli oggetti di lavoro attualmente gestiti in silos separati.

Questa versione include le seguenti funzioni:

* Un nuovo oggetto Workfront denominato Campaign

* Una nuova area Campagne (Beta) nel menu principale

* Elenco di campagne nell’area Campagne

* Una pagina Dettagli campagna che visualizza informazioni aggiuntive su una campagna

* Possibilità di aggiungere progetti a una campagna

* Possibilità di modificare le informazioni su una campagna

* Possibilità di rinominare l’oggetto Campaign dal modello di layout

  Gli amministratori di sistema e di gruppi di Workfront possono aggiungere l’area Campagne (Beta) nel menu principale di un modello di layout. Questo lo rende disponibile a tutti gli utenti assegnati al modello. Una volta disponibile, chiunque in Workfront può creare una campagna.




