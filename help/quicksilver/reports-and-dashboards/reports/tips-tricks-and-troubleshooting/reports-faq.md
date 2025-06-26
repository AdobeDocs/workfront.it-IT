---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Domande frequenti sui rapporti
description: Domande frequenti sui rapporti
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 04818bc054c3bab6e6208b6678365549664d1594
workflow-type: tm+mt
source-wordcount: '1500'
ht-degree: 0%

---

# Domande frequenti sui rapporti

<!--Audited: 05/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

Di seguito sono riportate le domande frequenti sui rapporti.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td><p>Nuovo: Standard</p> 
   <p>Corrente: Lavoro o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Perché il calcolo personalizzato per la differenza di un’ora non mostra il risultato corretto in una colonna?

<!--this section is linked from the Actual Hours article for Tasks in the Task Information folder; edit the links or do not delete or change this section-->

In un report di progetti ho un calcolo che sottrae le ore effettive legacy dalle ore pianificate.

Il risultato che ottengo non è corretto.

<!--this changed with this issue in May 2025; Actual Hours changed from actualWorkRequired to actualWorkRequiredDouble: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/68108e860000120e90a79cb82e5811c2/updates : On a project report I have a calculation that subtracts Actual Hours (2) from Planned Hours (4). The result I am getting is 120 when it should be 2.  -->

Il mio calcolo è:

`valueexpression=SUB(workRequired,actualWorkRequired)`

### Risposta

La maggior parte dei campi che utilizzano le ore in Workfront vengono memorizzati in minuti. Quando si utilizzano questi campi in un calcolo, il risultato sarà spesso in minuti. Per ottenere il risultato in ore, è necessario dividere per 60 il risultato del calcolo o il campo a cui si fa riferimento.

Il calcolo corretto è:

`valueexpression=SUB(workRequired,actualWorkRequired)/60`

>[!NOTE]
>
>Se nel calcolo si utilizzano le ore effettive, utilizzare `actualWorkRequiredDouble` per il campo valore. Le ore effettive vengono memorizzate in ore. Le ore pianificate vengono memorizzate in minuti.
>
>Il calcolo corretto per le ore effettive è:
>>`valueexpression=SUB(workRequired/60,actualWorkRequiredDouble)`


## Perché il valore di ogni elemento del grafico in un report non viene visualizzato nel grafico?

### Risposta

Se in un grafico del rapporto sono presenti più di 50 elementi del grafico, il valore di ciascun elemento non viene visualizzato nel grafico.

Se il grafico contiene meno di 50 elementi, il valore di ciascun elemento viene visualizzato nel grafico. Valuta l’aggiunta di un filtro o la modifica dei raggruppamenti nel rapporto per limitare la quantità di elementi visualizzati in ogni elemento del grafico.

## Perché il report restituisce troppi risultati per visualizzare il grafico?

Quando eseguo un report con un grafico, viene visualizzato il messaggio di errore &quot;Wow there... Questo report ha restituito MOLTI dati, rendendo il grafico illeggibile. È consigliabile limitare i risultati aggiungendo un filtro o modificando i raggruppamenti nel grafico.&quot;

### Risposta

Questo errore indica che il grafico contiene fino a 618 risultati distinti, ad esempio più di 618 barre in un grafico a barre. Per risolvere il problema di visualizzazione, è necessario perfezionare i risultati modificando il filtro e raggruppando le selezioni correnti.

Per informazioni sulla modifica di filtri e raggruppamenti, vedere gli articoli [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) e [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Perché trovo le mie attività (o problemi) quando accedo allo stesso rapporto (o calendario) del mio collega, il quale visualizza le sue attività?

### Risposta

È possibile che nel report o nel calendario sia presente una variabile di filtro con caratteri jolly che punta all&#39;utente connesso. In questo caso, il rapporto mostra informazioni in base all’utente che ha effettuato l’accesso. Regolare il filtro per rimuovere il carattere jolly che punta all&#39;utente connesso.\
![Variabile filtro ID utente](assets/qs--user.id-filter-variable-350x79.png)

Per un elenco completo delle variabili filtro con caratteri jolly basate sull&#39;utente, vedere [Panoramica delle variabili filtro con caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Perché i dati nel report sembrano incompleti?

### Risposta

Questo può accadere nella maggior parte dei casi se disponi di un accesso limitato che impedisce la visualizzazione degli elementi nel sistema. Inoltre, gli elementi che desideri visualizzare non sono condivisi con te.

Il creatore del report può modificarlo per eseguirlo con i diritti di accesso di un amministratore di sistema o di qualsiasi utente del piano che abbia accesso alla visualizzazione dei dati.

Per ulteriori informazioni, vedere [Eseguire e recapitare un report con i diritti di accesso di un altro utente](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## Come posso creare rapporti sulle attività (o problemi) a cui sono assegnato, che io sia il Proprietario o meno?

### Risposta

Per visualizzare tutte le attività o i problemi assegnati, sia che tu sia il Proprietario (o l’Assegnatario principale) o meno, utilizza il seguente filtro in un rapporto di attività o problemi:

1. Accedere a un report di attività o problemi.
1. Nella scheda **Filtri**, fai clic su **Aggiungi regola filtro**.

1. Nel campo **Inizia a digitare il nome del campo ...**, inizia a digitare **Nome utenti assegnazione**, quindi selezionalo quando viene visualizzato nell&#39;elenco.

   >[!NOTE]
   >
   >Non utilizzare il campo **Assegnato a nome**, poiché questo filtro viene applicato solo alle attività e ai problemi per i quali l&#39;utente è l&#39;assegnatario principale o il proprietario.

1. Seleziona il modificatore **Equal**.
1. Inizia a digitare *$$USER.ID* nella casella di testo e selezionalo dall&#39;elenco a discesa visualizzato.\
   In questo modo potrai visualizzare tutte le attività e i problemi assegnati all’utente connesso. È possibile sostituire il carattere jolly con un nome utente specifico.\
   ![Attività assegnate a me](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Fai clic su **Salva e Chiudi**.

## Perché i collegamenti Aggiungi problemi/Aggiungi attività non vengono visualizzati in fondo agli elenchi Problemi e attività di un progetto?

### Risposta

Innanzitutto, assicurati di disporre dell’accesso e delle autorizzazioni corretti per aggiungere problemi e attività a un progetto. In questo caso, dovresti visualizzare i collegamenti **Aggiungi problemi** e **Aggiungi attività** nella parte inferiore degli elenchi **Problemi** e **Attività**.

Tuttavia, ci sono alcuni elementi che potrebbero impedire la visualizzazione di questi collegamenti:

* Se a questi elenchi è applicato il filtro rapido, i collegamenti non vengono visualizzati. Rimuovi il filtro rapido per visualizzare i collegamenti che ti consentiranno di aggiungere problemi e attività ai progetti.\
  Per informazioni sul filtro rapido, vedere [Introduzione agli elenchi in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Se a questi elenchi è applicato un **Raggruppamento**, i collegamenti non vengono visualizzati. Rimuovi il **Raggruppamento** e i collegamenti da visualizzare per aggiungere problemi e attività ai progetti.\
  Per informazioni sulla creazione di raggruppamenti, vedere [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Se a questi elenchi è applicata una **Visualizzazione** con una valuta selezionata diversa da quella predefinita per il progetto, i collegamenti non vengono visualizzati. Modifica la **visualizzazione** in **valuta originale del progetto** e i collegamenti dovrebbero essere visualizzati in modo da poter aggiungere problemi e attività ai progetti.\
  Per ulteriori informazioni sulla modifica della valuta nella visualizzazione, vedere [Creare report di dati finanziari con tassi di cambio univoci](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![Valuta progetto](assets/nwe-project-original-currency-350x229.png)

## Le informazioni nel report o nel dashboard vengono aggiornate automaticamente?

### Risposta

Le informazioni nei rapporti o nelle dashboard non vengono aggiornate automaticamente.

Le informazioni possono essere aggiornate manualmente in un rapporto memorizzato nella cache.\
Per ulteriori informazioni sull&#39;aggiornamento di un report nella cache, vedere [Eseguire un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

Le informazioni possono essere aggiornate manualmente in un dashboard memorizzato nella cache.\
Per ulteriori informazioni sull&#39;aggiornamento di un dashboard memorizzato nella cache, vedere la sezione [Dashboard di visualizzazione](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) nell&#39;articolo [Introduzione ai dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Posso cambiare il proprietario di un report?

### Risposta

Non è possibile cambiare il proprietario di un report. Tuttavia, l’utente che ha creato il rapporto può consentire ad altri utenti di modificarlo. Il modo in cui puoi consentire agli utenti di modificare un rapporto dipende dal tipo di utente che sei.

* Gli amministratori di sistema possono consentire agli utenti con una licenza Pianificazione di modificare i rapporti configurando l’opzione Modifica nella riga Rapporti per includere l’accesso a Crea un rapporto.\
  Per ulteriori informazioni, vedere [Concedere l&#39;accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Tutti gli utenti finali con accesso per creare e condividere report possono consentire ad altri di modificare singoli report condividendoli e assegnando ad altri utenti le autorizzazioni di gestione per tali report.\
  Per ulteriori informazioni, vedere [Condividere un report in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Se disponi delle autorizzazioni necessarie per visualizzare o gestire un rapporto, puoi anche creare una copia del rapporto, di cui sarai il proprietario per impostazione predefinita. Per ulteriori informazioni sulla copia di un report, vedere [Creare una copia di un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Perché non posso accedere a un report di proprietà di un utente disattivato?

### Risposta

A volte, il proprietario del report è anche l&#39;utente specificato nel campo **Esegui report con i diritti di accesso di:** nel report. Se **Esegui il report con i diritti di accesso di:** utente è disattivato, il report non verrà più visualizzato per gli utenti che hanno condiviso il report con loro. In questo caso, è possibile rendere nuovamente accessibile il report lasciando vuoto **Esegui il report con i diritti di accesso di:** o immettendo un utente attivo nel campo.

Per ulteriori informazioni sul campo **Esegui il report con i diritti di accesso di:**, vedere [Esegui e recapita un report con i diritti di accesso di un altro utente](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Per informazioni sull&#39;identificazione di tutti i report di proprietà di utenti disattivati, vedere [Creare un report sulle attività di reporting](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## Come posso accedere a una dashboard contenente un report di proprietà di un utente eliminato?

### Risposta

Quando elimini un utente, puoi comunque accedere a tutti i rapporti creati, ma vengono eliminati anche tutti i dashboard che includevano il rapporto. Ciò significa che non è più possibile accedere ai seguenti elementi:

* Dashboard contenente il report
* Una sezione personalizzata che contiene una dashboard del report

Per ulteriori informazioni sulle implicazioni dell&#39;eliminazione di un utente, vedere [Elimina utenti](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Se disponi dell’accesso di visualizzazione al rapporto, puoi effettuare le seguenti operazioni:

1. Crea una copia del rapporto.\
   Per informazioni su come creare una copia di un report, vedere [Creare una copia di un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Aggiorna il dashboard in modo da includere il report copiato.\
   Per informazioni su come modificare un dashboard, vedere [Modificare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
