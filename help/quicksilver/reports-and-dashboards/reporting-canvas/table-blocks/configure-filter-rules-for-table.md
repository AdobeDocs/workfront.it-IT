---
title: Filtrare una tabella in Reporting Canvas (Area di lavoro rapporti)
description: Filtrare una tabella in Reporting Canvas (Area di lavoro rapporti)
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: ca70952bf0acd71f748b042852d434b560727a83
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 1%

---


# Filtrare una tabella in Reporting Canvas (Area di lavoro rapporti)

Dopo aver aggiunto un blocco di tabella a un rapporto, puoi impostare filtri per limitare le informazioni visualizzate nella tabella.

Una regola di filtro contiene 3 componenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campo</td> 
   <td> <p>Campo contenente le informazioni in base alle quali si desidera filtrare la tabella.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operatore</td> 
   <td> <p>Il modo in cui il filtro determina quali valori di campo sono inclusi o esclusi dalla tabella. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Valore</td> 
   <td> <p>I valori all’interno del campo selezionato che vengono valutati in base all’operatore.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** Se desideri limitare i risultati nel rapporto solo ai progetti di proprietà di Jane Doe, puoi creare una regola di filtro con il campo &quot;Proprietario progetto&quot;, l’operatore &quot;Uguale a&quot; e il valore &quot;Jane Doe&quot;.

Oppure potresti visualizzare solo i progetti a cui è assegnato un proprietario, con il campo &quot;Proprietario progetto&quot; e l’operatore &quot;Non è vuoto&quot;.

## Prerequisiti

Prima di iniziare, devi iscriverti alla versione beta di Reporting Canvas. Per ulteriori informazioni, consulta [Reporting Canvas beta: panoramica](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configurare le regole di filtro per una tabella

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Generazione rapporti**.

1. Clic **Nuovo rapporto**.

   Oppure

   Vai a un rapporto esistente, fai clic su **Menu Altro** icona ![](assets/more-icon.png) nell’intestazione del rapporto, seleziona quindi **Modifica**.

1. Per raggruppare le righe di una nuova tabella, trascinare o fare doppio clic su un blocco di tabella nell&#39;area di lavoro.

   Oppure

   Per raggruppare le righe di una tabella esistente, fare clic su **Modifica** icona ![](assets/edit-icon.png) nell’intestazione della tabella.

1. Nel pannello a destra, individua il campo in base al quale desideri filtrare la tabella, quindi trascinalo nella sezione Filtro.

   Viene visualizzato un set di regole di filtro con il nome del campo selezionato.

1. Seleziona l’operatore desiderato dal menu a discesa:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Uguale a</strong> </td> 
      <td> <p>Questo restituisce solo una corrispondenza esatta del valore cercato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Diverso da</strong> </td> 
      <td> <p>Questo restituisce solo risultati che non corrispondono esattamente al valore cercato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Blank</strong> </td> 
      <td> <p>Il campo esiste per l’oggetto, ma al campo non è ancora stato assegnato un valore.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Not Blank</strong> </td> 
      <td> <p>Il campo per il quale stai filtrando esiste ed è stato assegnato un valore.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>È minore di</strong> </td> 
      <td> <p>Consente di cercare tutti i risultati con un valore inferiore a quello immesso, senza includere il valore immesso.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>È minore o uguale a</strong> </td> 
      <td> <p>Consente di cercare tutti i risultati con un valore minore o uguale al valore immesso.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>È maggiore di</strong> </td> 
      <td> <p>Questa opzione consente di cercare tutti i risultati con un valore maggiore di quello immesso, senza includere il valore immesso.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>È maggiore di o uguale a</strong> </td> 
      <td> <p>Consente di cercare tutti i risultati con valori maggiori o uguali al valore immesso.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tra</strong> </td> 
      <td> <p>Fornisce 2 valori di campo obbligatori e cerca tutti i risultati all’interno dell’intervallo di entrambi i campi, inclusi i valori immessi.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contiene</strong> </td> 
      <td> <p>Consente di cercare il testo specificato in un'intera stringa di testo.</p> <p>Ad esempio, l’utilizzo di "Contiene info" acquisisce qualsiasi cosa contenente "Info" o "Info", ad esempio la parola "Infinito".</p> <p>Nota: Adobe Workfront cerca l’intera parola o frase immessa per ogni regola del filtro. Ad esempio, se cerchi campi il cui nome contiene la frase "nuovo progetto", Workfront non mostra i progetti il cui nome contiene solo "nuovo" o "progetto", né frasi che contengono termini aggiuntivi intermedi, ad esempio "nuovo progetto principale". Il filtro trova solo i progetti il cui nome contiene esattamente la frase "nuovo progetto".</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Non contiene</strong> </td> 
      <td> <p>Questo filtra gli elementi a cui manca il testo specificato.</p> <p>Ad esempio, "does not contain inf" restituisce tutti i campi senza "Inf" o "inf" nel loro nome.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Immetti l’ultimo valore per completare la regola del filtro, in base all’operatore selezionato.

   >[!NOTE]
   >
   >I valori immessi qui sono **non** distinzione tra maiuscole e minuscole.

1. (Facoltativo) Per aggiungere un’altra regola di filtro al set di regole, effettua le seguenti operazioni:

   1. Trascina un altro campo nel **Rilascia per aggiungere un&#39;altra regola** nella sezione Filtri sotto l’altra regola.
   1. Ripetere i passaggi 4-6.
   1. Nell’elenco a discesa operatore a sinistra della nuova regola, seleziona **E** o **OPPURE**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>E</p> </td> 
         <td> <p>Quando si uniscono regole di filtro o set di regole con l'operatore AND, si indica che si desidera che vengano soddisfatte tutte le regole dello stesso livello.</p> <p>Per impostazione predefinita, le istruzioni in un filtro sono unite dall'operatore AND.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>OPPURE</p> </td> 
         <td> <p>Quando si uniscono regole di filtro o set di regole con l'operatore OR si indica che si desidera <strong>almeno</strong> una regola, o set di regole, a tale livello da soddisfare.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >Gli operatori AND e OR allo stesso livello, che collegano più regole all&#39;interno di un set di regole o insiemi di regole interi, corrisponderanno sempre. Ad esempio, se modifichi l’operatore tra due regole all’interno di un set di regole, tutti gli altri operatori in tale set di regole cambieranno automaticamente in modo da corrispondere a esso.

1. (Condizionale) Per aggiungere un set di regole di filtro aggiuntivo, effettua le seguenti operazioni:

   1. Trascina il campo da aggiungere al **Aggiungere un set di regole** area sotto gli altri set di regole di filtro.
   1. Ripetere i passaggi 4-7.
   1. Nell’elenco a discesa operatore a sinistra del nuovo set di regole, seleziona **E** o **OPPURE**. Questi operatori funzionano come quelli elencati nel passaggio 7, ma si applicano a interi set di regole anziché a singole regole all’interno di un set.****
