---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Rapporto: Ora a budget'
description: '"Rapporto: Ora a budget'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# Rapporto: Ora budget

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

Se si desidera condividere le informazioni dell&#39;ora a budget con altri utenti che non hanno accesso al planner risorse, è possibile farlo creando un rapporto dell&#39;ora a budget. Puoi quindi condividere il rapporto con loro.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>Le ore previste vengono aggiornate ogni ora nel database Adobe Workfront. L’aggiornamento del rapporto non aggiorna necessariamente le informazioni relative all’ora. È possibile visualizzare il tempo trascorso dall&#39;ultimo aggiornamento nell&#39;angolo in alto a destra di ogni rapporto di orario previsto. L’aggiornamento del rapporto aggiorna le informazioni in esso contenute solo quando sono trascorse più di un’ora dall’ultimo aggiornamento.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

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

## Creare un rapporto orario previsto

1. Fai clic sul pulsante **Menu principale** ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **Rapporti**.

1. Fai clic su **Nuovo rapporto > Ora budget**.

   La visualizzazione predefinita viene applicata al rapporto.

1. (Facoltativo) Per semplificare la lettura del rapporto, fai clic sul pulsante **Ore previste** colonna **Passa alla modalità testo**, quindi cambia la

   ```
   valuefield
   ```

   linea a

   ```
   valueexpreesion
   ```

   e immettere l&#39;espressione di arrotondamento.

   In questo modo viene arrotondato il numero di ore previste a un numero di decimali specificato.

   Per informazioni su come arrotondare un numero in Workfront, consulta l’articolo [Espressioni dati calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (Facoltativo) Fai clic su **Aggiungi colonna** per aggiungere altre colonne.
1. (Facoltativo) Per semplificare la lettura del rapporto, ti consigliamo di aggiungere un raggruppamento. Suggeriamo il seguente raggruppamento:

   Fai clic sul pulsante **Raggruppamenti** , quindi effettua una o più delle seguenti operazioni:

   1. Fai clic su **Aggiungi raggruppamento** e inizia a digitare &quot;Nome progetto&quot;, quindi selezionalo quando viene visualizzato nell&#39;elenco.
   1. Fai clic su **Aggiungi raggruppamento** e iniziare a digitare &quot;Nome ruolo lavoro&quot;, quindi selezionarlo quando viene visualizzato nell&#39;elenco.
   1. Fai clic su **Aggiungi raggruppamento** e inizia a digitare **Data di allocazione**, selezionalo quando viene visualizzato nell’elenco, quindi seleziona l’intervallo di tempo in base al quale desideri raggruppare i dati nel **Raggruppa date per** campo .

1. (Facoltativo) Fai clic su **Filtri** per aggiungere filtri al rapporto.
1. (Facoltativo) Fai clic su **Grafico** per aggiungere un grafico al report.
1. Fai clic su **Salva e chiudi**.

## Revisione del rapporto sull&#39;ora prevista

Per impostazione predefinita, nel rapporto Ora a budget sono disponibili le seguenti informazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Progetto </td> 
   <td>Questo è il nome del progetto associato all'ora a budget.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ruolo</p> </td> 
   <td>Questo è il nome del ruolo del lavoro associato all'ora a budget. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utente</td> 
   <td>Questo è il nome dell'utente associato all'ora a budget.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Allc. Data</td> 
   <td> <p>Questa è la data di allocazione. È il primo giorno (una domenica) della settimana per cui hai preventivato le ore.</p> <p>Suggerimento:  <p>Se una settimana si estende per due mesi, questo genera due righe nel rapporto: una corrispondente al primo giorno della settimana (la domenica della settimana che si trova nel primo mese) e una seconda corrispondente al primo giorno del secondo mese (e che potrebbe essere qualsiasi giorno della settimana).</p> <p>Ad esempio, se effettui il budget di 8 ore per un utente per la settimana dal 30 giugno (domenica) al 6 luglio (sabato), le due righe mostrano una Data di allocazione del 30 giugno e la 1 luglio.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ore Bdg</td> 
   <td>Sono le ore previste assegnate all'utente nel Planner risorse.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Piano. Ore Bdg</td> 
   <td>Sono le ore previste assegnate al ruolo del lavoro o al progetto nel planner risorse.</td> 
  </tr> 
 </tbody> 
</table>
