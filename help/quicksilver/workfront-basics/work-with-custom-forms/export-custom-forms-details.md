---
title: Esportare moduli personalizzati e dettagli dell’oggetto
description: Esportare moduli personalizzati e dettagli dell’oggetto
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1670edf153e57152e51adcfbda052eb74541d931
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 1%

---

# Esportare moduli personalizzati e dettagli dell’oggetto

È possibile esportare la Panoramica e le informazioni sul modulo personalizzato dalla sezione Dettagli di un oggetto in un file PDF. È quindi possibile stampare o condividere PDF con altri utenti.

Questa funzionalità è supportata per i seguenti oggetti:

* Progetti
* Attività
* Problemi
* Portfolio
* Programmi

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>I campi nella sezione Dettagli rimossi dall’amministratore di Workfront o di gruppo utilizzando un modello di layout non vengono visualizzati.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licenza Adobe Workfront*</p> </td> 
   <td> <p>Richiesta o versione successiva di problemi</p> <p>Revisione o superiore per progetti e attività</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Visualizza o superiore per progetti, attività e problemi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorizzazioni oggetto</p> </td> 
   <td> <p>Visualizza o autorizzazioni superiori per il progetto, l'attività o il problema di cui si desidera esportare il modulo</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare, è necessario disporre di tutti i seguenti elementi:

1. Creare un modulo personalizzato per un oggetto specifico da cui si desidera esportarlo.
1. Associa il modulo personalizzato all’oggetto

   Oppure

   Avere l’accesso corretto per allegare un modulo personalizzato e modificare le informazioni sul modulo.

Per informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

Per informazioni sull’associazione dei moduli agli oggetti, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Informazioni sull’esportazione nella sezione Dettagli

L’esportazione di informazioni dalla sezione Dettagli di un oggetto è identica per tutti gli oggetti in cui è supportato.

1. Passa a un progetto, un task, un portfolio, un programma o un problema per il quale disponi almeno delle autorizzazioni di visualizzazione.
1. Fai clic sul pulsante **Elemento &quot;Dettagli&quot;** nel pannello di sinistra, ad esempio **Dettagli attività**.
1. (Facoltativo) Se all’oggetto non è associato alcun modulo personalizzato, inizia a digitare il nome di un modulo personalizzato nel **Aggiungi campo modulo personalizzato**, quindi fai clic su di esso quando viene visualizzato nell’elenco.

   È possibile aggiungere fino a 10 moduli.

1. (Facoltativo) Aggiorna le informazioni nella sezione Dettagli, quindi fai clic su **Salva modifiche**.
1. Fai clic sul pulsante **Esporta** menu a discesa nell&#39;angolo in alto a destra, seleziona **Panoramica** oppure i moduli da esportare, quindi fare clic su **Esporta**.

   Puoi anche selezionare **Seleziona tutto** per esportare l’area Panoramica e tutti i moduli personalizzati.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Possono esistere i seguenti scenari:
   >
   >   
   >   
   >   * Quando il gruppo o l’amministratore di Workfront deseleziona tutti i campi nell’area Panoramica e l’oggetto presenta moduli personalizzati collegati, la sezione Panoramica non viene visualizzata.
   >   * Quando il gruppo o l’amministratore di Workfront deseleziona tutti i campi nell’area Panoramica e l’oggetto non dispone di moduli personalizzati collegati, il menu a discesa Esporta non è visibile.
   >   * Se all’oggetto non è allegato alcun modulo personalizzato, è possibile esportare solo l’area Panoramica.
   >   * I campi personalizzati che si trovano dietro la logica e non sono visibili nel modulo non vengono esportati. Per informazioni sull’aggiunta di logica a un modulo personalizzato, consultare [Aggiungere logica di visualizzazione e ignorare la logica in un modulo personalizzato](../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md).


   Un file PDF viene prodotto e scaricato sul computer. Il file PDF contiene le seguenti informazioni:

   * Nome dell’oggetto a cui è associato il modulo
   * Nome dell’utente che ha esportato il PDF
   * Data e ora di produzione del PDF
   * Nome dei moduli esportati
   * Informazioni dai campi compilati sul modulo
