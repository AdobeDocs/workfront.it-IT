---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aggiorna lo stato del problema
description: Puoi aggiornare lo stato di un problema per informare gli altri su dove si trova il problema e come si sta verificando.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 3%

---

# Aggiorna lo stato del problema

Puoi aggiornare lo stato di un problema per informare gli altri su dove si trova il problema e come si sta verificando.

## Requisiti di accesso

<!--drafted for P&P;

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai problemi</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni al problema</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Stato del problema

Di seguito sono riportati gli stati predefiniti per i problemi in Workfront:

* Nuovo
* In corso
* In attesa di Riscontro
* In sospeso
* Non Risolvibile
* Ri-Aperto
* Chiuso
* Risolto

L’amministratore Adobe Workfront può aggiungere stati personalizzati per i problemi relativi all’organizzazione. Inoltre, possono rendere disponibili gli stati a seconda del tipo di problema.

Per ulteriori informazioni sugli stati personalizzati e sui tipi di problemi, consulta i seguenti articoli:

* [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [Creare problemi](../../../manage-work/issues/manage-issues/create-issues.md)

Puoi aggiornare manualmente gli stati dei problemi oppure puoi consentire a Workfront di aggiornarli automaticamente quando si verificano determinate azioni.

## Aggiorna manualmente lo stato del problema

Quando aggiorni lo stato di un problema, puoi anche aggiungere una spiegazione sul nuovo stato e modificare altre informazioni sul problema, come la data di commit.

1. Passa a un problema a cui sei assegnato per il quale vuoi aggiornare lo stato.
1. Fai clic sul pulsante **Stato** nell’intestazione del problema e seleziona un nuovo stato.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. Per fornire un’indicazione visiva del completamento del problema, trascina o fai doppio clic sulla bolla in **Percentuale completata** nell&#39;intestazione del problema.

   Oppure

   Fai clic all’interno della bolla nell’intestazione del problema per immettere una percentuale.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Facoltativo) Effettua una delle seguenti operazioni per fornire informazioni aggiuntive sull&#39;aggiornamento, quindi fai clic su **Aggiorna** oppure, se il problema presenta uno stato che corrisponde a Completo, fai clic su **Fatto:**

   * Per aggiungere una nota sull&#39;aggiornamento, vai alla sezione **Aggiornamenti** e fai clic su **Avvia un nuovo aggiornamento**, quindi digita la nota.

      ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Per informare alcuni utenti dell’aggiornamento, digita i loro nomi nel **Notifica** casella visualizzata quando si digita una nota relativa all&#39;aggiornamento. Per ulteriori informazioni, consulta [Assegnare tag agli altri utenti in caso di aggiornamenti](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Per aggiornare la condizione del problema, fai clic su **Condizione**, quindi seleziona la condizione che riflette al meglio la condizione corrente del problema. Seleziona tra le seguenti opzioni:

      * Senza problemi
      * Qualche dubbio
      * Problemi notevoli
   * Per aggiornare la data di commit del problema, espandi la **Data impegno** calendario a discesa e selezionare una nuova data.


## Aggiorna automaticamente lo stato del problema

Workfront aggiorna automaticamente lo stato esistente di un problema a uno stato diverso quando si verificano le azioni elencate nella tabella seguente.

>[!NOTE]
>
>Gli stati nella tabella seguente sono stati predefiniti del sistema. L’amministratore di Workfront o un amministratore di gruppo può rinominare gli stati nell’istanza di Workfront. Per informazioni sulla creazione e la gestione degli stati in Workfront, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Azione</td> 
   <td>Stato originale</td> 
   <td>Nuovo stato</td> 
  </tr> 
  <tr> 
   <td>Aggiorna la percentuale del problema completa al 100%</td> 
   <td>Novità o in corso</td> 
   <td>Chiuso</td> 
  </tr> 
  <tr> 
   <td>Aggiorna la percentuale di completamento del problema dal 100% a un numero inferiore</td> 
   <td>Chiuso </td> 
   <td>In corso</td> 
  </tr> 
  <tr> 
   <td>Aggiorna lo stato di un oggetto di risoluzione associato al problema</td> 
   <td>Vari stati</td> 
   <td> <p>Vari stati</p> <p>Per informazioni sulla risoluzione degli oggetti e sul loro impatto sullo stato dei problemi, vedere la sezione "Sincronizzazione dello stato dell'oggetto risolvibile con quello dell'oggetto di risoluzione" nell'articolo <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sulla risoluzione e risoluzione di oggetti </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Fai clic sul pulsante Start Issue per accettare di lavorare su un problema assegnato</span> </td> 
   <td><span>Nuovo</span> </td> 
   <td> <p>Qualsiasi stato associato al pulsante Start Issue nelle impostazioni Home Team. </p> <p>Per informazioni sulla sostituzione del pulsante Work On It con un pulsante Start Issue, vedere <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Sostituire il pulsante Work On It con un pulsante Start</a></span><span>.</span> </p> <p>Suggerimento: Clic <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">Pulsante Annulla</span> dopo aver fatto clic su Start Issue, lo stato viene ripristinato su Nuovo. </p> </td> 
  </tr> 
 </tbody> 
</table>
