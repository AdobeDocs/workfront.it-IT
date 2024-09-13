---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Importare progetti nei piani nella Pianificazione scenario
description: Puoi importare progetti esistenti in un piano. I progetti importati vengono convertiti in iniziative e puoi gestirle all’interno del piano come faresti con una nuova iniziativa. Il progetto originale resta collegato alla nuova iniziativa.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '1690'
ht-degree: 0%

---

# Importa progetti nei piani in [!DNL Scenario Planner]

Puoi importare progetti esistenti in un piano. I progetti importati vengono convertiti in iniziative e puoi gestirle all’interno del piano come faresti con una nuova iniziativa. Il progetto originale resta collegato alla nuova iniziativa.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] piano*</p> </td> 
   <td> <ul></li>
   <li><p>Nuovo: Ultimate </p></li>
   <p>Pianificazione scenario non disponibile per i nuovi piani Workfront Select o Workfront Prime. </p>
   <li><p>Corrente: [!UICONTROL Business] o versione successiva</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza*</p> </td> 
   <td> <p>Nuovo: Chiaro o superiore</p> 
   <p>Corrente: [!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td>Prodotto* </td> 
   <td> <ul><li><p>Per i nuovi piani Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Per i piani Workfront correnti: </p>
   <p>Adobe Workfront</p> <p>Pianificazione scenario Adobe Workfront</p></li></ul>

<p>Per ulteriori informazioni, vedere <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Livello di accesso </td> 
   <td> <p>Accesso di [!UICONTROL Edit] al [!DNL Scenario Planner]</p> <p>Accesso di visualizzazione o superiore ai progetti.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorizzazioni oggetto </p> </td> 
   <td> <p>Autorizzazioni [!UICONTROL Manage] per un piano</p> <p>Visualizza o autorizzazioni superiori per i progetti.</p><p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedere <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedere accesso a un piano in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso alla documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sull&#39;importazione di progetti nei piani come nuove iniziative

* È necessario creare progetti prima di importarli in un piano come nuove iniziative.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* Devi disporre almeno delle autorizzazioni [!UICONTROL Visualizza] per i progetti per poterli importare in un piano come nuova iniziativa.
* Puoi importare lo stesso progetto in più piani.
* I progetti da importare devono avere date incluse nell’intervallo di tempo del piano. Non puoi importare progetti con una [!UICONTROL Data di completamento pianificata] precedente all&#39;inizio del piano o una [!UICONTROL Data di inizio pianificata] successiva alla fine del piano.
* Non puoi importare più di 100 progetti alla volta.
* Alcune informazioni sul progetto vengono anche importate nel piano e diventano informazioni sull’iniziativa. Per informazioni su quali informazioni di progetto vengono importate nel piano e diventano informazioni sull&#39;iniziativa, vedere la sezione [Informazioni di progetto importate nel piano](#project-information-imported-into-the-plan) in questo articolo.
* Le modifiche che si verificano sui progetti collegati non influiscono sulle iniziative nel piano.
* Le modifiche apportate alle iniziative nel piano non influiscono automaticamente sui progetti collegati Le modifiche apportate all&#39;iniziativa interessano i progetti collegati solo quando si pubblica l&#39;iniziativa dal piano. Per informazioni su come la pubblicazione delle iniziative influisce sui progetti collegati, vedere [Aggiornare o creare progetti pubblicando iniziative in [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* L’eliminazione di un’iniziativa creata importando un progetto non comporta l’eliminazione del progetto.
* L’eliminazione di un progetto collegato a un’iniziativa non comporta l’eliminazione dell’iniziativa.

## Informazioni progetto importate nel piano {#project-information-imported-into-the-plan}

Quando si importa un progetto in un piano, alcune informazioni del progetto vengono importate anche nel piano e diventano informazioni sull&#39;iniziativa. Nella tabella seguente vengono illustrate le informazioni sul progetto che vengono convertite in informazioni sull&#39;iniziativa quando si importa un progetto in un piano:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Informazioni progetto</td> 
   <td>Informazioni iniziativa </td> 
  </tr> 
  <tr> 
   <td>Nome progetto</td> 
   <td>Nome iniziativa</td> 
  </tr> 
  <tr> 
   <td>Date pianificate Progetto</td> 
   <td> <p>Mesi di inizio e fine dell’iniziativa.</p> <p>Se un progetto inizia o termina a metà mese, le date importate vengono estese per coprire un mese intero nel piano. Ad esempio, se le date pianificate del progetto sono dal 20 marzo al 5 maggio 2020, le date dell’iniziativa importata sono dal marzo al maggio 2020.</p> <p>Se la data di inizio o completamento pianificata è successiva alla durata del piano, vi è un’indicazione visiva che l’iniziativa importata inizia prima o termina dopo il piano. </p> </td> 
  </tr> 
  <tr> 
   <td>Mansioni assegnate ad attività e problemi</td> 
   <td> <p>Ruoli iniziativa. </p> <p>Nota:   <p>Se un utente modifica i ruoli durante il progetto, i ruoli importati dipendono dallo stato dell’assegnazione al momento dell’importazione del progetto. Esistono i seguenti scenari:</p> 
     <ul> 
      <li> <p>Se un utente assegnato a un'attività o a un problema ha modificato il proprio ruolo dopo aver contrassegnato l'assegnazione come [!UICONTROL Done], [!DNL Workfront] importa nell'iniziativa il ruolo che l'utente ha svolto prima di contrassegnare l'assegnazione come [!UICONTROL Done].</p> </li> 
      <li> <p>Se un utente assegnato a un'attività o a un problema ha modificato il ruolo durante la durata del progetto, ma la sua assegnazione all'attività o al problema non è contrassegnata come [!UICONTROL Done] quando si importa il progetto, [!DNL Workfront] importa solo il ruolo corrente dell'utente assegnato. </p> </li> 
     </ul> <p>Per informazioni sullo stato di un'assegnazione, vedere "Stato assegnazione" in <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossario della terminologia dell'Adobe [!DNL Workfront]</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Progetto [!UICONTROL Lavoro Necessario] associato alle mansioni assegnate ad attività o problemi</td> 
   <td> <p><span>A seconda che il piano sia impostato per l'utilizzo di FTE o ore, le [!UICONTROL Ore pianificate] delle attività nel progetto diventano </span> [!UICONTROL FTE richieste] <span>o [!UICONTROL Ore richieste] nel piano</span>. </p> <p>Per informazioni sulla configurazione di un piano per l'utilizzo di FTE o ore, vedere <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Creare e modificare i piani in [!DNL Scenario Planner]</a>. </p> <p>Considera quanto segue:</p> 
    <ul> 
     <li> <p>[!DNL Workfront] utilizza le mansioni assegnate alle attività e ai problemi o le mansioni a cui gli utenti assegnati alle attività o ai problemi sono associati nel progetto e le trasferisce alla nuova iniziativa come Mansioni richieste. </p> </li> 
     <li> <p>Quando il piano è impostato per l’utilizzo di FTE, le ore pianificate associate ai ruoli sulle attività e sui problemi del progetto vengono prima convertite in FTE. Questo FTE viene quindi assegnato alla mansione dell’iniziativa. <span>Le ore pianificate sono equamente distribuite in [!DNL Workfront]. Se un'attività o un problema dura più mesi, la quantità di ore pianificate per ogni mese della durata dell'iniziativa viene convertita in FTE mensile e trasferita a ogni mese dell'iniziativa.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><span>Ad esempio, se un'attività è assegnata a una mansione per 80 ore pianificate in settembre, la mansione importata visualizza 0,5 FTE per l'iniziativa in settembre.</span> </p> </li> 
     <li> <p>[!DNL Workfront] calcola l’FTE dei Ruoli richiesti associati all’iniziativa utilizzando la formula seguente:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Suggerimento: [!DNL Scenario Planner] presuppone che vi siano 160 ore lavorative in un mese.</p> <p>Ad esempio, se un progetto ha una durata di 1200 minuti e una mansione sul progetto è associata a 600 minuti di ore pianificate, il valore FTE è 0,5. Durante l’importazione del progetto, l’FTE del ruolo richiesto per la nuova iniziativa creata è 0,5 per ogni mese dell’iniziativa. </p> </li> 
     <li>Quando una mansione viene assegnata a un'attività sul progetto con zero ore pianificate, l'FTE richiesto per la mansione dell'iniziativa è zero per impostazione predefinita. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>Quando una mansione viene assegnata a un'attività sul progetto con una durata pari a zero [!UICONTROL Duration], l'FTE <span>o le ore</span> richieste per la mansione dell'iniziativa è pari a zero per impostazione predefinita, anche se l'attività ha le ore pianificate. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Importare progetti in un piano

>[!IMPORTANT]
>
>Dopo aver importato i progetti in un piano, diventano iniziative sul piano. Anche se i due elementi sono collegati, esistono come entità indipendenti e non si influenzano automaticamente a vicenda quando vengono aggiornati.
>
>Si verificano le seguenti situazioni:
>
>* Le modifiche apportate al progetto non influiscono mai sull&#39;iniziativa dopo l&#39;importazione del progetto nel piano. Tali modifiche includono modifiche alle allocazioni dei ruoli.
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* Le modifiche apportate all&#39;iniziativa hanno effetto sulle informazioni nell&#39;area [!DNL Scenario Planner] del progetto solo quando si pubblica l&#39;iniziativa nel progetto corrispondente. In caso contrario, non influiscono sulle informazioni relative alle [!UICONTROL ore pianificate] per le attività e i problemi del progetto.
>
>  Per informazioni su come la pubblicazione delle iniziative influisce sui progetti collegati, vedere [Aggiornare o creare progetti pubblicando iniziative nella Pianificazione scenario](../scenario-planner/publish-scenarios-update-projects.md).
>

{{step1-to-scenario-planner}}

1. Fare clic sul nome di un piano in cui si desidera importare i progetti.
1. Fai clic su **[!UICONTROL Nuova iniziativa]**, quindi su **[!UICONTROL Importa progetti]**.

   Viene visualizzata la casella [!UICONTROL Importa progetti]. I progetti con date incluse nell’intervallo di tempo del piano vengono visualizzati in un elenco.

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >I progetti con qualsiasi stato vengono visualizzati nell’elenco.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Filtro]** ![](assets/filter-nwepng.png)e seleziona un filtro disponibile dall&#39;elenco per ridurre la quantità di progetti nel tuo elenco. Per impostazione predefinita, l’elenco dei progetti viene filtrato in base al filtro di progetto attualmente selezionato dall’utente in un elenco di progetti.

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Ricerca]** ![](assets/search-icon.png) e aggiungi una parola chiave visualizzata in qualsiasi campo dello schermo. Gli elementi contenenti la parola da cercare vengono visualizzati automaticamente nell&#39;elenco e tutti gli elementi sono nascosti.

1. (Condizionale) Fai clic sull&#39;icona **[!UICONTROL X]** per rimuovere la ricerca e visualizzare tutti i progetti.
1. Seleziona fino a 100 progetti e fai clic su **[!UICONTROL Importa]**.

   I progetti vengono importati come nuove iniziative.

   Osserva quanto segue:

   * A destra del nome dell&#39;iniziativa viene visualizzata l&#39;icona di progetto ![](assets/project-icon-sp.png).
   * Se la sequenza temporale del progetto supera la durata del piano, la barra dell&#39;iniziativa termina con un margine puntato a sinistra (quando la data di inizio è precedente alla data del piano) o a destra (quando la data di fine è successiva alla data del piano).

     ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * Il numero di mesi e mansioni è stato aggiornato per corrispondere a quelli del progetto.

   >[!TIP]
   >
   >I costi associati alle mansioni vengono aggiornati a livello di iniziativa e non vengono importati dal progetto.

1. Fai clic sulla barra che rappresenta la nuova iniziativa per aprire il pannello dei dettagli dell’iniziativa a destra.

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   Nell&#39;area **[!UICONTROL Durata iniziativa]** esaminare le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Duration]</td> 
      <td>Questa è la durata dell'iniziativa in mesi. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>Le date di inizio e fine dell’iniziativa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progetto [!UICONTROL]</td> 
      <td> <p>[!UICONTROL Planned Start] (Inizio pianificato) e [!UICONTROL Completion dates] (Date di completamento previste) del progetto collegato.</p> <p>Suggerimento: se mancano le informazioni del progetto [!UICONTROL], il progetto è stato eliminato.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Modifica il nome dell’iniziativa. Per impostazione predefinita, corrisponde al nome del progetto.
1. (Facoltativo) Effettuate una delle seguenti operazioni:

   * Aggiorna i ruoli nella sezione **[!UICONTROL Ruoli richiesti]**
   * Aggiorna **[!UICONTROL Costi fissi]** nella sezione **[!UICONTROL Costi]**

   * Fai clic su **[!UICONTROL Aggiorna ruoli disponibili]** o **[!UICONTROL Aggiorna budget disponibile]** per risolvere i conflitti tra la nuova iniziativa e altre iniziative nel piano.

1. (Condizionale) Fai clic su **[!UICONTROL Applica]** per salvare le modifiche apportate all&#39;iniziativa.
1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche apportate al piano.
1. (Facoltativo) Per aggiornare le modifiche apportate all&#39;iniziativa al progetto da cui è stata importata, pubblicare il progetto dal piano. Per informazioni sulla pubblicazione dei piani, vedere [Aggiornare o creare progetti pubblicando iniziative in [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. (Facoltativo) Fai clic sull’icona del progetto per accedere al progetto collegato.

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
