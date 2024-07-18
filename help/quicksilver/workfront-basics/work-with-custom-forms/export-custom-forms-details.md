---
title: Esportare moduli personalizzati e dettagli oggetto
description: Esportare moduli personalizzati e dettagli oggetto
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 1%

---

# Esportare moduli personalizzati e dettagli oggetto

È possibile esportare le informazioni relative alla panoramica e al modulo personalizzato dalla sezione Dettagli di un oggetto in un file PDF. È quindi possibile stampare o condividere il PDF con altri utenti.

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
>I campi nella sezione Dettagli rimossi dal Workfront o dall&#39;amministratore del gruppo utilizzando un modello di layout non vengono visualizzati.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licenza Adobe Workfront*</p> </td> 
   <td> <p>Richiedi o superiore per problemi</p> <p>Revisione o successiva per progetti e attività</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong> </td> 
   <td> <p>Visualizza o successiva per Progetti, Attività e Problemi</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorizzazioni oggetto</p> </td> 
   <td> <p>Visualizza o autorizzazioni superiori per il progetto, l'attività o il problema di cui si desidera esportare il modulo</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Prerequisiti

Prima di iniziare, è necessario disporre di tutti i seguenti elementi:

1. Creare un modulo personalizzato per un oggetto specifico da cui esportare.
1. Far allegare il modulo personalizzato all’oggetto

   Oppure

   Disporre dell&#39;accesso corretto per allegare un modulo personalizzato e modificare le informazioni nel modulo.

Per informazioni sulla creazione di moduli personalizzati, vedere [Progettare un modulo con Progettazione moduli](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Per informazioni su come allegare i moduli agli oggetti, vedere [Aggiungere un modulo personalizzato a un oggetto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Esportare le informazioni nella sezione Dettagli

L&#39;esportazione delle informazioni dalla sezione Dettagli di un oggetto è identica per tutti gli oggetti in cui è supportato.

1. Vai a un progetto, attività, portfolio, programma o problema per il quale disponi almeno delle autorizzazioni di visualizzazione.
1. Fare clic sull&#39;elemento **&quot;Dettagli&quot;** nel pannello sinistro, ad esempio **Dettagli attività**.
1. (Facoltativo) Se all&#39;oggetto non è allegato alcun modulo personalizzato, iniziare a digitare il nome di un modulo personalizzato nel **Aggiungi campo modulo personalizzato**, quindi fare clic su di esso quando viene visualizzato nell&#39;elenco.

   Puoi aggiungere fino a 10 moduli.

1. (Facoltativo) Aggiorna le informazioni nella sezione Dettagli, quindi fai clic su **Salva modifiche**.
1. Fai clic sul menu a discesa **Esporta** nell&#39;angolo superiore destro, seleziona **Panoramica** o i moduli da esportare, quindi fai clic su **Esporta**.

   È inoltre possibile selezionare **Seleziona tutto** se si desidera esportare l&#39;area Panoramica e tutti i moduli personalizzati.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Possono esistere i seguenti scenari:
   >
   >   
   >   
   >   * Quando il gruppo o l’amministratore Workfront deseleziona tutti i campi nell’area Panoramica e all’oggetto sono allegati moduli personalizzati, la sezione Panoramica non viene visualizzata.
   >   * Quando l’amministratore del gruppo o di Workfront deseleziona tutti i campi nell’area Panoramica e all’oggetto non sono allegati moduli personalizzati, il menu a discesa Esporta non è visibile.
   >   * Se all’oggetto non sono allegati moduli personalizzati, è possibile esportare solo l’area Panoramica.
   >   * I campi personalizzati che si trovano dietro la logica e non sono visibili nel modulo non vengono esportati. Per informazioni sull&#39;aggiunta della logica a un modulo personalizzato, vedere [Aggiungere logica di visualizzazione e ignorare la logica a un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
   >   
   >

   Un file PDF viene prodotto e scaricato sul computer. Il file PDF contiene le seguenti informazioni:

   * Nome dell&#39;oggetto a cui è associato il modulo
   * Nome dell&#39;utente che ha esportato il PDF
   * Data e ora di produzione del PDF
   * Nome dei moduli esportati
   * Informazioni contenute nei campi compilati nel modulo
