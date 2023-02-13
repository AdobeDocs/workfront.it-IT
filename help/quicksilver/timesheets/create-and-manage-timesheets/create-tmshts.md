---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Creare una scheda attività a uso singolo
description: È possibile creare manualmente una scheda attività a uso singolo se si desidera una scheda attività non ricorrente. Quando viene raggiunta la data di fine della scheda attività e sono necessarie più schede attività, è necessario crearne di nuove.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 1%

---

# Creare una scheda attività a uso singolo

È possibile creare manualmente una scheda attività a uso singolo se si desidera una scheda attività non ricorrente. Quando viene raggiunta la data di fine della scheda attività e sono necessarie più schede attività, è necessario crearne di nuove.

Per informazioni sulla creazione di un profilo foglio presenze che genera fogli presenze ricorrenti per gli utenti senza ulteriori interventi da parte dell&#39;utente (consigliato), vedere [Creare, modificare e assegnare profili della scheda attività](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* Non è possibile creare fogli presenze a uso singolo per i gruppi.

>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* Quando si crea una scheda attività a uso singolo, non è possibile selezionare tipi di ora generali specifici da includere nella scheda attività. Tutti i tipi di ora generale attivati nel sistema vengono visualizzati nei fogli presenze creati manualmente.
>
>  Se si desidera selezionare solo alcuni tipi di ore generali da visualizzare nei fogli presenze, utilizzare un profilo scheda attività. Per ulteriori informazioni sui profili della scheda attività, vedere [Creare, modificare e assegnare profili della scheda attività](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>È necessario disporre dell’accesso amministrativo ai fogli presenze. </p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> <p><b> NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Creare una scheda attività a uso singolo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Schede temporali**. La **Tutto** Il filtro è selezionato per impostazione predefinita. Vengono visualizzati tutti i fogli presenze a cui hai accesso.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facoltativo) Per aggiornare il filtro nell’elenco dei fogli presenze, effettuare una delle seguenti operazioni:

   * Seleziona **Approvazioni foglio presenze personali** nell’angolo in alto a destra della pagina per visualizzare solo i fogli presenze approvati

      Oppure

      Seleziona **Fogli orari personali** per visualizzare solo i fogli presenze.

      Questo applica le approvazioni della scheda attività personale o i filtri della scheda attività personale all&#39;elenco dei fogli presenze.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Fai clic sull’icona Filtro ![](assets/filter-nwepng.png) per applicare un filtro diverso o crearne uno nuovo. Per informazioni sulla creazione o l’aggiornamento dei filtri, consulta [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Pagine attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo hanno rimosso le approvazioni della scheda attività personale e i filtri della scheda attività personale dai controlli elenco nell&#39;area Configurazione o dal modello di layout. Per ulteriori informazioni, consulta i seguenti articoli:
   > 
   >   * [Personalizzare filtri, visualizzazioni e gruppi utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)



1. (Facoltativo) Fai clic sul pulsante **Ricerca** icona ![](assets/search-icon.png) digitare una parola chiave e cercare una scheda attività specifica. Ad esempio, è possibile cercare un intervallo di tempo della scheda attività del nome del proprietario.

1. (Facoltativo) Fai clic sul pulsante **Visualizza** ![](assets/view-icon.png) o **Raggruppamento** ![](assets/grouping.png) per applicare una visualizzazione o un raggruppamento diversi o per crearne uno nuovo.

   Per informazioni sulla creazione di filtri, visualizzazioni o raggruppamenti, consulta i seguenti articoli:

   * [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Creare o modificare visualizzazioni in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creare raggruppamenti in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Fai clic su **Nuova scheda attività** nella parte superiore dell&#39;elenco dei fogli presenze.

   Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Crea scheda orario per</strong> </td> 
      <td>Iniziare a immettere il nome dell'utente, un ruolo o un team per il quale si sta creando la scheda attività e fare clic su di essi quando vengono visualizzati nell'elenco.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Data di inizio</strong> </td> 
      <td>Data di inizio della scheda attività.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Data di fine</strong> </td> 
      <td> Data di fine della scheda attività.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Approvatori</strong> </td> 
      <td>Gli approvatori sono utenti che approvano la scheda attività per gli utenti associati alla scheda attività. È possibile impostare come approvatori solo gli utenti con diritti di amministrazione della scheda attività. Per ulteriori informazioni sui diritti amministrativi della scheda attività, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.<br>Iniziare a immettere i nomi degli approvatori della scheda attività e fare clic su di essi quando vengono visualizzati nell'elenco.<br>È possibile avere più approvatori in una scheda attività. In questo caso, dopo che uno degli approvatori approva la scheda attività, la scheda attività viene contrassegnata come <strong>Chiuso</strong> e scompare dall'elenco delle approvazioni della scheda attività di tutti gli approvatori rimanenti.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Può modificare l’ora</strong> </td>

   <td> <p>Selezionare questa opzione se si desidera consentire agli approvatori di modificare le ore nella scheda attività.</p>

   Questa opzione funziona insieme al **Limita la modifica della scheda attività a proprietari e amministratori** nell&#39;area Configurazione > Scheda attività e ore > Preferenze. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurare le preferenze relative a schede attività e ora</a>.

   Esistono i seguenti scenari:

   <ul>
      <li>Quando il <b>Limita la modifica della scheda attività a proprietari e amministratori</b> è abilitata:</li>
   <ul><li>Gli approvatori possono solo approvare e rifiutare la scheda attività, indipendentemente dal fatto che la <b>Può modificare il tempo</b> è abilitato o meno. </li>
   <li>I responsabili dei proprietari dei fogli presenze possono visualizzare solo i fogli presenze dei loro rapporti diretti.</li></ul>
   <li>Quando il <b>Limita la modifica della scheda attività a proprietari e amministratori</b> è disabilitata:</li>
   <ul><li>Quando il <b>Può modificare il tempo</b> è abilitato, gli approvatori possono inviare, riaprire o chiudere la scheda attività e possono modificare l'ora.</li>
   <li>Quando il <b>Può modificare il tempo</b> è disabilitato, gli approvatori non possono inviare, riaprire o chiudere la scheda attività e non possono modificare l'ora. Gli approvatori possono solo approvare o rifiutare la scheda attività. </li>
   <li>I responsabili dei proprietari dei fogli presenze possono inviare, richiamare, riaprire e modificare i fogli presenze dei loro report diretti.</li></ul>
   </ul>

   <p><b>NOTA</b>

   Dopo aver inviato una scheda attività per l&#39;approvazione, non è più possibile modificare le ore. Per restituire una scheda attività inviata a uno stato modificabile, richiamare la scheda attività o chiedere al responsabile approvazione di rifiutare la scheda attività. Per ulteriori informazioni, consulta <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Invia una scheda attività per l&#39;approvazione</a> e <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approva una scheda attività</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Straordinari</span> </td> 
      <td>È possibile scegliere di nascondere la casella Overtime nella scheda attività. Questa opzione è disabilitata per impostazione predefinita.</td> 
      </tr> 
      </tbody> 
   </table>

1. Fai clic su **Crea foglio presenze**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Quando attività e problemi vengono visualizzati sui fogli presenze degli utenti

Un&#39;attività o un problema assegnato a un utente viene visualizzato automaticamente nella scheda attività di un utente se l&#39;attività o il problema soddisfa uno dei seguenti criteri:

* L&#39;utente ha registrato ore sull&#39;attività o sul problema
* Le date pianificate dell&#39;attività o del problema rientrano nelle date della scheda attività
* L&#39;attività o il problema ha una data di inizio effettiva (lo stato dell&#39;attività o del problema è In corso)
* L&#39;attività o il problema è fissato alla scheda attività
* La data di completamento pianificata rientra nell&#39;intervallo di date della scheda attività e lo stato è In corso

Se la **Precompilazione fogli preselezionati con ...** le preferenze (che si trovano nelle preferenze Fascicolo e Ora) sono deselezionate, la scheda attività mostra i problemi e le attività che presentano lo stato In corso. Per ulteriori informazioni sulle schede attività e preferenze ora, consulta [Configurare le preferenze relative a schede attività e ora](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
