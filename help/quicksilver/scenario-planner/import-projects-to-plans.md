---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Importare progetti in piani nel planner scenario
description: È possibile importare progetti esistenti in un piano. I progetti importati vengono convertiti in iniziative e puoi gestirli all’interno del piano come gestiresti una nuova iniziativa. Il progetto originale rimane legato alla nuova iniziativa.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 844dddec944b6cfb0957eecf09c2980e9d0577cc
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---

# Importa progetti nei piani [!DNL Scenario Planner]

È possibile importare progetti esistenti in un piano. I progetti importati vengono convertiti in iniziative e puoi gestirli all’interno del piano come gestiresti una nuova iniziativa. Il progetto originale rimane legato alla nuova iniziativa.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> piano*</b> </p> </td> 
   <td>[!UICONTROL Business] o superiore</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licenza*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td><b>Prodotto</b> </td> 
   <td> <p>È necessario acquistare una licenza aggiuntiva per [!DNL Adobe Workfront Scenario Planner] per accedere alla funzionalità descritta in questo articolo.</p> <p>Per informazioni su come ottenere [!DNL Workfront Scenario Planner], vedi <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accesso necessario per utilizzare [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Accesso o superiore a [!DNL Scenario Planner]</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Autorizzazioni di gestione per un piano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo a un piano, vedi <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Richiedere l'accesso a un piano nel Planner scenario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Considerazioni sull&#39;importazione di progetti nei piani come nuove iniziative

* È necessario creare progetti prima di poterli importare in un piano come nuove iniziative.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* Devi avere almeno [!UICONTROL Visualizza] autorizzazioni ai progetti per poterli importare in un piano come nuova iniziativa.
* È possibile importare lo stesso progetto in più piani.
* I progetti da importare devono avere date incluse nell’intervallo di tempo del piano. Non è possibile importare progetti con un [!UICONTROL Data completamento pianificata] prima dell&#39;inizio del piano o [!UICONTROL Data di inizio prevista] oltre la fine del piano.
* Non puoi importare più di 100 progetti alla volta.
* Alcune informazioni di progetto vengono importate nel piano e diventano informazioni di iniziativa. Per informazioni sulle informazioni relative al progetto che vengono importate nel piano e che diventano informazioni relative all’iniziativa, consulta la [Informazioni di progetto importate nel piano](#project-information-imported-into-the-plan) in questo articolo.
* Le modifiche apportate ai progetti collegati non incidono sulle iniziative del piano.
* Le modifiche apportate alle iniziative del piano non influiscono automaticamente sui progetti collegati Le modifiche dell&#39;iniziativa riguardano i progetti collegati solo quando l&#39;iniziativa viene pubblicata dal piano. Per informazioni su come le iniziative di pubblicazione influiscono sui progetti collegati, vedi [Aggiornare o creare progetti pubblicando iniziative nel [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* L’eliminazione di un’iniziativa creata importando un progetto non comporta l’eliminazione del progetto.
* L&#39;eliminazione di un progetto collegato a un&#39;iniziativa non comporta l&#39;eliminazione dell&#39;iniziativa.

## Informazioni di progetto importate nel piano {#project-information-imported-into-the-plan}

Quando si importa un progetto in un piano, alcune informazioni vengono importate nel piano e diventano informazioni di iniziativa. La tabella seguente mostra quali informazioni di progetto diventano informazioni di iniziativa quando si importa un progetto in un piano:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Informazioni sul progetto</td> 
   <td>Informazioni sull'iniziativa </td> 
  </tr> 
  <tr> 
   <td>Nome progetto</td> 
   <td>Nome dell'iniziativa</td> 
  </tr> 
  <tr> 
   <td>Date pianificate Progetto</td> 
   <td> <p>Iniziativa mesi di inizio e fine.</p> <p>Se un progetto inizia o termina a metà mese, le date importate vengono estese in modo da includere un mese intero nel piano. Ad esempio, se le date previste per il progetto sono dal 20 marzo al 5 maggio 2020, le date dell’iniziativa importata saranno da marzo a maggio 2020.</p> <p>Se la data di inizio o di completamento pianificata supera la durata del piano, è presente un'indicazione visiva che l'iniziativa importata inizia prima o termina dopo il piano. </p> </td> 
  </tr> 
  <tr> 
   <td>Ruoli di lavoro assegnati a attività e problemi</td> 
   <td> <p>Mansioni iniziativa. </p> <p>Nota:   <p>Se un utente cambia ruoli durante la durata del progetto, i ruoli importati dipendono dallo stato dell'assegnazione al momento dell'importazione del progetto. Esistono i seguenti scenari:</p> 
     <ul> 
      <li> <p>Se un utente assegnato a un'attività o a un problema ha modificato il proprio ruolo dopo aver contrassegnato l'assegnazione come [!UICONTROL Done], [!DNL Workfront] importa nell'iniziativa il ruolo svolto dall'utente prima che abbia contrassegnato l'assegnazione come [!UICONTROL Done].</p> </li> 
      <li> <p>Se un utente assegnato a un'attività o a un problema ha modificato il ruolo durante la durata del progetto ma la loro assegnazione all'attività o al problema non è contrassegnata come [!UICONTROL Fine] quando si importa il progetto, [!DNL Workfront] importa solo il ruolo corrente dell'utente assegnato. </p> </li> 
     </ul> <p>Per informazioni sullo stato di un'assegnazione, vedere "Stato assegnazione" in <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossario dell'Adobe [!DNL Workfront] terminologia</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Progetto [!UICONTROL Pianificato ore] associato a ruoli di lavoro assegnati a attività o problemi</td> 
   <td> <p><span>A seconda che il piano sia impostato per l’utilizzo di FTE o ore, le [!UICONTROL Pianificato ore] dalle attività del progetto diventano</span> [!UICONTROL FTE richieste] <span>o [!UICONTROL Ore richieste] sul piano</span>. </p> <p>Per informazioni sull'impostazione di un piano per l'uso di FTE o ore, vedi <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crea e modifica piani in [!DNL Scenario Planner]</a>. </p> <p>Considera quanto segue:</p> 
    <ul> 
     <li> <p>[!DNL Workfront] utilizza i ruoli job assegnati a task e problemi o i ruoli job a cui sono associati gli utenti assegnati a task o problemi nel progetto e li trasferisce alla nuova iniziativa come Ruoli job richiesti. </p> </li> 
     <li> <p>Quando il piano è impostato per l’utilizzo di FTE, le ore pianificate associate ai ruoli del lavoro sulle attività e sui problemi del progetto vengono prima convertite in FTE. Questo ETP viene quindi assegnato al ruolo di lavoro dell'iniziativa. <span>Gli orari pianificati sono equamente distribuiti in [!DNL Workfront]. Se un’attività o un problema si estende per più mesi, l’importo di Orari pianificati per ogni mese nella durata dell’iniziativa viene convertito in ETP mensile e trasferito a ogni mese dell’iniziativa.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><span>Ad esempio, se un’attività viene assegnata a un ruolo di lavoro per 80 ore pianificate in settembre, il ruolo di lavoro importato visualizza 0,5 FTE per l’iniziativa in settembre.</span> </p> </li> 
     <li> <p>[!DNL Workfront] calcola l’FTE dei ruoli di lavoro richiesti associati all’iniziativa utilizzando la seguente formula:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Suggerimento: La [!DNL Scenario Planner] presuppone che ci siano 160 ore lavorative in un mese.</p> <p>Ad esempio, se un progetto ha una durata di 1200 minuti e un ruolo di lavoro nel progetto è associato a 600 minuti di ore pianificate, l’ETP corrispondente è 0,5. Durante l’importazione del progetto, l’ETP con ruolo di lavoro obbligatorio nell’iniziativa appena creata è 0,5 per ogni mese dell’iniziativa. </p> </li> 
     <li>Quando un ruolo di lavoro viene assegnato a un'attività del progetto con zero ore pianificate, l'FTE richiesto per il ruolo di lavoro dell'iniziativa è zero per impostazione predefinita. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>Quando un ruolo di lavoro viene assegnato a un'attività del progetto con una [!UICONTROL Duration] pari a zero, l'FTE richiesto <span>o ore</span> per impostazione predefinita, il ruolo di lavoro dell'iniziativa è zero, anche se l'attività ha un orario pianificato. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## Importare progetti in un piano

>[!IMPORTANT]
>
>Dopo aver importato i progetti in un piano, diventano iniziative sul piano. Sebbene i due elementi siano collegati, esistono come entità indipendenti e non si influenzano automaticamente una volta aggiornati.
>
>Si verifica quanto segue:
>
>* Le modifiche al progetto non influiscono mai sull&#39;iniziativa dopo l&#39;importazione del progetto nel piano. Queste modifiche includono le modifiche alle allocazioni dei ruoli di lavoro.
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* Le modifiche apportate all&#39;iniziativa influiscono sulle informazioni contenute nella [!DNL Scenario Planner] nell’area del progetto solo quando l’iniziativa viene pubblicata nel progetto corrispondente. In caso contrario, non influiscono sul [!UICONTROL Orari pianificati] informazioni relative alle attività e ai problemi del progetto.
>
>  Per informazioni su come le iniziative di pubblicazione influiscono sui progetti collegati, vedi  [Aggiornare o creare progetti pubblicando iniziative nel Planner scenario](../scenario-planner/publish-scenarios-update-projects.md).

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Workfront], quindi fai clic su [!DNL Scenarios] per accedere al [!DNL Scenario Planner].

1. Fare clic sul nome del piano in cui si desidera importare i progetti.
1. Fai clic su **[!UICONTROL Nuova iniziativa]**, quindi fai clic su **[!UICONTROL Importa progetti]**.

   La [!UICONTROL Importa progetti] viene visualizzata la casella . I progetti con date incluse nell’intervallo di tempo del piano vengono visualizzati in un elenco.

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >I progetti in qualsiasi stato vengono visualizzati nell’elenco.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Icona Filtro]** ![](assets/filter-nwepng.png)e seleziona un filtro disponibile dall’elenco per ridurre la quantità di progetti nell’elenco. Per impostazione predefinita, l’elenco dei progetti viene filtrato dal filtro di progetto attualmente selezionato dall’utente in un elenco di progetti.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Icona Ricerca]** ![](assets/search-icon.png) e aggiungi una parola chiave visualizzata su qualsiasi campo sullo schermo. Gli elementi contenenti la parola di ricerca vengono visualizzati automaticamente nell’elenco e tutti gli elementi sono nascosti.

1. (Condizionale) Fai clic sul pulsante **[!UICONTROL Icona X]** per rimuovere la ricerca e visualizzare tutti i progetti.
1. Seleziona fino a 100 progetti e fai clic su **[!UICONTROL Importa]**.

   I progetti vengono importati come nuove iniziative.

   Osserva quanto segue:

   * Icona di un progetto ![](assets/project-icon-sp.png) viene visualizzato a destra del nome dell&#39;iniziativa.
   * Se la tempistica del progetto supera la durata del piano, la barra dell&#39;iniziativa termina con un margine puntato a sinistra (quando la data di inizio è precedente alla data del piano) o a destra (quando la data di fine è successiva alla data del piano).

      ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * Il numero di mesi e i ruoli di lavoro sono stati aggiornati in modo da corrispondere a quelli del progetto.
   >[!TIP]
   >
   >I costi associati ai ruoli di lavoro vengono aggiornati a livello di iniziativa e non vengono importati dal progetto.

1. Fai clic sulla barra che rappresenta la nuova iniziativa per aprire il pannello dei dettagli dell&#39;iniziativa a destra.

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   In **[!UICONTROL Durata dell&#39;iniziativa]** esaminare le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Iniziativa Durata]</td> 
      <td>Questa è la durata dell'iniziativa in mesi. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>Le date di inizio e di fine dell'iniziativa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Project]</td> 
      <td> <p>Le [!UICONTROL Pianificato inizio] e [!UICONTROL Date di completamento] del progetto collegato.</p> <p>Suggerimento: Se mancano le informazioni sul progetto, il progetto è stato eliminato.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Modifica il nome dell’iniziativa. Per impostazione predefinita, corrisponde al nome del progetto.
1. (Facoltativo) Effettua una delle seguenti operazioni:

   * Aggiornare i ruoli del lavoro nel **[!UICONTROL Ruoli di lavoro richiesti]** sezione
   * Aggiorna **[!UICONTROL Costi fissi]** in **[!UICONTROL Costi]** sezione

   * Fai clic su **[!UICONTROL Aggiorna ruoli di lavoro disponibili]** o **[!UICONTROL Aggiorna budget disponibile]** risolvere i conflitti tra la nuova iniziativa e le altre iniziative del piano.

1. (Condizionale) Fai clic su **[!UICONTROL Applica]** per salvare le modifiche apportate all’iniziativa.
1. Fai clic su **[!UICONTROL Salva piano]** per salvare le modifiche apportate al piano.
1. (Facoltativo) Per aggiornare le modifiche apportate all’iniziativa al progetto da cui è stata importata, pubblica il progetto dal piano. Per informazioni sui piani di pubblicazione, consulta [Aggiornare o creare progetti pubblicando iniziative nel [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. (Facoltativo) Fai clic sull’icona del progetto per accedere al progetto collegato.

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
