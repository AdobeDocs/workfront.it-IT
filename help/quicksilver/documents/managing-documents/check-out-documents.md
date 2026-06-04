---
product-area: documents
navigation-topic: manage-documents
title: Estrarre i documenti
description: È possibile estrarre un documento per impedire ad altri utenti di eliminarlo o di caricarne una nuova versione. Un documento può essere estratto da un solo utente alla volta. Puoi estrarre qualsiasi documento caricato su Adobe Workfront, nonché i documenti collegati a provider di documenti di terze parti (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint o qualsiasi altro provider personalizzato).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/kkWxK2NzQtSfeRqsd0vEB-2AUYFrO6WIU3A752w7kM4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 593
ht-degree: 9%

---

# Estrarre i documenti

È possibile estrarre un documento per impedire ad altri utenti di eliminarlo o di caricarne una nuova versione. Un documento può essere estratto da un solo utente alla volta. Puoi estrarre qualsiasi documento caricato su Adobe Workfront, nonché i documenti collegati a provider di documenti di terze parti (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint o qualsiasi altro provider personalizzato). 

>[!NOTE]
>
>Questa funzionalità non è disponibile nella nuova area Documenti.<br>
>Se la tua organizzazione utilizza l&#39;archiviazione cloud Adobe, quando accedi ai documenti in Workfront visualizzerai la nuova area Documenti. Per ulteriori informazioni sull&#39;archiviazione cloud di Adobe, consulta [Panoramica sull&#39;archiviazione cloud di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

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
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o successiva</p>
   <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso in modifica ai documenti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Accesso in gestione al documento</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
