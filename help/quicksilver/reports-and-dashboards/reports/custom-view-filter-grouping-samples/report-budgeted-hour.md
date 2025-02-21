---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Report: Ore preventivate'
description: 'Report: Ore preventivate'
author: Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 1%

---

# Report: Ore preventivate

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

Quando desideri condividere le informazioni sulle Ore preventivate con altri utenti che non hanno accesso alla Programmazione delle risorse, puoi creare un rapporto sulle Ore preventivate. Puoi quindi condividere il rapporto con loro.

>[!IMPORTANT]
>
>Le ore preventivate vengono di solito aggiornate ogni ora (raramente, può richiedere un massimo di tre ore) nel database di Adobe Workfront. L’aggiornamento del rapporto non aggiorna necessariamente le informazioni sulle ore in esso contenute. Puoi visualizzare il tempo trascorso dall’ultimo aggiornamento nell’angolo in alto a destra di ogni rapporto sulle ore preventivate. L’aggiornamento del rapporto aggiorna le informazioni in esso contenute solo quando è trascorsa più di un’ora dall’ultimo aggiornamento.
>
>![Avviso sincronizzazione ore report preventivate](assets/budgeted-hour-report-time-sync-warning-350x74.png)

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
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
    <p>Nuovo:</p>
   <ul><li><p>Collaboratore per modificare un filtro </p></li>
   <li><p>Standard per modificare un rapporto</p></li> </ul>

<p>Corrente:</p>
   <ul><li><p>Richiesta di modifica di un filtro </p></li>
   <li><p>Pianificare la modifica di un rapporto</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un rapporto sulle ore preventivate

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro o sull&#39;icona **Main Menu** ![Main Menu lines](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibile, quindi fai clic su **Reports**.

1. Fai clic su **Nuovo rapporto** > **Altro** > **Ora preventivata**.

   Al report viene applicata la visualizzazione predefinita.

1. (Facoltativo) Per semplificare la lettura del report, fare clic sul **Bud. Colonna ore**, quindi **Passa alla modalità testo**, quindi fai clic su **Modifica modalità testo**.
1. Modificare la riga `valuefield` in `valueexpreesion` e immettere l&#39;espressione di arrotondamento.

   In questo modo il numero di ore preventivate viene arrotondato al numero di decimali specificato.

   Per informazioni sull&#39;arrotondamento di un numero in Workfront, vedere l&#39;articolo [Panoramica delle espressioni di dati calcolati](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Fai clic su **Fine**.
1. (Facoltativo) Fai clic su **Aggiungi colonna** per aggiungere altre colonne.
1. (Facoltativo) Per semplificare la lettura del rapporto, si consiglia di aggiungervi un raggruppamento. Consigliamo il seguente raggruppamento:

   Fai clic sulla scheda **Raggruppamenti**, quindi effettua una o più delle seguenti operazioni:

   * Fare clic su **Aggiungi raggruppamento** e iniziare a digitare &quot;Nome progetto&quot;, quindi selezionarlo quando viene visualizzato nell&#39;elenco.
   * Fare clic su **Aggiungi raggruppamento** e iniziare a digitare &quot;Nome mansione&quot;, quindi selezionarlo quando viene visualizzato nell&#39;elenco.
   * Fai clic su **Aggiungi raggruppamento** e inizia a digitare &quot;Data di allocazione&quot;, selezionala quando viene visualizzata nell&#39;elenco, quindi seleziona l&#39;intervallo di tempo in base al quale desideri eseguire il raggruppamento dal campo **Raggruppa date per**.

1. (Facoltativo) Fai clic su **Filtri** per aggiungere filtri al report.
1. (Facoltativo) Fare clic su **Grafico** per aggiungere un grafico al report.
1. Fai clic su **Salva e Chiudi**.

## Esamina il rapporto Ore preventivate

Per impostazione predefinita, nel rapporto Ore preventivate sono disponibili le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Progetto </td> 
   <td>Questo è il nome del progetto associato all'Ora preventivata.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ruolo</p> </td> 
   <td>Questo è il nome della mansione associata all'Ora preventivata. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utente</td> 
   <td>Questo è il nome dell'utente associato all'Ora preventivata.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dat Allc.</td> 
   <td> <p>Si tratta della data di allocazione. È il primo giorno (una domenica) della settimana per il quale hai preventivato le ore.</p> <p>Suggerimento  <p>Se una settimana dura due mesi, vengono generate due righe nel rapporto: una corrispondente al primo giorno della settimana (la domenica della settimana che si trova durante il primo mese) e una seconda corrispondente al primo giorno del secondo mese (che potrebbe essere qualsiasi giorno della settimana).</p> <p>Ad esempio, se preventivi 8 ore per un utente per la settimana dal 30 giugno (domenica) al 6 luglio (sabato), le due righe mostrano la data di allocazione 30 giugno e 1 luglio.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ore Bdg</td> 
   <td>Queste sono le ore preventivate assegnate all'utente nella Programmazione delle risorse.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pian Ore Bdg</td> 
   <td>Si tratta delle ore preventivate allocate alla mansione o al progetto nella pianificazione risorse.</td> 
  </tr> 
 </tbody> 
</table>
