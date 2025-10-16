---
product-area: requests
navigation-topic: create-requests
title: Creare richieste da bozze
description: Oltre a utilizzare le bozze disponibili suggerite da Workfront quando si immette una nuova richiesta, è possibile accedere a una bozza di richiesta dalla sezione Bozze e completare l'invio da tale sezione.
author: Becky
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 1a56846647e443cf3f5f09eed8c3084434de5ddb
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 1%

---

# Creare richieste da bozze

Oltre a utilizzare le bozze disponibili suggerite da Workfront quando si immette una nuova richiesta, è possibile accedere a una bozza di richiesta dalla sezione Bozze e completare l&#39;invio da tale sezione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Collaboratore o versione successiva</p>
   <p>Richiedi o superiore</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Prodotto</td> 
   <td> <ul><li>Adobe Workfront</li><li>È necessario disporre di Adobe Workfront Planning per visualizzare le richieste o i moduli di richiesta di Planning</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti per la creazione di richieste da bozze

Prima di creare una richiesta da una bozza, è necessario effettuare le seguenti operazioni: 

* Inizia a creare una richiesta. In questo modo la richiesta viene salvata automaticamente come bozza nella sezione Bozze.

  Per informazioni sulla creazione di richieste, vedere [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Creare richieste da bozze

{{step1-to-requests}}

1. Seleziona **Bozze** nel pannello a sinistra.

   In questo elenco viene visualizzata una bozza per ogni argomento della coda di ogni coda di richieste.

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. (Facoltativo) Fare clic su un&#39;intestazione di colonna per ordinare l&#39;elenco in base a tale colonna.

1. Esaminate le informazioni relative a ciascuna bozza nelle seguenti colonne dell&#39;elenco Bozze:

   | Oggetto | Questo è il nome che hai assegnato alla richiesta quando hai iniziato a crearla. |
   |---|---|
   | Percorso | Nome della coda di richieste, dei gruppi di argomenti e degli argomenti della coda in cui si intendeva inviare la richiesta. |
   | Data inserimento | La data in cui hai iniziato a creare la richiesta. |
   | Data ultimo aggiornamento | Ultimo aggiornamento. Se non l&#39;hai aggiornato da quando hai iniziato la richiesta, la Data di ingresso e la Data dell&#39;ultimo aggiornamento devono essere uguali. |

   {style="table-layout:auto"}

1. (Facoltativo) Utilizzando il filtro rapido nell&#39;angolo superiore destro dell&#39;elenco Bozze, iniziare a digitare il nome di una bozza di richiesta, coda di richieste, argomento della coda o gruppo di argomenti, quindi fare clic sul nome di una bozza per aprirla.

   >[!TIP]
   >
   >Non è possibile applicare filtri permanenti nella sezione Bozze dell’area Richieste. Non sono inoltre disponibili opzioni per modificare o modificare la visualizzazione dell&#39;elenco delle bozze.

1. Aggiornare le informazioni per la richiesta come descritto in [Creare e inviare richieste Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (Facoltativo e condizionale) In qualsiasi momento durante l&#39;immissione della richiesta, fare clic su **Elimina** bozza per eliminare la bozza. In questo modo viene eliminata la bozza che non può essere recuperata. Per ulteriori informazioni sull&#39;eliminazione delle bozze, vedere [Eliminare una bozza di richiesta](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Facoltativo) Fai clic su **Annulla** nell&#39;angolo inferiore sinistro della pagina per ripristinare l&#39;azione e mantenere la bozza.

1. Dopo aver completato le informazioni per la richiesta, eseguire una delle operazioni seguenti:

   * Fare clic su **Invia** per inviare la richiesta. La richiesta viene salvata nella sezione Inviata. A seconda della Regola di indirizzamento della Coda richieste, questa richiesta potrebbe essere indirizzata a un progetto diverso da quello designato come Coda richieste. Per informazioni sulle regole di routing, vedere [Creare regole di routing](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     Oppure

     Fai clic su **Chiudi** se non sei ancora pronto per inviarlo e potresti tornare indietro e terminarlo in un secondo momento. La richiesta viene salvata nella sezione Bozze e sarà disponibile al prossimo invio di una richiesta per questa coda di richieste.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

     Quando si invia la richiesta, la bozza viene eliminata e non può essere ripristinata.

   >[!NOTE]
   >
   >Nella nuova esperienza di richiesta, le bozze si trovano nello stesso elenco delle richieste inviate.
   >Per ulteriori informazioni sulla creazione di richieste nella nuova esperienza, consulta [Creare richieste e generare bozze nell&#39;app Web Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md#create-requests-and-generate-drafts-in-the-workfront-web-app) nell&#39;articolo Creare e inviare richieste.

