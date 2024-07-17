---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configurare i ruoli di verifica predefiniti
description: In qualità di amministratore di Adobe Workfront, puoi configurare i ruoli di bozza predefiniti per gli utenti e gli utenti guest che accedono alle bozze create in Workfront. Chiunque aggiunga utenti a una bozza può modificarli in base a tali ruoli.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 1%

---

# Configurare i ruoli di verifica predefiniti

In qualità di amministratore di Adobe Workfront, puoi configurare i ruoli di bozza predefiniti per gli utenti e gli utenti guest che accedono alle bozze create in Workfront. Chiunque aggiunga utenti a una bozza può modificarli in base a tali ruoli.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Devi essere un amministratore di Workfront. Per informazioni sugli amministratori di Workfront, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Configurare i ruoli di verifica predefiniti

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Fai clic su **Rivedi e approva** in fondo all&#39;elenco visualizzato a sinistra.
1. Nella sezione **Ruoli per i destinatari designati di una bozza di documento** selezionare il ruolo predefinito per gli utenti e gli utenti guest aggiunti al flusso di lavoro di una bozza.

   Consulta [Diritti associati ai ruoli di verifica](#rights-associated-with-proofing-roles) di seguito per un elenco di ogni ruolo di verifica e dei diritti associati.

   >[!NOTE]
   >
   >* Questa impostazione è valida solo per gli utenti creati nel sistema Workfront dopo l&#39;impostazione del ruolo e non per gli utenti esistenti.
   >* La persona che aggiunge utenti alla bozza può modificare questo ruolo, come descritto in [Aggiungere utenti a una bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Condividere una bozza in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

1. Nella sezione **Ruoli per i non destinatari che aprono una bozza del documento** selezionare il ruolo predefinito per gli utenti e gli utenti guest che possono accedere a una bozza, ma che non vengono aggiunti al flusso di lavoro della bozza.

   Questa situazione si verifica quando utenti e ospiti hanno accesso a un documento per il quale è stata creata una bozza: anche se non sono stati aggiunti al flusso di lavoro della bozza, possono aprire la bozza.

   **Esempi:** Di seguito sono riportati alcuni esempi di utilizzo di questa impostazione:

   * Seleziona **Sola lettura** per limitare tutte le attività della bozza, ad esempio l&#39;aggiunta di commenti e l&#39;adozione di decisioni a coloro a cui è stato richiesto di farlo.
   * Si seleziona **Revisore** perché si desidera consentire a qualsiasi membro del team di aggiungere commenti e commenti a una bozza.

1. Fai clic su **Salva**.

## Diritti associati ai ruoli di verifica {#rights-associated-with-proofing-roles}

Nella tabella seguente vengono illustrati i ruoli e i diritti associati:

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
   <th> <p><strong>Visualizza una bozza</strong> </p> </th> 
   <th> <p><strong>Aggiungi markup</strong> </p> </th> 
   <th> <p><strong>Aggiungi commenti</strong> </p> </th> 
   <th> <p><strong>Modificare i propri commenti in assenza di risposte</strong> </p> </th> 
   <th> <p><strong>Decidi</strong> </p> </th> 
   <th> <p><strong>Elimina commenti aggiunti da altri</strong> </p> </th> 
   <th>Risolvi commenti</th> 
   <th>Applica azioni ai commenti</th> 
   <th> <p><strong>Modifica la bozza</strong> </p> </th> 
   <th>Condividi la bozza con altri utenti</th> 
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
   <td> <p>✓ <strong></strong> </p> </td> 
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
>Gli utenti dei nuovi piani di Workfront possono assegnare ruoli di autore o moderatore a qualsiasi utente del sistema. Gli utenti che usano piani precedenti possono concedere ruoli di autore o moderatore a qualsiasi utente con una licenza Verifica nel sistema.
