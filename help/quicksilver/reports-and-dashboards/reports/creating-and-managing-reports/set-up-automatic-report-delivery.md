---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Pianificare la consegna automatica dei rapporti
description: Pianificare la consegna automatica dei rapporti
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1197'
ht-degree: 2%

---

# Pianificare la consegna automatica dei rapporti

<!-- Audited: 11/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

Puoi pianificare i rapporti in modo che vengano consegnati automaticamente agli utenti in base a una pianificazione definita, oppure puoi inviare manualmente i rapporti in una sola volta. Quando invii un rapporto da Adobe Workfront, l’utente riceve un’e-mail con il rapporto Workfront in un allegato separato.

Per ulteriori informazioni, inclusi i limiti di dimensione che possono influenzare la consegna dei report, vedi [Panoramica sulla consegna dei report](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
      <td> 
      <p>Nuovo:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Corrente:</p>
         <ul>
         <li><p>Piano</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p></td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare, è necessario creare un rapporto. Per ulteriori informazioni sulla creazione di report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Pianificare la consegna di un rapporto

Per pianificare la consegna automatica di un report o per modificare o eliminare una consegna di report esistente:&#x200B;

1. Vai a un rapporto che desideri pianificare per la consegna.

   >[!NOTE]
   >
   >Le consegne dei rapporti non contengono prompt. Se desideri limitare i dati in una consegna di rapporti, ti consigliamo di applicare filtri al rapporto che desideri inviare.

1. Fai clic su **Azioni report**, quindi su **Invia report**.

   Viene visualizzata la finestra di dialogo **Invia report**.

   >[!TIP]
   >
   >Per inviare un report manualmente in un determinato momento, passa al report, quindi fai clic su **Azioni report** > **Invia report** > **Invia ora**.

1. Selezionare la scheda **Consegne ripetute**.
1. (Condizionale) Per modificare una consegna report ripetuta esistente, seleziona la consegna report nella sezione **Consegne ripetute**.
1. Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Invia a</p> </td> 
      <td> <p>Inizia a digitare il nome dell’utente, del gruppo, del team o del ruolo a cui inviare il rapporto, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.</p> <p>Oppure</p> <p>Specifica l’indirizzo e-mail di una persona esterna al sistema Workfront a cui desideri avere accesso al rapporto.</p> <p>Ripeti questa procedura per inviare il rapporto a più utenti, gruppi, team o ruoli.</p> <p>Nota:  <p>Quando aggiungi destinatari di consegna del rapporto, tieni presente quanto segue:</p> 
        <ul> 
         <li>Se la tua organizzazione limita le notifiche di Workfront a specifici domini e-mail, potresti essere in grado di inviare rapporti solo agli indirizzi e-mail elencati nel inserisco nell'elenco Consentiti di e-mail per l’invio di messaggi e-mail a un altro utente.<p>Per informazioni sul modo in cui un amministratore di Workfront aggiorna il inserisco nell'elenco Consentiti di e-mail, consulta la sezione <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Configurare il tuo inserisco nell'elenco Consentiti di e-mail di</a>.</p></li> 
         <li> <p>L’aggiunta di un numero elevato di utenti come destinatari può causare un errore di consegna. In caso di errori di consegna, puoi pianificare più consegne di rapporti con gruppi di utenti più piccoli.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Oggetto e-mail</p> </td> 
      <td> <p>Specifica un oggetto per la notifica e-mail.</p> <p>Per impostazione predefinita, l’oggetto dell’e-mail è:</p> <p><em>Rapporto Workfront: [Nome del rapporto] [Data]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Messaggio e-mail</p> </td> 
      <td> <p>Specifica un messaggio da includere nell’e-mail.</p> <p>Per impostazione predefinita, il messaggio e-mail è:</p> <p><em>In allegato è riportato il report [Nome del report] generato da Workfront il [Data].</em> </p> <p>Nota: per i rapporti consegnati solo come file Excel, viene aggiunto anche il seguente messaggio all’e-mail: "Tieni presente che con i tipi di file MS Excel (XLS), esiste un limite (65.530) sul numero di collegamenti ipertestuali supportati da questi tipi di file. Se tali limiti vengono superati, il file non verrà aperto e si consiglia di inviarlo di nuovo senza i collegamenti ipertestuali. Torna alla pianificazione del report per rimuovere i collegamenti ipertestuali e inviare nuovamente il report." La frase "torna alla pianificazione dei rapporti" è un collegamento per tornare al rapporto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Consegna il report con i diritti di accesso di</p> </td> 
      <td> <p>Inizia a digitare il nome di un utente che ha accesso al report, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa. Agli utenti che ricevono il report verrà concesso lo stesso livello di accesso al report dell'utente qui specificato.<br> Per ulteriori informazioni, vedere <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Eseguire e recapitare un report con i diritti di accesso di un altro utente</a>.</p> <p>Nota: questo campo non supporta i caratteri jolly. Ad esempio, l’utilizzo del carattere jolly $$User.ID non esegue il report con i diritti di accesso dell’utente che riceve il report.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Formato</p> </td> 
      <td> <p>Selezionare il formato desiderato per il rapporto consegnato:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Se selezioni questa opzione, puoi formattare l'output utilizzando le opzioni aggiuntive <strong>Dimensioni carta</strong> e <strong>Orientamento</strong> visualizzate.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Includi i link</p> </td> 
      <td> <p>Questa opzione è disponibile solo quando è selezionato <strong>MS Excel</strong> nel menu a discesa <strong>Formato</strong>. Quando questa opzione è attivata, tutti i collegamenti ipertestuali vengono inclusi nel documento di Excel esportato.</p> <p>Non è possibile aprire i documenti che contengono più di 65.530 collegamenti. Se il documento esportato contiene più di 65.530 collegamenti, deselezionare questa opzione.</p> <p>Questa opzione è attivata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Riepilogo</p> </td> 
      <td> <p>Visualizza un riepilogo di quando la consegna si ripete.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Si ripete</p> </td> 
      <td> <p>Seleziona se il rapporto deve essere consegnato giornalmente, settimanalmente, mensilmente o annualmente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Si ripete ogni</p> </td> 
      <td> <p>Seleziona la frequenza con cui desideri ripetere la consegna. Il valore selezionato per questa opzione si basa sull'opzione selezionata nell'elenco a discesa <strong>Ripeti</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Ora</p> </td> 
      <td> <p>Seleziona l’ora del giorno per la consegna da inviare.</p> <p>Suggerimento: poiché i carichi di sistema possono influire sui tempi di consegna dei rapporti, potrebbe verificarsi un ritardo di 24 ore tra l’ora pianificata e l’ora di consegna effettiva. Se hai bisogno di un rapporto consegnato entro un orario specifico, ti consigliamo di pianificarlo prima del momento in cui è necessario. In generale, consigliamo di pianificare la consegna almeno un giorno prima della data in cui è necessaria.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Si ripete il</p> </td> 
      <td> <p>Questa opzione è disponibile quando l'opzione <strong>Ripeti</strong> è impostata su <strong>Settimanale</strong> o <strong>Mensile</strong>:</p> 
       <ul> 
        <li> <p>Quando l'opzione <strong>Repeats</strong> è impostata su <strong>Weekly</strong>: selezionare i giorni della settimana in cui viene inviata la consegna.</p> </li> 
        <li> <p>Quando l'opzione <strong>Ripeti</strong> è impostata su <strong>Mensile</strong>: selezionare se la consegna viene inviata il giorno del mese, del giorno della settimana o dell'ultimo giorno del mese (queste opzioni sfruttano la data selezionata nel campo <strong>Inizia il</strong>).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Inizia il</p> </td> 
      <td>Seleziona la data di inizio della consegna pianificata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Termina il</p> </td> 
      <td>Seleziona una data di fine per la consegna programmata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Mai</p> </td> 
      <td>Seleziona <strong>Mai</strong> se desideri che la consegna pianificata duri a tempo indefinito.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva** per salvare la consegna del report.

   Il report viene visualizzato nella sezione **Consegne ripetute** (nella finestra di dialogo **Invia report**) e verrà inviato all&#39;ora pianificata.

   Per informazioni sui limiti di dimensione che possono influenzare la consegna dei report, vedi le sezioni [Limiti di consegna dei report](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) e [Limiti di esportazione](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

>[!IMPORTANT]
>
>I rapporti pianificati sono soggetti a un limite di tempo interno durante l’elaborazione per la consegna. Nel caso in cui un rapporto richieda più tempo del limite da inviare, riceverai una notifica e non verrà più consegnato, indipendentemente dalle consegne pianificate rimanenti. Per continuare a inviare il rapporto, prova innanzitutto a ridurne le dimensioni tramite filtri e visualizzazioni, quindi crea una nuova consegna pianificata.
>
>Se utilizzi una consegna di rapporti pianificata per analizzare i dati di Workfront tramite uno strumento di business intelligence, ti consigliamo invece di utilizzare Workfront Data Connect. Per ulteriori informazioni, vedere [Panoramica di Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

1. (Facoltativo) Per eliminare una consegna programmata:

   1. Nel pannello **Consegne ripetute**, fai clic sulla consegna pianificata, quindi su **Elimina**.
   1. Fai clic su **Elimina** per confermare.

<!--## Video walk-through

View the following video to learn how to schedule a report delivery. This video was recorded in Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![Video walkthrough of report delivery](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)


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
