---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Panoramica sulla consegna dei rapporti
description: Panoramica sulla consegna dei rapporti
author: Nolan
feature: Reports and Dashboards
exl-id: 1637df59-ca1d-4cf6-b83d-2b27936cdb96
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1528'
ht-degree: 0%

---

# Panoramica sulla consegna dei rapporti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is linked to the UI in the Send Report box inside the Preview sandbox. If you change title, log bug for Dev to fix the link) </p>
-->

Puoi pianificare la consegna automatica dei rapporti agli utenti in base a una pianificazione definita, oppure puoi inviare manualmente i rapporti una tantum. Quando invii un rapporto da Adobe Workfront, l’utente riceve un’e-mail con il rapporto Workfront in un allegato separato.

Per informazioni sull’impostazione di un rapporto per la consegna, consulta l’articolo [Pianificare una consegna automatica dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

Non puoi pianificare i rapporti per la consegna, né distribuirli manualmente nell’ambiente Sandbox di anteprima. Per ulteriori informazioni sulla Sandbox di anteprima, consulta l’articolo [Ambiente Sandbox di anteprima di Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).\
Per ulteriori informazioni sulla distribuzione dei rapporti nell’ambiente Sandbox di anteprima, consulta l’articolo [Inviare un rapporto nell’ambiente Sandbox di anteprima](../../../reports-and-dashboards/reports/creating-and-managing-reports/send-report-preview-sandbox-environment.md).

## Limiti di consegna dei rapporti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."])</p>
-->

Quando pianifichi i rapporti per la consegna, considera quanto segue:

* Puoi pianificare fino a 10 consegne ripetute di report per un determinato report.
* Puoi pianificare l’invio di un rapporto solo se sei l’autore del rapporto. Se devi inviare un rapporto che non hai creato, puoi inviarlo manualmente.

## Limiti di esportazione

Esistono diversi limiti di dimensione che influiscono sul modo in cui i rapporti vengono visualizzati in Workfront e sulle loro modalità di esportazione tramite un’esportazione manuale, un rapporto consegnato o tramite l’API:

* **Dimensione del file di 5 MB:** Limite di dimensioni del file per qualsiasi rapporto esportato pianificato per la consegna. Se un file esportato allegato a un&#39;e-mail ha dimensioni superiori a 5 MB, viene inviato via e-mail un collegamento in cui è possibile scaricare il file invece del rapporto esportato allegato. 

   >[!NOTE]
   >
   >I file Excel .xlsx di dimensioni superiori a 5 MB non generano un messaggio e-mail. Puoi esportare manualmente il rapporto in questo formato. Per informazioni sull&#39;esportazione dei rapporti, vedi [Esportare i dati](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* **50.000 righe:** Il numero di righe di dati consentite in un&#39;esportazione di report per file .pdf e delimitati da tabulazioni.

   Per i file Excel .xls questo limite è **65.000 righe**.

   Per i file Excel .xlsx questo limite è **100.000 righe**.

   Questi limiti escludono le intestazioni di colonna e le righe per i raggruppamenti nel rapporto. Ad esempio, se in un rapporto sono presenti 6 raggruppamenti e 50.000 righe o dati, il file esportato avrà 50.000 righe.

   Se il rapporto ha più elementi di questi limiti, viene visualizzato un errore che indica che l’esportazione e la consegna del rapporto non sono riuscite. Riduci il numero di elementi visualizzati sullo schermo a un numero minore o uguale a questi limiti per poter fornire i risultati. Se desideri esportare tutti i dati, consigliamo di utilizzare i filtri per ottenere carichi di dati più piccoli, quindi eseguire più esportazioni. Per ulteriori informazioni, consulta [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

   Tali limiti si applicano:

   * Esportazione manuale di un report.
   * Un rapporto pianificato.
   * Un’esportazione tramite un’integrazione API. 
   * Dati esportati tramite un avvio a scatto.

      Per ulteriori informazioni sull&#39;esportazione dei dati tramite i kick-started, vedi l&#39;articolo [Esportare dati da Adobe Workfront tramite Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

      >[!NOTE]
      È possibile esportare 50.000 righe in un file di avvio, ma solo in un file in formato Excel. 

   * Esportazione delle informazioni di utilizzo per un progetto.

      Per ulteriori informazioni sull&#39;esportazione delle informazioni sull&#39;utilizzo di un progetto, vedi [Panoramica del rapporto Utilizzo risorse](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* **65.530 collegamenti ipertestuali:** Questo è un limite imposto da Excel sui documenti che contengono più di 65.530 collegamenti ipertestuali. Questi documenti non possono essere aperti quando vengono esportati manualmente o inviati in un rapporto consegnato. Si noti che un documento Excel può contenere solo 200 righe di dati, ma se il documento contiene più di 65.530 collegamenti, il documento non viene aperto. Questo limite esiste solo per i file Excel, non per gli altri formati supportati. 
* **256 colonne**: questo è un limite imposto da Excel sui documenti che contengono più di 256 colonne. Questi documenti non possono essere esportati manualmente o inviati in un rapporto consegnato. Questo limite esiste solo per i file Excel, non per gli altri formati supportati. 

Se tenti di esportare dati oltre il limite, potresti non ricevere tutti i dati previsti nell’esportazione. Piuttosto, viene prodotto un rapporto modificato entro i limiti stabiliti. 

Inoltre, i rapporti che richiedono più di 60 minuti per essere eseguiti verranno interrotti.

In caso di dubbi o problemi relativi al limite, contatta il supporto tecnico Workfront.

## Comprendere le marche temporali nei report consegnati

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Note about if this is delivered at a time based on the user's time zone settings?)</p>
-->

Quando ricevi un rapporto in un’e-mail, la data e il formato dell’ora del rapporto potrebbero non corrispondere a quelli in Workfront, se lo visualizzassi in Workfront nello stesso momento in cui è stato consegnato. 

Considera quanto segue: 

* Quando visualizzi un rapporto nel browser, la marca temporale e il formato del rapporto corrispondono alle impostazioni internazionali e al fuso orario del browser, come definito nelle impostazioni del browser.
* Quando il rapporto viene consegnato in un’e-mail, viene consegnato con la marca temporale e il formato corrispondenti alle impostazioni internazionali e al fuso orario dell’utente specificati nel profilo Workfront.\
   Per ulteriori informazioni sulle impostazioni internazionali utente e sul fuso orario in Workfront, consulta l’articolo [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Report con visualizzazione speciale {#reports-with-a-special-view}

Quando applichi una visualizzazione speciale a un rapporto, la visualizzazione speciale viene visualizzata nella scheda Dettagli del rapporto in Workfront.

Quando pianifichi la consegna di un rapporto con una visualizzazione speciale, la scheda Dettagli predefinita viene consegnata nell’allegato dell’e-mail inviata, anziché nella visualizzazione speciale.

Sono considerate punti di vista speciali:

* Visualizzazione Milestone in un report di progetto
* Visualizzazione Gantt in un rapporto Progetto o Attività
* Rapporti con grafico come scheda predefinita

>[!NOTE]
Se sul rapporto è presente anche una scheda Matrice oltre alla scheda predefinita con una visualizzazione speciale, il rapporto viene consegnato così come viene visualizzato nella scheda Matrice.

Per ulteriori informazioni su come applicare una visualizzazione speciale a un rapporto, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Utilizzare il file consegnato

 Quando invii un rapporto da Workfront, l’utente riceve un messaggio e-mail con il rapporto in un allegato separato. 

* [Oggetto, nome allegato e titolo del rapporto](#subject-line-attachment-name-and-report-title)
* [Marca temporale](#timestamps)
* [Branding](#branding)
* [Formattazione](#formatting)
* [Collegamenti](#links)

### Oggetto, nome allegato e titolo del rapporto {#subject-line-attachment-name-and-report-title}

Per ulteriori informazioni sull’oggetto dell’e-mail del rapporto consegnato, consulta [Pianificare una consegna automatica dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

Il nome del rapporto allegato è: *Nome_Del_Rapporto_Rapporto_Nome* seguito dal formato file esportato. 

Se hai pianificato che il rapporto consegnato venga formattato come file PDF o HTML, il titolo del rapporto sarà:

*Nome del report.*

I rapporti pianificati per essere consegnati in un formato Excel, Excel (.xlsx) o TSV non hanno un titolo.

>[!NOTE]
Se il report ha una descrizione, verrà incluso nel file esportato se il file è formattato come file PDF o HTML.

### Marca temporale {#timestamps}

Una marca temporale viene visualizzata sul file allegato solo se il formato del file è .pdf. La marca temporale si trova nel piè di pagina del file allegato.

La marca temporale include:

* Data
* Ora
* Fuso orario in cui è stato inviato il rapporto

### Branding {#branding}

Se l’amministratore di Workfront ha aggiunto branding personalizzato alla tua istanza Workfront, i rapporti inviati in formato .pdf includono anche il tuo logo personalizzato.

I rapporti inviati in tutti gli altri formati non possono essere personalizzati con il tuo logo.

Per ulteriori informazioni sul branding dell’istanza Workfront, consulta l’articolo [Brand your Adobe Workfront instance](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### Formattazione {#formatting}

Quando un rapporto viene inviato o pianificato per una consegna, viene sempre visualizzata la scheda predefinita di un rapporto, a meno che il rapporto non disponga di una visualizzazione speciale.

Se il report ha una formattazione speciale nell&#39;applicazione Web, il report deve essere consegnato con la formattazione speciale quando le schede Dettagli e Matrice vengono consegnate solo per i file .pdf ed Excel.

Il filtro, la visualizzazione o il raggruppamento del rapporto non sono inclusi nel file consegnato. La descrizione del rapporto è inclusa solo quando lo si invia come file PDF.

Per ulteriori informazioni sulla ricezione di rapporti con una visualizzazione speciale, consulta l’articolo [Report con visualizzazione speciale](#reports-with-a-special-view).\
Per ulteriori informazioni sulla selezione della scheda predefinita di un rapporto e sulla formattazione speciale, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Collegamenti {#links}

Quando si invia un rapporto da Workfront al formato PDF o Excel, tutti i collegamenti di lavoro presenti nel documento originale rimangono attivi nel file inviato. I collegamenti possono puntare a qualsiasi oggetto in Workfront che supporta il collegamento.

Anche il nome del rapporto nel messaggio e-mail è un collegamento.

## Rapporto sui rapporti programmati

Puoi verificare se un rapporto è stato configurato per essere consegnato creando quanto segue:

* **Una vista** per l&#39;oggetto Report in un elenco o in un report per i report: Crea una visualizzazione in un elenco di rapporti o in un rapporto per i rapporti e aggiungi la seguente colonna alla visualizzazione:\
   *Nome report programmato.\
   *I nomi di tutte le consegne programmate per quel rapporto sono elencati nella colonna di un elenco puntato.\
   ![scheduled_reports_info_in_view.png](assets/scheduled-reports-info-in-view-350x294.png)

* **Filtro** per l&#39;oggetto Report: creare un filtro per un elenco di report o in un report per i report con la seguente istruzione: *L&#39;ID del rapporto pianificato non è vuoto*.\
   Verranno visualizzati solo i rapporti pianificati nell’elenco o nel rapporto.\
   ![](assets/qs-scheduled-report-filter-350x101.png)\
   Per ulteriori informazioni sulla creazione di rapporti, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Per informazioni sulla creazione di un rapporto sui rapporti, vedi [Creare un rapporto sulle attività di reporting](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Scheduling a Repeating&nbsp;Report Delivery</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can schedule up to 10 repeating report deliveries for any given report.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can schedule a report to be delivered only if you are the creator of the report. If you need to send a report that you did not create, you can send it on a manual basis.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To schedule&nbsp;a report for automatic delivery or to edit an existing report delivery:&nbsp;​</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report for which you want to schedule delivery.&nbsp;</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The <strong>Send Report</strong> dialog box is displayed.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the <strong>Repeating Deliveries</strong>&nbsp;tab.<br><img src="assets/report-delivery-schedule-350x169.png" alt="" style="width: 350;height: 169;"></li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Conditional)&nbsp;To modify an existing repeating report delivery, select the report delivery in the <strong>Repeating Deliveries</strong>&nbsp;section.</li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Specify the following information:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Send to:</strong> Begin typing the name of the user, group, team, or role who you want to send&nbsp;the report to, then click the name when it appears in the drop-down list.<br>Or<br>Specify the email address of a person external to the Workfront system who you want to have access to the report.<br> Repeat this process to send the report to multiple users, groups, teams, or roles.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Subject:</strong> Specify a subject for the email notification.<br> By default, the email subject is: <em>Workfront Report: <Name of the report> Date of the Export</em>.<strong></strong></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Message:</strong> Specify a message to include in the email.<br>By default, the email message is:&nbsp;<em>Attached is the <report frequency> report <Name of the report> generated by Workfront on <Date>.</em><br>
   <note type="note">
   For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks.&nbsp;Please go back to the report scheduler&nbsp;to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report.&nbsp;
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Deliver this report with the Access Rights of:</strong>&nbsp;Begin typing the name of a user who has access to the report, then click the name when it appears&nbsp;in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify&nbsp;here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>
   <note type="note">
   This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Format:</strong> Select in which of the following formats you want the report to be delivered:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> HTML</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">PDF</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS&nbsp;Excel</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel (.xlsx)</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">TSV &nbsp;</li>
   </ul></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Include Links:</strong>&nbsp;This option is available&nbsp;only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document. <br>Documents that contain more than 65,530 links cannot be opened. If the exported document will contain more than 65,530 links, deselect this option.<br>This option is enabled by default.&nbsp;</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Summary:</strong> Displays a summary of when the delivery repeats.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats:</strong> Select whether the report should be delivered daily, weekly, monthly, or yearly.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats Every:</strong> Select the frequency with which you want&nbsp;the delivery to repeat. The value you select for this option is&nbsp;based on the option that is selected in the <strong>Repeats</strong>&nbsp;drop-down list.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Time:</strong> Select the time of day for the delivery to be sent.</li>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats On:</strong>&nbsp;This option is available when the <strong>Repeats</strong>&nbsp;option is set to either <strong>Weekly</strong>&nbsp;or <strong>Monthly</strong>.</p>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the <strong>Repeats</strong>&nbsp;option is set to <strong>Weekly</strong>: Select the days of the week that the delivery is sent.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the <strong>Repeats</strong>&nbsp;option is set to <strong>Monthly</strong>: Select whether the delivery is sent on the day of the month, day of the week, or last day of the month (these options leverage the date that you select in the <strong>Starts On</strong>&nbsp;field).</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Starts On:</strong> Select the date for the scheduled delivery to begin.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Ends On:</strong> Select a date for the scheduled delivery to end. <br>Or</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Never</strong>&nbsp;if you want the scheduled delivery to last indefinitely.</li>
   -->

<!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save</strong>&nbsp;to save the report delivery.<br> The report is saved in the <strong>Repeating Deliveries</strong>&nbsp;section&nbsp;(in the <strong>Send Report</strong> dialog box).<br> The report will be sent at the schedule time<br>Or<br>To manually send the report, click <strong>Send Now</strong>.<br>For more information about sending the report instantly or manually, see&nbsp;.</li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a Scheduled Report Delivery</h2>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to the report with the delivery you want to delete.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then <strong>Send Report</strong>.&nbsp;</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Repeating Deliveries</strong>.&nbsp;</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the name of the scheduled delivery you want to delete, then click <strong>Delete</strong>. The report is no longer set up for the scheduled delivery.&nbsp;</li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Sending a Report Manually, on a One-Time Basis</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can manually send a report&nbsp;that has been previously scheduled, or you can create a single-use report delivery.​</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a title="Setting Up Report Deliveries" href="#sending-a-scheduled-report-now" class="MCXref xref">Sending a Scheduled Report Now</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a title="Setting Up Report Deliveries" href="#sending-a-report-one-time-only" class="MCXref xref">Sending a Report (One Time Only)</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="sending-a-scheduled-report-now">Sending a Scheduled Report Now</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">After a scheduled report has been set up, you can manually send the report rather than&nbsp;waiting until the scheduled time.</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report that you want to send now.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The Send Report dialog box is displayed.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>Repeating Deliveries</strong> tab.</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Repeating Deliveries</strong>&nbsp;section, select the report delivery that was previously created.<br><img src="assets/report-delivery-schedule-send-350x160.png" alt="" style="width: 350;height: 160;"></li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Send Now</strong>.<br> The report is sent to all users identified in the scheduled delivery.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="sending-a-report-one-time-only">Sending a Report (One Time Only)</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can manually send a report at any time. When you send a report in this way, delivery information (such as&nbsp;the users you are sending to and&nbsp;the email subject) are not saved. If you want to create a report delivery that you can save for later use, create a repeating scheduled report.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To send a report to users (one time only):</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report that you want to send now.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The <strong>Send Report</strong> dialog box is displayed.<br><img src="assets/report-delivery-sendnow-350x351.png" alt="" style="width: 350;height: 351;"></li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">On the <strong>Send Now</strong>&nbsp;tab, specify the following information:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Send to:</strong> Begin typing the name of the user, group, team, or role who you want to send&nbsp;the report to, then click the name when it appears in the drop-down list.&nbsp;Or, specify the email address of a person external to the Workfront system who you want to have access to the report.<br> Repeat this process to send the report to multiple users, groups, teams, or roles.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Subject:</strong> Specify a subject for the email notification.<br> By default, the email subject is: <em>Workfront Report: <Name of the report> Date of the Export</em>.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Message:</strong> Specify a message to include in the email.<br>By default, the email message is:&nbsp;<em>Attached is the <report frequency> report <Name of the report> generated by Workfront on <Date>.</em><br>
   <note type="note">
   For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks.&nbsp;Please go back to the report scheduler&nbsp;to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report.&nbsp;
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Deliver this report with the Access Rights of:</strong>&nbsp;Begin typing the name of a user who has access to the report, then click the name when it appears&nbsp;in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify&nbsp;here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>.
   <note type="note">
   This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Format:</strong> Select in which of the following formats you want the report to be delivered:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> HTML</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">PDF</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS&nbsp;Excel (.xlsx)</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">TSV</li>
   </ul></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Include Links:</strong>&nbsp;This option is available&nbsp;only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document. <br>Documents that contain more than 65,000 links cannot be opened. If the exported document will contain more than 65,000 links, deselect this option.<br>This option is enabled by default.</li>
   </ul></li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Send Now</strong>.<br> The report is sent to all users that you identified.<br> Or<br> Click <strong>Make Repeating Delivery</strong>&nbsp;if you want to set up&nbsp;a scheduled delivery with this same information, then complete the additional information regarding the frequency of when the report is sent.</li>
   -->
