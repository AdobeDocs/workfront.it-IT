---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Modificare i filtri dei rapporti in un dashboard di Canvas
description: Puoi modificare i filtri dei rapporti dopo averli applicati a un dashboard Area di lavoro.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 5205c342-7f63-438e-97c8-e74f7dfecfd0
source-git-commit: 64a71767c88362b55470e5eeffc2f41bb7482734
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 9%

---

# Modificare i filtri dei rapporti in un dashboard di Canvas

>[!IMPORTANT]
>
>La funzione Dashboard di Canvas è attualmente disponibile solo per gli utenti che partecipano alla fase beta. Alcune parti della caratteristica potrebbero non essere complete o non funzionare come previsto in questa fase. Invia un feedback relativo alla tua esperienza seguendo le istruzioni riportate nella sezione [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) dell&#39;articolo di panoramica della versione beta di Canvas Dashboards.<br>
>&#x200B;>Tieni presente che questa versione beta non è disponibile sui seguenti provider cloud:
>
>* Porta la tua chiave per Amazon Web Services
>* Azure
>* Piattaforma Google Cloud

Puoi modificare i filtri dei rapporti una volta applicati a un dashboard di Canvas per aggiornare i dati visualizzati durante l’avanzamento di un progetto.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>piano Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td> 
<p>Corrente: Piano </p> 
<p>Nuovo: Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td> 
   <td><p>Modificare l’accesso a rapporti, dashboard e calendari</p>
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td><p>Gestire le autorizzazioni per il dashboard</p>
  </td> 
  </tr>
</tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Prerequisiti

È necessario aggiungere un filtro a un report prima di modificarlo.

## Modificare un filtro per la generazione di rapporti

>[!NOTE]
>
>Sono disponibili molti strumenti di configurazione per la creazione e la modifica di un filtro per rapporti. Per ulteriori informazioni su questi strumenti, vedere la sezione seguente in questo articolo: [Considerazioni durante la modifica di un filtro per report](#considerations-when-editing-a-report-filter).


{{step1-to-dashboards}}

1. Nel pannello a sinistra, fai clic su **Dashboard Canvas**.

1. Nella pagina **Dashboard canvas**, fai clic sull&#39;icona **Altro** ![Altro](assets/more-icon.png) nell&#39;angolo superiore destro del report che contiene il filtro da modificare, quindi seleziona **Modifica**.

   ![Modifica un report](assets/edit-report-box.png)

1. Sul lato sinistro della finestra di dialogo **Configura**, selezionare il pannello **Filtri**.

1. Fare clic su **Modifica filtro**.

1. Seleziona il campo o il modificatore da modificare, quindi regola le selezioni correnti in base alle esigenze.

   ![Aggiungi condizione](assets/add-condition.png)

1. (Facoltativo) Fai clic su **Aggiungi gruppo di filtri** per aggiungere un altro set di criteri di filtro. L&#39;operatore di default tra i set è AND. Fai clic sull’operatore per modificarlo in O.

1. Fai clic su **Salva**.

## Considerazioni durante la modifica di un filtro per report

### Variabili filtro per caratteri jolly basati sulla data

Le opzioni con caratteri jolly basate sulla data possono essere utilizzate in combinazione con qualsiasi attributo del filtro data. Per informazioni sull&#39;aggiunta di un carattere jolly basato sulla data a un report, vedere l&#39;articolo [Utilizzare caratteri jolly basati sulla data per generalizzare i report](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Se crei un calcolo di data e ora che non include una porzione di ora o che utilizza i caratteri jolly $$TODAY o $$NOW, il sistema utilizza la data in base al fuso orario UTC (Coordinated Universal Time) e non al fuso orario locale. Questo può causare un risultato di data imprevisto.

Puoi scegliere uno dei seguenti caratteri jolly basati sulla data:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$OGGI</strong> </p> </td> 
   <td> <p>È consigliabile creare filtri sensibili alla data utilizzando questo carattere jolly in modo da evitare di creare nuovamente il filtro domani, la prossima settimana o il mese prossimo.</p> <p>Ad esempio, se desideri visualizzare tutte le attività con scadenza precedente a oggi, puoi utilizzare la seguente regola in un filtro attività: <em>Data inizio pianificata inferiore a $$TODAY</em>.</p> <p>$$TODAY è sempre uguale a mezzanotte per il giorno corrente.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>È simile al carattere jolly $$TODAY ma include la data e l'ora correnti. $$NOW corrisponde alla data e all'ora correnti.</p> <p>Ad esempio, se desideri visualizzare tutte le ore inserite fino all'ora corrente, puoi usare la seguente regola nel filtro ore: <em>Data inizio pianificata minore di $$NOW</em>.</p> <p>Nota: questo carattere jolly non è supportato nella pianificazione risorse.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per indicare vari periodi di tempo e vari punti nel tempo (futuri o passati), è possibile combinare i caratteri jolly riportati sopra con i seguenti:

| Attributi |   |
|---|---|
| **q** | trimestre del calendario |
| **h** | ora |
| **d** | giorno |
| **w** | settimana |
| **m** | mese |
| **a** | anno |

{style="table-layout:auto"}

| **Qualificatori** | |
|---|---|
| **b** | inizio del periodo (senza un attributo specificato, per impostazione predefinita inizia la settimana: domenica) |
| **e** | fine periodo (senza un attributo specificato, per impostazione predefinita fine settimana: sabato) |

{style="table-layout:auto"}

| **Operatori** | |
|---|---|
| **+** | aggiungi valore al valore jolly |
| **-** | sottrai valore da valore jolly |

{style="table-layout:auto"}

Ad esempio, il carattere jolly `$$TODAYb+2w` fa riferimento a &quot;2 settimane dall&#39;inizio di questa settimana&quot;. Il carattere jolly *`$$NOW+2h` fa riferimento a &quot;2 ore da ora&quot;.

### Variabili filtro con caratteri jolly dell&#39;utente connesso

* Quando si applica un filtro all&#39;attributo utente `name`, verrà visualizzata l&#39;opzione **Utente connesso**.

  ![Attributo nome utente](assets/user-name-attribute.png)

* Quando si applica un filtro a un attributo gruppo `name`, verranno visualizzate le opzioni **Gruppo predefinito personale (gruppo utenti connesso)** e **Altri gruppi personali (gruppi utenti connessi)** da utilizzare in una condizione filtro.

  ![Attributo nome gruppo](assets/group-name-attribute.png)

* Quando si applica un filtro a un attributo del team `name`, verranno visualizzate le opzioni **Il mio team predefinito (Team utente connesso)** e **Altri team personali (Team utenti connessi)** tra cui scegliere nella condizione del filtro.

  ![Attributo nome team](assets/team-name-attribute.png)


### Riferimento a oggetti figlio

Le relazioni disponibili per colonne aggiuntive, opzioni di filtro e attributi di raggruppamento sono in genere limitate agli oggetti più in alto nella gerarchia degli oggetti di Workfront oppure dispongono di una singola selezione sull&#39;oggetto dell&#39;entità di base del report. Esistono alcune eccezioni a questo, tra cui:

* Progetto > Attività
* Approvazione documento > Fasi di approvazione documento
* Fasi di approvazione documento > Partecipanti fase di approvazione documento

Quando si utilizza una delle relazioni padre-figlio elencate sopra, nella tabella viene visualizzata una riga per ogni record figlio connesso all&#39;oggetto padre.

### Operatori campo per tipo di campo

+++ Espandi per visualizzare l’elenco degli operatori di campo per tipo di campo. 

<table>
    <tr>
        <td><b>Tipo di campo</b></td>
        <td><b>Esempio</b></td>
       <td><b>Operatori</b></td>
        <td><b>Caratteri jolly</b></td>
    </tr>
    <tr>
        <td>Nome oggetto/riferimento</td>
        <td>Qualsiasi attributo di nome nativo o ricerca personalizzata</td>
              <td><ul>
        <li>Uguale</li>
        <li>Non uguale</li>
        <li>Contiene</li>
          <li>Non contiene</li>
            <li>È null</li>
              <li>Non è null</li>
        </ul></td>
        <td>Utente: nome
        <ul>
        <li>Io (utente connesso)</li>
        </ul>
        Gruppo: Nome
        <ul>
          <li>Il mio gruppo predefinito (gruppo utente connesso)</li>
            <li>I miei altri gruppi (gruppi utenti connessi)</li>
          </ul>
          Team: Nome
                  <ul>
          <li>Il mio team predefinito (team utente connesso)</li>
            <li>Altri miei team (team utente connessi)</li>
          </ul>
        </td>
    </tr>
    <tr>
        <td>Input stringa/testo </td>
                <td>Progetto: Descrizione</td>
                      <td><ul>
             <li>Uguale</li>
        <li>Non uguale</li>
        <li>Contiene</li>
          <li>Non contiene</li>
            <li>È null</li>
              <li>Non è null</li>
        </ul></td>
        <td></td>
    </tr>
    <tr>
        <td>Intero/Doppio</td>
             <td>Progetto: Lavoro Necessario
        <br>Attività: percentuale di completamento</td>
              <td><ul>
        <li>Uguale</li>
        <li>Non uguale</li>
        <li>Maggiore di</li>
          <li>Maggiore di o uguale a</li>
          <li>Minore di</li>
          <li>Minore di o uguale a</li>
            <li>È null</li>
              <li>Non è null</li>
        </ul></td>
        <td></td>
    </tr>
       <tr>
        <td> Data / Data e ora </td>
                    <td>Progetto: Data Inizio Pianificata
        <br>Hour: Data Inserimento</td>
              <td><ul>
        <li>Uguale</li>
        <li>Non uguale</li>
        </ul></td>
        <td>Attivando l'opzione <b>Imposta data relativa</b>, è possibile applicare caratteri jolly per la data relativa per rendere il report più dinamico e adattabile autonomamente in base a periodi di date comuni. 
         <ul><li>$$OGGI</li>
         <li>$$NOW</li>
         </ul>
        </td>
    </tr>
       <tr>
        <td>Booleano </td>
                  <td>Progetto: con documenti
        <br>Attività: Critica
        <br> Utente: Attivo</td>
        <td><ul>
        <li>Uguale</li>
        <li>Non uguale</li>
        </ul></td>
        <td> </td>
    </tr>
   </table>

+++
