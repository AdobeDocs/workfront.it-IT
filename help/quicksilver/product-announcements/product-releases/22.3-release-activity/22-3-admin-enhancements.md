---
title: Miglioramenti dell’amministratore 2.3
description: Miglioramenti dell’amministratore 2.3
author: Luke
draft: false
feature: Product Announcements
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# Miglioramenti dell’amministratore 2.3

Questa pagina descrive tutti i miglioramenti apportati dall’amministratore all’ambiente di anteprima con la versione 22.3. Questi miglioramenti sono stati resi disponibili la settimana dell’11 luglio 2022. Per un elenco di tutte le modifiche disponibili con la versione 22.3, vedi [Panoramica sulla versione 22.3](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Integrare Adobe Workfront con JumpSeat

È ora possibile integrare JumpSeat con Workfront per creare una guida personalizzata all’interno del prodotto per i propri utenti. Per abilitare l’integrazione, devi disporre di una licenza Enterprise Adobe Workfront e di un abbonamento JumpSeat attivo.

Per ulteriori informazioni, consulta [Configurare l’integrazione JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Impostazioni predefinite di prova spostate in Workfront

È ora possibile modificare le seguenti impostazioni di bozza nell’area di installazione di Workfront:

* Impostazioni predefinite bozza

* Impostazioni delle decisioni di prova

Per ulteriori informazioni, consulta [Configurare le impostazioni di bozza predefinite](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Utilizzare gli stati sbloccati in un processo di approvazione

**Nota:** Rimosso dalla versione 22.3 Production . Questa funzione verrà rilasciata in Produzione il 15 settembre 2022.

Per ottenere un maggiore controllo sui processi e gli stati di approvazione del sistema, abbiamo reso possibile creare un processo di approvazione basato sullo stato di un sistema sbloccato. Inoltre, ora puoi sbloccare qualsiasi stato già utilizzato in un processo di approvazione.

In precedenza, era necessario bloccare lo stato di un sistema utilizzato in un processo di approvazione. Ciò lo ha reso disponibile per tutti i gruppi, senza la possibilità di rimuoverlo o rinominarlo, in modo che gli amministratori dei gruppi non potessero semplificare l&#39;elenco degli stati del loro gruppo in base alle loro esigenze specifiche.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Creazione di un processo di approvazione per gli elementi di lavoro](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Creare o modificare uno stato](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [Stati bloccati e sbloccati a livello di sistema](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## Aggiungere un file PDF a un modulo personalizzato

Stiamo continuando ad aiutarti a rendere i moduli personalizzati più visivi e informativi con i nuovi widget per risorse che puoi aggiungere, ad esempio immagini e video. Ora è possibile aggiungere un collegamento a un file PDF a un modulo personalizzato. Quando il modulo è associato a un oggetto, gli utenti che lavorano con esso possono visualizzare e interagire con PDF dall’interno del modulo.

Per ulteriori informazioni, consulta [Aggiungere o modificare un’immagine o un altro widget di risorse in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Nell’editor per il calcolo dei campi del modulo personalizzato vengono visualizzate informazioni di errore

>[!NOTE]
>
>Funzione temporaneamente non disponibile. Questa pagina verrà aggiornata quando la funzione sarà disponibile.

La modifica dei calcoli per i campi personalizzati è ora più semplice grazie alle utili informazioni di errore indicate direttamente nel calcolo. Durante la creazione di un campo calcolato in un modulo personalizzato, gli errori vengono evidenziati in rosa. Quando passi il cursore del mouse sulla parte evidenziata, viene visualizzata una descrizione del problema.

Per ulteriori informazioni, consulta [Aggiungere dati calcolati a un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Personalizzazione dell’intestazione del progetto

In qualità di amministratore di gruppo o di Workfront, è ora possibile personalizzare i campi visualizzati nell’intestazione di un progetto quando si utilizza un modello di layout.

Questo aggiornamento include i seguenti miglioramenti:

* Rimuovi i campi esistenti dall’intestazione del progetto.

* Aggiungi nuovi campi Panoramica progetto non modificabili. Non è possibile aggiungere campi o campi personalizzati che è possibile modificare. I campi modificabili attualmente nell’intestazione del progetto possono rimanere nell’intestazione.

* L’intestazione dell’oggetto può includere fino a cinque campi.


Prima di questa versione, i campi nelle intestazioni dell’oggetto non potevano essere personalizzati.

Per ulteriori informazioni, consulta [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Controllo creazione di un progetto vuoto

In qualità di amministratore di sistema o di gruppo, è ora possibile controllare se gli utenti possono creare progetti vuoti senza utilizzare un modello. Nell’area Preferenze progetto di Configurazione è stata introdotta una nuova impostazione che consente di disattivare la creazione di progetti vuoti nelle aree seguenti:

* Dall’opzione Nuovo progetto in un elenco di progetti

* Durante la conversione di un problema in un progetto dalla pagina del problema


La nuova impostazione è &quot;Consenti agli utenti di creare progetti senza utilizzare un modello&quot; ed è abilitata per impostazione predefinita.

**Nota:** Gli utenti possono comunque convertire un’attività in un progetto vuoto.

Per ulteriori informazioni, consulta [Configurare le preferenze del progetto a livello di sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Disattivare un gruppo dalla pagina Gruppi

Recentemente, abbiamo aggiunto la possibilità di disattivare e riattivare i gruppi. Per rendere l’azione più rapida e semplice, l’abbiamo aggiunta alla pagina di un gruppo. Ora, dopo aver fatto clic sul nome di un gruppo per passare alla relativa pagina, puoi selezionare il menu Altro ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) accanto al nome del gruppo, selezionare Disattiva o Riattiva.

In precedenza era possibile disattivare o riattivare un gruppo solo utilizzando la casella di controllo È attivo nella pagina Dettagli del gruppo.

Per ulteriori informazioni, consulta [Disattivare o riattivare un gruppo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Aggiungere video ai moduli personalizzati

È ora possibile fornire una nuova modalità di informazioni, interesse visivo e creatività a un modulo personalizzato aggiungendo un video. Quando il modulo è associato a un oggetto, gli utenti che lavorano con esso possono riprodurre il video in qualsiasi momento.

In precedenza era possibile aggiungere solo campi e immagini basati su testo a un modulo personalizzato.

Per ulteriori informazioni, consulta [Aggiunta o modifica di un widget di risorsa immagine o video in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

