---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Domande frequenti sui rapporti
description: Domande frequenti sui rapporti
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1502'
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
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano, Lavoro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Perché il mio calcolo personalizzato per una differenza di ora non mostra il risultato corretto in una colonna?

In un rapporto del progetto ho un calcolo che sottrae le ore effettive (2) dalle ore pianificate (4). Il risultato che ottengo è 120 quando dovrebbe essere 2.\
Il mio calcolo è:
<pre>valueexpression=SUB(workRequired,effectiveWorkRequired)</pre>

### Risposta

I campi che utilizzano ore in Workfront vengono memorizzati in minuti. Quando si utilizza il campo in un calcolo, il risultato sarà espresso in minuti. Per ottenere il risultato in ore, è necessario dividere il risultato del calcolo per 60.

Il calcolo corretto è il seguente:

<pre>valueexpression=SUB(workRequired,effectiveWorkRequired)/60</pre>

## Perché il valore di ciascuno degli elementi del grafico in un rapporto non viene visualizzato nel grafico?

### Risposta

Se il grafico contiene più di 50 elementi grafico, il valore di ciascun elemento non viene visualizzato nel grafico.

Se in un grafico sono presenti meno di 50 elementi, il valore di ciascun elemento viene visualizzato nel grafico. È consigliabile aggiungere un filtro o modificare i raggruppamenti nel rapporto per limitare la quantità di elementi visualizzati in ciascun elemento del grafico.

## Perché il rapporto restituisce troppi risultati per visualizzare il grafico?

Quando eseguo un report con un grafico, vedo il messaggio di errore &quot;Wow qui... Questo report ha restituito UN SACCO di dati che rende il grafico illeggibile. È consigliabile restringere i risultati aggiungendo un filtro o modificando i raggruppamenti nel grafico.&quot;

### Risposta

Questo errore significa che il grafico contiene fino a 618 risultati distinti, ad esempio più di 618 barre in un grafico a barre. Per risolvere il problema di visualizzazione, è necessario perfezionare i risultati modificando il filtro corrente e raggruppando le selezioni.

Per informazioni sulla modifica di filtri e raggruppamenti, consulta gli articoli [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) e [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Perché visualizzo le mie attività (o problemi) quando accedo allo stesso rapporto (o calendario) del mio collega e questi visualizza le loro attività?

### Risposta

Il report o il calendario potrebbe avere una variabile di filtro con caratteri jolly che punta all&#39;utente che ha effettuato l&#39;accesso. In questo caso, il rapporto mostra le informazioni in base all&#39;utente che ha effettuato l&#39;accesso. Regola il filtro per rimuovere il carattere jolly che punta all&#39;utente connesso.\
![](assets/qs--user.id-filter-variable-350x79.png)

Per un elenco completo delle variabili filtro dei caratteri jolly basate sull’utente, consulta [Variabili filtro caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Perché i dati nel mio rapporto sembrano incompleti?

### Risposta

Questo può accadere nella maggior parte dei casi se si dispone di un accesso limitato che impedisce la visualizzazione di elementi nel sistema. Inoltre, gli elementi che desideri visualizzare non vengono condivisi con te.

Il creatore del rapporto può modificare il rapporto per eseguirlo con i diritti di accesso di un amministratore di sistema o di qualsiasi utente di Plan che ha accesso per visualizzare i dati.

Per ulteriori informazioni, consulta [Eseguire e distribuire un rapporto con i diritti di accesso di un altro utente](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## Come faccio a segnalare le attività (o i problemi) a cui sono assegnato, se sono il proprietario o meno?

### Risposta

Per visualizzare tutte le attività o i problemi assegnati all&#39;utente, indipendentemente dal fatto che si sia il proprietario (o l&#39;assegnatario principale) o meno, utilizzare il filtro seguente in un report attività o problema:

1. Accedere a un report attività o problema.
1. Sulla **Filtri** scheda , fai clic su **Aggiungere una regola filtro**.

1. In **Inizia a digitare il nome del campo ...** campo, inizia a digitare **Nome utente assegnazione**, quindi selezionalo quando viene visualizzato nell’elenco.

   >[!NOTE]
   >
   >Non utilizzare il **Assegnato al nome** , poiché questo filtra solo le attività e i problemi per i quali sei l&#39;assegnatario principale o il proprietario.

1. Seleziona la **Uguale** modificatore.
1. Inizia a digitare *$$USER.ID* nella casella di testo e selezionarla dall&#39;elenco a discesa visualizzato.\
   In questo modo puoi visualizzare tutte le attività e i problemi assegnati all’utente connesso. È possibile sostituire il carattere jolly con un nome utente specifico.\
   ![](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Fai clic su **Salva e chiudi**.

## Perché i collegamenti Aggiungi problemi/Aggiungi attività non vengono visualizzati nella parte inferiore degli elenchi Problemi e attività di un progetto?

### Risposta

In primo luogo, assicurati di disporre dell’accesso e delle autorizzazioni corrette per aggiungere problemi e attività a un progetto. In questo caso, dovresti visualizzare il **Aggiungi problemi** e **Aggiungi attività** collegamenti nella parte inferiore del **Problemi** e **Attività** elenchi.

Tuttavia, esistono alcuni elementi che possono impedire la visualizzazione di questi collegamenti:

* Se il filtro rapido è applicato a questi elenchi, i collegamenti non vengono visualizzati. Rimuovi il filtro rapido e i collegamenti devono essere visualizzati in modo da poter aggiungere problemi e attività ai progetti.\
   Per informazioni sul filtro rapido, consulta [Guida introduttiva agli elenchi in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Se hai **Raggruppamento** applicati a questi elenchi, i collegamenti non vengono visualizzati. Rimuovi **Raggruppamento** e i collegamenti devono essere visualizzati in modo da poter aggiungere problemi e attività ai progetti.\
   Per informazioni sulla creazione di gruppi, consulta [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Se hai **Visualizza** applicati a questi elenchi in cui è selezionata una valuta diversa da quella predefinita per il progetto, i collegamenti non vengono visualizzati. Modificare la **Visualizza** a **Valuta originale del progetto** e i collegamenti devono essere visualizzati in modo da poter aggiungere problemi e attività ai progetti.\
   Per ulteriori informazioni sulla modifica della valuta nella visualizzazione, vedere [Creare rapporti di dati finanziari con tassi di cambio univoci](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![](assets/nwe-project-original-currency-350x229.png)

## Le informazioni nel rapporto o nel dashboard vengono aggiornate automaticamente?

### Risposta

Le informazioni nei rapporti o nelle dashboard non vengono aggiornate automaticamente.

Le informazioni possono essere aggiornate manualmente in un rapporto memorizzato nella cache.\
Per ulteriori informazioni sull’aggiornamento di un rapporto nella cache, consulta [Eseguire un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

Le informazioni possono essere aggiornate manualmente in un dashboard memorizzato nella cache.\
Per ulteriori informazioni sull’aggiornamento di un dashboard memorizzato nella cache, consulta la sezione . [Visualizza dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) nell&#39;articolo [Guida introduttiva alle dashboard](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Posso cambiare il proprietario di un report?

### Risposta

Non è possibile modificare il proprietario di un report. Tuttavia, l’utente che ha creato il rapporto può consentire ad altri utenti di modificarlo. La modalità di modifica di un rapporto da parte degli utenti dipende dal tipo di utente.

* Gli amministratori di sistema possono consentire agli utenti con una licenza Pianifica di modificare i rapporti configurando l’opzione Modifica nella riga Rapporti per includere l’accesso a Crea un rapporto.\
   Per ulteriori informazioni, consulta [Consentire l’accesso a report, dashboard e calendari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Gli utenti finali con accesso per creare e condividere rapporti possono consentire ad altri di modificare singoli rapporti condividendoli e concedendo ad altri utenti le autorizzazioni di gestione.\
   Per ulteriori informazioni, consulta [Condivisione di un rapporto in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Se disponi delle autorizzazioni necessarie per visualizzare o gestire un rapporto, puoi anche creare una copia del rapporto, di cui sei il proprietario per impostazione predefinita. Per ulteriori informazioni sulla copia di un rapporto, consulta [Creare una copia di un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Perché non posso accedere a un report di proprietà di un utente disattivato?

### Risposta

A volte, il proprietario del report è anche l&#39;utente specificato nel **Esegui questo rapporto con i diritti di accesso di:** sul report. Se la **Esegui questo rapporto con i diritti di accesso di:** l’utente è disattivato; il rapporto non viene più visualizzato per gli utenti che hanno condiviso con loro il rapporto. In questo caso, puoi rendere nuovamente accessibile il rapporto lasciando il **Esegui questo rapporto con i diritti di accesso di:** vuoto o immissione di un utente attivo nel campo .

Per ulteriori informazioni sulle **Esegui questo rapporto con i diritti di accesso di:** campo, vedi [Eseguire e distribuire un rapporto con i diritti di accesso di un altro utente](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Per informazioni sull&#39;identificazione di tutti i rapporti di proprietà di utenti disattivati, vedi [Creare un rapporto sulle attività di reporting](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## Come posso accedere a un dashboard contenente un report di proprietà di un utente eliminato?

### Risposta

Quando elimini un utente, puoi comunque accedere a tutti i rapporti creati, ma vengono eliminati anche tutti i dashboard che includevano il rapporto. Ciò significa che non è più possibile accedere ai seguenti elementi:

* Dashboard contenente il report
* Sezione personalizzata contenente una dashboard del report

Per ulteriori informazioni sulle implicazioni dell&#39;eliminazione di un utente, consulta [Eliminare gli utenti](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Se disponi dell’accesso Visualizza al rapporto, puoi effettuare le seguenti operazioni:

1. Crea una copia del rapporto.\
   Per scoprire come creare una copia di un rapporto, vedi [Creare una copia di un rapporto](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Aggiorna il dashboard per includere il report copiato.\
   Per informazioni su come modificare un dashboard, consulta [Modificare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
