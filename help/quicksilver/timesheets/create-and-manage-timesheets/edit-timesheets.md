---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Modificare le informazioni dei timesheet
description: In qualità di utente con accesso amministrativo alle schede orario, puoi modificare le informazioni sulle schede orario esistenti in Adobe Workfront. Ad esempio, puoi modificare il Proprietario, gli Approvatori o l’intervallo di tempo della scheda orario.
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
TQID: https://experienceleague.adobe.com/--QshuygnTfcEJtt6-Tx-2QtNT-5p9TrTWaQTMBZNAg
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
source-wordcount: '739'
ht-degree: 9%
---
# Modificare le informazioni dei timesheet

In qualità di utente con accesso amministrativo alle schede orario, puoi modificare le informazioni sulle schede orario esistenti in Adobe Workfront. Ad esempio, puoi modificare il Proprietario, gli Approvatori o l’intervallo di tempo della scheda orario.

È possibile modificare le informazioni su un&#39;unica scheda orario oppure modificare più schede orario in blocco.

>[!IMPORTANT]
>
>Se gli utenti sono associati ai profili delle schede orario e queste vengono generate automaticamente, le modifiche apportate alle schede esistenti non verranno applicate alle schede orario che verranno generate per le date future. Tutte le schede orario generate automaticamente hanno le impostazioni stabilite nei Profili delle schede orario. Per ulteriori informazioni, consulta [Creare profili scheda orario](../create-and-manage-timesheets/create-timesheet-profiles.md)

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

## Modifica schede orario

{{step1-to-timesheets}}

Tutte le schede orario a cui hai accesso vengono visualizzate per impostazione predefinita.

![Elenco schede orario](assets/list-of-all-timesheets.png)

1. (Facoltativo) Fai clic sull&#39;icona **ricerca** ![icona di ricerca](assets/search-icon.png) e digita una parola chiave per cercare una scheda orario specifica. Ad esempio, puoi cercare un intervallo di tempo della scheda orario o il nome del proprietario.

1. (Facoltativo) Per aggiornare il filtro nell’elenco delle schede orario, effettua una delle seguenti operazioni:

   * Seleziona **Le mie approvazioni schede orario** nell&#39;angolo superiore destro della pagina per visualizzare solo le schede orario che hai approvato,

     Oppure

     Seleziona **Le mie schede orario** per visualizzare solo le tue schede orario.

     Questa operazione applica i filtri **Le mie approvazioni schede orario** o **Le mie schede orario** all&#39;elenco delle schede orario.

   * Fai clic sull&#39;icona **Filtro** ![Icona Filtro](assets/filter-nwepng.png) per applicare un filtro o crearne uno nuovo. Per informazioni sulla creazione o l&#39;aggiornamento dei filtri, vedere [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Le opzioni Approvazioni schede attività personali e Schede attività personali non vengono visualizzate nella parte superiore dell&#39;elenco delle schede attività o nell&#39;elenco dei filtri se l&#39;amministratore di Workfront o un amministratore di gruppo ha rimosso tali filtri dai controlli elenco nell&#39;area Configura o dal modello di layout. Per ulteriori informazioni, vedere [Personalizzare filtri, visualizzazioni e raggruppamenti utilizzando un modello di layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Facoltativo) Fai clic sull&#39;icona **Visualizza** ![Visualizza](assets/view-icon.png) o **Raggruppamento** ![Icona Raggruppamento](assets/grouping.png) per applicare una visualizzazione o un raggruppamento o crearne uno nuovo.

   Per informazioni sulla creazione di filtri, viste o raggruppamenti, vedere i seguenti articoli:

   * [Creare o modificare filtri in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Creare o modificare le visualizzazioni in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creare raggruppamenti in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Seleziona una o più schede orario, quindi fai clic sull&#39;icona **Modifica** ![Modifica icona](assets/edit-icon.png) nella parte superiore dell&#39;elenco delle schede orario.
1. Visualizzare o immettere le informazioni seguenti:

   | Nome campo | Descrizione |
   | --------- | ---------- |
   | Proprietario | <p>Questo è il nome dell&#39;utente per cui è stata creata la scheda orario. Impossibile modificare questo campo.</p><p>Questo campo non viene visualizzato quando si selezionano più schede orario.</p> |
   | Data di inizio | Questa è la data di inizio della scheda orario. |
   | Data di fine | Questa è la data di fine della scheda orario. |
   | Stato | <p>Questo è lo stato della scheda orario. Di seguito sono riportate le possibili opzioni di stato della scheda orario:</p><ul><li>**Apri**: la scheda orario è aperta e le ore possono essere modificate.</li><li>**Inviato**: la scheda orario viene inviata per l&#39;approvazione agli approvatori designati.</li><li>**Rifiutato**: la scheda orario non è stata approvata dagli approvatori ed è ora nuovamente disponibile per consentire all&#39;utente di modificare le voci relative all&#39;ora.</li><li>**Chiusa**: la scheda orario è stata chiusa dall&#39;utente o approvata dall&#39;approvatore e di conseguenza è ora chiusa. Non è possibile aggiungere un orario a una scheda orario chiusa.</li></ul> |
   | Approvatori | <p>Gli approvatori sono utenti che approvano la scheda orario per gli utenti associati alla scheda orario. Solo gli utenti con diritti di amministrazione della scheda orario possono essere impostati come approvatori. Per ulteriori informazioni sui diritti amministrativi delle schede orario, vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).</p> <p>Inizia a immettere i nomi degli approvatori della scheda orario e selezionali quando vengono visualizzati nell’elenco.</p> <p>In una scheda orario possono essere presenti più approvatori. In questo caso, dopo che uno degli approvatori ha approvato la scheda orario, la scheda viene contrassegnata come **Chiusa** e scompare dall&#39;elenco delle approvazioni della scheda orario di tutti gli approvatori rimanenti.</p> |
   | Può modificare l’ora | <p>Selezionare questa opzione se si desidera consentire agli approvatori di modificare le ore nella scheda orario.</p><p>Questa opzione non è disponibile quando si selezionano più schede orario.</p> |
   | Straordinari | <p>È possibile scegliere di nascondere la casella Straordinari nella scheda attività.</p><p>Questa opzione è disabilitata per impostazione predefinita.</p> |

1. Fai clic su **Salva**.
