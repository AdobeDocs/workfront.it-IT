---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront
description: I risultati misurano il progresso di un obiettivo. Senza associare risultati, attività o obiettivi allineati a un obiettivo, non è possibile attivare l'obiettivo e non registrare l'avanzamento su di esso.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 1%

---

# Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront

I risultati misurano il progresso di un obiettivo. Senza associare risultati, attività o obiettivi allineati a un obiettivo, non è possibile attivare l&#39;obiettivo e non registrare l&#39;avanzamento su di esso.

## Requisiti di accesso

<!--drafted for P&P release: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>

-->

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze di Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td> <p>Devi acquistare una licenza aggiuntiva per la funzionalità Obiettivi di Adobe Workfront per accedere alla descritta in questo articolo. </p> <p>Per informazioni, consulta <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l'accesso agli obiettivi</p> <p><b>NOTA</b>

<p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Concedere l’accesso agli obiettivi di Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> 
    <div> 
     <p>Gestione delle autorizzazioni per l'obiettivo</p> 
     <p>Per informazioni sulla condivisione degli obiettivi, vedi <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario disporre dei seguenti elementi prima di poter iniziare:

* Modello di layout che include l’area Obiettivi del menu principale.
* Un obiettivo esistente.

   Per informazioni sulla creazione degli obiettivi, vedi [Creare obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>Un obiettivo non può avere più di 1000 attività, risultati, progetti o obiettivi allineati.

## Aggiungere un risultato a un obiettivo

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![](assets/results-value-initial-target-boxes-350x49.png)

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

1. Fai clic sul menu principale ![](assets/main-menu-icon.png), quindi **Obiettivi**.

1. Da **Elenco obiettivi**, fai clic sul nome di un obiettivo per aprire la pagina dell’obiettivo.
1. Fai clic su **Indicatori di progresso** nel pannello a sinistra.
1. Espandi la **Nuovo indicatore di avanzamento** menu a discesa, quindi fai clic su **Crea risultato**.

   Viene visualizzata la casella Nuovo risultato.

   ![](assets/new-result-box-unshimmed.png)

1. Immetti un nome per il risultato nel **Nome del risultato** campo . Questo è un campo obbligatorio.
1. (Facoltativo) Rimuovi il tuo nome dal **Proprietario del risultato** se si desidera assegnare il risultato a un altro utente. Per impostazione predefinita, sei il proprietario di un’attività creata.

   >[!NOTE]
   >
   >Non è possibile assegnare un team, un gruppo o la società come proprietario del risultato.

1. In **Come vuoi misurare il tuo risultato?** specificare le seguenti informazioni:
   * **Tipo di valore**: Indica come si desidera misurare l&#39;avanzamento del risultato. È possibile misurare l&#39;avanzamento numericamente, con un valore percentuale o utilizzando un importo in valuta.

      Selezionare un tipo di valore dalle opzioni elencate nella tabella seguente:

      | Tipo di valore | Descrizione |
      |---------------------------------------------------------|------------------|
      | Numero | Valore numerico |
      | % | Valore percentuale |
      | CN¥,DKK,KR,Mex$, R, R$, zł, £ , ¥ , € , ₹, ฿, MYR, ₪, $ | Valori valuta |

   * **Valore iniziale**: Il valore che il risultato ha all&#39;inizio, prima che qualsiasi progresso su di esso sia stato registrato.
   * **Valore di destinazione**: Il valore che il risultato ha lo scopo di ottenere quando viene considerato completato.
1. Fai clic su **Crea risultato**.

   Il risultato viene visualizzato nella sezione Indicatori di avanzamento della pagina dell&#39;obiettivo, sotto il raggruppamento Risultato.

   Dopo aver attivato l&#39;obiettivo, l&#39;avanzamento dell&#39;obiettivo viene aggiornato automaticamente quando si aggiorna l&#39;avanzamento di un risultato. Per informazioni sull&#39;attivazione di un obiettivo, vedi [Attivare gli obiettivi in Obiettivi di Adobe Workfront](../goal-management/activate-goals.md).
