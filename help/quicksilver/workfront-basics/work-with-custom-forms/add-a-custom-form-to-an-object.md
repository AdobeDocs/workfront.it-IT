---
product-area: projects;user-management
keywords: attaccare,applicare
navigation-topic: work-with-custom-forms
title: Aggiungere un modulo personalizzato a un oggetto
description: È possibile aggiungere un modulo personalizzato esistente a uno qualsiasi degli oggetti elencati di seguito. Un modulo personalizzato contiene campi personalizzati in cui è possibile memorizzare informazioni sull’oggetto.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: addcff71ff067be22e9ee80f997af545293fa5db
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 1%

---

# Aggiungere un modulo personalizzato a un oggetto

<span class="preview">Le informazioni evidenziate in questa pagina fanno riferimento a funzionalità non ancora disponibili al pubblico. È disponibile per tutti i clienti nell’ambiente Anteprima e per un gruppo selezionato di clienti nell’ambiente Produzione.</span>

È possibile aggiungere un modulo personalizzato esistente a uno qualsiasi degli oggetti elencati di seguito. Un modulo personalizzato contiene campi personalizzati in cui è possibile memorizzare informazioni sull’oggetto.

* Progetti (compresi i casi aziendali)
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

È possibile aggiungere un modulo personalizzato solo ai tipi di oggetti per i quali è stato creato il modulo.

## Requisiti di accesso

Per eseguire le azioni descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso agli oggetti per i quali si gestiscono moduli personalizzati</p> <p><b>NOTA</b></p>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Consente di gestire le autorizzazioni per l’oggetto per il quale si desidera allegare un modulo personalizzato.</p> <p>Visualizza o autorizzazioni superiori per il modulo personalizzato, con l’autorizzazione per <b>Allega a dati personalizzati</b> oggetti (progetti, attività e problemi). Per ulteriori informazioni, consulta <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Condivisione di un modulo personalizzato</a>.</p> <p>Importante: Se non si dispone di una licenza Plan con accesso amministrativo a Custom Forms, è necessario disporre di autorizzazioni specifiche per visualizzare almeno il modulo personalizzato, come descritto in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Condivisione di un modulo personalizzato</a>. Tali autorizzazioni devono essere concesse anche se il modulo è visibile a livello di sistema. </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisito

Prima di poter essere aggiunti agli oggetti, l’amministratore di Workfront o un utente con una licenza Pianifica e l’accesso amministrativo ai moduli personalizzati deve creare moduli personalizzati nell’ambiente dell’utente. Per ulteriori informazioni, consulta [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Aggiungere un modulo personalizzato a un oggetto

È possibile aggiungere un modulo personalizzato a un oggetto in due modi:

* [Aggiungere un modulo personalizzato a un oggetto modificando l’oggetto](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Aggiungere un modulo personalizzato a un oggetto dall’area Dettagli](#add-a-custom-form-to-an-object-from-the-details-area)

### Aggiungere un modulo personalizzato a un oggetto modificando l’oggetto {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Passare all’oggetto in cui si desidera aggiungere il modulo personalizzato.
1. Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Modifica** ![](assets/edit-icon.png).
1. Fai clic su **Forms personalizzato** > **Aggiungi Forms**, quindi seleziona fino a 10 moduli dal menu a discesa.

1. (Facoltativo) Aggiornare le informazioni nei campi modificabili del modulo personalizzato.

   È necessario aggiornare tutti i campi obbligatori nei moduli aggiunti.

1. Fai clic su **Salva**.

### Aggiungere un modulo personalizzato a un oggetto dall’area Dettagli {#add-a-custom-form-to-an-object-from-the-details-area}

1. Passare all’oggetto in cui si desidera aggiungere il modulo personalizzato.
1. Fai clic sul pulsante **`<Object type>`Dettagli** nel pannello a sinistra. Ad esempio, fai clic su **Dettagli progetto** per aggiungere moduli personalizzati a un progetto o **Dettagli del problema** per aggiungere moduli personalizzati a un problema.
1. Fai clic sul pulsante **Aggiungi modulo personalizzato** nell’angolo in alto a destra, quindi seleziona fino a 10 moduli personalizzati dall’elenco visualizzato.

   Se il modulo contiene campi obbligatori (contrassegnati da un asterisco rosso), non è necessario completarli in questo momento.

   I moduli selezionati vengono automaticamente collegati all’oggetto.

1. (Facoltativo) Aggiorna le informazioni nei campi personalizzati del modulo, quindi fai clic su **Salva modifiche**.

## Più moduli personalizzati su un oggetto

È possibile aggiungere fino a 10 moduli personalizzati su un dato oggetto, per consentire ad alcuni utenti di rendere disponibili i campi per altri utenti o per soddisfare meglio i requisiti dei moduli di più progetti.

**Esempio:** Se un progetto esistente dispone già di un modulo personalizzato e sono necessari più campi personalizzati in un altro modulo personalizzato, è possibile aggiungere al progetto un secondo modulo con i campi aggiuntivi, anziché aggiungere i campi al modulo personalizzato esistente, se tali campi sono necessari solo per questo progetto.

## Aggiungere un modulo personalizzato a più oggetti in blocco

È possibile aggiungere moduli personalizzati a più oggetti selezionandoli in un elenco.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
><span class="preview">Per informazioni sull’aggiunta in blocco di moduli personalizzati a progetti nell’ambiente di anteprima, consulta l’articolo [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md)</span>.


1. Passare a un elenco di oggetti.
1. Selezionare più oggetti nell’elenco.

1. Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Modifica** icona  ![](assets/edit-icon.png)oppure fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png).
1. Fai clic su **Forms personalizzato** nel pannello a sinistra.
1. Selezionare il modulo che si desidera associare a tutti gli oggetti selezionati nella **Selezione** menu a discesa.
   >[!NOTE]
   >
   >Se non è possibile trovare il modulo nel menu a discesa, almeno uno degli oggetti presenta il modulo già associato. Prima di aggiungere il modulo agli oggetti rimanenti, è necessario determinare l’oggetto selezionato ed eliminarlo dalla selezione.

1. Fai clic su **Salva modifiche**.

   Se il modulo contiene campi obbligatori (contrassegnati da un asterisco rosso), non è necessario completarli in questo momento.
