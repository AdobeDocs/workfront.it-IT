---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Creare una scheda orario monouso
description: Puoi creare manualmente una scheda orario monouso se desideri una scheda orario non ricorrente. Quando viene raggiunta la data di fine della scheda orario e sono necessarie altre schede orario, è necessario crearne di nuove.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---

# Creare una scheda orario monouso

Puoi creare manualmente una scheda orario monouso se desideri una scheda orario non ricorrente. Quando viene raggiunta la data di fine della scheda orario e sono necessarie altre schede orario, è necessario crearne di nuove.

Per informazioni sulla creazione di un profilo di scheda orario che generi schede orario ricorrenti per gli utenti senza alcun ulteriore intervento da parte tua (consigliato), consulta [Creare, modificare e assegnare profili di scheda orario](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* Non è possibile creare schede orario monouso per i gruppi.
>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* Quando si crea una scheda orario monouso, non è possibile selezionare tipi di ore generici specifici da includere nella scheda orario. Tutti i tipi di ore generali attivati nel sistema vengono visualizzati nelle schede orario create manualmente.
>
>  Se desideri selezionare solo determinati tipi di ore generali da visualizzare nelle schede orario, utilizza un profilo scheda orario. Per ulteriori informazioni sui profili delle schede orario, vedere [Creare, modificare e assegnare profili delle schede orario](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
>

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
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>È necessario disporre dell'accesso amministrativo alle schede orario. </p> <p>Per ulteriori informazioni, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo ad alcune aree</a>.</p> <p><b> NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

## Creare una scheda orario monouso

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront.

1. Fai clic su **Schede orario**. Il filtro **All** è selezionato per impostazione predefinita. In questo modo vengono visualizzate tutte le schede orario a cui hai accesso.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facoltativo) Per aggiornare il filtro nell’elenco delle schede orario, effettua una delle seguenti operazioni:

   * Seleziona **Le mie approvazioni schede orario** nell&#39;angolo superiore destro della pagina per visualizzare solo le schede orario che hai approvato

     Oppure

     Seleziona **Le mie schede orario** per visualizzare solo le tue schede orario.

     In questo modo all’elenco delle schede orario vengono applicate le approvazioni delle mie schede orario o i filtri delle mie schede orario.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Fare clic sull&#39;icona Filtro ![](assets/filter-nwepng.png) per applicare un filtro diverso o crearne uno nuovo. Per informazioni sulla creazione o l&#39;aggiornamento dei filtri, vedere [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Schede attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo ha rimosso i filtri Approvazioni schede attività personali e Schede attività personali dall&#39;area Controlli elenco nella configurazione o dal modello di layout. Per ulteriori informazioni, consulta i seguenti articoli:
   > 
   >   * [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Facoltativo) Fai clic sull&#39;icona **Ricerca** ![](assets/search-icon.png) per digitare una parola chiave e cercare una scheda orario specifica. Ad esempio, puoi cercare un intervallo di tempo della scheda orario con il nome del proprietario.

1. (Facoltativo) Fai clic sulle icone **Visualizza** ![](assets/view-icon.png) o **Raggruppamento** ![](assets/grouping.png) per applicare una visualizzazione o un raggruppamento diverso o per crearne uno nuovo.

   Per informazioni sulla creazione di filtri, viste o raggruppamenti, vedere i seguenti articoli:

   * [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Creare o modificare le visualizzazioni in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creare raggruppamenti in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Fai clic su **Nuova scheda orario** nella parte superiore dell&#39;elenco delle schede orario.

   Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Crea scheda orario per</strong> </td> 
      <td>Inizia a immettere il nome dell’utente, una mansione o un team per il quale stai creando la scheda orario e fai clic su di essi quando vengono visualizzati nell’elenco.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Data inizio</strong> </td> 
      <td>Questa è la data di inizio della scheda orario.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Data di fine</strong> </td> 
      <td> Questa è la data di fine della scheda orario.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Approvatori</strong> </td> 
      <td>Gli approvatori sono utenti che approvano la scheda orario per gli utenti associati alla scheda orario. Solo gli utenti con diritti di amministrazione della scheda orario possono essere impostati come approvatori. Per ulteriori informazioni sui diritti amministrativi delle schede orario, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo ad alcune aree</a>.<br>Inizia a immettere i nomi degli approvatori della scheda orario e fai clic su di essi quando compaiono nell'elenco.<br>In una scheda orario possono essere presenti più approvatori. In questo caso, dopo che uno degli approvatori ha approvato la scheda orario, la scheda viene contrassegnata come <strong>Chiusa</strong> e scompare dall'elenco delle approvazioni della scheda orario di tutti gli approvatori rimanenti.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Modifica ora</strong> </td>

   <td> <p>Selezionare questa opzione se si desidera consentire agli approvatori di modificare le ore nella scheda orario.</p>

   Questa opzione funziona con l&#39;impostazione **Limita la modifica della scheda orario a proprietari e amministratori** nell&#39;area Configurazione > Scheda orario e ore > Preferenze. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurare le preferenze di orario e scheda orario</a>.

   Esistono i seguenti scenari:

   <ul>
      <li>Quando l'opzione <b>Limita la modifica della scheda orario a proprietari e amministratori</b> è abilitata:</li>
   <ul><li>Gli approvatori possono solo approvare e rifiutare la scheda orario, indipendentemente dal fatto che l'<b>orario di modifica</b> sia abilitato o meno. </li>
   <li>I responsabili dei proprietari delle schede orario possono visualizzare solo le schede orario dei loro referenti diretti.</li></ul>
   <li>Quando l'opzione <b>Limita la modifica della scheda orario a proprietari e amministratori</b> è disabilitata:</li>
   <ul><li>Quando l'ora <b>Può modificare</b> è abilitata, gli approvatori possono inviare, riaprire o chiudere la scheda orario e modificare l'ora.</li>
   <li>Se l'ora <b>Può modificare</b> è disabilitata, gli approvatori non possono inviare, riaprire o chiudere la scheda orario e non possono modificare l'ora. Gli approvatori possono approvare o rifiutare solo la scheda orario. </li>
   <li>I responsabili dei proprietari delle schede orario possono inviare, richiamare, riaprire e modificare le schede orario dei loro referenti diretti.</li></ul>
   </ul>

   <p><b>NOTA</b>

   Dopo aver inviato una scheda orario per l&#39;approvazione, non è più possibile modificare le ore. Per ripristinare lo stato modificabile di una scheda orario inviata, richiamarla o richiedere all&#39;approvatore di rifiutarla. Per ulteriori informazioni, vedere <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Inviare una scheda orario per l&#39;approvazione</a> e <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approvare una scheda orario</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Straordinari</span> </td> 
      <td>È possibile scegliere di nascondere la casella Straordinari nella scheda attività. Questa opzione è disabilitata per impostazione predefinita.</td> 
      </tr> 
      </tbody> 
   </table>

1. Fai clic su **Crea scheda orario**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Quando le attività e i problemi vengono visualizzati nelle schede orario degli utenti

Un’attività o un problema assegnato a un utente viene visualizzato automaticamente sulla scheda orario di un utente se l’attività o il problema soddisfa uno dei seguenti criteri:

* L’utente ha registrato ore sull’attività o sul problema
* Le date pianificate per l&#39;attività o il problema rientrano nelle date della scheda orario
* L&#39;attività o il problema ha una data di inizio effettiva (lo stato dell&#39;attività o del problema è In corso)
* L&#39;attività o il problema è fissato alla scheda orario
* La data di completamento pianificata rientra nell’intervallo di date della scheda orario e lo stato è In corso

Se le **Precompila schede orario con le preferenze ...** (che si trovano nelle preferenze Timesheets &amp; Hour) sono deselezionate, la scheda mostra i problemi e le attività con lo stato In corso. Per ulteriori informazioni sulle preferenze per le schede orario e le ore, vedere [Configurare le preferenze per le ore e le schede orario](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
