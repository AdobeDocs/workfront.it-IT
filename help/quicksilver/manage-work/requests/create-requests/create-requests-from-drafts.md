---
product-area: requests
navigation-topic: create-requests
title: Creare richieste dalle bozze
description: Oltre a utilizzare le bozze disponibili suggerite da Workfront quando si inserisce una nuova richiesta, è possibile accedere a una richiesta di bozza dalla sezione Bozze e completarla con l'invio.
author: Alina
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 345f63fc78d9bc2b2eff8f19a8a9196641567764
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 1%

---

# Creare richieste dalle bozze

<span class="preview">Le informazioni evidenziate in questa pagina fanno riferimento a funzionalità non ancora disponibili al pubblico. È disponibile solo nell’ambiente Anteprima.</span>

Oltre a utilizzare le bozze disponibili suggerite da Workfront quando si inserisce una nuova richiesta, è possibile accedere a una richiesta di bozza dalla sezione Bozze e completarla con l&#39;invio.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td> <p>Modifica accesso ai problemi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti per la creazione di richieste da bozze

È necessario eseguire le operazioni seguenti prima di creare una richiesta da una bozza: 

* Inizia a creare una richiesta. In questo modo la richiesta viene salvata automaticamente come bozza nella sezione Bozze .

   Per informazioni sulla creazione delle richieste, vedi [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Creare richieste dalle bozze

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra di Workfront.
1. Fai clic su **Richieste** > **Bozze**.

   In questo elenco viene visualizzata una bozza per ogni argomento della coda di ogni richiesta.

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. <span class="preview">(Facoltativo) Fai clic su un’intestazione di colonna per ordinare l’elenco in base a tale colonna.</span>

1. Rivedere le informazioni su ogni bozza nelle colonne seguenti dell&#39;elenco Bozze:

   | Oggetto | Questo è il nome che hai dato alla tua richiesta mentre hai iniziato a crearla. |
   |---|---|
   | Percorso | Nome della coda delle richieste, dei gruppi di argomenti e degli argomenti della coda in cui si intendeva originariamente inviare la richiesta. |
   | Data inserimento | Data di inizio della creazione della richiesta. |
   | Data ultimo aggiornamento | Ultimo aggiornamento. Se non lo hai aggiornato dalla prima volta che hai avviato la richiesta, la data di ingresso e la data dell&#39;ultimo aggiornamento devono essere uguali. |

   {style="table-layout:auto"}

1. <span class="preview">(Facoltativo) Utilizzando il filtro rapido nell&#39;angolo in alto a destra dell&#39;elenco Bozze, inizia a digitare il nome di una richiesta di bozza, di una coda di richiesta, di un argomento della coda o di un gruppo di argomenti, quindi fai clic sul nome di una bozza per aprirla. </span>
1. Aggiorna le informazioni per la richiesta come descritto in [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (Facoltativo e condizionale) In qualsiasi momento durante l’immissione della richiesta, fai clic su **Elimina** bozza per eliminare la bozza. Questo elimina la bozza che non può essere recuperata. Per ulteriori informazioni sull&#39;eliminazione delle bozze, vedere [Eliminare una bozza di richiesta](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Facoltativo) Fai clic su **Annulla** nell’angolo in basso a sinistra della pagina per ripristinare l’azione e mantenere la bozza.

1. Dopo aver completato le informazioni per la richiesta, effettua una delle seguenti operazioni:

   * Fai clic su **Invia** se sei pronto a inviare la richiesta. La richiesta viene salvata nella sezione Inviata . A seconda della regola di routing della coda di richiesta, questa richiesta potrebbe essere indirizzata a un progetto diverso da quello designato come coda di richiesta. Per informazioni sulle regole di routing, vedi [Creare regole di routing](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

      Oppure

      Fai clic su **Chiudi** se non sei pronto a inviarlo e potresti tornare e finirlo più tardi. La richiesta viene salvata nella sezione Bozze e sarà disponibile al prossimo invio di una richiesta per questa coda di richiesta.

      ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

      Quando invii la richiesta, la bozza viene eliminata e non può essere ripristinata.
