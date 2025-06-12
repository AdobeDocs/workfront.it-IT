---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Filtrare i rapporti per intervalli temporali
description: È possibile filtrare un report in base all'intervallo temporale di una data esistente su un oggetto. Ad esempio, puoi filtrare un report delle ore per un particolare arco temporale di quando sono state inserite le ore.
author: Courtney
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 5%

---

# Filtrare i rapporti per intervalli temporali

<!-- Audited: 4/2025 -->

È possibile filtrare un report in base all&#39;intervallo temporale di una data esistente su un oggetto. Ad esempio, puoi filtrare un report delle ore per un particolare arco temporale di quando sono state inserite le ore.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
      <td> 
      <p>Nuovo: Standard</p>
       <p> Oppure</p>
      <p>Corrente: Piano</p>
   </td>

</tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

È necessario creare il report prima di filtrarne i risultati.

Per ulteriori informazioni sulla creazione di report, vedere [Creare un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Filtrare un rapporto in base all’arco temporale di una data {#filter-a-report-by-the-timeframe-of-a-date}

{{step1-to-reports}}

1. Nell&#39;angolo in alto a sinistra, fai clic su **Nuovo report**, quindi seleziona il tipo di report che desideri creare.

1. Nella pagina **Nuovo report** selezionare la scheda **Filtri**.

1. Fai clic su **Aggiungi regola filtro**, quindi su **Seleziona un campo**.

1. Nella finestra di dialogo **Seleziona un campo**, seleziona **Ora**, quindi **Data di ingresso**.
   ![Filtraggio del report delle ore per intervallo temporale](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. Nell’elenco a discesa visualizzato, seleziona una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Equal</td> 
      <td>Dopo aver selezionato questo modificatore, specifica la data in cui sono state inserite le ore.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Not Equal</td> 
      <td>Dopo aver selezionato questo modificatore, specifica la data in cui sono state inserite le ore per escludere questa data dal rapporto. Il rapporto mostra le ore registrate in tutte le date, in base alla data specificata.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Minore di</td> 
      <td>Dopo aver selezionato questo modificatore, specifica una data prima della quale sono state inserite le ore. Il rapporto mostra le ore inserite prima della data specificata, esclusa la data specificata.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Less Than Equal</td> 
      <td>Dopo aver selezionato questo modificatore, specifica una data prima della quale sono state inserite le ore. Il rapporto mostra le ore inserite prima della data specificata, inclusa la data specificata.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Maggiore di</td> 
      <td>Dopo aver selezionato questo modificatore, specifica una data dopo la quale sono state inserite le ore. Il rapporto mostra le ore inserite dopo la data specificata, esclusa la data specificata.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Greater Than Equal</td> 
      <td> Dopo aver selezionato questo modificatore, specifica una data dopo la quale sono state inserite le ore. Il rapporto mostra le ore inserite dopo la data specificata, inclusa la data specificata. </td> 
     </tr>

   <tr> 
      <td role="rowheader">Tra</td> 
      <td>Dopo aver selezionato questo modificatore, specifica un intervallo di date in cui sono state immesse le ore. Il rapporto mostra le ore inserite tra le date specificate.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Nullo</td> 
      <td>Selezionare questo modificatore per visualizzare solo le ore in cui manca la data di immissione.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Non nullo</td> 
      <td>Selezionare questo modificatore per visualizzare solo le ore per le quali la data di immissione ha un valore.</td> 
     </tr>

   </tbody> 
   </table>

1. Fai clic su **Salva e Chiudi**.

## Modificatori di intervallo temporale incorporati {#built-in-timeframe-modifiers}

Adobe Workfront dispone di modificatori di intervallo temporale incorporati che è possibile utilizzare senza definire una data specifica. Questi modificatori sono disponibili per qualsiasi campo data in un filtro o in un prompt in qualsiasi rapporto.

Ad esempio, se desideri visualizzare le ore inserite in un determinato arco temporale durante la creazione di un rapporto orario, puoi scegliere tra le seguenti opzioni di filtro integrate:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Oggi</td> 
   <td>Visualizza le ore in cui la data di immissione è oggi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Questa settimana</td> 
   <td>Visualizza le ore in cui la Data immissione è una data della settimana corrente, in cui la settimana inizia di domenica e termina di sabato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Settimana Prossima</td> 
   <td>Visualizza le ore in cui la Data immissione è una data della settimana successiva alla settimana corrente, in cui la settimana inizia di domenica e termina di sabato. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Settimana scorsa</td> 
   <td>Visualizza le ore in cui la Data immissione è una data della settimana precedente alla settimana corrente, in cui la settimana inizia di domenica e termina di sabato. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Questo mese</td> 
   <td>Visualizza le ore in cui la Data immissione è una data del mese corrente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mese Prossimo</td> 
   <td>Visualizza le ore in cui la Data immissione è una data nel mese successivo al mese corrente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mese scorso</td> 
   <td>Visualizza le ore in cui la Data immissione è una data nel mese precedente il mese corrente</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Questo TriMestre</td> 
   <td> <p>Visualizza le ore in cui Data inserimento è una data del trimestre corrente, in cui i trimestri sono definiti come:</p> 
    <ul> 
     <li>Primo Trimestre: 1° gennaio - 30 marzo</li> 
     <li>Secondo Trimestre: 1 Aprile - 30 Giugno</li> 
     <li>Terzo Trimestre: 1 Luglio - 30 Settembre</li> 
     <li>Quarto Trimestre: 1 ottobre - 31 dicembre</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prossimo TriMestre</td> 
   <td>Visualizza le ore in cui la Data inserimento è una data nel trimestre successivo al trimestre corrente, in cui i trimestri sono definiti in precedenza.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ultimo TriMestre</td> 
   <td> <p>Visualizza le ore in cui la Data inserimento è una data nel trimestre precedente il trimestre corrente, in cui i trimestri sono definiti in precedenza.</p> <p>Nota: se l'amministratore di Workfront ha abilitato e definito i trimestri personalizzati per il sistema, i filtri incorporati per i trimestri vengono sostituiti con le informazioni personalizzate relative al trimestre. Per ulteriori informazioni sull'abilitazione dei trimestri personalizzati, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Abilitare i trimestri personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quest'anno</td> 
   <td>Visualizza le ore in cui Data immissione è una data dell'anno corrente, in cui l'anno corrente inizia il 1 gennaio e termina il 31 dicembre.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ultimo anno</td> 
   <td>Visualizza le ore in cui la Data immissione è una data dell'anno precedente, in cui l'anno precedente inizia 12 mesi prima della data corrente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Anno scorso</td> 
   <td> <p>Visualizza le ore in cui Data immissione è una data dell'ultimo anno, in cui l'ultimo anno inizia il 1 gennaio e termina il 31 dicembre dell'anno precedente l'anno corrente.</p> <p>Nota: non esiste un periodo di tempo predefinito per l'anno fiscale. È possibile creare un rapporto e filtrare le informazioni per data utilizzando un modificatore personalizzato per l'intervallo di date dell'anno fiscale, come definito nell'organizzazione. Se desideri scegliere un periodo temporale per un anno fiscale sul posto, utilizza un prompt invece di un filtro. </p> </td> 
  </tr> 
 </tbody> 
</table>
