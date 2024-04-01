---
content-type: overview
product-area: timesheets
navigation-topic: timesheets-navigation-topic
title: Panoramica del layout della scheda orario
description: Questo articolo descrive il layout delle schede orario in Adobe Workfront, consentendoti di comprendere meglio come personalizzare e utilizzare le schede orario per registrare l’ora.
author: Alina
feature: Timesheets
exl-id: 31c48a50-5235-495c-8e46-0974ed98ede1
source-git-commit: ee957e319941fe5eabb9144eed184372e5402197
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 1%

---

# Panoramica del layout della scheda orario

<!-- Audited: 12/2023 -->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti o in produzione per i clienti che hanno abilitato le versioni rapide. </span>

<span class="preview">Per informazioni sulle versioni rapide, consulta [Abilitare o disabilitare le versioni rapide per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Per informazioni sulla pianificazione della versione corrente, consulta [Panoramica sulla versione del secondo trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Questo articolo descrive il layout delle schede orario in Adobe Workfront, consentendoti di comprendere meglio come personalizzare e utilizzare le schede orario per registrare l’ora.

Le preferenze delle ore e della scheda orario controllano ciò che viene visualizzato su una scheda orario. Questo articolo fornisce una panoramica di tutte le opzioni disponibili. Per informazioni sulla selezione delle opzioni, consulta [Configurare le preferenze di orario e scheda orario](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Per informazioni su come registrare l&#39;ora in una scheda orario, vedere [Tempo di connessione](../../timesheets/create-and-manage-timesheets/log-time.md).

![Layout scheda orario](assets/timesheet-layout-unshimmed.png)

Di seguito sono riportate le aree di una scheda orario:

* [Intestazione scheda orario](#timesheet-header)
* [Pannello a sinistra](#the-left-panel)
* [Elementi di lavoro](#work-items)
* [Barra Strumenti](#toolbar)
* [Piè di pagina scheda orario](#timesheet-footer)
* [Ruolo](#job-role)
* [Tipo di ora](#hour-type)
* [Area Aggiornamenti nel pannello a sinistra](#updates-area-in-the-left-panel)
* [Pannello di Riepilogo](#summary-panel)
* [Intervallo temporale e area di immissione ore](#time-frame-and-hour-entry-area)
* [Commenti immissione ore](#hour-entry-comments)
* [Ore](#hours)
* [Totali](#totals)

## Intestazione scheda orario

![Intestazione scheda orario](assets/timesheet-title-unshimmed-redesign.png)

L’intestazione della scheda orario include le seguenti informazioni:

* L’intervallo di tempo della scheda orario.
* L&#39;area Azioni che include quanto segue:
   * Un&#39;icona stella per aggiungere le schede orario all&#39;elenco dei preferiti.
   * L’icona Altro con l’opzione Elimina che consente di eliminare la scheda orario.
* Nome del proprietario della scheda orario.
* Il numero di ore totali per le ore registrate per gli elementi visualizzati nella scheda orario.
* Il numero di ore di straordinario. Questa è una voce manuale ed è visibile solo quando **Straordinari** l&#39;impostazione è abilitata su una scheda orario. Per ulteriori informazioni, consulta [Modifica informazioni scheda orario](../create-and-manage-timesheets/edit-timesheets.md).

>[!TIP]
>
>Non è possibile registrare un numero di ore di straordinario maggiore delle ore totali correnti nella scheda orario. Ad esempio, se hai registrato 7 ore sulla scheda orario finora, non puoi registrare 8 ore di lavoro straordinario.

* Lo stato della scheda orario.

## Pannello a sinistra

![Pannello sinistro scheda orario](assets/timesheet-left-panel-unshimmed-redesign.png)

Potete accedere alle seguenti sezioni nel pannello a sinistra:

* **Scheda orario**: visualizza la scheda orario effettiva.
* **Aggiornamenti**: visualizza commenti e aggiornamenti di sistema per la scheda orario. Per ulteriori informazioni, vedere [Area Aggiornamenti nel pannello a sinistra](#updates-area-in-the-left-panel) in questo articolo.

## Elementi di lavoro

![Elementi di lavoro scheda orario](assets/timesheet-object-names-unshimmed-redesign.png)

Gli elementi di lavoro sono i progetti, le attività e i problemi per i quali si desidera registrare l&#39;ora. Facendo clic sulla freccia rivolta verso il basso nella riga di intestazione, i progetti e le attività e i problemi elencati di seguito vengono compressi. Facendo clic sulla freccia rivolta verso il basso accanto al nome di un progetto, gli elementi di lavoro del progetto vengono compressi.

Le attività, i problemi e i progetti in cui il tempo viene registrato al di fuori della scheda orario o gli elementi pianificati durante l’arco temporale della scheda orario vengono visualizzati qui automaticamente.

## Barra Strumenti

![Barra degli strumenti Scheda orario](assets/timesheet-toolbar-unshimmed-redesign.png)

La barra degli strumenti include le seguenti opzioni:

* Il **Aggiungi elemento** che consente di aggiungere progetti, attività o problemi.
* L’icona del filtro rapido per cercare attività o problemi nella scheda orario.
* Il **Mostra commenti** impostazione che consente di visualizzare o nascondere i commenti sulle ore registrati per le voci relative alle ore progetto, attività o problema.
* L’icona a schermo intero per visualizzare la scheda orario in modalità a schermo intero.
* Il **Apri riepilogo** (o **Chiudi riepilogo**) per aprire o chiudere il pannello Riepilogo e visualizzare informazioni aggiuntive relative ad attività o problemi. Questo pulsante non è disponibile per i progetti.

Per ulteriori informazioni, consulta [Tempo di connessione](../create-and-manage-timesheets/log-time.md).

## Piè di pagina scheda orario

![Piè di pagina scheda orario](assets/timesheet-footer-unshimmed-redesign.png)

Puoi fare clic su **Invia per approvazione**, **Chiudi**, **Approva**, e **Rifiuta** pulsanti in quest&#39;area per chiudere o rifiutare l&#39;approvazione di una scheda orario.

Questa area contiene anche informazioni sull’ultimo salvataggio della scheda orario. Tutte le modifiche apportate alle informazioni nella scheda orario vengono salvate automaticamente.

## Ruolo

![Ruoli](assets/timesheet-job-role-area-unshimmed-redesign.png)

È possibile selezionare una mansione diversa da associare alle ore inserite. L&#39;amministratore di Workfront deve abilitare **Assegna mansioni alle ore inserite** impostazione manuale. La mansione specificata al momento dell’assegnazione dell’attività o il problema viene visualizzato per impostazione predefinita. Se non ti è stata assegnata una mansione per l’attività o il problema, il tuo Ruolo principale viene visualizzato come predefinito. Per ulteriori informazioni, consulta [Configurare le preferenze di orario e scheda orario](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

È possibile registrare più ore per lo stesso elemento di lavoro per ruoli diversi. Per ulteriori informazioni, consulta [Tempo di connessione](../create-and-manage-timesheets/log-time.md).

## Tipo di ora

![Tipi di ore](assets/timesheet-hour-type-unshimmed-redesign.png)

È possibile selezionare diversi tipi di ore da associare alle ore inserite in ogni elemento. Questo campo viene visualizzato solo quando l’amministratore di Workfront lo abilita per il tuo ambiente. Per informazioni, consulta [Configurare le preferenze di orario e scheda orario](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

È possibile registrare più ore per lo stesso elemento di lavoro per tipi di ore diversi. Per ulteriori informazioni, consulta [Tempo di connessione](../create-and-manage-timesheets/log-time.md).

## Area Aggiornamenti nel pannello a sinistra

<div class="preview">

![Area Aggiornamenti nel pannello Timesheet a sinistra](assets/timesheet-updates-with-all-tab.png)

</div>

È possibile aggiungere commenti a una scheda orario per comunicare con gli approvatori della scheda orario o altri utenti nella sezione Aggiornamenti nel pannello sinistro della scheda orario.

Eventuali commenti aggiunti alla scheda orario vengono visualizzati in quest&#39;area.

## Pannello di Riepilogo

<div class="preview">

![Pannello Riepilogo](assets/timesheet-summary-panel-on-updates.png)

</div>

Puoi accedere al pannello Riepilogo per le attività o i problemi visualizzati in una scheda orario. Da qui puoi aggiungere commenti ad attività e problemi, o aggiornarne le informazioni. Per ulteriori informazioni, consulta [Panoramica di riepilogo](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

I commenti immessi per gli elementi di lavoro nel pannello Riepilogo scheda orario vengono visualizzati nell’area Aggiornamenti dell’attività o del problema. Il pannello Riepilogo non è disponibile per i progetti.

## Intervallo temporale e area di immissione ore

![Intervallo temporale scheda orario](assets/timesheet-time-frame-log-time-area.png)

L’intervallo di tempo della scheda orario viene visualizzato a destra degli elementi di lavoro.

Puoi creare schede orario per una, due o quattro settimane.

L’intervallo di tempo viene visualizzato con incrementi di una settimana intera. I giorni che non rientrano nell’intervallo di tempo specificato per la scheda orario non sono attivi. Non è possibile registrare il tempo per i giorni che non rientrano nell&#39;intervallo di tempo della scheda orario.

Per informazioni, consulta [Creare una scheda orario monouso](../create-and-manage-timesheets/create-tmshts.md) o [Creare, modificare e assegnare profili di schede orario](../create-and-manage-timesheets/create-timesheet-profiles.md).

<!--drafted for the resize columns in timesheets story - make this blurb a TIP when the story is released: 
You can resize the columns that display different weeks, the time frame, or the work item areas by dragging and dropping the vertical lines that separate them.-->

## Commenti immissione ore

![Commenti immissione ore](assets/timesheet-hour-entry-comment-button-unshimmed-redesign.png)

È possibile aggiungere un commento per ogni voce oraria aggiunta alla scheda orario.

I commenti immessi nella casella di commento della voce ore vengono visualizzati nella scheda attività, sotto ogni elemento di lavoro in cui è stata registrata l&#39;ora in cui **Mostra commenti** nella barra degli strumenti.

![](assets/hour-entry-comment-under-task-in-timesheet-unshimmed-redesign.png)

## Ore

![Ore Timesheet](assets/timesheet-hours-area-unshimmed-redesign.png)

La scheda orario fornisce campi di input per ogni elemento di lavoro e giorno dell&#39;intervallo della scheda orario per registrare il tempo impiegato per lavorare sull&#39;elemento. Quando si registra l&#39;ora, l&#39;elemento per il quale si registra l&#39;ora viene evidenziato in blu chiaro e la casella ore viene evidenziata in blu scuro.

## Totali

![Totali schede orario](assets/timesheet-totals-column-and-header-unshimmed-redesign.png)

Rivedi la somma di tutte le ore inserite nella scheda orario, riepilogate per giorno (nell’intestazione della scheda orario) e per oggetto (nell’ultima colonna).
