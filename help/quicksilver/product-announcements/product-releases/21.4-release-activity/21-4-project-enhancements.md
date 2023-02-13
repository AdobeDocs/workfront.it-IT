---
title: 21.4 Miglioramenti al progetto
description: 21.4 Miglioramenti al progetto
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 21.4 Miglioramenti al progetto

Questa pagina descrive tutti i miglioramenti apportati a Project con la versione 21.4 nell’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione la settimana del 4 ottobre 2021.

Per un elenco di tutte le modifiche disponibili con la versione 21.4, vedi [Panoramica sulla versione 21.4](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Includere immagini negli aggiornamenti

Nella scheda Aggiornamenti di un oggetto, è ora possibile aggiungere immagini facendo clic sull’icona Immagine sulla barra degli strumenti. Puoi anche trascinare un’immagine nell’area di aggiornamento. Tieni presente che l’amministratore di Workfront deve abilitare l’aggiunta di immagini prima di poter visualizzare l’icona Immagine .

È possibile aggiungere immagini sia negli aggiornamenti che nelle risposte. Una miniatura dell’immagine nell’aggiornamento indica che i destinatari possono visualizzare l’anteprima dell’immagine nel browser o scaricarla, e le notifiche e-mail e in-app mostrano che le immagini sono allegate all’aggiornamento.

In precedenza, l&#39;unico modo per condividere un&#39;immagine in Workfront era allegarla a un oggetto come documento. Le immagini aggiunte nella scheda Aggiornamenti sono disponibili solo in tale scheda e non nella scheda Documenti.

Per ulteriori informazioni, consulta [Aggiorna lavoro](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Prima che gli utenti di Workfront possano includere immagini negli aggiornamenti, questa funzione deve essere abilitata dall’amministratore di Adobe Workfront, come descritto in [Configurare le preferenze per gli aggiornamenti utente](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## Algoritmo aggiornato per le assegnazioni avanzate

Abbiamo migliorato l’algoritmo utilizzato per le assegnazioni intelligenti. Con il nuovo miglioramento, Workfront esamina le 30 assegnazioni più recenti effettuate dall’utente connesso per formulare suggerimenti quando assegna attività e problemi. L’elenco dei suggerimenti può contenere fino a 50 utenti.

Prima di questo miglioramento, Workfront stava prendendo in considerazione le assegnazioni relative alle attività principali e ad altri attributi utente relativi a tali assegnazioni quando si suggerivano gli utenti.

Per informazioni sulle assegnazioni avanzate, vedere [Panoramica delle assegnazioni intelligenti](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Nuova esperienza durante la creazione di un progetto da un modello

Per rendere coerente l’utilizzo di Workfront con la nuova esperienza Workfront, abbiamo riprogettato l’interfaccia per la creazione di un progetto da modello. La funzionalità per la creazione di un progetto utilizzando un modello non è stata modificata. Tuttavia, alcuni dei miglioramenti di questa nuova interfaccia riprogettata includono:

* Anteprima delle informazioni sul modello prima di allegarlo
* Aggiunta di modelli a un elenco di preferiti durante il processo di creazione del progetto

È stata aggiornata l’interfaccia per la creazione del progetto sia quando lo si crea da Progetti sia dall’area Modelli .

Per informazioni, [Creare un progetto utilizzando un modello](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Nuova esperienza durante l’associazione di modelli ai progetti

>[!NOTE]
>
>Questa funzione è disponibile solo nella nuova esperienza Adobe Workfront.

Per rendere coerente l’utilizzo di Workfront con la nuova esperienza Workfront, abbiamo riprogettato l’interfaccia per allegare un modello a un progetto. La funzionalità di collegamento di un modello non è stata modificata. Tuttavia, esistono alcuni dei miglioramenti di questa nuova interfaccia riprogettata che includono:

* Anteprima delle informazioni sul modello prima di allegarlo
* Aggiunta di modelli a un elenco di preferiti durante il processo di allegato
* Visualizza tutte le opzioni per la gestione delle impostazioni di modelli e progetti in un’unica pagina continua

Per informazioni, consulta [Allegare un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Valori unitari di durata e durata unificati per le attività

Per un’esperienza utente più pulita e più semplice, abbiamo unito il valore del campo Durata con l’unità di tempo per la durata. Prima di questo miglioramento, l’unità di tempo visualizzata in un campo a discesa separato dopo il campo Durata .

Oltre ai campi Durata nelle caselle Dettagli attività, Modifica attività e Nuova attività , vengono aggiornati anche i campi seguenti per corrispondere a questa esperienza:

* Campo Durata durante l&#39;esecuzione di assegnazioni avanzate
* Campo Ritardo livellamento durante la creazione o la modifica di un’attività
* Campo di frequenza durante la creazione di un’attività ricorrente (disponibile a breve)
* Campo Ritardo per l’aggiunta di un predecessore (disponibile a breve)

Per informazioni, consulta [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## Disattiva l&#39;aggiunta di problemi in linea nei progetti

Per garantire che gli utenti forniscano informazioni accurate quando aggiungono problemi ai progetti compilando un modulo per la segnalazione dei problemi, è stata introdotta una nuova impostazione che consente di gestire l’aggiunta di problemi a un progetto o alle sue attività in linea. Questa impostazione è attivata per impostazione predefinita nella nuova area Impostazioni problema della casella Modifica progetto. La sua disattivazione disattiva l’opzione Aggiungi altri problemi nella sezione Problemi di un progetto, in modo che gli utenti non possano aggiungere altri problemi nell’elenco. Gli utenti possono comunque aggiungere problemi ai progetti utilizzando l’opzione Nuovo problema nella sezione Problemi o utilizzando una coda di richiesta se è configurata per il progetto.

>[!NOTE]
>
>Questa impostazione è disponibile solo nella nuova esperienza Workfront. Gli utenti che lavorano in Workfront Classic possono comunque aggiungere problemi in linea a un progetto o alle sue attività anche se questa impostazione è stata disabilitata per il progetto da un utente che lavora nella nuova esperienza Workfront.

Per ulteriori informazioni, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

## Miglioramento della visualizzazione dei campi personalizzati per le caselle di controllo e i pulsanti di scelta

Le opzioni relative alle caselle di controllo e ai pulsanti di scelta nei moduli personalizzati sono diventate più semplici: un campo personalizzato con molte opzioni di casella di controllo o di pulsante di scelta ora viene visualizzato in più colonne della pagina. Precedentemente, venivano visualizzate in una singola colonna, che richiedeva uno scorrimento aggiuntivo per gli utenti che compilavano il modulo.

Questo dipende dal modo in cui i campi vengono posizionati nel modulo personalizzato. Se si posiziona un altro campo nella stessa riga con il campo casella di controllo o pulsante di scelta, lo spazio orizzontale delle opzioni può essere sufficiente per essere visualizzato in una singola colonna.

Per informazioni sulla compilazione di un modulo personalizzato, vedere [Modificare le informazioni nei campi modulo personalizzati](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

Per informazioni sulla creazione di un campo casella di controllo o pulsante di scelta in un modulo personalizzato, vedere le sezioni [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) e [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#configur) nell&#39;articolo [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

