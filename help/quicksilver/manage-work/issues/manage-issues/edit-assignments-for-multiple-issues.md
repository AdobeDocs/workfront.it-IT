---
product-area: projects
navigation-topic: manage-issues
title: Modificare le assegnazioni utente per più problemi in un elenco
description: Modificare le assegnazioni utente per più problemi in un elenco
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 1%

---

# Modificare le assegnazioni utente per più problemi in un elenco

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

È possibile modificare simultaneamente le assegnazioni degli utenti a più problemi. Per informazioni sulla modifica o l’assegnazione di problemi uno alla volta, consulta anche i seguenti articoli:

* [Modifica problemi](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Assegna problemi](../../../manage-work/issues/manage-issues/assign-issues.md)

Per informazioni generali sull&#39;assegnazione dei problemi, vedere [Panoramica sulla modifica delle assegnazioni dei problemi](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>È necessario disporre almeno delle autorizzazioni Contribute per un problema per poter effettuare assegnazioni al problema.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il problema</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:&nbsp;drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Modificare le assegnazioni per più problemi

1. Passare all&#39;elenco dei problemi contenente i problemi di cui si desidera modificare le assegnazioni.
1. (Facoltativo) Crea un filtro per visualizzare solo i problemi assegnati all’assegnatario che desideri modificare.

   Ad esempio, puoi creare un filtro per visualizzare solo i problemi con un ruolo specifico come assegnatario. Quindi, puoi sostituire il ruolo con un utente specifico. Effettua le seguenti operazioni:

   1. Fai clic sull&#39;elenco a discesa **Filtro**, quindi fai clic su **Nuovo filtro**.

      Viene visualizzata la finestra di dialogo Nuovo filtro.

   1. Fare clic su **Aggiungi regola filtro.**
   1. Per filtrare per un ruolo specifico, espandi **Ruoli assegnazione,** quindi fai clic su **ID.**

      Oppure

      Per filtrare per un utente specifico, espandi **Utenti assegnazione,** quindi fai clic su **ID.**

      >[!TIP]
      >
      >Non utilizzare **Assegnato a** perché questo campo fa riferimento solo al proprietario del problema e non a tutti gli assegnatari.

   1. Nell&#39;elenco a discesa, selezionare **Uguale** come qualificatore del filtro.
   1. Inizia a digitare il nome dell’utente o del ruolo per cui desideri filtrare, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.
   1. Fai clic su **Salva filtro.**

1. Seleziona i problemi per i quali vuoi modificare le assegnazioni, quindi fai clic sull&#39;icona **Modifica** ![](assets/qs-edit-icon.png).

   Viene visualizzato **Modifica problemi**. Gli elementi modificati vengono visualizzati nell&#39;angolo superiore sinistro della pagina.

1. Vai alla sezione **Assegnazioni**, quindi seleziona **Assegnatario**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Esegui una delle operazioni seguenti:

   1. Per aggiungere un nuovo assegnatario:

      1. Inizia a digitare il nome di un utente, ruolo o team, quindi selezionalo quando viene visualizzato nell’elenco. L&#39;assegnazione viene aggiunta e non sostituisce le assegnazioni correnti sui problemi selezionati.

         >[!TIP]
         >
         >Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team.
         >
         >Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
         >
         >* Riassegnare l&#39;elemento di lavoro alle risorse attive.
         >* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.

         Vengono visualizzate le informazioni comuni a tutti i problemi selezionati. Ad esempio, se lo stesso utente è assegnato a tutti i problemi, viene visualizzato nella colonna **Assegnatario**. Se le informazioni non sono comuni tra i problemi selezionati, non viene visualizzata alcuna informazione.

   1. Per rimuovere singoli assegnatari:

      1. Fare clic sull&#39;icona **X** accanto al nome dell&#39;assegnatario che si desidera rimuovere se l&#39;assegnatario viene visualizzato nell&#39;elenco Assegnazioni.

         Oppure

         (Condizionale) Se l&#39;assegnatario che si desidera rimuovere non viene visualizzato nella sezione Assegnazioni perché l&#39;assegnatario è assegnato solo ad alcuni dei problemi selezionati, fare clic su **Rimuovi assegnatario** e iniziare a digitare il nome dell&#39;assegnatario che si desidera rimuovere, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

      1. Fai di nuovo clic su **Rimuovi assegnatario** per aggiungere un altro assegnatario da rimuovere.

   1. Per rimuovere tutti gli assegnatari:

      1. Fai clic su **Rimuovi tutti gli assegnatari esistenti**, quindi fai clic su **Sì, elimina tutti gli assegnatari**.

         In questo modo vengono rimossi non solo gli assegnatari comuni (assegnatari visualizzati nella finestra di dialogo di modifica), ma anche tutti gli assegnatari per tutti i problemi selezionati.

1. (Facoltativo) Modificare una delle seguenti opzioni per gli assegnatari selezionati da associare ai problemi:

   * **Proprietario problema:** Selezionare il pulsante di opzione per indicare l&#39;assegnatario designato come proprietario dei problemi. Se non è selezionata, Adobe Workfront designa il primo assegnatario come Proprietario del problema. Questa opzione non è disponibile per le assegnazioni del team.
   * **Ruolo assegnatario**: selezionare un ruolo dall&#39;elenco a discesa. Se non è selezionata, Workfront seleziona automaticamente il ruolo principale dell’utente.

1. Fai clic su **Salva modifiche**.
