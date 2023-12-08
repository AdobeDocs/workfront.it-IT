---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Domande frequenti sui rapporti
description: Domande frequenti sui rapporti
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: d8e3c2da7f8fcd062e1bf2bb5de43a6238f5eadd
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# Domande frequenti sui rapporti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

Di seguito sono riportate le domande frequenti sui rapporti.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano, Lavoro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Perché il calcolo personalizzato per la differenza di un’ora non mostra il risultato corretto in una colonna?

In un report di progetti ho un calcolo che sottrae le ore effettive (2) dalle ore pianificate (4). Il risultato che ottengo è 120 quando dovrebbe essere 2.\
Il mio calcolo è:
<pre>valueexpression=SUB(workRequired,actualWorkRequired)</pre>

### Risposta

I campi che utilizzano le ore in Workfront vengono memorizzati in minuti. Quando si utilizza il campo in un calcolo, il risultato sarà in minuti. Per ottenere il risultato in ore, è necessario dividere il risultato del calcolo per 60.

Il calcolo corretto è:

<pre>valueexpression=SUB(workRequired,actualWorkRequired)/60</pre>

## Perché il valore di ogni elemento del grafico in un report non viene visualizzato nel grafico?

### Risposta

Se in un grafico del rapporto sono presenti più di 50 elementi del grafico, il valore di ciascun elemento non viene visualizzato nel grafico.

Se il grafico contiene meno di 50 elementi, il valore di ciascun elemento viene visualizzato nel grafico. Valuta l’aggiunta di un filtro o la modifica dei raggruppamenti nel rapporto per limitare la quantità di elementi visualizzati in ogni elemento del grafico.

## Perché il report restituisce troppi risultati per visualizzare il grafico?

Quando eseguo un report con un grafico, viene visualizzato il messaggio di errore &quot;Wow there... Questo report ha restituito MOLTI dati, rendendo il grafico illeggibile. È consigliabile limitare i risultati aggiungendo un filtro o modificando i raggruppamenti nel grafico.&quot;

### Risposta

Questo errore indica che il grafico contiene fino a 618 risultati distinti, ad esempio più di 618 barre in un grafico a barre. Per risolvere il problema di visualizzazione, è necessario perfezionare i risultati modificando il filtro e raggruppando le selezioni correnti.

Per informazioni sulla modifica di filtri e raggruppamenti, consulta gli articoli [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) e [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Perché trovo le mie attività (o problemi) quando accedo allo stesso rapporto (o calendario) del mio collega, il quale visualizza le sue attività?

### Risposta

È possibile che nel report o nel calendario sia presente una variabile di filtro con caratteri jolly che punta all&#39;utente connesso. In questo caso, il rapporto mostra informazioni in base all’utente che ha effettuato l’accesso. Regolare il filtro per rimuovere il carattere jolly che punta all&#39;utente connesso.\
![](assets/qs--user.id-filter-variable-350x79.png)

Per un elenco completo delle variabili filtro con caratteri jolly basate sull&#39;utente, vedere [Panoramica delle variabili filtro con caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Perché i dati nel report sembrano incompleti?

### Risposta

Questo può accadere nella maggior parte dei casi se disponi di un accesso limitato che impedisce la visualizzazione degli elementi nel sistema. Inoltre, gli elementi che desideri visualizzare non sono condivisi con te.

Il creatore del report può modificarlo per eseguirlo con i diritti di accesso di un amministratore di sistema o di qualsiasi utente del piano che abbia accesso alla visualizzazione dei dati.

Per ulteriori informazioni, consulta [Eseguire e consegnare un report con i diritti di accesso di un altro utente](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## Come posso creare rapporti sulle attività (o problemi) a cui sono assegnato, che io sia il Proprietario o meno?

### Risposta

Per visualizzare tutte le attività o i problemi assegnati, sia che tu sia il Proprietario (o l’Assegnatario principale) o meno, utilizza il seguente filtro in un rapporto di attività o problemi:

1. Accedere a un report di attività o problemi.
1. Il giorno **Filtri** , fare clic su **Aggiungere una regola di filtro**.

1. In **Inizia a digitare il nome del campo ...** campo, inizia a digitare **Nome utenti assegnazione**, quindi selezionarla quando viene visualizzata nell&#39;elenco.

   >[!NOTE]
   >
   >Non utilizzare il **Assegnato a Nome** come questo filtra solo per le attività e i problemi per i quali sei l’assegnatario principale o il proprietario.

1. Seleziona la **Uguale** modificatore.
1. Inizia a digitare *$$USER.ID* nella casella di testo e selezionarla dall&#39;elenco a discesa visualizzato.\
   In questo modo potrai visualizzare tutte le attività e i problemi assegnati all’utente connesso. È possibile sostituire il carattere jolly con un nome utente specifico.\
   ![](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Clic **Salva e chiudi**.

## Perché i collegamenti Aggiungi problemi/Aggiungi attività non vengono visualizzati in fondo agli elenchi Problemi e attività di un progetto?

### Risposta

Innanzitutto, assicurati di disporre dell’accesso e delle autorizzazioni corretti per aggiungere problemi e attività a un progetto. In questo caso, dovresti visualizzare **Aggiungi problemi** e **Aggiungi attività** collegamenti nella parte inferiore della sezione **Problemi** e **Attività** elenchi.

Tuttavia, ci sono alcuni elementi che potrebbero impedire la visualizzazione di questi collegamenti:

* Se a questi elenchi è applicato il filtro rapido, i collegamenti non vengono visualizzati. Rimuovi il filtro rapido per visualizzare i collegamenti che ti consentiranno di aggiungere problemi e attività ai progetti.\
  Per informazioni sul filtro rapido, consulta [Introduzione agli elenchi in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Se si dispone di **Raggruppamento** applicati a questi elenchi, i collegamenti non vengono visualizzati. Rimuovi il **Raggruppamento** e i collegamenti dovrebbero essere visualizzati per consentire di aggiungere problemi e attività ai progetti.\
  Per informazioni sulla creazione di raggruppamenti, consulta [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Se si dispone di **Visualizza** applicati a questi elenchi la cui valuta è diversa da quella predefinita per il progetto, i collegamenti non vengono visualizzati. Modificare il **Visualizza** a **Valuta originale del progetto** e i collegamenti dovrebbero essere visualizzati per consentire di aggiungere problemi e attività ai progetti.\
  Per ulteriori informazioni sulla modifica della valuta nella visualizzazione, vedere [Creazione di report di dati finanziari con tassi di cambio univoci](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![](assets/nwe-project-original-currency-350x229.png)

## Le informazioni nel report o nel dashboard vengono aggiornate automaticamente?

### Risposta

Le informazioni nei rapporti o nelle dashboard non vengono aggiornate automaticamente.

Le informazioni possono essere aggiornate manualmente in un rapporto memorizzato nella cache.\
Per ulteriori informazioni sull’aggiornamento di un rapporto memorizzato nella cache, consulta [Eseguire un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

Le informazioni possono essere aggiornate manualmente in un dashboard memorizzato nella cache.\
Per ulteriori informazioni sull’aggiornamento di un dashboard memorizzato in cache, consulta la sezione [Visualizza dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) nell’articolo [Introduzione alle dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Posso cambiare il proprietario di un report?

### Risposta

Non è possibile cambiare il proprietario di un report. Tuttavia, l’utente che ha creato il rapporto può consentire ad altri utenti di modificarlo. Il modo in cui puoi consentire agli utenti di modificare un rapporto dipende dal tipo di utente che sei.

* Gli amministratori di sistema possono consentire agli utenti con una licenza Pianificazione di modificare i rapporti configurando l’opzione Modifica nella riga Rapporti per includere l’accesso a Crea un rapporto.\
  Per ulteriori informazioni, consulta [Concedere l’accesso a rapporti, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Tutti gli utenti finali con accesso per creare e condividere report possono consentire ad altri di modificare singoli report condividendoli e assegnando ad altri utenti le autorizzazioni di gestione per tali report.\
  Per ulteriori informazioni, consulta [Condividere un rapporto in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Se disponi delle autorizzazioni necessarie per visualizzare o gestire un rapporto, puoi anche creare una copia del rapporto, di cui sarai il proprietario per impostazione predefinita. Per ulteriori informazioni sulla copia di un report, consulta [Creare una copia di un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Perché non posso accedere a un report di proprietà di un utente disattivato?

### Risposta

A volte, il proprietario del rapporto è anche l’utente specificato nel **Esegui questo report con i diritti di accesso di:** sul report. Se il **Esegui questo report con i diritti di accesso di:** se l’utente è disattivato, il rapporto non viene più visualizzato per gli utenti che hanno il rapporto condiviso con loro. In questo caso, puoi rendere nuovamente accessibile il rapporto lasciando **Esegui questo report con i diritti di accesso di:** vuoto o inserendo un utente attivo nel campo.

Per ulteriori informazioni su **Esegui questo report con i diritti di accesso di:** campo, vedi [Eseguire e consegnare un report con i diritti di accesso di un altro utente](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Per informazioni sull’identificazione di tutti i rapporti di proprietà di utenti disattivati, consulta [Creare un rapporto sulle attività di reporting](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## Come posso accedere a una dashboard contenente un report di proprietà di un utente eliminato?

### Risposta

Quando elimini un utente, puoi comunque accedere a tutti i rapporti creati, ma vengono eliminati anche tutti i dashboard che includevano il rapporto. Ciò significa che non è più possibile accedere ai seguenti elementi:

* Dashboard contenente il report
* Una sezione personalizzata che contiene una dashboard del report

Per ulteriori informazioni sulle implicazioni dell’eliminazione di un utente, consulta [Elimina utenti](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Se disponi dell’accesso di visualizzazione al rapporto, puoi effettuare le seguenti operazioni:

1. Crea una copia del rapporto.\
   Per informazioni su come creare una copia di un report, consulta [Creare una copia di un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Aggiorna il dashboard in modo da includere il report copiato.\
   Per informazioni su come modificare un dashboard, consulta [Modificare una dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
