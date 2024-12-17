---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Ripristina elementi eliminati
description: Se sei un amministratore di Workfront, puoi ripristinare progetti, attività, problemi, documenti e modelli in Adobe Workfront se sono stati eliminati negli ultimi 30 giorni. Dopo 30 giorni, questi elementi vengono eliminati definitivamente e non possono essere ripristinati.
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 2%

---

# Ripristinare elementi eliminati

<!--Audited: 12/2023-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Se sei un amministratore di Workfront, puoi ripristinare progetti, attività, problemi, documenti e modelli in Adobe Workfront se sono stati eliminati negli ultimi 30 giorni. Dopo 30 giorni, questi elementi vengono eliminati definitivamente e non possono essere ripristinati.

Quando si ripristina un oggetto, vengono ripristinati anche tutti gli oggetti e i campi figlio. Ad esempio, se ripristini un progetto, vengono ripristinate anche tutte le attività, i problemi, i documenti, le ore, le note, le assegnazioni e i dati personalizzati del progetto.

Un amministratore di gruppo può inoltre ripristinare questi oggetti per un gruppo che gestisce.

>[!IMPORTANT]
>
>* Se elimini un report, un dashboard, un utente, un gruppo, un team o un’iterazione, non è possibile ripristinarlo.
>* In un gruppo, quando un utente diverso dall&#39;amministratore del gruppo carica un documento direttamente nell&#39;area Documenti di un oggetto, solo l&#39;amministratore di Workfront può ripristinare il documento.
>
>* Se sposti un’attività o un problema e scegli di non spostare anche i documenti allegati all’attività o al problema, i documenti vengono eliminati e posizionati nel Cestino per 30 giorni. Un amministratore può ripristinarli e ricollegarli all’attività o al problema spostato. Se l’attività o il problema è stato eliminato dopo lo spostamento, i documenti vengono ripristinati nell’area Documenti della pagina utente dell’amministratore che li ripristina.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>Oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informazioni recuperate quando si ripristina un progetto, un&#39;attività o un problema

Quando ripristini un progetto, un’attività o un problema, vengono recuperate anche le seguenti informazioni associate:

* Commenti e risposte nell’area Aggiornamenti
* Approvazioni
* Assegnazioni
* Moduli personalizzati
* Configurazione coda
* Casi aziendali, inclusi scorecard, obiettivi e rischi
* Team di progetto
* Date
* Problemi
* Attività
* Sottoattività
* Stati
* Informazioni finanziarie:

   * Record di fatturazione
   * Tariffe di fatturazione
   * Spese

* Informazioni sequenza temporale:

   * Predecessori
   * Vincoli delle attività
   * Tipo di durata

* Linee di base

  Le previsioni delle attività vengono recuperate quando si ripristina il progetto o l&#39;attività padre, ma non quando si ripristinano le attività eliminate singolarmente.

* Ore (e ID ore)

  Se le ore vengono ripristinate sull&#39;elemento eliminato dipende dalle impostazioni scelte durante la configurazione delle preferenze per le schede orario e le ore. Per ulteriori informazioni, vedere [Configurare gli effetti sulle ore di eliminazione e ripristino di un oggetto](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* URL dell&#39;elemento

  Una volta ripristinato, l’URL dell’elemento rimane invariato. Gli utenti che hanno creato segnalibri del browser per l&#39;elemento rimangono validi.

* Accesso e autorizzazioni

  Gli utenti che avevano accesso all’elemento prima che fosse eliminato recuperano l’accesso dopo il ripristino.

* Documenti (inclusi i documenti di prova)

  Durante il ripristino di documenti e versioni di documenti, tenere presente quanto segue:

   * I documenti eliminati singolarmente possono essere ripristinati singolarmente.

     I documenti eliminati insieme al progetto, all&#39;attività o al problema principale vengono recuperati quando si ripristina il documento principale, ma non è possibile ripristinarlo singolarmente.

   * Tutte le versioni di un documento o di una bozza di documento vengono ripristinate al momento del ripristino del documento.\
     Non è possibile recuperare singole versioni di un documento o di una bozza di documento eliminate singolarmente.

## Informazioni che non vengono recuperate quando si ripristina un progetto, un’attività o un problema

Quando ripristini un progetto, un’attività o un problema, le seguenti informazioni associate non vengono recuperate insieme a esso:

* Mi piace
* Valutazioni positive
* Inserire l’indirizzo e-mail in una coda di richieste
* Preferiti

  Un progetto, un&#39;attività o un problema aggiunto al menu Preferiti prima di essere eliminato non viene nuovamente visualizzato nel menu Preferiti dopo essere stato ripristinato.

* Risoluzione di oggetti

  Un oggetto di risoluzione è un problema convertito configurato con l&#39;opzione **Mantieni il problema originale e collegane la risoluzione a questa** &lt;**(progetto** o **attività)**>. Se si elimina il progetto o l&#39;attività padre, il problema non viene più identificato come oggetto di risoluzione perché non esiste più un collegamento che lo collega al progetto o all&#39;attività. Se ripristini l’elemento padre, il collegamento non viene ripristinato.

  Per ulteriori informazioni su come un amministratore di Workfront o un amministratore di gruppo configura i problemi in modo che corrispondano all&#39;oggetto di risoluzione quando viene convertito, vedere [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) e [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

  Per ulteriori informazioni sulla conversione dei problemi, vedere [Panoramica sulla conversione dei problemi in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Ripristina elementi

{{step-1-to-setup}}

1. Fai clic su **Cestino** > **Eliminato di recente**.
1. Fai clic sulla scheda **Progetti**, **Attività**, **Problemi**, **Modelli** o **Documenti**, a seconda del tipo di elemento da ripristinare.

   Per impostazione predefinita, gli elementi sono ordinati in base alla colonna **Data eliminazione**.

1. Selezionare fino a 10 elementi da ripristinare.

   Se si elimina un&#39;attività figlio, questa viene visualizzata nell&#39;elenco.

   Se si elimina un&#39;attività padre, nell&#39;elenco viene visualizzata solo l&#39;attività padre. Tuttavia, quando si ripristina un&#39;attività padre, vengono ripristinate tutte le attività figlio.

1. Fai clic su **Ripristina** per ripristinare gli elementi selezionati nella posizione originale.
1. (Facoltativo) Per visualizzare rapidamente l&#39;elemento ripristinato, seguire i passaggi descritti in [Visualizza elemento ripristinato](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   Per ulteriori informazioni su ciò che accade dopo il ripristino di un elemento, vedere la sezione [Cosa succede dopo il ripristino degli elementi](#what-happens-after-you-restore-items) in questo articolo.

## Cosa succede dopo il ripristino degli elementi {#what-happens-after-you-restore-items}

* Quando si ripristinano le attività e le sottoattività, queste vengono visualizzate nell&#39;ordine in cui erano prima di essere eliminate.

  Tuttavia, se l&#39;ordine delle altre attività cambia durante l&#39;eliminazione dell&#39;attività, è possibile che l&#39;attività venga ripristinata in fondo all&#39;elenco delle attività o delle sottoattività.

* Dopo aver ripristinato un elemento:

   * Viene visualizzato un messaggio per comunicare se l’operazione è stata completata correttamente.

     Ricevi anche una notifica e-mail. Se hai ripristinato più elementi, l’e-mail li elenca.

   * Un commento viene visualizzato nell&#39;area Aggiornamenti del progetto, dell&#39;attività o del problema e in quella dell&#39;oggetto padre.

     Ciò non si verifica quando si ripristina un documento o un modello.

## Bozze ripristinate

Quando un utente ripristina un documento che dispone di una bozza, nella pagina Attività bozza della bozza potrebbe essere visualizzato il nome del primo amministratore Workfront attivo elencato per l’istanza dell’organizzazione (in ordine di ID profilo) invece della persona effettiva che ha ripristinato la bozza.
