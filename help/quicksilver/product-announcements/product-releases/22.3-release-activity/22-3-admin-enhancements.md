---
title: 22.3 Miglioramenti per gli amministratori
description: 22.3 Miglioramenti per gli amministratori
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# 22.3 Miglioramenti per gli amministratori

Questa pagina descrive tutti i miglioramenti per gli amministratori apportati con la versione 22.3 all’ambiente di anteprima. Questi miglioramenti sono stati resi disponibili la settimana dell’11 luglio 2022. Per un elenco di tutte le modifiche disponibili con la versione 22.3, vedere [Panoramica sulla versione 22.3](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Integrare Adobe Workfront con JumpSeat

Ora puoi integrare JumpSeat con Workfront per creare guide personalizzate interne al prodotto per i tuoi utenti. Per abilitare l’integrazione, è necessario disporre di una licenza Enterprise di Adobe Workfront e di un abbonamento JumpSeat attivo.

Per ulteriori informazioni, vedere [Configurare l&#39;integrazione JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Impostazioni predefinite bozza spostate in Workfront

Ora è possibile modificare le seguenti impostazioni di bozza nell’area di configurazione di Workfront:

* Impostazioni predefinite bozza

* Impostazioni decisione bozza

Per ulteriori informazioni, vedere [Configurare le impostazioni di bozza predefinite](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Utilizzare gli stati sbloccati in un processo di approvazione

**Nota:** rimosso dalla versione di produzione 22.3. Questa funzione verrà rilasciata in produzione il 15 settembre 2022.

Per avere un maggiore controllo sui processi e sugli stati di approvazione nel sistema, è stato possibile creare un processo di approvazione basato sullo stato sbloccato del sistema. Inoltre, ora puoi sbloccare qualsiasi stato già utilizzato in un processo di approvazione.

In precedenza, era necessario bloccare uno stato di sistema utilizzato in un processo di approvazione. Questo lo ha reso disponibile per tutti i gruppi, senza la possibilità di rimuoverlo o rinominarlo, pertanto gli amministratori dei gruppi non hanno potuto semplificare l’elenco degli stati del gruppo in base alle loro esigenze specifiche.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Creare un processo di approvazione per gli elementi di lavoro](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Creare o modificare uno stato](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [Stati bloccati e sbloccati a livello di sistema](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## Aggiungere un file PDF a un modulo personalizzato

Stiamo continuando a aiutarti a rendere i moduli personalizzati più visivi e informativi con nuovi widget di risorse che puoi aggiungere, come immagini e video. Ora è possibile aggiungere un collegamento a un file PDF a un modulo personalizzato. Quando il modulo viene allegato a un oggetto, gli utenti che lavorano con l’oggetto possono visualizzare e interagire con il PDF dall’interno del modulo.

Per ulteriori informazioni, consulta [Aggiungere o modificare un&#39;immagine o un altro widget di risorse in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## L’editor di calcolo per i campi modulo personalizzati visualizza le informazioni sull’errore

>[!NOTE]
>
>Questa funzione non è al momento disponibile. Questa pagina verrà aggiornata quando la funzione sarà disponibile.

La modifica dei calcoli per i campi personalizzati è ora più semplice grazie alle utili informazioni sugli errori indicate direttamente nel calcolo. Durante la creazione di un campo calcolato in un modulo personalizzato, gli errori vengono evidenziati in rosa. Quando passi il cursore del mouse sulla parte evidenziata, viene visualizzata una descrizione per descrivere il problema.

Per ulteriori informazioni, vedere [Aggiungere dati calcolati a un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Personalizzazione dell’intestazione del progetto

In qualità di amministratore di Workfront o di gruppo, ora puoi personalizzare i campi visualizzati nell’intestazione di un progetto quando utilizzi un modello di layout.

Questo aggiornamento include i seguenti miglioramenti:

* Rimuovi i campi esistenti dall’intestazione del progetto.

* Aggiungere nuovi campi non modificabili per la panoramica del progetto. Non è possibile aggiungere campi personalizzati o campi modificabili. I campi modificabili che si trovano attualmente nell’intestazione del progetto possono rimanere nell’intestazione.

* L&#39;intestazione dell&#39;oggetto può includere fino a cinque campi.


Prima di questa versione, non era possibile personalizzare i campi nelle intestazioni dell’oggetto.

Per ulteriori informazioni, vedere [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Controllo creazione di un progetto vuoto

In qualità di amministratore di sistema o di gruppo, ora puoi controllare se gli utenti possono creare progetti vuoti senza utilizzare un modello. Nell’area Preferenze progetto di Configura è stata introdotta una nuova impostazione che consente di disabilitare la creazione di progetti vuoti nelle seguenti aree:

* Dall’opzione Nuovo progetto in un elenco di progetti

* Quando si converte un problema in un progetto dalla pagina del problema


La nuova impostazione è &quot;Consenti agli utenti di creare progetti senza utilizzare un modello&quot; ed è abilitata per impostazione predefinita.

**Nota:** gli utenti possono comunque convertire un&#39;attività in un progetto vuoto.

Per ulteriori informazioni, vedere [Configurare le preferenze di progetto a livello di sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Disattivare un gruppo dalla pagina Gruppi

Di recente, è stata aggiunta la possibilità di disattivare e riattivare i gruppi. Per rendere l’azione più rapida e semplice, l’abbiamo aggiunta alla pagina di un gruppo. Ora, dopo aver fatto clic sul nome di un gruppo per passare alla relativa pagina, è possibile selezionare il menu Altro ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) accanto al nome del gruppo, quindi selezionare Disattiva o Riattiva.

In precedenza, era possibile disattivare o riattivare un gruppo solo utilizzando la casella di controllo È attivo nella relativa pagina Dettagli.

Per ulteriori informazioni, vedere [Disattivare o riattivare un gruppo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Aggiungere video ai moduli personalizzati

È ora possibile aggiungere un video per fornire a un modulo personalizzato una nuova modalità di informazioni, interesse visivo e creatività. Quando il modulo viene allegato a un oggetto, gli utenti che lo utilizzano possono riprodurre il video in qualsiasi momento.

In precedenza era possibile aggiungere a un modulo personalizzato solo campi e immagini basati su testo.

Per ulteriori informazioni, consulta [Aggiungere o modificare un widget di immagini o risorse video in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

