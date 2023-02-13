---
product-previous: workfront-goals
navigation-topic: goal-management
title: Filtrare le informazioni negli obiettivi di Adobe Workfront
description: Puoi visualizzare gli obiettivi che hai aggiunto o chiunque altro in Obiettivi di Adobe Workfront. Per informazioni sulla creazione degli obiettivi, consulta Creare obiettivi in Obiettivi di Adobe Workfront. Quando visualizzi gli obiettivi, puoi filtrare le informazioni in Obiettivi di Workfront per visualizzare solo gli obiettivi importanti per te.
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '1342'
ht-degree: 2%

---

# Filtrare le informazioni negli obiettivi di Adobe Workfront

Puoi visualizzare gli obiettivi che hai aggiunto o chiunque altro in Obiettivi di Adobe Workfront. Per informazioni sulla creazione degli obiettivi, vedi [Creare obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md). Quando visualizzi gli obiettivi, puoi filtrare le informazioni in Obiettivi di Workfront per visualizzare solo gli obiettivi importanti per te.

## Requisiti di accesso

<!--drafted - replace the table below with this one when P&P releases: 

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

Per eseguire le azioni descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Visualizzare o accedere in modo più rapido agli obiettivi</p> <p><b>NOTA</b>

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
     <p>Visualizza o autorizzazioni superiori per gli obiettivi</p> 
     <p>Per informazioni sulla condivisione degli obiettivi, vedi <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario disporre dei seguenti elementi prima di poter iniziare:

* Modello di layout che include l’area Obiettivi del menu principale.

## Panoramica dei filtri negli obiettivi di Workfront

>[!NOTE]
>
>Per trovare e concentrarsi in modo efficiente sugli obiettivi giusti, ti consigliamo di utilizzare i filtri in Obiettivi di Workfront. Questo ti consente di visualizzare le informazioni corrette prima di iniziare a gestire gli obiettivi che sono importanti per te. Per impostazione predefinita, Obiettivi di Workfront mostra tutti gli obiettivi del sistema.

Puoi individuare e filtrare gli obiettivi nelle seguenti sezioni dell’area Obiettivi di Workfront:

* Elenco obiettivi
* Grafi
* Allineamento obiettivo

Per informazioni sulle sezioni dell&#39;area Obiettivi, vedi [Panoramica delle sezioni Obiettivi di Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

>[!IMPORTANT]
>
>Puoi configurare i filtri per una sezione che restano persistenti quando vieni spostato in un’altra sezione degli obiettivi di Workfront.

Quando si lavora con i filtri negli obiettivi di Workfront, considera quanto segue:

* È possibile creare e applicare un filtro senza salvarlo oppure salvare un filtro da riutilizzare in un secondo momento.

   Esistono i seguenti scenari:

   * Quando salvi un filtro, questo diventa il filtro predefinito per ogni accesso a Obiettivi di Workfront.
   * Quando applichi un filtro senza salvarlo, puoi ripristinare gli elenchi originali aggiornando la pagina.

* Puoi visualizzare e applicare solo i filtri creati. I filtri creati da altri utenti vengono visualizzati solo per tali utenti.
* Non puoi condividere i filtri creati con altri utenti.

## Applicazione di un filtro rapido negli obiettivi di Workfront

Puoi utilizzare un filtro rapido in un elenco di obiettivi per individuare solo gli elementi importanti per te. Non è possibile salvare i filtri rapidi e non sono persistenti. Workfront cancella i risultati di un filtro rapido quando si aggiorna la pagina.

Per ulteriori informazioni, consulta [Applicare il filtro rapido a un elenco](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

## Creare e applicare un filtro in Obiettivi di Workfront

La procedura per la creazione di filtri è la stessa per qualsiasi sezione di Obiettivi di Workfront.

Puoi creare un filtro da zero o modificare uno dei filtri incorporati.

1. Vai agli obiettivi di Workfront.

   Per informazioni sull&#39;accesso agli obiettivi di Workfront, vedi [Accedere e aprire gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)

   Per impostazione predefinita, viene visualizzata la sezione Elenco obiettivi .

1. Fai clic su **Filtro** nell&#39;angolo superiore destro dell&#39;elenco.

   ![](assets/filter-icon-and-label.png)

   Per impostazione predefinita, in Workfront viene applicato il **Tutto** , che visualizza tutti gli obiettivi del sistema.

   >[!TIP]
   >
   >Non è possibile modificare o eliminare il filtro Tutto.

1. Esegui una delle operazioni seguenti:

   * Fai clic su uno dei seguenti filtri predefiniti per visualizzare gli obiettivi solo per i seguenti proprietari:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>Tutti</td> 
        <td> <p>Tutti gli obiettivi del sistema, indipendentemente da chi li ha creati, dal periodo di tempo in cui si trovano o dal proprietario. Questo è il filtro predefinito e non è possibile modificarlo. </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>Personale</td> 
        <td>Gli obiettivi per i quali sei il proprietario.</td> 
       </tr> 
       <tr> 
        <td>I miei team</td> 
        <td> <p>Obiettivi per i quali uno dei team viene selezionato come proprietario. </p> <p><b>SUGGERIMENTO</b>

      Non viene visualizzato alcun obiettivo quando non sei assegnato ad alcun team. </p> </td>
      </tr> 
       <tr> 
        <td>I miei gruppi</td> 
        <td>Gli obiettivi per i quali uno dei tuoi gruppi viene selezionato come proprietario. </td> 
       </tr> 
       <tr> 
        <td>Azienda</td> 
        <td> <p>Gli obiettivi associati alla tua organizzazione. </p> <p><b>SUGGERIMENTO</b>
        <p>In Obiettivi di Adobe Workfront, il filtro Azienda visualizza gli obiettivi per i quali la tua organizzazione è selezionata come proprietario. </p> <p>Non è possibile cercare le aziende che utilizzano questo campo. Per impostazione predefinita viene selezionata solo l’organizzazione proprietaria dell’istanza Workfront. </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * Passa il puntatore del mouse sul nome di un filtro, quindi fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png) accanto al nome per personalizzarlo e aggiungere nomi specifici di utenti, team, gruppi o nome della tua organizzazione, quindi selezionalo quando compaiono nell’elenco.

   * Fai clic su **Nuovo filtro** per creare un nuovo filtro, seleziona una delle seguenti opzioni per personalizzare il nuovo filtro:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Periodo</td> 
        <td>Seleziona un periodo di tempo nel menu a discesa. È possibile selezionare più periodi di tempo. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Stato</td> 
        <td> <p>Seleziona uno stato nel menu a discesa dalle seguenti opzioni:</p> 
         <ul> 
          <li> <p>Attivi</p> </li> 
          <li> <p>Bozza</p> </li> 
          <li> <p>Inattiva</p> </li> 
          <li> <p>Chiuso</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Avanzamento</td> 
        <td> <p>Seleziona un avanzamento nel menu a discesa dalle seguenti opzioni: </p> 
         <ul> 
          <li> <p>In difficoltà</p> </li> 
          <li> <p>A Rischio</p> </li> 
          <li> <p>Puntuale</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Proprietario</td> 
        <td> <p>Inizia a digitare il nome di un proprietario, quindi selezionalo quando viene visualizzato nell’elenco. </p> <p>È possibile digitare i nomi degli utenti, dei team, dei gruppi o del nome della propria organizzazione oppure selezionare una delle opzioni predefinite. </p> <p>Le seguenti opzioni di filtro predefinite fanno sempre riferimento all’utente attualmente connesso: </p> 
         <ul> 
          <li> <p><strong>Me</strong>: Visualizza gli obiettivi in cui sei il proprietario.</p> </li> 
          <li> <p><strong>Gruppo home personale</strong> e <strong>Tutti i miei team</strong>: Visualizza gli obiettivi in cui il team principale o uno dei team è designato come proprietario. </p> <p>Suggerimento: Non viene visualizzato alcun obiettivo quando non sei assegnato ad alcun team. </p> </li> 
          <li> <p><strong>Gruppo Home personale</strong> e <strong>Tutti i gruppi</strong>: Visualizza gli obiettivi in cui il gruppo principale o uno dei gruppi sono designati come proprietari.</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. (Facoltativo) Fai clic su **Reimposta** nell’angolo in basso a destra della casella del filtro per cancellare tutti i campi selezionati e iniziare a creare il filtro da zero.
1. (Facoltativo) Fai clic su **Applica** per applicare il filtro senza salvarlo.

   Il filtro viene visualizzato nella **Non salvato** area del generatore di filtri come **Nuovo filtro**.

   Non è possibile rinominare un filtro non salvato.

   I filtri non salvati vengono rimossi dall’area Obiettivi alla successiva disconnessione da Workfront e successivo accesso.

   >[!TIP]
   >
   >È disponibile un solo nuovo filtro non salvato alla volta.

1. Fai clic su **Salva** per salvare il filtro e utilizzarlo in un secondo momento, aggiungi un nome per il filtro nel **Aggiungi nome filtro** campo e fai clic su **Fine**.

   In questo modo il filtro viene salvato nella **Salvato** nel generatore di filtri. Puoi utilizzare questo filtro in futuro.

   L’ultimo filtro salvato e applicato viene visualizzato per impostazione predefinita al successivo accesso a Workfront

1. (Facoltativo) Fai clic sul pulsante **freccia rivolta a sinistra** accanto a **Nuovo filtro** per uscire dal generatore di filtri e tornare all’elenco dei filtri.
1. (Facoltativo) Passa il puntatore del mouse sul nome di un filtro personalizzato, quindi fai clic sul pulsante **Altro** menu, quindi fai clic su **Elimina**, quindi **Elimina**. Questo elimina il filtro e non è possibile ripristinarlo.

   >[!TIP]
   >
   >Non è possibile eliminare nessuno dei filtri predefiniti.

1. Fai clic sul pulsante **Icona X** nell’angolo in alto a destra del generatore di filtri per chiudere il generatore di filtri.

   Il nome del filtro attualmente applicato viene visualizzato a destra dell’icona Filtro , nell’angolo in alto a destra dell’elenco degli obiettivi.

   L’elenco degli obiettivi viene filtrato in base ai criteri di filtro.

1. (Facoltativo e condizionale) Quando si visualizzano gli obiettivi nella sezione Allineamento obiettivo, fare clic su **Mostra loro** per visualizzare gli obiettivi filtrati.

   ![](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   Il nome del filtro è evidenziato in giallo per indicare che viene ignorato.

   ![](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. (Facoltativo e condizionale) Fai clic su **Riapplica filtro** per applicare il filtro e omettere gli elementi visualizzati nel passaggio precedente.


