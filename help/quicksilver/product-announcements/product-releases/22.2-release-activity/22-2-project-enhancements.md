---
title: 22.2 Miglioramenti al progetto
description: 22.2 Miglioramenti al progetto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 43ea91db-d6f2-4218-9261-580a7e5b31d0
source-git-commit: 8425f8be7d30d36986ac1c062603e680c69902c6
workflow-type: tm+mt
source-wordcount: '1093'
ht-degree: 1%

---

# 22.2 Miglioramenti al progetto

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di anteprima con la versione 22.2 di. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la settimana del 4 aprile 2022. Per un elenco di tutte le modifiche disponibili con la versione 22.2, vedere [Panoramica sulla versione 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Le schede madri Adobe Workfront sono ora disponibili.

Le bacheche sono strumenti flessibili che consentono la collaborazione in team fornendo l’accesso a una bacheca condivisa contenente colonne e schede.

Utilizzando le bacheche è possibile:

* Impostazione rapida di un&#39;area attività con più colonne
* Configurare le colonne per mostrare uno stato o una categoria
* Aggiungi altri utenti alla bacheca e assegnali alle schede
* Aggiungi rapidamente schede e elenchi di controllo aperti

Tieni presente che le schede su una bacheca non sono collegate a oggetti ed elementi di lavoro in Adobe Workfront.

Un amministratore di sistema deve abilitare le Schede nei modelli di layout per rendere l’opzione disponibile a tutti gli utenti nel menu principale.

Per ulteriori informazioni, vedere [Panoramica delle bacheche](../../../agile/boards-overview.md).

## Ulteriori miglioramenti alle schede madri Workfront

Sono ora disponibili i seguenti miglioramenti aggiuntivi per le schede madri Workfront:

* Assegnare tag alle schede su schede

  Ora puoi categorizzare le schede sulla tua bacheca con tag codificati per colore. I tag consentono di identificare rapidamente le schede. Puoi anche ordinare la bacheca in base ai tag applicati.

* Gestione schede su Bacheche

  Abbiamo aggiunto le seguenti funzioni per aiutarti a gestire le schede sulla tua bacheca:

   * Copiare una scheda: crea una copia di una scheda esistente sulla bacheca.
   * Spostare una scheda: sposta rapidamente le schede nella parte superiore o inferiore di una bacheca con le nuove opzioni di menu Superiore a colonna e Inferiore a colonna.

* Cerca nelle bacheche

  Abbiamo aggiunto una barra di ricerca per aiutarti a cercare tutte le schede sulla tua bacheca.

* Impostare una data di scadenza per una scheda in Bacheche

  Ora puoi impostare una data di scadenza per le singole schede sulla tua bacheca.

Per ulteriori informazioni, vedere [Introduzione alle bacheche in Adobe Workfront](../../../agile/get-started-with-boards/get-started-with-boards.md).

## Opzione Annulla per Aggiorna post

È ora più facile rilevare gli errori durante la pubblicazione di un aggiornamento. La finalizzazione di un commento nella scheda Aggiorna di un oggetto ora crea una finestra pop-up per 7 secondi che consente di annullare il post e tornare alla modifica prima che il sistema lo indichi con marca temporale o invia e-mail e notifiche in-app. Se salti la finestra pop-up, esci dalla pagina o attendi 7 secondi prima che la finestra si interrompa, il post verrà creato normalmente.

Per ulteriori informazioni, vedere [Aggiorna lavoro](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Esperienza aggiornata durante la copia e lo spostamento dei problemi

Per rendere l’utilizzo di Workfront coerente con la nuova esperienza Adobe Workfront, abbiamo riprogettato l’interfaccia per copiare e spostare i problemi. Questa funzione è attualmente disponibile quando si copia o si sposta un singolo problema oppure quando si copiano o si spostano problemi in blocco da un elenco o da un rapporto.

Alcuni dei miglioramenti apportati a questa nuova interfaccia includono:

* Tutte le informazioni da aggiornare prima che lo spostamento venga visualizzato in una pagina continua.
* Workfront controlla se hai accesso al progetto di destinazione subito dopo aver scelto il progetto. Prima di questo miglioramento, Workfront ti aveva avvisato che non disponi dell’accesso corretto dopo aver confermato lo spostamento, che ha comportato passaggi aggiuntivi e che lo spostamento non era consentito.
* Possibilità di richiedere l’accesso per un progetto in cui si desidera spostare i problemi senza uscire dalla casella Sposta attività.
* Possibilità di rimuovere elementi (assegnazioni, avanzamento, documenti, autorizzazioni, aggiornamenti) da un problema quando lo si sposta in un&#39;altra posizione. Questa funzionalità in precedenza era disponibile solo per la copia dei problemi.
* Possibilità di selezionare un’attività di destinazione oltre a un progetto di destinazione durante la copia di un problema.

Per ulteriori informazioni sullo spostamento o sulla copia dei problemi, vedi i seguenti articoli:

* [Problemi relativi alla copia](../../../manage-work/issues/manage-issues/copy-issues.md)
* [Sposta i problemi](../../../manage-work/issues/manage-issues/move-issues.md)

## Nuova esperienza durante la copia di un progetto

Per rendere l’utilizzo di Workfront coerente con la nuova esperienza Adobe Workfront, abbiamo riprogettato l’interfaccia per copiare i progetti. Questa funzione è attualmente disponibile quando si copia un progetto dalla pagina del progetto o quando si copia un progetto da un elenco o da un rapporto. Prima di questo aggiornamento era possibile copiare un progetto solo dalla pagina del progetto.

Per ulteriori informazioni, vedere [Copiare un progetto](../../../manage-work/projects/manage-projects/copy-project.md).

## Possibilità di gestire progetti da elenchi e report da un nuovo menu Altro

È stato aggiunto un nuovo menu Altro negli elenchi e nei rapporti dei progetti per consentire di eseguire le seguenti azioni da queste aree:

* Per più progetti alla volta:
* Ricalcola la timeline
* Ricalcola Finanze
* Ricalcolare Espressioni Customizzate
* Per un singolo progetto:
* Allega Modello
* Esporta in MS Project
* Iscrizione

Per ulteriori informazioni, consulta i seguenti articoli:

* [Ricalcolare le sequenze temporali del progetto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)
* [Ricalcola dati finanziari progetto](../../../manage-work/projects/project-finances/recalculate-project-finances.md)
* [Modifica informazioni nei campi modulo personalizzati](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)
* [Allega un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)
* [Esporta un progetto in Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Iscriviti agli elementi in Adobe Workfront](../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Mantieni gli utenti sul dashboard, elenco o rapporto dopo la conversione del problema in progetto

Per aumentare l’efficienza ed eliminare il numero di clic, è stato introdotto un miglioramento durante la conversione dei problemi in progetti da un elenco, un rapporto o una dashboard.

Gli utenti rimangono nell’elenco, nel report o in un dashboard dopo aver convertito un problema in un progetto invece di essere reindirizzati alla pagina del progetto. Al termine della conversione, viene visualizzata una notifica di successo con il collegamento al progetto, per consentirti di passare facilmente al progetto, se necessario.

Per ulteriori informazioni, vedere [Convertire un problema in un progetto in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Le ore di allocazione non verranno più rimosse quando si apportano modifiche alle assegnazioni

>[!NOTE]
>
>Questa funzione era stata originariamente pianificata per il rilascio con la versione 22.2. Sarà rilasciato in produzione il 21 aprile 2022.

Per garantire la precisione dei dati, è stata apportata una modifica per mantenere le ore di allocazione e le ore pianificate dell&#39;attività invariate quando si apportano modifiche alle assegnazioni dell&#39;attività.

Sono state apportate le seguenti modifiche alle attività con un tipo di durata semplice:

* Le ore pianificate vengono mantenute quando si rimuovono tutti gli assegnatari.
* Le singole allocazioni di assegnazione vengono mantenute durante la sostituzione di utenti e ruoli.
* Le singole allocazioni di assegnazione vengono mantenute nel ruolo quando si rimuove l&#39;utente. (Rimosso dalla versione. Ora, le ore pianificate saranno impostate su 0 dopo la rimozione di tutti gli assegnatari.)

Per ulteriori informazioni sulle ore pianificate, vedi [Panoramica sulle ore pianificate](../../../manage-work/tasks/task-information/planned-hours.md).

## Condividere cartelle solo nei primi cinque livelli di una gerarchia di cartelle

>[!NOTE]
>
>Questa funzione non è al momento disponibile. Questa nota sulla versione verrà aggiornata quando la funzione sarà disponibile in Produzione.

Per garantire le migliori prestazioni agli utenti che condividono cartelle, attualmente la condivisione è limitata ai primi cinque livelli di una gerarchia di cartelle su un oggetto.

Ogni cartella al sesto livello o inferiore eredita le configurazioni di condivisione dalla cartella direttamente al di sopra di essa.

Per ulteriori informazioni sulla condivisione di cartelle, vedere [Condividere una cartella di documenti](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

