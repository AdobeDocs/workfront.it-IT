---
product-area: home
navigation-topic: new-home
title: Panoramica dei filtri dei widget Home
description: È possibile scegliere tra diversi widget per personalizzare il contenuto visualizzato nella home page. Questi widget possono essere ridimensionati e disposti nella home page.
author: Courtney
feature: Get Started with Workfront
exl-id: 58f79e81-df6b-456f-9e91-4e00a1c2a8a2
source-git-commit: 884ade1102e685ec01af2790b17acb50c2114ca7
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 11%

---

# Panoramica dei filtri dei widget Home

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedi [Abilitare o disabilitare le versioni rapide per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

Per trovare e organizzare il lavoro, potete utilizzare i filtri dei seguenti widget:

* [I miei progetti](#my-projects)
* [Le mie attività](#my-tasks)
* [I miei problemi](#my-issues)
* [Le mie richieste](#my-requests)
* [Il mio lavoro](#my-work)
* [Le mie approvazioni](#my-approvals)

>[!IMPORTANT]
>
>* Per visualizzare le attività e i problemi nei widget Home, il progetto principale deve essere nello stato Corrente o in uno stato equivalente a Corrente.
>* I progetti devono anche essere nello stato Corrente o uno stato che equivalga allo stato corrente da visualizzare.

## I miei progetti

Potete usare i seguenti filtri nel widget Progetti personali:

<table>
  <tr>
    <td>Attivo</td>
    <td>Visualizza i progetti con i seguenti stati: Attuale, Pianificato e Approvato </td>
  </tr>
  <tr>
    <td>A Rischio</td>
    <td>Visualizza i progetti in Stato A rischio </td>
  </tr>
  <tr>
    <td>Progetti in ritardo rispetto alla pianificazione</td>
    <td>Visualizza i progetti nello stato Indietro</td>
  </tr>
  <tr>
    <td>Attuali</td>
    <td>Visualizza i progetti nello stato Corrente </td>
  </tr>
  <tr>
    <td>Scadenze del Mese</td>
    <td>Visualizza i progetti con date di completamento pianificate che rientrano nel mese di calendario corrente</td>
  </tr>
  <tr>
    <td>In Ritardo</td>
    <td>Visualizza i progetti in stato di ritardo</td>
  </tr>
  <tr>
    <td>I miei progetti</td>
    <td>Visualizza i progetti assegnati a me o al mio team di progetto nello stato Corrente</td>
  </tr>
  <tr>
    <td>Nei Tempi</td>
    <td>Visualizza i progetti nello stato On Time</td>
  </tr>
  <tr>
    <td>Budget Sovra Costo</td>
    <td>Visualizza i progetti in cui il valore del costo effettivo è maggiore del valore del costo pianificato</td>
  </tr>
  <tr>
    <td>Oltre il Budget di Lavoro</td>
    <td>Visualizza i progetti in cui il valore Lavoro richiesto effettivo è maggiore del valore Lavoro richiesto</td>
  </tr>
  <tr>
    <td>Solo code</td>
    <td>Visualizza i progetti designati come code di richieste</td>
  </tr>
  <tr>
    <td>Richiesto il</td>
    <td>Visualizza i progetti nello stato Richiesto</td>
  </tr>
  <tr>
    <td>Progetti Pianificazione scenario</td>
    <td>Visualizza i progetti con un ID iniziativa impostato tramite Scenario Planner</td>
  </tr>
</table>

## Le mie attività

Potete usare i seguenti filtri nel widget Attività personali:

<table>
  <tr>
    <td>Attività attive</td>
    <td><p>Visualizza le attività senza data di handoff o data di handoff odierna o precedente e</p>
<ul>
  <li>Percentuale di completamento inferiore al 100%</li>
  <li>Il valore Can Start è impostato su True</li>
</ul>
</td>
  </tr>
   <!-- <tr>
    <td>All Unassigned Tasks</td>
    <td></td>
  </tr> -->
  <tr>
    <td>Attività approvabili</td>
    <td>Visualizza le attività nello stato In attesa di approvazione</td>
  </tr>
  <tr>
    <td>Può iniziare</td>
    <td><p>Visualizza le attività assegnate a me che</p>
<ul>
  <li>Non si trovano in uno stato uguale a completato</li>
  <li>Avere un valore Can Start che è true</li>
</ul>
</td>
  </tr>
  <tr>
    <td>Percorso critico</td>
    <td>Visualizza le attività designate come critiche</td>
  </tr>
  <tr>
    <td>Attività non completate</td>
    <td>Visualizza le attività con gli stati impostati su un valore diverso da Completato</td>
  </tr>
  <tr>
    <td>Attività Milestone</td>
    <td>Visualizza le attività associate a un'attività cardine. Per ulteriori informazioni, vedere <a href="/help/quicksilver/manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Associa attività cardine alle attività</a>.
</td>
  </tr>
  <tr>
    <td>Attività dei miei progetti</td>
    <td>Visualizza le attività nello stato Corrente in cui sono membro del team di progetto </td>
  </tr>
    <tr>
    <td>Le mie attività</td>
    <td>Visualizza le attività assegnate a me</td>
  </tr>
  <tr>
    <td>Non assegnato a un'iterazione</td>
    <td>Visualizza le attività non assegnate a un'iterazione</td>
  </tr>
  <tr>
    <td>Interessante di recente</td>
    <td><p>Visualizza le attività in cui si è verificato l'ultimo aggiornamento nelle ultime due settimane e</p>
<ul>
  <li>La data di conferma è successiva alla data di completamento pianificata</li>
  oppure
  <li>La durata del progetto è maggiore della durata pianificata</li>
  oppure
  <li>La condizione sta andando liscia o qualche preoccupazione</li>
  oppure
  <li>L'assegnatario dell'attività principale ha iniziato a lavorare sull'attività</li>
</ul>
</td>
  </tr>
  <tr>
    <td>Le Attività non assegnate nel Mio Ruolo</td>
    <td><p>Visualizza le attività che sono</p>
<ul>
  <li>Assegnato al mio Ruolo</li>
  <li>Incompleto</li>
</ul>
</td>
  </tr>
  <tr>
    <td>Le prossime attività</td>
    <td><p>Visualizza le attività che</p>
<ul>
  <li>Sono incompleti</li>
  <li>Appartenere a un progetto nello stato Attuale</li>
  <li>Hanno una data di inizio pianificata entro due settimane dalla data di oggi</li>
</ul>
</td>
  </tr>
</table>

## I miei problemi

Puoi utilizzare i seguenti filtri nel widget Problemi personali:

<table>
<tr>
    <td>Tutte non assegnate</td>
    <td>Visualizza tutti i problemi non assegnati e a cui non è associato un oggetto di risoluzione </td>
  </tr>
  <tr>
    <td>Assegnato a me</td>
    <td>Visualizza i problemi in cui l'assegnatario principale è io</td>
  </tr>
  <tr>
    <td>Completato</td>
    <td>Visualizza problemi con date di completamento </td>
  </tr>
  <tr>
    <td>Inserito da me</td>
    <td>Visualizza le Issues che ho inserito</td>
  </tr>
  <tr>
    <td>Problemi dei miei progetti</td>
    <td><p>Visualizza i problemi in cui</p>
<ul>
  <li>Sono l’assegnatario principale</li>
  <li>Stato incompleto</li>
  <li>Nessun oggetto di risoluzione associato</li>
</ul>
</td>
  </tr>
    <tr>
    <td>Problemi inviati recentemente da me</td>
    <td><p>Visualizza i problemi che</p>
<ul>
  <li>Ho inviato</li>
  <li>Nessun oggetto di risoluzione associato</li>
  <li>Lo stato non è Completato e non è presente alcuna Data di completamento</li>
  <li>Sono stati inviati entro tre mesi dalla data odierna</li>
</ul>
</td>
  </tr>
    </tr>
    <tr>
    <td>Problemi inviati</td>
    <td>Visualizza i problemi di mia proprietà</td>
  </tr>
  <tr>
    <td>Open</td>
    <td>Visualizza i problemi che non hanno una data di completamento</td>
  </tr>
  <tr>
    <td>Risolvibili</td>
    <td>Visualizza i problemi a cui sono allegati oggetti di risoluzione</td>
  </tr>
  <tr>
    <td>Non assegnate al mio ruolo</td>
    <td>Visualizza tutti i problemi a cui non è stato assegnato un utente principale ma a cui è stato assegnato un ruolo </td>
  </tr>
</table>

## Le mie richieste

Nell’ambiente di produzione:

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tutto</td> 
      <td>Visualizza tutte le richieste inviate, indipendentemente dallo stato o da chi le ha inviate.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Open</td> 
      <td> <p>Visualizza tutte le richieste inviate 
      <ul>
      <li>Attualmente aperte, indipendentemente da chi le ha inviate. Solo le richieste per le quali disponi almeno delle autorizzazioni di visualizzazione vengono visualizzate qui se non le hai inviate personalmente.</li>
      <li>Senza una data di completamento effettiva o per i quali l'oggetto di risoluzione non dispone di una data di completamento effettiva è disponibile l'elenco nella scheda secondaria Apri.</li> 
      </ul>
      <p><b>NOTA</b> 
      Le richieste con uno stato diverso da Chiuso vengono considerate aperte.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le mie richieste</td> 
      <td>Visualizza le richieste inviate indipendentemente dal loro stato. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le mie richieste aperte</td> 
      <td> <p>Visualizza le richieste 
      <ul>
      <li>Che hai inviato e che sei ancora aperto. </li> 
      <li>Senza una data di completamento effettiva o per i quali l'oggetto di risoluzione non dispone di una data di completamento effettiva è disponibile la scheda secondaria Richieste personali aperte. </li> 
      </ul>
      <p><b>NOTA</b> 
      Le richieste che non si trovano in uno stato che equivale a Chiuso vengono considerate aperte.</p> </td> 
     </tr> 
    </tbody> 
   </table>

<div class="preview">

Nell’ambiente di anteprima:

Il widget Richieste personali dispone di un filtro personalizzabile che consente di controllare quali richieste vengono visualizzate nel widget. Puoi configurare questo filtro per campi e valori diversi e sovrapporre le condizioni utilizzando gli operatori AND e OR.

Per istruzioni sulla configurazione del filtro nel widget Richieste personali, vedere [Filtrare le richieste](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md#filter-requests) nell&#39;articolo Utilizzare il widget Richieste personali.

</div>

## Il mio lavoro

È possibile utilizzare i seguenti filtri nel widget Il mio lavoro:

<table>
  <tbody>
    <tr>
      <td>Lavori</td>
      <td>Visualizza gli elementi su cui si sta lavorando</td>
    </tr>
    <tr>
      <td>È il momento di iniziare?</td>
      <td>Visualizza gli elementi con 
      <ul>
      <li>Nessun predecessore o vincolo di attività incompleto</li>
      <li>La data di inizio pianificata è nel passato o è prevista entro due settimane</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>Non pronto</td>
      <td>Visualizza gli elementi con
       <ul>
      <li>Predecessori incompleti o vincoli di attività che impediscono la lavorazione dell'elemento</li>
      oppure
      <li>La data di inizio pianificata nel futuro è tra più di due settimane</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>Richiesto il</td>
      <td>Visualizza i problemi per i quali non hai iniziato a lavorare</td>
    </tr>
    <tr>
      <td>Delegata da me</td>
      <td>Visualizza gli elementi delegati ad altri utenti</td>
    </tr>
    <tr>
      <td>Delegata a me</td>
      <td>Visualizza gli elementi che gli utenti ti hanno delegato</td>
    </tr>
    <tr>
      <td>Completato</td>
      <td>Visualizza il lavoro completato nelle ultime due settimane. Questa opzione di filtro non include le approvazioni.</td>
    </tr>
  </tbody>
</table>

## Le mie approvazioni

Potete usare i seguenti filtri nel widget Approvazioni personali:

<table>
  <tbody>
    <tr>
      <td>Approvazioni delegate</td>
      <td>Visualizza le approvazioni delegate all'utente</td>
    </tr>
    <tr>
      <td>Le mie approvazioni</td>
      <td>Visualizza gli elementi che richiedono la tua approvazione
      </td>
    </tr>
    <tr>
      <td>Approvazioni che ho inviato</td>
      <td>Visualizza gli elementi inviati per l'approvazione
       </td>
    </tr>
  </tbody>
</table>
