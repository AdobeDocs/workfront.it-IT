---
product-area: projects;user-management
keywords: allega,applica
navigation-topic: work-with-custom-forms
title: Aggiungere un modulo personalizzato a un oggetto
description: È possibile aggiungere un modulo personalizzato esistente a uno qualsiasi degli oggetti elencati di seguito. Un modulo personalizzato contiene campi personalizzati in cui è possibile memorizzare informazioni sull'oggetto.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 2%

---

# Aggiungere un modulo personalizzato a un oggetto

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

È possibile aggiungere un modulo personalizzato esistente a uno qualsiasi degli oggetti elencati di seguito. Un modulo personalizzato contiene campi personalizzati in cui è possibile memorizzare informazioni sull&#39;oggetto.

* Progetti (inclusi casi aziendali)
* Attività
* Problemi
* Aziende
* Portfolio
* Programmi
* Documenti
* Utenti
* Iterazioni
* Spese
* Record di fatturazione

È possibile aggiungere un modulo personalizzato solo ai tipi di oggetti per i quali è stato creato.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire le azioni descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Licenza Adobe Workfront</td> 
  <td> <p>Nuovo: Collaboratore o versione successiva </p>
 <p>oppure</p> 
<p>Corrente: richiesta o successiva </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso agli oggetti per i quali si gestiscono i moduli personalizzati</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Consente di gestire le autorizzazioni per l'oggetto al quale si desidera allegare un modulo personalizzato.</p> <p>Visualizzare o accedere ad altre autorizzazioni per il modulo personalizzato, con l'autorizzazione per <b>Allega a dati personalizzati</b> oggetti (progetti, attività e problemi). Per ulteriori informazioni, consulta <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Condividere un modulo personalizzato</a>.</p> <p>Importante: se non si dispone di una licenza Pianificazione con accesso amministrativo a Custom Forms, è necessario disporre di autorizzazioni specifiche per visualizzare almeno il modulo personalizzato, come descritto in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Condividere un modulo personalizzato</a>. Queste autorizzazioni devono essere concesse anche se il modulo è visibile a livello di sistema. </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

L’amministratore di Workfront o un utente con una licenza Pianificazione e l’accesso amministrativo ai moduli personalizzati deve creare moduli personalizzati nel tuo ambiente prima di poterli aggiungere agli oggetti. Per ulteriori informazioni, consulta [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Aggiungere un modulo personalizzato a un oggetto

È possibile aggiungere un modulo personalizzato a un oggetto in due modi:

* [Aggiungere un modulo personalizzato a un oggetto modificando l&#39;oggetto](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Aggiungere un modulo personalizzato a un oggetto dall&#39;area Dettagli](#add-a-custom-form-to-an-object-from-the-details-area)

### Aggiungere un modulo personalizzato a un oggetto modificando l&#39;oggetto {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Passare all&#39;oggetto in cui si desidera aggiungere il modulo personalizzato.
1. Fai clic su **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Modifica** ![](assets/edit-icon.png).
1. Clic **Forms personalizzato** > **Aggiungi Forms**, quindi seleziona fino a 10 moduli dal menu a discesa.

1. (Facoltativo) Aggiorna le informazioni nei campi modificabili del modulo personalizzato.

   È necessario aggiornare tutti i campi obbligatori nei moduli aggiunti.

1. Fai clic su **Salva**.

### Aggiungere un modulo personalizzato a un oggetto dall&#39;area Dettagli {#add-a-custom-form-to-an-object-from-the-details-area}

1. Passare all&#39;oggetto in cui si desidera aggiungere il modulo personalizzato.
1. Fai clic su **`<Object type>`Dettagli** nel pannello a sinistra. Ad esempio, fai clic su **Dettagli progetto** per aggiungere moduli personalizzati a un progetto o **Dettagli problema** per aggiungere moduli personalizzati a un problema.
1. Fai clic su **Aggiungi modulo personalizzato** nell’angolo in alto a destra, quindi seleziona fino a 10 moduli personalizzati dall’elenco visualizzato.

   Se il modulo contiene campi obbligatori contrassegnati da un asterisco rosso, non è necessario completarli in questo momento.

   I moduli selezionati vengono automaticamente allegati all&#39;oggetto.

1. (Facoltativo) Aggiorna le informazioni nei campi personalizzati del modulo, quindi fai clic su **Salva modifiche**.

## Più moduli personalizzati su un oggetto

È possibile aggiungere fino a 10 moduli personalizzati a un determinato oggetto, consentendo di rendere i campi disponibili per alcuni utenti e non per altri o di soddisfare meglio i requisiti di modulo di più progetti.

**Esempio:** Se un progetto esistente dispone già di un modulo personalizzato e sono necessari più campi personalizzati per questo progetto, che esistono in un altro modulo personalizzato, è possibile aggiungere al progetto un secondo modulo con i campi aggiuntivi, anziché aggiungere i campi al modulo personalizzato esistente.

## Aggiungere un modulo personalizzato a più oggetti in blocco

È possibile aggiungere moduli personalizzati a più oggetti selezionandoli in un elenco.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>L’aggiunta di moduli personalizzati agli oggetti è identica per tutti gli oggetti ad eccezione dei progetti.
>
>Per informazioni sull’aggiunta di moduli personalizzati a progetti in blocco, consulta l’articolo [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).


1. Passare a un elenco di oggetti.
1. Selezionare più oggetti nell&#39;elenco.

1. Fai clic su **Altro** menu ![](assets/more-icon.png), quindi fare clic su **Modifica** icona  ![](assets/edit-icon.png).

   Oppure

   Fai clic su **Modifica** icona ![](assets/edit-icon.png) nella parte superiore dell’elenco.
1. Clic **Forms personalizzato** nel pannello a sinistra.
1. nel **Effettua una selezione** selezionare il modulo che si desidera associare a tutti gli oggetti selezionati.

   >[!NOTE]
   >
   >Se non è possibile trovare il modulo nel menu a discesa, significa che il modulo è già associato ad almeno uno degli oggetti. Determinare l&#39;oggetto ed eliminarlo dalla selezione prima di aggiungere il modulo agli oggetti rimanenti.


1. Fai clic su **Salva modifiche**.

   Se il modulo contiene campi obbligatori contrassegnati da un asterisco rosso, non è necessario completarli in questo momento.
