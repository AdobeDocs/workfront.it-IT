---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront
description: I risultati misurano l’avanzamento di un obiettivo. Senza associare risultati, attività o obiettivi allineati a un obiettivo, non puoi attivare l’obiettivo e non puoi registrarne l’avanzamento.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 3%

---

# Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront

<!--Audited for P&P only: 10/2025-->

I risultati misurano l’avanzamento di un obiettivo. Senza associare risultati, attività o obiettivi allineati a un obiettivo, non puoi attivare l’obiettivo e non puoi registrarne l’avanzamento.

## Requisiti di accesso

>[!NOTE]
>
>La tua azienda potrebbe scegliere di continuare a utilizzare gli obiettivi di Adobe Workfront se ha acquistato questo pacchetto in passato. Per ulteriori dettagli, rivolgiti al rappresentante del tuo account.
>
>Adobe Workfront Goals non è più disponibile per l’acquisto.

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Pacchetto Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licenza Adobe Workfront</td>
 <td>
 <p>Collaboratore o versione successiva</p>
<p>Richiedi o superiore</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configurazione del livello di accesso</td>
 <td> <p>Modifica accesso agli obiettivi</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorizzazioni oggetto</td>
 <td>
  <div>
  <p>Visualizza o autorizzazioni superiori per l’obiettivo per visualizzarlo</p>
  <p>Gestire le autorizzazioni per l’obiettivo per modificarlo</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di sistema, deve essere assegnato un modello di layout che includa l'area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Prerequisiti

Prima di iniziare, è necessario disporre dei seguenti elementi:

* Modello di layout che include l&#39;area Obiettivi nel menu principale.
* Un obiettivo esistente.

  Per informazioni sulla creazione degli obiettivi, vedere [Creare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>Un obiettivo può avere un totale di 1000 attività, risultati, progetti o obiettivi allineati.

## Aggiungere un risultato a un obiettivo

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![Add result inside goal](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![Results value](assets/results-value-initial-target-boxes-350x49.png)

   Select from the following options:

   |Option|Value type|
   |---|---|
   | # |Number value |
   | % |Percentage value |
   |$, CN¥, DKK, KR, Mex$, R, R$, zł, £ , ¥ , &euro; , ₹, ฿, MYR, ₪  |Currency values |

   For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value.

   >[!TIP]
   >
   >The result Type is always Metric and cannot be edited.

1. In the Initial field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. 
1. In the Target field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.
1. Click **Save**.

   The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result.

-->

1. Fai clic sull&#39;icona del menu principale ![Main Menu](assets/main-menu-icon.png), quindi su **Goals**.

1. Dalla **lista obiettivi**, fare clic sul nome di un obiettivo per aprire la pagina obiettivo.
1. Fai clic su **Indicatori di avanzamento** nel pannello a sinistra.
1. Espandi il menu a discesa **Nuovo indicatore di avanzamento**, quindi fai clic su **Crea risultato**.

   Viene visualizzata la casella Nuovo risultato (New result).

   ![Nuova casella dei risultati](assets/new-result-box-unshimmed.png)

1. Immettere un nome per il risultato nel campo **Nome risultato**. Questo è un campo obbligatorio.
1. (Facoltativo) Rimuovi il tuo nome dal campo **Proprietario risultato** se desideri assegnare il risultato a un altro utente. Per impostazione predefinita, sei il proprietario di un’attività creata.

   >[!NOTE]
   >
   >Non è possibile assegnare un team, un gruppo o l&#39;azienda come proprietario dei risultati.

1. In **Come si desidera misurare il risultato?** area, specificare le informazioni seguenti:
   * **Tipo di valore**: indica come misurare l&#39;avanzamento del risultato. Puoi misurare l’avanzamento numericamente, con un valore percentuale o utilizzando un importo in valuta.

     Selezionare un tipo di valore tra le opzioni elencate nella tabella seguente:

     | Tipo di valore | Descrizione |
     |---------------------------------------------------------|------------------|
     | Numero | Valore numerico |
     | % | Valore percentuale |
     | CN¥,DKK,KR,Mex$, R, R$, zł, £ , ¥ , € , ₹, ฿, MYR, ₪, $ | Valori valuta |

   * **Valore iniziale**: il valore iniziale del risultato prima che sia stato registrato qualsiasi avanzamento.
   * **Valore di destinazione**: il valore che il risultato intende ottenere quando viene considerato completato.
1. Fai clic su **Crea risultato**.

   Il risultato viene visualizzato nella sezione Indicatori di avanzamento della pagina dell’obiettivo, sotto il raggruppamento Risultato.

   Dopo aver attivato l’obiettivo, l’avanzamento dell’obiettivo viene aggiornato automaticamente quando si aggiorna l’avanzamento di un risultato. Per informazioni sull&#39;attivazione di un obiettivo, vedere [Attivare gli obiettivi negli Obiettivi di Adobe Workfront](../goal-management/activate-goals.md).
