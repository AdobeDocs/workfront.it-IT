---
title: Filtrare una tabella in Reporting Canvas
description: Filtrare una tabella in Reporting Canvas
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 1%

---


# Filtrare una tabella in Reporting Canvas

Dopo aver aggiunto un blocco di tabella a un rapporto, puoi impostare filtri per limitare le informazioni visualizzate nella tabella.

In una regola di filtro sono disponibili 3 componenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campo</td> 
   <td> <p>Il campo contenente le informazioni in base alle quali desideri filtrare la tabella .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operatore</td> 
   <td> <p>Il modo in cui il filtro determina quali valori di campo vengono inclusi o esclusi dalla tabella. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Valore</td> 
   <td> <p>I valori all’interno del campo selezionato che vengono valutati in base all’operatore .</p> </td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** Se desideri limitare i risultati nel rapporto in modo da visualizzare solo i progetti di proprietà di Jane Doe, puoi creare una regola di filtro con il campo &quot;Proprietario progetto&quot;, l’operatore &quot;Uguale a&quot; e il valore &quot;Jane Doe&quot;.

Oppure puoi visualizzare solo i progetti con un proprietario di progetto assegnato, che avranno il campo &quot;Proprietario progetto&quot; e l’operatore &quot;Non è vuoto&quot;.

## Prerequisiti

Prima di iniziare, è necessario iscriversi alla versione beta di Reporting Canvas. Per ulteriori informazioni, consulta [Reporting Canvas beta: panoramica](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Configurare le regole di filtro per una tabella

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Reporting**.

1. Fai clic su **Nuovo rapporto**.

   Oppure

   Passa a un rapporto esistente e fai clic sul pulsante **Menu Altro** icona ![](assets/more-icon.png) nell’intestazione del rapporto, seleziona **Modifica**.

1. Per raggruppare le righe in una nuova tabella, trascinare o fare doppio clic su un blocco di tabella nell’area di lavoro.

   Oppure

   Per raggruppare le righe in una tabella esistente, fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png) nell’intestazione della tabella.

1. Individua il campo in base al quale vuoi filtrare la tabella nel pannello di destra, quindi trascinalo nella sezione Filtro .

   Viene visualizzato un set di regole di filtro con il nome del campo selezionato.

1. Seleziona l’operatore desiderato dal menu a discesa:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Uguale a</strong> </td> 
      <td> <p>Questo restituisce solo una corrispondenza esatta del valore ricercato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Diverso da</strong> </td> 
      <td> <p>Questo restituisce solo risultati che non corrispondono esattamente al valore ricercato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Blank</strong> </td> 
      <td> <p>Il campo esiste per l’oggetto ma al campo non è stato ancora assegnato un valore.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Not Blank</strong> </td> 
      <td> <p>Il campo a cui si sta filtrando esiste ed è stato assegnato un valore.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Less Than</strong> </td> 
      <td> <p>Cerca tutti i risultati con un valore inferiore a quello immesso, senza includere il valore inserito.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Less Than Or Equal To</strong> </td> 
      <td> <p>Cerca tutti i risultati con un valore minore o uguale al valore inserito.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Greater Than</strong> </td> 
      <td> <p>Cerca tutti i risultati con un valore maggiore del valore inserito, senza includere il valore inserito.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Greater Than Or Equal To</strong> </td> 
      <td> <p>Cerca tutti i risultati con valori maggiori o uguali al valore inserito.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tra</strong> </td> 
      <td> <p>Fornisce 2 valori di campo obbligatori e cerca tutti i risultati compresi nell’intervallo di entrambi i campi, inclusi i valori immessi.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contiene</strong> </td> 
      <td> <p>Cerca il testo specificato in tutta una stringa di testo.</p> <p>Ad esempio, l’utilizzo di "Contains Inf" acquisisce qualsiasi elemento con "Inf" o "inf", come la parola "Infinity".</p> <p>Nota: Adobe Workfront cerca l’intera parola o frase immessa per ogni regola di filtro. Ad esempio, se stai cercando campi con la frase "nuovo progetto" nel loro nome, Workfront non visualizza progetti che hanno solo "nuovo" o "progetto" nei loro nomi o frasi che contengono parole extra tra loro, ad esempio "nuovo progetto principale". Il filtro trova solo i progetti con la frase esatta "nuovo progetto" nel nome.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Non contiene</strong> </td> 
      <td> <p>Questo filtra gli elementi per i quali manca il testo specificato.</p> <p>Ad esempio, "non contiene inf" restituisce qualsiasi campo senza "Inf" o "inf" nei loro nomi.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Immetti l’ultimo valore per completare la regola del filtro, in base all’operatore selezionato.

   >[!NOTE]
   >
   >I valori inseriti sono **not** sensibile a maiuscole e minuscole.

1. (Facoltativo) Per aggiungere un&#39;altra regola di filtro al set di regole, procedi come segue:

   1. Trascina un altro campo nella **Rilascia per aggiungere un’altra regola** nella sezione Filtri sotto l’altra regola.
   1. Ripetere i passaggi 4-6.
   1. Nel menu a discesa operatore a sinistra della nuova regola, seleziona **E** o **O**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>AND</p> </td> 
         <td> <p>Quando si uniscono regole di filtro o set di regole con l’operatore AND, si indica che si desidera soddisfare tutte le regole allo stesso livello.</p> <p>Per impostazione predefinita, le istruzioni in un filtro sono collegate dall’operatore AND.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>O</p> </td> 
         <td> <p>Quando si uniscono regole di filtro o set di regole con l'operatore OR si indica che si desidera <strong>almeno</strong> una regola, o un set di regole, a quel livello da soddisfare.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >Gli operatori AND e OR allo stesso livello, ovvero che collegano più regole all&#39;interno di un set di regole o interi set di regole insieme, corrisponderanno sempre. Ad esempio, se modifichi l’operatore tra due regole all’interno di un set di regole, tutti gli altri operatori in quel set di regole cambieranno automaticamente per farli corrispondere.

1. (Condizionale) Per aggiungere un set di regole di filtro aggiuntivo, procedi come segue:

   1. Trascina il campo da aggiungere al **Aggiungi un set di regole** area sotto gli altri set di regole del filtro.
   1. Ripetere i passaggi 4-7.
   1. Nel menu a discesa operatore a sinistra del nuovo set di regole, seleziona **E** o **O**. Questi operatori funzionano allo stesso modo di quelli elencati al passaggio 7, ma si applicano a set di regole interi anziché a singole regole all’interno di un set.****
