---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Rapporto: Ore preventivate"
description: "Rapporto: Ore preventivate"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 1%

---

# Report: Ore preventivate

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

Quando desideri condividere le informazioni sulle Ore preventivate con altri utenti che non hanno accesso alla Programmazione delle risorse, puoi creare un rapporto sulle Ore preventivate. Puoi quindi condividere il rapporto con loro.

>[!IMPORTANT]
>
>Le ore preventivate vengono di solito aggiornate ogni ora (raramente, può richiedere un massimo di tre ore) nel database di Adobe Workfront. L’aggiornamento del rapporto non aggiorna necessariamente le informazioni sulle ore in esso contenute. Puoi visualizzare il tempo trascorso dall’ultimo aggiornamento nell’angolo in alto a destra di ogni rapporto sulle ore preventivate. L’aggiornamento del rapporto aggiorna le informazioni in esso contenute solo quando è trascorsa più di un’ora dall’ultimo aggiornamento.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

## Requisiti di accesso

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Creare un rapporto sulle ore preventivate

1. Fai clic sul **menu principale** ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **Rapporti**.

1. Fai clic su **Nuovo rapporto > Ora preventivata**.

   Al report viene applicata la visualizzazione predefinita.

1. (Facoltativo) Per semplificare la lettura del report, fai clic sulla colonna **Ore preventivate**, quindi **Passa alla modalità testo**, quindi modifica il

   ```
   valuefield
   ```

   riga a

   ```
   valueexpreesion
   ```

   e immettere l&#39;espressione di arrotondamento.

   In questo modo il numero di ore preventivate viene arrotondato al numero di decimali specificato.

   Per informazioni sull&#39;arrotondamento di un numero in Workfront, vedere l&#39;articolo [Panoramica delle espressioni di dati calcolati](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (Facoltativo) Fai clic su **Aggiungi colonna** per aggiungere altre colonne.
1. (Facoltativo) Per semplificare la lettura del rapporto, si consiglia di aggiungervi un raggruppamento. Consigliamo il seguente raggruppamento:

   Fai clic sulla scheda **Raggruppamenti**, quindi effettua una o più delle seguenti operazioni:

   1. Fai clic su **Aggiungi raggruppamento** e inizia a digitare &quot;Nome progetto&quot;, quindi selezionalo quando viene visualizzato nell&#39;elenco.
   1. Fare clic su **Aggiungi raggruppamento** e iniziare a digitare &quot;Nome mansione&quot;, quindi selezionarlo quando viene visualizzato nell&#39;elenco.
   1. Fai clic su **Aggiungi raggruppamento** e inizia a digitare **Data di allocazione**, selezionala quando viene visualizzata nell&#39;elenco, quindi seleziona l&#39;intervallo di tempo in base al quale desideri eseguire il raggruppamento dal campo **Raggruppa date per**.

1. (Facoltativo) Fai clic su **Filtri** per aggiungere filtri al report.
1. (Facoltativo) Fare clic su **Grafico** per aggiungere un grafico al report.
1. Fai clic su **Salva + Chiudi**.

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
