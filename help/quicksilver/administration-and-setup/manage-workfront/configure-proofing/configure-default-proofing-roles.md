---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configurare i ruoli di correzione predefiniti
description: In qualità di amministratore di Adobe Workfront, puoi configurare i ruoli di correzione predefiniti per gli utenti e gli utenti ospiti che accedono alle bozze create in Workfront. Chiunque aggiunga utenti a una bozza può regolare questi ruoli per loro.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Configurare i ruoli di correzione predefiniti

In qualità di amministratore di Adobe Workfront, puoi configurare i ruoli di correzione predefiniti per gli utenti e gli utenti ospiti che accedono alle bozze create in Workfront. Chiunque aggiunga utenti a una bozza può regolare questi ruoli per loro.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Devi essere un amministratore Workfront. Per informazioni sugli amministratori di Workfront, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Configurare i ruoli di correzione predefiniti

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Fai clic su **Revisione e approvazione** vicino alla parte inferiore dell’elenco che appare a sinistra.
1. In **Ruoli per i destinatari designati di una bozza del documento** seleziona il ruolo predefinito per gli utenti e gli utenti ospiti che vengono aggiunti al flusso di lavoro di una bozza.

   Vedi [Diritti associati ai ruoli di correzione](#rights-associated-with-proofing-roles) di seguito per un elenco di ciascun ruolo di correzione e dei diritti ad esso associati.

   >[!NOTE]
   >
   >* Questa impostazione si applica solo agli utenti che vengono creati nel sistema Workfront dopo l’impostazione del ruolo; non agli utenti esistenti.
   >* L’utente che aggiunge utenti alla bozza può regolare questo ruolo, come descritto in [Aggiungere utenti a una bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Condividere una bozza in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).


1. In **Ruoli per non destinatari che aprono una bozza di documento** seleziona il ruolo predefinito per gli utenti e gli utenti ospiti che possono accedere a una bozza ma non vengono aggiunti al flusso di lavoro della bozza.

   Questa situazione si verifica quando gli utenti e gli ospiti hanno accesso a un documento per il quale è stata creata una prova: anche se non sono stati aggiunti al flusso di lavoro della bozza, possono aprire la bozza.

   **Esempi:** Di seguito sono riportati alcuni esempi di utilizzo di questa impostazione:

   * Seleziona **Sola lettura** limitare tutte le attività di prova, ad esempio aggiungere commenti e prendere decisioni a coloro a cui è stato chiesto di farlo.
   * Seleziona **Revisore** perché vuoi che un membro del team sia in grado di aggiungere annotazioni e commenti su una bozza.

1. Fai clic su **Salva**.

## Diritti associati ai ruoli di correzione {#rights-associated-with-proofing-roles}

La tabella seguente mostra ogni ruolo e i diritti associati:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Visualizzare una bozza</strong> </p> </th> 
   <th> <p><strong>Aggiungi marcature</strong> </p> </th> 
   <th> <p><strong>Aggiungi commenti</strong> </p> </th> 
   <th> <p><strong>Modifica commenti personalizzati in assenza di risposte</strong> </p> </th> 
   <th> <p><strong>Prendere una decisione</strong> </p> </th> 
   <th> <p><strong>Elimina i commenti degli altri</strong> </p> </th> 
   <th>Risolvere i commenti</th> 
   <th>Applicare azioni ai commenti</th> 
   <th> <p><strong>Modificare la bozza</strong> </p> </th> 
   <th>Condividi la bozza con altri</th> 
   <th>Crea nuova versione</th> 
   <th> <p><strong>Visualizza richieste di approvazione nell'area Home</strong> </p> </th> 
   <th>Aggiungi nuovi revisori</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Sola lettura</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Revisore</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Approvatore</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Revisore e Approvatore</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autore</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Moderatore</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Gli utenti che utilizzano nuovi piani Workfront possono assegnare ruoli di autore o moderatore a qualsiasi utente del sistema. Gli utenti che utilizzano piani legacy possono assegnare ruoli di autore o moderatore a qualsiasi utente con una licenza a prova nel sistema.
