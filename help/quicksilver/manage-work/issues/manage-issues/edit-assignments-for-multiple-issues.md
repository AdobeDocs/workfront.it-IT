---
product-area: projects
navigation-topic: manage-issues
title: Modificare le assegnazioni utente per più problemi in un elenco
description: Modificare le assegnazioni utente per più problemi in un elenco
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: ac5552f1c235f595b1c0d2558fcf88b1e03f5a8e
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 1%

---

# Modificare le assegnazioni utente per più problemi in un elenco

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

È possibile modificare simultaneamente le assegnazioni degli utenti a più problemi. Per informazioni sulla modifica o l’assegnazione di problemi uno alla volta, consulta anche i seguenti articoli:

* [Modifica problemi](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Assegna problemi](../../../manage-work/issues/manage-issues/assign-issues.md)

Per informazioni generali sull&#39;assegnazione dei problemi, vedere [Panoramica sulla modifica delle assegnazioni dei problemi](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>È necessario disporre almeno delle autorizzazioni Contribuisci a un problema per poter effettuare assegnazioni al problema.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Richiedi o superiore</p> </td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p>Accesso di visualizzazione o superiore a progetti e attività per assegnare un problema</p> </td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il problema</p> <p>Quando si assegnano più problemi, contribuire con autorizzazioni o versioni successive al progetto o all’attività in cui si trova il problema.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Modificare le assegnazioni per più problemi

1. Passare all&#39;elenco dei problemi contenente i problemi di cui si desidera modificare le assegnazioni.
1. (Facoltativo) Crea un filtro per visualizzare solo i problemi assegnati all’assegnatario che desideri modificare.

   Ad esempio, puoi creare un filtro per visualizzare solo i problemi con un ruolo specifico come assegnatario.  Quindi, puoi sostituire il ruolo con un utente specifico. Effettua le seguenti operazioni:

   1. Fai clic sull&#39;elenco a discesa **Filtri**, quindi fai clic su **Nuovo filtro**.

   1. Nel primo campo, inizia a digitare **Ruoli assegnazione** e scegli **Ruoli assegnazione: Nome** dall&#39;elenco.
   1. Selezionare **Is any of** dal menu a discesa del modificatore, quindi iniziare a digitare il nome di un ruolo e selezionarlo quando viene visualizzato nell&#39;elenco. È possibile digitare più ruoli.

      >[!TIP]
      >
      >Non utilizzare **Assegnato a** perché questo campo fa riferimento solo al proprietario del problema e non a tutti gli assegnatari.

      L’elenco dei problemi filtra automaticamente in base ai criteri di filtro.
   1. (Facoltativo) Fai clic su **Salva come nuovo**, quindi su **Salva**.

1. Seleziona i problemi per i quali vuoi modificare le assegnazioni, quindi fai clic sull&#39;icona **Modifica** ![Icona Modifica](assets/qs-edit-icon.png).

   Viene visualizzato **Modifica problemi**. Il numero di elementi selezionati viene visualizzato nell&#39;angolo superiore sinistro della pagina.

1. (Condizionale) Nell’ambiente di produzione, effettua le seguenti operazioni:

   1. Vai alla sezione **Assegnazioni**, quindi seleziona **Assegnatario**.

      ![Area assegnazioni](assets/classic-assignmens-area-on-edit-box-350x119.png)

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

            Se l&#39;assegnatario che si desidera rimuovere non viene visualizzato nella sezione Assegnazioni perché l&#39;assegnatario è assegnato solo ad alcuni dei problemi selezionati, fare clic su **Rimuovi assegnatario** e iniziare a digitare il nome dell&#39;assegnatario che si desidera rimuovere, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

         1. Fai di nuovo clic su **Rimuovi assegnatario** per aggiungere un altro assegnatario da rimuovere.

      1. Per rimuovere tutti gli assegnatari:

         1. Fai clic su **Rimuovi tutti gli assegnatari esistenti**, quindi fai clic su **Sì, elimina tutti gli assegnatari**.

            In questo modo vengono rimossi non solo gli assegnatari comuni (assegnatari visualizzati nella finestra di dialogo di modifica), ma anche tutti gli assegnatari per tutti i problemi selezionati.

         1. (Facoltativo) Modificare una delle seguenti opzioni per gli assegnatari selezionati da associare ai problemi:

            * **Proprietario problema:** Selezionare il pulsante di opzione per indicare l&#39;assegnatario designato come proprietario dei problemi. Se non è selezionata, Adobe Workfront designa il primo assegnatario come Proprietario del problema. Questa opzione non è disponibile per le assegnazioni del team.
            * **Ruolo assegnatario**: selezionare un ruolo dall&#39;elenco a discesa. Se non è selezionata, Workfront seleziona automaticamente il ruolo principale dell’utente.

      1. Fai clic su **Salva modifiche**.

1. <span class="preview">Nell&#39;ambiente di anteprima eseguire le operazioni seguenti:</span>

   1. <span class="preview">Fai clic su **Assegnazioni** nel pannello a sinistra, quindi fai clic sull&#39;icona **x** accanto all&#39;assegnatario da rimuovere. </span>

      >[!TIP]
      >
      ><span class="preview">Solo gli assegnatari assegnati a tutti i problemi selezionati vengono visualizzati nell&#39;area **Assegnazioni**. </span>

      ![Area assegnazioni in problemi di modifica in blocco](assets/assignments-area-on-bulk-edit-issues.png)

   1. <span class="preview">Inizia a digitare il nome di un utente, ruolo o team per aggiungere gli assegnatari a tutti i problemi selezionati. </span>

      >[!TIP]
      >
      >Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team.
      >
      >Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
      >
      >* Riassegnare l&#39;elemento di lavoro alle risorse attive.
      >* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.

      <span class="preview">Gli assegnatari aggiunti vengono aggiunti a quelli esistenti. Non sostituiscono quelli esistenti per ogni problema selezionato. </span>
   1. <span class="preview">(Facoltativo) Fai clic su **Assegna a me** per assegnare tutti i problemi a te stesso.</span>
   1. <span class="preview">Fai clic su **Salva**. </span>




