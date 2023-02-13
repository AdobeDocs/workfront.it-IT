---
product-area: documents
navigation-topic: manage-documents
title: Estrarre documenti
description: È possibile estrarre un documento per impedire ad altri utenti di eliminarlo o di caricarne una nuova versione. Un solo utente può estrarre un documento alla volta. È possibile estrarre qualsiasi documento caricato in Adobe Workfront e i documenti collegati a provider di documenti di terze parti (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint o qualsiasi altro provider personalizzato).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Estrarre documenti

È possibile estrarre un documento per impedire ad altri utenti di eliminarlo o di caricarne una nuova versione. Un solo utente può estrarre un documento alla volta. È possibile estrarre qualsiasi documento caricato in Adobe Workfront e i documenti collegati a provider di documenti di terze parti (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint o qualsiasi altro provider personalizzato). 

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci l'accesso al documento</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Azioni consentite sui documenti estratti

Gli utenti con accesso gestito al documento possono effettuare le seguenti operazioni:

* Modificare il documento (nome del documento, descrizione, dati personalizzati)
* Sposta il documento
* Condividere il documento
* Anteprima del documento
* Scarica il documento

   >[!TIP]
   >
   > Anche se un utente può scaricare un documento quando è estratto da un altro utente, si consiglia agli utenti di attendere che il documento sia stato archiviato nuovamente prima di scaricarlo. Quando un documento viene estratto, indica spesso che il lavoro sul documento è ancora in corso. L&#39;attesa del Check-In di un documento per il download assicura che l&#39;utente disponga della versione più recente.

* Approvare un documento o applicare un&#39;approvazione al documento.
* Rivedere il documento nel visualizzatore di correzione

   Per ulteriori informazioni sulla correzione, consulta [Copertura](../../review-and-approve-work/proofing/proofing.md)

## Estrarre un documento

Se si dispone delle autorizzazioni di gestione per un documento, è possibile estrarlo per impedire determinate azioni sul documento. 

1. Passare all&#39;area in cui è memorizzato il documento, quindi selezionare il documento. 

   Per informazioni sull&#39;aggiunta di documenti, vedere [Aggiungere documenti ad Adobe Workfront dal file system](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Fai clic sul pulsante **Estrai** icona ![](assets/check-out-25x23.png).

1. Icona a forma di lucchetto ![](assets/lock-icon-locked-qs.png) viene visualizzato a destra del nome del documento. Il documento rimane estratto dopo la disconnessione da Workfront.
1. Solo l&#39;utente che ha estratto il documento o l&#39;amministratore Workfront può archiviarlo.

## Gestisci documenti estratti

Considera quanto segue sui documenti estratti:

* Prima di poter eliminare un oggetto in cui è memorizzato un documento estratto, è necessario eseguire nuovamente il Check-In del documento. 
* Se l’amministratore di Workfront elimina un utente che ha estratto un documento di cui non era proprietario, Workfront controlla automaticamente il documento.
* Se l&#39;amministratore di Workfront elimina un utente che ha estratto un documento di cui è proprietario e il documento viene caricato su un oggetto, il documento rimane estratto. Solo un amministratore Workfront può effettuare nuovamente il check-in.
* Se l&#39;amministratore di Workfront elimina un utente che ha estratto un documento di propria proprietà e il documento viene caricato solo nell&#39;area Documenti (non in un oggetto), il documento viene eliminato insieme all&#39;utente.

   Per informazioni sull&#39;eliminazione degli utenti, vedere [Eliminare gli utenti](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Se l’amministratore di Workfront disattiva un utente, tutti i documenti estratti rimangono estratti. Solo un amministratore Workfront può effettuare nuovamente il check-in. 

## Archiviare un documento

È necessario archiviare nuovamente un documento prima di caricarne o eliminarlo. 

Per archiviare un documento:

1. Passare all&#39;area in cui è memorizzato il documento e selezionare il documento. 

   Icona a forma di lucchetto ![](assets/lock-icon-locked-qs.png) viene visualizzato a destra del nome del documento.

1. Fai clic sul pulsante **Archivia** icona ![](assets/check-in-25x22.png).
