---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Pianificare una consegna automatica dei rapporti
description: Pianificare una consegna automatica dei rapporti
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 2%

---

# Pianificare una consegna automatica dei rapporti

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

Puoi pianificare la consegna automatica dei rapporti agli utenti in base a una pianificazione definita oppure puoi inviare manualmente i rapporti una tantum. Quando invii un rapporto da Adobe Workfront, l’utente riceve un’e-mail con il rapporto Workfront in un allegato separato.

Per ulteriori informazioni, compresi i limiti di dimensione che possono influenzare la consegna dei rapporti, vedi [Panoramica sulla consegna dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Prima di iniziare, è necessario creare un rapporto. Per ulteriori informazioni sulla creazione dei rapporti, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Pianificare una consegna del rapporto

Per pianificare la consegna automatica di un rapporto o per modificarne o eliminarne una esistente: &#x200B;

1. Passa a un rapporto che desideri pianificare per la consegna.

   >[!NOTE]
   >
   >Le consegne dei rapporti non contengono prompt. Se desideri limitare i dati nella consegna di un rapporto, ti consigliamo di applicare filtri al rapporto che desideri inviare.

1. Fai clic su **Azioni dei rapporti**, quindi **Invia rapporto**.

   La **Invia rapporto** viene visualizzata la finestra di dialogo.

   >[!TIP]
   >
   >Per inviare manualmente un rapporto in un dato momento, passa al rapporto, quindi fai clic su **Azioni dei rapporti** > **Invia rapporto** > **Invia subito**.

1. Seleziona la **Consegne ripetute** scheda .
1. (Condizionale) Per modificare una consegna di report ripetuta esistente, seleziona la consegna del report nel **Consegne ripetute** sezione .
1. Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Invia a</p> </td> 
      <td> <p>Inizia a digitare il nome dell’utente, del gruppo, del team o del ruolo a cui desideri inviare il rapporto, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.</p> <p>Oppure</p> <p>Specifica l’indirizzo e-mail di una persona esterna al sistema Workfront a cui desideri accedere al rapporto.</p> <p>Ripeti questa procedura per inviare il rapporto a più utenti, gruppi, team o ruoli.</p> <p>Nota:  <p>Quando aggiungi i destinatari della consegna dei rapporti, considera quanto segue:</p> 
        <ul> 
         <li>Se la tua organizzazione limita le notifiche Workfront a specifici domini e-mail, puoi solo inviare i rapporti agli indirizzi e-mail elencati nell’inserire nell'elenco Consentiti e-mail.<p>Per informazioni su come un amministratore di Workfront aggiorna l’inserire nell'elenco Consentiti e-mail, consulta la sezione . <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Configurare l’inserire nell'elenco Consentiti e-mail</a>.</p></li> 
         <li> <p>Se si aggiunge un numero elevato di utenti come destinatari, la consegna potrebbe non riuscire. In caso di errori di consegna, puoi pianificare più consegne di rapporti con gruppi di utenti più piccoli.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Oggetto e-mail</p> </td> 
      <td> <p>Specifica un oggetto per la notifica e-mail.</p> <p>Per impostazione predefinita, l’oggetto dell’e-mail è:</p> <p><em>Rapporto Workfront: [Nome del report] [Data]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Messaggio e-mail</p> </td> 
      <td> <p>Specifica un messaggio da includere nell’e-mail.</p> <p>Per impostazione predefinita, il messaggio e-mail è:</p> <p><em>In allegato è presente il report [report frequency] [Name of the report] generato da Workfront il [Date].</em> </p> <p>Nota: Per i report consegnati solo come file Excel, viene aggiunto anche il seguente messaggio all'e-mail: "Tieni presente che con i tipi di file MS Excel (XLS), esiste un limite (65.530) al numero di collegamenti ipertestuali supportati da questi tipi di file. Se superi tali limiti, il file non si aprirà e si consiglia di inviare nuovamente senza i collegamenti ipertestuali. Torna alla pianificazione dei report per rimuovere i collegamenti ipertestuali e inviare nuovamente il report." La frase "per favore torna alla scheduler dei report" è un link alla relazione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Fornire questo rapporto con i diritti di accesso di</p> </td> 
      <td> <p>Inizia a digitare il nome di un utente che ha accesso al rapporto, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa. Gli utenti che ricevono il rapporto avranno lo stesso livello di accesso al rapporto dell’utente specificato qui.<br> Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Eseguire e distribuire un rapporto con i diritti di accesso di un altro utente</a>.</p> <p>Nota: Questo campo non supporta i caratteri jolly. Ad esempio, l'utilizzo del carattere jolly $$User.ID non esegue il rapporto con i diritti di accesso dell'utente che riceve il rapporto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Formato</p> </td> 
      <td> <p>Selezionare il formato desiderato per il rapporto consegnato:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Selezionando questa opzione, è possibile formattare l'output utilizzando l'opzione aggiuntiva <strong>Formato carta</strong> e <strong>Orientamento</strong> opzioni visualizzate.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Includi i link</p> </td> 
      <td> <p>Questa opzione è disponibile solo quando <strong>MS Excel</strong> è selezionato in <strong>Formato</strong> menu a discesa. Quando questa opzione è attivata, tutti i collegamenti ipertestuali vengono inclusi nel documento Excel esportato.</p> <p>Non è possibile aprire i documenti contenenti più di 65.530 collegamenti. Se il documento esportato contiene più di 65.530 collegamenti, deselezionare questa opzione.</p> <p>Questa opzione è attivata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Riepilogo</p> </td> 
      <td> <p>Visualizza un riepilogo di quando la consegna si ripete.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Si ripete</p> </td> 
      <td> <p>Seleziona se il rapporto deve essere consegnato quotidianamente, settimanalmente, mensilmente o annualmente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Si ripete ogni</p> </td> 
      <td> <p>Seleziona la frequenza con cui vuoi ripetere la consegna. Il valore selezionato per questa opzione si basa sull’opzione selezionata nella <strong>Ripeti</strong> elenco a discesa.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Ora</p> </td> 
      <td> <p>Seleziona l’ora del giorno della consegna da inviare.</p> <p>Suggerimento: Poiché i carichi di sistema possono influire sui tempi di consegna dei rapporti, potrebbe verificarsi un ritardo tra l’ora pianificata e l’ora effettiva di consegna. Se hai bisogno di un rapporto consegnato entro un momento specifico, ti consigliamo di pianificare la consegna prima del tempo necessario. Ad esempio, consigliamo di pianificare la consegna un giorno prima della data in cui è necessaria.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Si ripete il</p> </td> 
      <td> <p>Questa opzione è disponibile quando <strong>Ripeti</strong> è impostata su <strong>Settimanale</strong> o <strong>Mensile</strong>:</p> 
       <ul> 
        <li> <p>Quando il <strong>Ripeti</strong> è impostata su <strong>Settimanale</strong>: Seleziona i giorni della settimana in cui viene inviata la consegna.</p> </li> 
        <li> <p>Quando il <strong>Ripeti</strong> è impostata su <strong>Mensile</strong>: Seleziona se la consegna viene inviata il giorno del mese, del giorno della settimana o dell’ultimo giorno del mese (queste opzioni sfruttano la data selezionata nella <strong>Inizia</strong> (campo).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Inizia il</p> </td> 
      <td>Seleziona la data di inizio della consegna pianificata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Termina il</p> </td> 
      <td>Seleziona una data di fine della consegna pianificata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Mai</p> </td> 
      <td>Seleziona <strong>Mai</strong> se desideri che la consegna pianificata duri indefinitamente.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva** per salvare la consegna del report.

   Il rapporto viene visualizzato nel **Consegne ripetute** (nella sezione **Invia rapporto** (finestra di dialogo) e viene inviato all&#39;ora pianificata.

   Per informazioni sui limiti di dimensione che possono influenzare la consegna dei rapporti, consulta le sezioni [Limiti di consegna dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) e [Limiti di esportazione](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

1. (Facoltativo) Per eliminare una consegna pianificata:

   1. In **Consegne ripetute** , fai clic sulla consegna pianificata, quindi fai clic su **Elimina**.
   1. Fai clic su **Elimina** per confermare.

## Procedura dettagliata sui video

Per scoprire come pianificare la consegna di un rapporto, guarda il video seguente. Questo video è stato registrato in Workfront Classic. Tuttavia, il contenuto si applica anche alla nuova esperienza Workfront.

[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->
