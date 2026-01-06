---
product-area: projects;user-management
keywords: allega,applica
navigation-topic: work-with-custom-forms
title: Aggiungere un modulo personalizzato a un oggetto
description: È possibile aggiungere un modulo personalizzato esistente a uno qualsiasi degli oggetti elencati di seguito. Un modulo personalizzato contiene campi personalizzati in cui è possibile memorizzare informazioni sull'oggetto.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 4%

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
* Gruppi
* Iterazioni
* Spese
* Record di fatturazione

È possibile aggiungere un modulo personalizzato solo ai tipi di oggetti per i quali è stato creato.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Licenza Adobe Workfront</td> 
  <td> <p>Collaboratore o versione successiva</p>
 <p>Richiedi o superiore</p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso agli oggetti per i quali si gestiscono i moduli personalizzati</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Consente di gestire le autorizzazioni per l'oggetto al quale si desidera allegare un modulo personalizzato.</p> <p>Autorizzazioni di visualizzazione o superiori per il modulo personalizzato, con autorizzazione per <b>Allega a dati personalizzati</b> oggetti (progetti, attività e problemi).</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfront license</td> 
  <td> <p>New: Contributor or higher </p>
 <p>or</p> 
<p>Current: Request or higher </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the objects for which you manage custom forms</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the object for which you want to attach a custom form.</p> <p>View or higher permissions to the custom form, with permission to <b>Attach to Custom Data</b> objects (projects, tasks, and issues). For more information, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Share a custom form</a>.</p> <p>Important: If you do not have a Plan license with administrative access to  Custom  Forms, you must have specific permissions to at least view the custom form, as described in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Share a custom form</a>. These permissions must be granted to you even if the form is visible system-wide. </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Prerequisiti

L’amministratore di Workfront o un utente con una licenza Pianificazione e l’accesso amministrativo ai moduli personalizzati deve creare moduli personalizzati nel tuo ambiente prima di poterli aggiungere agli oggetti. Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Aggiungere un modulo personalizzato a un oggetto

È possibile aggiungere un modulo personalizzato a un oggetto in due modi:

* [Aggiungere un modulo personalizzato a un oggetto modificando l&#39;oggetto](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Aggiungere un modulo personalizzato a un oggetto dall&#39;area Dettagli](#add-a-custom-form-to-an-object-from-the-details-area)

### Aggiungere un modulo personalizzato a un oggetto modificando l&#39;oggetto {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Passare all&#39;oggetto in cui si desidera aggiungere il modulo personalizzato.
1. Fai clic sul menu **Altro** ![](assets/more-icon.png), quindi fai clic su **Modifica** ![](assets/edit-icon.png).
1. Fai clic su **Forms** personalizzato > **Aggiungi Forms**, quindi seleziona fino a 10 moduli dal menu a discesa.

1. (Facoltativo) Aggiorna le informazioni nei campi modificabili del modulo personalizzato.

   È necessario aggiornare tutti i campi obbligatori nei moduli aggiunti.

1. Fai clic su **Salva**.

### Aggiungere un modulo personalizzato a un oggetto dall&#39;area Dettagli {#add-a-custom-form-to-an-object-from-the-details-area}

1. Passare all&#39;oggetto in cui si desidera aggiungere il modulo personalizzato.
1. Fai clic sulla sezione **`<Object type>`Dettagli** nel pannello a sinistra. Ad esempio, fai clic su **Dettagli progetto** per aggiungere moduli personalizzati a un progetto oppure su **Dettagli problema** per aggiungere moduli personalizzati a un problema.
1. Fai clic sul campo **Aggiungi modulo personalizzato** nell&#39;angolo superiore destro, quindi seleziona fino a 10 moduli personalizzati dall&#39;elenco visualizzato.

   Se il modulo contiene campi obbligatori contrassegnati da un asterisco rosso, non è necessario completarli in questo momento.

   I moduli selezionati vengono automaticamente allegati all&#39;oggetto.

1. (Facoltativo) Aggiorna le informazioni nei campi personalizzati del modulo, quindi fai clic su **Salva modifiche**.

## Più moduli personalizzati su un oggetto

È possibile aggiungere fino a 10 moduli personalizzati a un determinato oggetto, consentendo di rendere i campi disponibili per alcuni utenti e non per altri o di soddisfare meglio i requisiti di modulo di più progetti.

**Esempio:** se un progetto esistente ha già un modulo personalizzato e sono necessari altri campi personalizzati per questo progetto, che esistono in un altro modulo personalizzato, è possibile aggiungere al progetto un secondo modulo con i campi aggiuntivi, anziché aggiungere i campi al modulo personalizzato esistente.

## Aggiungere un modulo personalizzato a più oggetti in blocco

È possibile aggiungere moduli personalizzati a più oggetti selezionandoli in un elenco.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>L’aggiunta di moduli personalizzati agli oggetti è identica per tutti gli oggetti ad eccezione dei progetti.
>
>Per informazioni sull&#39;aggiunta di moduli personalizzati a progetti in blocco, vedere l&#39;articolo [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).


1. Passare a un elenco di oggetti.
1. Selezionare più oggetti nell&#39;elenco.

1. Fai clic sul menu **Altro** ![](assets/more-icon.png), quindi fai clic sull&#39;icona **di** Modifica![](assets/edit-icon.png).

   Oppure

   Fai clic sull&#39;icona **Modifica** ![](assets/edit-icon.png) nella parte superiore dell&#39;elenco.
1. Fai clic su **Forms personalizzato** nel pannello a sinistra.
1. nel menu a discesa **Effettua una selezione**, seleziona il modulo da associare a tutti gli oggetti selezionati.

   >[!NOTE]
   >
   >Se non è possibile trovare il modulo nel menu a discesa, significa che il modulo è già associato ad almeno uno degli oggetti. Determinare l&#39;oggetto ed eliminarlo dalla selezione prima di aggiungere il modulo agli oggetti rimanenti.


1. Fai clic su **Salva modifiche**.

   Se il modulo contiene campi obbligatori contrassegnati da un asterisco rosso, non è necessario completarli in questo momento.
