---
product-area: projects
navigation-topic: manage-issues
title: Modificare le assegnazioni utente per più problemi in un elenco
description: Modificare le assegnazioni utente per più problemi in un elenco
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 7e77223595d3c9cf0d6592a09e893142439adb2c
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# Modificare le assegnazioni utente per più problemi in un elenco

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

È possibile modificare contemporaneamente le assegnazioni utente in più problemi. Per informazioni su come modificare i problemi o assegnarli uno alla volta, consulta anche i seguenti articoli:

* [Modifica dei problemi](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Assegnare i problemi](../../../manage-work/issues/manage-issues/assign-issues.md)

Per informazioni generali sull’assegnazione dei problemi, consulta [Modifica della panoramica delle assegnazioni dei problemi](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>È necessario disporre di almeno le autorizzazioni di Contribute per un problema in grado di eseguire le assegnazioni al problema.

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
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai problemi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni al problema</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

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

   1. Fai clic sul pulsante **Filtro** elenco a discesa, quindi fai clic su **Nuovo filtro**.

      Viene visualizzata la finestra di dialogo Nuovo filtro.

   1. Fai clic su **Aggiungi una regola di filtro.**
   1. Per filtrare un ruolo specifico, espandi **Ruoli assegnazione,** quindi fai clic su **ID.**

      Oppure

      Per filtrare un utente specifico, espandi **Utenti assegnazione,** quindi fai clic su **ID.**

      >[!TIP]
      >
      >Non utilizzare **Assegnato a** perché questo campo fa riferimento solo al proprietario del problema e non a tutti gli assegnatari.

   1. Nell’elenco a discesa , seleziona **Uguale** come qualificatore del filtro.
   1. Inizia a digitare il nome dell’utente o del ruolo per il quale desideri filtrare, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.
   1. Fai clic su **Salva filtro.**

1. Selezionare i problemi per i quali si desidera modificare le assegnazioni, quindi fare clic sul pulsante **Modifica** icona ![](assets/qs-edit-icon.png).

   La **Modifica problemi** viene visualizzato. Gli elementi modificati vengono visualizzati nell’angolo in alto a sinistra della pagina.

1. Vai a **Assegnazioni** , quindi seleziona **Assegnatario**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Esegui una delle operazioni seguenti:

   1. Per aggiungere un nuovo assegnatario:

      1. Inizia a digitare il nome di un utente, un ruolo o un team, quindi selezionalo quando viene visualizzato nell’elenco. L&#39;assegnazione viene aggiunta e non sostituisce le assegnazioni correnti sui problemi selezionati.

         >[!TIP]
         È possibile assegnare più utenti, ruoli o team. È possibile assegnare solo utenti attivi, ruoli e team.
         Se un utente, un ruolo di lavoro o un team è stato assegnato prima della disattivazione, rimangono assegnati all&#39;elemento di lavoro. In questo caso, si consiglia quanto segue:
         * Riassegna l&#39;elemento di lavoro alle risorse attive.
         * Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.


         Vengono visualizzate le informazioni comuni a tutti i problemi selezionati. Ad esempio, se lo stesso utente viene assegnato a tutti i problemi, viene visualizzato nel **Assegnatario** colonna. Se le informazioni non sono comuni tra i problemi selezionati, non vengono visualizzate informazioni.
   1. Per rimuovere singoli assegnatari:

      1. Fai clic sul pulsante **Icona X** accanto al nome dell&#39;assegnatario che si desidera rimuovere se l&#39;assegnatario viene visualizzato nell&#39;elenco Assegnazioni.

         Oppure

         (Condizionale) Se l&#39;assegnatario che si desidera rimuovere non viene visualizzato nella sezione Assegnazioni in quanto l&#39;assegnatario è assegnato solo ad alcuni dei problemi selezionati, fare clic su **Rimuovi assegnatario** e iniziare a digitare il nome dell&#39;assegnatario che si desidera rimuovere, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

      1. Fai clic su **Rimuovi assegnatario** per aggiungere un altro assegnatario da rimuovere.
   1. Per rimuovere tutti gli assegnatari esistenti:

      1. Fai clic su **Rimuovi tutti gli assegnatari esistenti**, quindi fai clic su **Sì, Elimina tutti gli assegnatari**.

         Questo rimuove non solo gli assegnatari comuni (assegnatari visualizzati nella finestra di dialogo di modifica), ma anche tutti gli assegnatari su tutti i problemi selezionati.



1. (Facoltativo) Modifica una delle seguenti opzioni per gli assegnatari selezionati per associare i problemi:

   * **Proprietario del problema:** Selezionare il pulsante di scelta per indicare quale assegnatario è designato come proprietario dei problemi. Se questa opzione è deselezionata, Adobe Workfront designa il primo assegnatario come proprietario del problema. Non disponibile per le assegnazioni di team.
   * **Ruolo dell&#39;assegnatario**: Seleziona un ruolo dall’elenco a discesa. Se viene lasciato deselezionato, Workfront seleziona automaticamente il Ruolo principale dell’utente.

1. Fai clic su **Salva modifiche**.
