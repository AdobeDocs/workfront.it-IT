---
product-previous: workfront-goals
navigation-topic: goal-management
title: Filtrare le informazioni negli obiettivi di Adobe Workfront
description: Puoi visualizzare gli obiettivi che tu o chiunque altro hai aggiunto negli Obiettivi di Adobe Workfront. Per informazioni sulla creazione degli obiettivi, consulta Creare gli obiettivi in Obiettivi di Adobe Workfront. Quando visualizzi gli obiettivi, puoi filtrare le informazioni in Obiettivi di Workfront per visualizzare solo gli obiettivi che ti interessano.
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 2%

---

# Filtrare le informazioni in Obiettivi di Adobe Workfront

<!--Audited for P&P only: 4/2025-->

Puoi visualizzare gli obiettivi che tu o chiunque altro hai aggiunto negli Obiettivi di Adobe Workfront. Per informazioni sulla creazione degli obiettivi, vedere [Creare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md). Quando visualizzi gli obiettivi, puoi filtrare le informazioni in Obiettivi di Workfront per visualizzare solo gli obiettivi che ti interessano.

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
  <p>Visualizza o autorizzazioni superiori per gli obiettivi da visualizzare</p>
  <p>Gestire le autorizzazioni per gli obiettivi per modificarli</p>
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
   <p> New product requirement: Workfront</p>
  <p>Or</p>
   <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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

## Panoramica dei filtri negli Obiettivi di Workfront

>[!NOTE]
>
>Per trovare e focalizzare in modo efficiente gli obiettivi giusti, ti consigliamo di utilizzare i filtri in Obiettivi di Workfront. Questo consente di visualizzare le informazioni corrette prima di iniziare a gestire gli obiettivi che ritieni importanti. Per impostazione predefinita, in Obiettivi Workfront vengono visualizzati tutti gli obiettivi del sistema.

Puoi individuare e filtrare gli obiettivi nelle seguenti sezioni dell’area Obiettivi in Workfront:

* Elenco obiettivi
* Grafi
* Allineamento obiettivi

Per informazioni sulle sezioni dell&#39;area Obiettivi, vedere [Panoramica delle sezioni Obiettivi di Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

>[!IMPORTANT]
>
>È possibile configurare i filtri per una sezione e mantenerli persistenti quando si passa a un’altra sezione di Obiettivi di Workfront.

Quando si lavora con i filtri negli Obiettivi di Workfront, considera quanto segue:

* Puoi creare e applicare un filtro senza salvarlo, oppure salvare un filtro da riutilizzare in un secondo momento.

  Esistono i seguenti scenari:

   * Quando salvi un filtro, questo diventa il filtro predefinito per te ogni volta che accedi a Workfront Goals.
   * Quando applichi un filtro senza salvarlo, puoi ripristinare gli elenchi originali aggiornando la pagina.

* Puoi solo visualizzare e applicare i filtri creati. I filtri creati da altri utenti vengono visualizzati solo per tali utenti.
* Non puoi condividere i filtri creati con altri utenti.

## Applicare un filtro rapido in Obiettivi di Workfront

Puoi utilizzare un filtro rapido in un elenco di obiettivi per individuare solo gli elementi che ti interessano. Non è possibile salvare i filtri rapidi e non sono persistenti. Workfront cancella i risultati di un filtro rapido quando aggiorni la pagina.

Per ulteriori informazioni, vedere [Applicare il filtro rapido a un elenco](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

## Creare e applicare un filtro in Obiettivi di Workfront

Il processo di creazione dei filtri è lo stesso per qualsiasi sezione degli Obiettivi di Workfront.

Puoi creare un filtro da zero o modificare uno dei filtri incorporati.

1. Vai a Obiettivi Workfront.

   Per informazioni sull&#39;accesso agli obiettivi di Workfront, vedere [Accesso e apertura degli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)

   Per impostazione predefinita, viene visualizzata la sezione Elenco obiettivi.

1. Fai clic su **Filtro** nell&#39;angolo superiore destro dell&#39;elenco.

   ![Icona filtro](assets/filter-icon-and-label.png)

   Per impostazione predefinita, Workfront applica il filtro **All** che visualizza tutti gli obiettivi nel sistema.

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
        <td>Tutto</td> 
        <td> <p>Tutti gli obiettivi nel sistema, indipendentemente da chi li ha creati, da quale periodo di tempo si riferiscono o da chi sia il proprietario. Questo è il filtro predefinito e non puoi modificarlo. </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>Personale</td> 
        <td>Gli obiettivi di cui sei il proprietario.</td> 
       </tr> 
       <tr> 
        <td>I miei team</td> 
        <td> <p>Gli obiettivi per i quali qualsiasi team è selezionato come proprietario. </p> <p><b>SUGGERIMENTO</b>

     Non viene visualizzato alcun obiettivo se non si è assegnati ad alcun team. </p> </td>
     </tr> 
       <tr> 
        <td>I miei gruppi</td> 
        <td>Gli obiettivi per i quali uno qualsiasi dei tuoi gruppi è selezionato come proprietario. </td> 
       </tr> 
       <tr> 
        <td>Azienda</td> 
        <td> <p>Gli obiettivi associati alla tua organizzazione. </p> <p><b>SUGGERIMENTO</b>
        <p>In Obiettivi di Adobe Workfront, il filtro Azienda visualizza gli obiettivi per i quali l’organizzazione è selezionata come proprietario. </p> <p>Non è possibile cercare società utilizzando questo campo. Per impostazione predefinita, viene selezionata solo l’organizzazione proprietaria dell’istanza di Workfront. </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * Passa il puntatore del mouse sul nome di un filtro, quindi fai clic sull&#39;icona **Modifica** ![Modifica icona](assets/edit-icon.png) accanto al nome per personalizzarlo e aggiungere nomi specifici di utenti, team, gruppi o il nome della tua organizzazione, quindi selezionalo quando vengono visualizzati nell&#39;elenco.

   * Fai clic su **Nuovo filtro** per creare un nuovo filtro, quindi seleziona una delle seguenti opzioni per personalizzare il nuovo filtro:

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
        <td> <p>Seleziona uno stato nel menu a discesa tra le seguenti opzioni:</p> 
         <ul> 
          <li> <p>Attivo</p> </li> 
          <li> <p>Bozza</p> </li> 
          <li> <p>Inattiva</p> </li> 
          <li> <p>Chiuso</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Avanzamento</td> 
        <td> <p>Seleziona un avanzamento nel menu a discesa tra le seguenti opzioni: </p> 
         <ul> 
          <li> <p>In difficoltà</p> </li> 
          <li> <p>A Rischio</p> </li> 
          <li> <p>Puntuale</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Proprietario</td> 
        <td> <p>Inizia a digitare il nome di un proprietario, quindi selezionalo quando viene visualizzato nell’elenco. </p> <p>Puoi digitare i nomi di utenti, team, gruppi o il nome della tua organizzazione oppure puoi scegliere tra opzioni predefinite. </p> <p>Le seguenti opzioni di filtro predefinite fanno sempre riferimento all’utente attualmente connesso: </p> 
         <ul> 
          <li> <p><strong>Me</strong>: visualizza gli obiettivi di cui sei il proprietario.</p> </li> 
          <li> <p><strong>Il mio team predefinito</strong> e <strong>Tutti i miei team</strong>: visualizza gli obiettivi per i quali il tuo team predefinito o uno qualsiasi dei tuoi team è designato come proprietario. </p> <p>Suggerimento: non viene visualizzato alcun obiettivo quando non si è assegnati ad alcun team. </p> </li> 
          <li> <p><strong>Il mio gruppo predefinito</strong> e <strong>Tutti i miei gruppi</strong>: visualizza gli obiettivi in cui il tuo gruppo predefinito o uno qualsiasi dei tuoi gruppi sono designati come proprietari.</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. (Facoltativo) Fai clic su **Reimposta** nell&#39;angolo inferiore destro della casella del filtro per cancellare tutti i campi selezionati e iniziare a creare il filtro da zero.
1. (Facoltativo) Fai clic su **Applica** per applicare il filtro senza salvarlo.

   Il filtro viene visualizzato nell&#39;area **Non salvato** del generatore di filtri come **Nuovo filtro**.

   Impossibile rinominare un filtro non salvato.

   I filtri non salvati vengono rimossi dall’area Obiettivi al successivo accesso a Workfront.

   >[!TIP]
   >
   >Puoi avere un solo nuovo filtro non salvato alla volta.

1. Fai clic su **Salva** per salvare il filtro e utilizzarlo in seguito, quindi aggiungi un nome per il filtro nel campo **Aggiungi nome filtro** e fai clic su **Fine**.

   Il filtro verrà salvato nella sezione **Salvato** del generatore di filtri. Puoi utilizzare questo filtro in futuro.

   L’ultimo filtro salvato e applicato viene visualizzato per impostazione predefinita al successivo accesso a Workfront

1. (Facoltativo) Fai clic sulla **freccia rivolta a sinistra** accanto a **Nuovo filtro** per uscire dal generatore di filtri e tornare all&#39;elenco dei filtri.
1. (Facoltativo) Passa il puntatore del mouse sul nome di un filtro personalizzato, fai clic sul menu **Altro**, quindi su **Elimina**, quindi su **Elimina**. Il filtro verrà eliminato e non sarà più possibile ripristinarlo.

   >[!TIP]
   >
   >Non è possibile eliminare i filtri predefiniti.

1. Fai clic sull&#39;icona **X** nell&#39;angolo superiore destro del generatore di filtri per chiudere il generatore di filtri.

   Il nome del filtro attualmente applicato viene visualizzato a destra dell&#39;icona Filtro, nell&#39;angolo superiore destro dell&#39;elenco degli obiettivi.

   L’elenco degli obiettivi viene filtrato in base ai criteri di filtro.

1. (Facoltativo e condizionale) Quando visualizzi gli obiettivi nella sezione Allineamento obiettivi, fai clic su **Mostra** per visualizzare gli obiettivi esclusi.

   ![Mostra collegamento agli elementi filtrati](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   Il nome del filtro è evidenziato in giallo per indicare che viene ignorato.

   ![Filtra contorno giallo](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. (Facoltativo e condizionale) Fare clic su **Riapplica filtro** per applicare il filtro e omettere gli elementi visualizzati nel passaggio precedente.


