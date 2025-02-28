---
product-area: documents
navigation-topic: manage-documents
title: Estrai documenti
description: È possibile estrarre un documento per impedire ad altri utenti di eliminarlo o di caricarne una nuova versione. Un documento può essere estratto da un solo utente alla volta. Puoi estrarre qualsiasi documento caricato su Adobe Workfront, nonché i documenti collegati a provider di documenti di terze parti (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint o qualsiasi altro provider personalizzato).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 0%

---

# Estrai documenti

È possibile estrarre un documento per impedire ad altri utenti di eliminarlo o di caricarne una nuova versione. Un documento può essere estratto da un solo utente alla volta. Puoi estrarre qualsiasi documento caricato su Adobe Workfront, nonché i documenti collegati a provider di documenti di terze parti (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint o qualsiasi altro provider personalizzato). 

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire l’accesso al documento</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Azioni consentite per i documenti estratti

Gli utenti con accesso in gestione al documento possono effettuare le seguenti operazioni:

* Modificare il documento (nome del documento, descrizione, dati personalizzati)
* Spostare il documento
* Condividi il documento
* Anteprima del documento
* Scarica il documento

  >[!TIP]
  >
  > Sebbene un utente possa scaricare un documento estratto da un altro utente, si consiglia di attendere che il documento sia stato archiviato di nuovo prima di scaricarlo. Quando un documento viene estratto, indica spesso che il lavoro è ancora in corso sul documento. In attesa che un documento venga archiviato di nuovo per scaricarlo, l&#39;utente disporrà della versione più recente.

* Approvare un documento o applicare un&#39;approvazione al documento.
* Esaminare il documento nel visualizzatore di bozze

  Per ulteriori informazioni sulla verifica, vedere [Verifica](../../review-and-approve-work/proofing/proofing.md)

## Estrarre un documento

Se si dispone delle autorizzazioni di gestione per un documento, è possibile estrarlo per impedire determinate azioni sul documento. 

1. Passare all&#39;area in cui è memorizzato il documento, quindi selezionare il documento. 

   Per informazioni sull&#39;aggiunta di documenti, vedere [Aggiungere documenti ad Adobe Workfront dal file system](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Fai clic sull&#39;icona **Estrai** ![Estrai](assets/check-out-25x23.png).

1. A destra del nome del documento viene visualizzata l&#39;icona del lucchetto ![Icona del lucchetto](assets/lock-icon-locked-qs.png). Il documento rimane estratto dopo la disconnessione da Workfront.
1. Solo l&#39;utente che ha estratto il documento o l&#39;amministratore di Workfront può archiviare il documento.

## Gestisci documenti estratti

Considerare le seguenti informazioni sui documenti estratti:

* Prima di poter eliminare un oggetto in cui è memorizzato un documento estratto, è necessario archiviare nuovamente il documento. 
* Se l&#39;amministratore di Workfront elimina un utente che ha estratto un documento di cui non era proprietario, Workfront archivia automaticamente il documento.
* Se l&#39;amministratore di Workfront elimina un utente che ha estratto un documento di sua proprietà e il documento viene caricato su un oggetto, il documento rimane estratto. Solo un amministratore di Workfront può archiviarlo di nuovo.
* Se l&#39;amministratore di Workfront elimina un utente che ha estratto un documento di sua proprietà e il documento viene caricato solo nell&#39;area Documenti (non su un oggetto), il documento viene eliminato insieme all&#39;utente.

  Per informazioni sull&#39;eliminazione degli utenti, vedere [Elimina utenti](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Se l&#39;amministratore di Workfront disattiva un utente, tutti i documenti estratti rimangono estratti. Solo un amministratore di Workfront può archiviarli di nuovo. 

## Archiviare un documento

È necessario archiviare nuovamente un documento prima di caricarne una nuova versione o eliminarlo. 

Per archiviare un documento:

1. Passare all&#39;area in cui è memorizzato il documento e selezionarlo. 

   A destra del nome del documento viene visualizzata l&#39;icona del lucchetto ![Icona del lucchetto](assets/lock-icon-locked-qs.png).

1. Fai clic sull&#39;icona **Archivia** ![Icona Archivia](assets/check-in-25x22.png).
