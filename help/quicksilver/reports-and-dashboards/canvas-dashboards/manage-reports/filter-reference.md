---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Riferimento filtro rapporto per dashboard Canvas
description: Riferimento per campi, operatori, caratteri jolly e regole speciali che è possibile utilizzare quando si filtra un report in un dashboard di Canvas.
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 85ae49708acf2c472816ac848ce15429577b934e
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 40%
---
# Riferimento filtro rapporto per dashboard Canvas

>[!IMPORTANT]
>
>La funzione Dashboard di Canvas è attualmente disponibile solo per gli utenti che partecipano alla fase beta. Alcune parti della caratteristica potrebbero non essere complete o non funzionare come previsto in questa fase. Invia un feedback relativo alla tua esperienza seguendo le istruzioni riportate nella sezione [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) dell&#39;articolo di panoramica di Canvas Dashboards beta.<br>
>In caso di feedback su un possibile bug o problema tecnico, invia un ticket al supporto Workfront. Per ulteriori informazioni, consulta [Contattare l’Assistenza clienti](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Tieni presente che questa versione beta non è disponibile sui seguenti provider cloud:
>
>* Porta la tua chiave per Amazon Web Services
>* Azure
>* Piattaforma Google Cloud

In questo articolo vengono descritti i campi, gli operatori, i caratteri jolly e le regole speciali disponibili quando si filtra un report. Per i passaggi necessari per generare o modificare un filtro, vedere [Filtrare un report in un dashboard Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-a-report.md).

## Operatori campo per tipo di campo

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
         <ul><li>$$TODAY</li>
         <li>$$NOW</li>
         </ul>
        </td>
    </tr>
       <tr>
        <td>Booleano </td>
                  <td>Progetto: con documenti
        <br>Attività: Critica
        Utente <br>: Attivo</td>
        <td><ul>
        <li>Uguale</li>
        <li>Non uguale</li>
        </ul></td>
        <td> </td>
    </tr>
   </table>

+++

## Variabili filtro con caratteri jolly basati sulla data

Le opzioni con caratteri jolly basati sulla data possono essere utilizzate in combinazione con qualsiasi attributo del filtro data. Per informazioni sull&#39;aggiunta di un carattere jolly basato sulla data a un report, vedere [Utilizzare caratteri jolly basati sulla data per generalizzare i report](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Se crei un calcolo di data e ora che non include una parte oraria o che utilizza i caratteri jolly $$TODAY o $$NOW, il sistema utilizza la data in base al fuso orario UTC (Tempo coordinato universale) e non al fuso orario locale. Questo può causare un risultato di data imprevisto.

Puoi scegliere uno dei seguenti caratteri jolly basati sulla data:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$TODAY</strong> </p> </td> 
   <td> <p>È consigliabile creare filtri basati sulle date per utilizzare questo carattere jolly in modo da evitare di creare nuovamente il filtro domani, la prossima settimana o il mese prossimo.</p> <p>Ad esempio, se desideri visualizzare tutte le attività con scadenza precedente a oggi, puoi utilizzare la seguente regola in un filtro attività: <em>Data di inizio pianificata precedente a $$TODAY</em>.</p> <p>$$TODAY è sempre uguale a mezzanotte per il giorno corrente.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>È simile al carattere jolly $$TODAY ma include la data e l’ora correnti. $$NOW corrisponde alla data e all’ora correnti.</p> <p>Ad esempio, se desideri visualizzare tutte le ore inserite fino all’ora corrente, puoi utilizzare la seguente regola in un filtro ore: <em>Data di inizio pianificata precedente a $$NOW</em>.</p> <p>Nota: questo carattere jolly non è supportato nella pianificazione risorse.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per indicare vari periodi di tempo e vari punti nel tempo (futuri o passati), puoi combinare i caratteri jolly indicati in precedenza con i seguenti:

| Attributi |   |
|---|---|
| **q** | trimestre del calendario |
| **h** | ora |
| **d** | giorno |
| **w** | settimana |
| **m** | mese |
| **y** | anno |

{style="table-layout:auto"}

| **Qualificatori** |   |
|---|---|
| **b** | inizio del periodo (senza un attributo specificato, il valore predefinito è impostato all’inizio della settimana: domenica) |
| **e** | fine del periodo (senza un attributo specificato, il valore predefinito è impostato alla fine della settimana: sabato) |

{style="table-layout:auto"}

| **Operatori** |   |
|---|---|
| **+** | aggiungi valore al valore carattere jolly |
| **-** | sottrai valore dal valore carattere jolly |

{style="table-layout:auto"}

Ad esempio, il carattere jolly `$$TODAYb+2w` fa riferimento a “2 settimane dall’inizio di questa settimana”. Il carattere jolly `$$NOW+2h` si riferisce a &quot;2 ore da ora&quot;.

## Variabili filtro con caratteri jolly dell&#39;utente connesso

* Quando si applica un filtro all&#39;attributo utente `name`, verrà visualizzata l&#39;opzione **Utente connesso**.

  ![Attributo nome utente](assets/user-name-attribute.png)

* Quando si applica un filtro a un attributo gruppo `name`, verranno visualizzate le opzioni **Gruppo predefinito personale (gruppo utenti connesso)** e **Altri gruppi personali (gruppi utenti connessi)** da utilizzare in una condizione filtro.

  ![Attributo nome gruppo](assets/group-name-attribute.png)

* Quando si applica un filtro a un attributo del team `name`, verranno visualizzate le opzioni **Il mio team predefinito (Team utente connesso)** e **Altri team personali (Team utenti connessi)** tra cui scegliere nella condizione del filtro.

  ![Attributo nome team](assets/team-name-attribute.png)

## Riferimento a oggetti figlio

Le relazioni disponibili per colonne aggiuntive, opzioni di filtro e attributi di raggruppamento sono in genere limitate agli oggetti più in alto nella gerarchia degli oggetti di Workfront oppure dispongono di una singola selezione sull&#39;oggetto dell&#39;entità di base del report. Esistono alcune eccezioni a questo, tra cui:

* Progetto > Attività
* Approvazione documento > Fasi di approvazione documento
* Fasi di approvazione documento > Partecipanti fase di approvazione documento

Quando si utilizza una delle relazioni padre-figlio elencate sopra, nella tabella viene visualizzata una riga per ogni record figlio connesso all&#39;oggetto padre.

<!--
<div class="preview">

## Filter on collection relationships in Preview

A collection is a field that links to a group of related records rather than to a single record. For example, the participants on a project's approval stages are a collection. When you build a filter, you can filter on collections directly, without switching to text mode.

To filter on a collection, open the Select a field panel, then select Collections. This section lists only collection relationships. Single-record relationships stay under Relationships.

![collection relationships](assets/collections.png)

After you select a collection, you can do two things:

* Filter on the collection's own fields. For example, from a portfolio's projects, you can filter on a project's status.
* Follow one single-record relationship out of the collection. For example, from a portfolio's projects, you can reach the project owner.

Collections don't support deeper navigation. You can't open a collection nested inside another collection, follow more than one relationship, or select the relationship that leads back to where you started.

The Collections section appears only when you build a filter. It doesn't appear in other field choosers, such as those for table columns, groupings, or chart fields.

</div>

-->

## Escludi progetti personali, attività e utenti bot

>[!NOTE]
>
>Se un rapporto di Dashboard Canvas restituisce più risultati di quanto previsto rispetto a un rapporto classico simile, per impostazione predefinita possono essere inclusi progetti personali, attività personali o utenti bot. Aggiungi una condizione di filtro per escluderli.

Nei report Progetto e Attività delle dashboard di Canvas, il filtro `isPersonal` non viene applicato automaticamente, pertanto i progetti personali e le attività personali vengono inclusi nei risultati per impostazione predefinita. Per escluderli, aggiungere una condizione di filtro come `isPersonal=false`.

Analogamente, i rapporti utente delle dashboard di Canvas includono tutti gli utenti per impostazione predefinita, inclusi i collaboratori IA (utenti bot). Per escludere gli utenti bot, aggiungere una condizione di filtro come `isBot=false`.

I report classici per progetti e attività escludono automaticamente i progetti personali e le attività personali, mentre i report classici per utenti escludono automaticamente gli utenti bot. Per includerli in un report classico, aggiungere una condizione di filtro come `isPersonal=true` (solo elementi personali) o `isPersonal_Mod=notnull` (elementi personali e non personali).
