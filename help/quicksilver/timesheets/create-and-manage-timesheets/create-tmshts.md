---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Creare una scheda orario monouso
description: Puoi creare manualmente una scheda orario monouso se desideri una scheda orario non ricorrente. Quando viene raggiunta la data di fine della scheda orario e sono necessarie altre schede orario, è necessario crearne di nuove.
author: Lisa
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
TQID: https://experienceleague.adobe.com/6ngmKzkpxxHYM7L9Z16JsJKcEW7CdFjJcdp6B6hgTtc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a3c1ab8fc8012199d9863fc978cca7418fa0a2f5
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 6%
---
# Creare un timesheet per utilizzo singolo

<!--Audited: 6/2025-->

Puoi creare manualmente una scheda orario monouso se desideri una scheda orario non ricorrente. Quando viene raggiunta la data di fine della scheda orario e sono necessarie altre schede orario, è necessario crearne di nuove.

Per informazioni sulla creazione di un profilo di scheda orario che generi schede orario ricorrenti per gli utenti senza alcun ulteriore intervento da parte tua (consigliato), consulta [Creare, modificare e assegnare profili di scheda orario](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Per informazioni sulla generazione manuale delle schede orario per tutti gli utenti del sistema associati a un profilo di scheda orario, vedere [Generazione manuale delle schede orario](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

>[!NOTE]
>
>* Non è possibile creare schede orario monouso per i gruppi.
>* Quando si crea una scheda orario monouso, non è possibile selezionare tipi di ore generici specifici da includere nella scheda orario. Tutti i tipi di ore generali attivati nel sistema vengono visualizzati nelle schede orario create manualmente.
>
>Se desideri selezionare solo determinati tipi di ore generali da visualizzare nelle schede orario, utilizza un profilo scheda orario. Per ulteriori informazioni sui profili delle schede orario, vedere [Creare, modificare e assegnare profili delle schede orario](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td><p>Accesso amministrativo alle schede orario</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un timesheet per utilizzo singolo

{{step1-to-timesheets}}

Tutte le schede orario a cui hai accesso vengono visualizzate per impostazione predefinita.

![Elenco schede orario](assets/list-of-all-timesheets.png)

1. (Facoltativo) Per aggiornare il filtro nell’elenco delle schede orario, effettua una delle seguenti operazioni:

   * Seleziona **Le mie approvazioni schede orario** nell&#39;angolo superiore destro della pagina per visualizzare solo le schede orario che hai approvato,

     Oppure

     Seleziona **Le mie schede orario** per visualizzare solo le tue schede orario.

     Questa operazione applica i filtri **Le mie approvazioni schede orario** o **Le mie schede orario** all&#39;elenco delle schede orario.

   * Fai clic sull&#39;icona **Filtro** ![Icona Filtro](assets/filter-nwepng.png) per applicare un filtro o crearne uno nuovo. Per informazioni sulla creazione o l&#39;aggiornamento dei filtri, vedere [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Schede attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo ha rimosso i filtri Approvazioni schede attività personali e Schede attività personali dall&#39;area Controlli elenco nella configurazione o dal modello di layout. Per ulteriori informazioni, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Facoltativo) Fai clic sull&#39;icona **Ricerca** ![Icona Ricerca](assets/search-icon.png) per digitare una parola chiave e cercare una scheda orario specifica. Ad esempio, puoi cercare un intervallo di tempo della scheda orario con il nome del proprietario.

1. (Facoltativo) Fai clic sull&#39;icona **Visualizza** ![Visualizza](assets/view-icon.png) o **Raggruppamento** ![Icona Raggruppamento](assets/grouping.png) per applicare una visualizzazione o un raggruppamento o crearne uno nuovo.

   Per informazioni sulla creazione di filtri, viste o raggruppamenti, vedere i seguenti articoli:

   * [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Creare o modificare le visualizzazioni in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creare raggruppamenti in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Fai clic su **Nuova scheda orario** nella parte superiore dell&#39;elenco delle schede orario.

   Immettere le seguenti informazioni:

   | Nome campo | Descrizione |
   | --------- | ---------- |
   | Crea scheda orario per | Inizia a immettere il nome dell’utente, una mansione o un team per il quale stai creando la scheda orario e fai clic su di essi quando vengono visualizzati nell’elenco. |
   | Data di inizio | Questa è la data di inizio della scheda orario. |
   | Data di fine | Questa è la data di fine della scheda orario. |
   | Approvatori | <p>Gli approvatori sono utenti che approvano la scheda orario per gli utenti associati alla scheda orario. Solo gli utenti con diritti di amministrazione della scheda orario possono essere impostati come approvatori. Per ulteriori informazioni sui diritti amministrativi delle schede orario, vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).</p> <p>Inizia a immettere i nomi degli approvatori della scheda orario e selezionali quando vengono visualizzati nell’elenco.</p> <p>In una scheda orario possono essere presenti più approvatori. In questo caso, dopo che uno degli approvatori ha approvato la scheda orario, la scheda viene contrassegnata come **Chiusa** e scompare dall&#39;elenco delle approvazioni della scheda orario di tutti gli approvatori rimanenti.</p> |
   | Può modificare l’ora | <p>Selezionare questa opzione se si desidera consentire agli approvatori di modificare le ore nella scheda orario.</p><p>Questa opzione funziona con l&#39;impostazione **Limita la modifica della scheda orario a proprietari e amministratori** nell&#39;area Configurazione > Scheda orario e ore > Preferenze. Per ulteriori informazioni, consulta [Configurare le preferenze di orario e scheda orario](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).</p><p>Esistono i seguenti scenari:</p><p>Quando l&#39;opzione **Limita la modifica della scheda orario a proprietari e amministratori** è abilitata:</p><ul><li>Gli approvatori possono solo approvare e rifiutare la scheda orario, indipendentemente dal fatto che **L&#39;ora di modifica** sia abilitata o meno.</li><li>I responsabili dei proprietari delle schede orario possono visualizzare solo le schede orario dei loro referenti diretti.</li></ul><p>Quando l&#39;opzione **Limita la modifica della scheda orario a proprietari e amministratori** è disabilitata:</p><ul><li>Quando **Può modificare l&#39;ora** è abilitato, gli approvatori possono inviare, riaprire o chiudere la scheda orario e modificare l&#39;ora.</li><li>Se **L&#39;ora di modifica** è disabilitata, gli approvatori non possono inviare, riaprire o chiudere la scheda orario e non possono modificare l&#39;ora. Gli approvatori possono approvare o rifiutare solo la scheda orario.</li><li>I responsabili dei proprietari delle schede orario possono inviare, richiamare, riaprire e modificare le schede orario dei loro referenti diretti.</li></ul><p>**NOTA**</br> Una volta inviata una scheda orario per l&#39;approvazione, non è più possibile modificare le ore. Per ripristinare lo stato modificabile di una scheda orario inviata, richiamarla o richiedere all&#39;approvatore di rifiutarla. Per ulteriori informazioni, vedere [Inviare una scheda orario per l&#39;approvazione](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) e [Approvare una scheda orario](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md). |
   | Straordinari | Puoi scegliere di nascondere la casella **Straordinari** nella scheda orario. Questa opzione è disabilitata per impostazione predefinita. |

1. Fai clic su **Crea scheda orario**.

## Quando le attività e i problemi vengono visualizzati nelle schede orario degli utenti

Un’attività o un problema assegnato a un utente viene visualizzato automaticamente sulla scheda orario di un utente se l’attività o il problema soddisfa uno dei seguenti criteri:

* L’utente ha registrato ore sull’attività o sul problema
* Le date pianificate per l&#39;attività o il problema rientrano nelle date della scheda orario
* L&#39;attività o il problema ha una data di inizio effettiva (lo stato dell&#39;attività o del problema è In corso)
* L&#39;attività o il problema è fissato alla scheda orario
* La data di completamento pianificata rientra nell’intervallo di date della scheda orario e lo stato è In corso

Se le **Precompila schede orario con le preferenze ...** (che si trovano nelle preferenze Timesheets &amp; Hour) sono deselezionate, la scheda mostra i problemi e le attività con lo stato In corso. Per ulteriori informazioni sulle preferenze per le schede orario e le ore, vedere [Configurare le preferenze per le ore e le schede orario](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
