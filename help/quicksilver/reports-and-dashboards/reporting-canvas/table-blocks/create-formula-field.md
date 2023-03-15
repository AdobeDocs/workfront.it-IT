---
title: Creare un campo formula in Reporting Canvas
description: Creare un campo formula in Reporting Canvas
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
source-git-commit: d649decb2875a3af4fd40c323a7836d4468bf04b
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 7%

---


# Creare un campo formula in Reporting Canvas

Il generatore di campi in Reporting Canvas consente di creare campi che eseguono calcoli personalizzati.

## Prerequisiti

Prima di iniziare, è necessario iscriversi alla versione beta di Reporting Canvas. Per ulteriori informazioni, consulta [Reporting Canvas beta: panoramica](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Creazione di un campo formula

1. Crea o passa a un blocco di tabella, come descritto in [Aggiungere o modificare un blocco di tabella in Reporting Canvas](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md).
1. Nell’intestazione della tabella del rapporto, fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Se la tabella è stata creata e non sono stati ancora aggiunti campi, fare clic sul pulsante Modifica al centro della tabella.

1. Fai clic su **Nuovo +** nella parte superiore del **Campi** nel pannello a destra.
1. Nella nuova pagina visualizzata, fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png) accanto al nome del campo nell&#39;angolo in alto a sinistra per modificare il nome del campo formula.
1. Trascina **Funzioni** o **Campi** dal pannello di sinistra al generatore di campi al centro per aggiungerli al campo formula.


   >[!TIP]
   >
   >Quando si crea il campo formula, la **Anteprima campo** a destra vengono visualizzati esempi del campo risultante.

   Ogni funzione contiene un numero di rettangoli punteggiati vuoti che verranno utilizzati come argomenti per calcolare un risultato. È possibile popolare immettendo testo statico o numeri, trascinando e rilasciando un campo dal pannello di sinistra (utilizzando il valore del campo nel calcolo) oppure trascinando e rilasciando un&#39;altra funzione (creando una funzione nidificata). Le possibili funzioni includono:

   | Funzione | Descrizione | Uscita |
   |---|---|---|
   | IF | Confrontare due argomenti in base a un modificatore selezionato, quindi eseguire un&#39;azione specifica in base al valore True (Is True:) o False (Is False:) risultante. Nota: attualmente, il secondo argomento non può essere un valore True o False statico. È invece possibile utilizzare una funzione nidificata come ISBLANK(Project Name) che restituisce sempre False come soluzione alternativa. | True/False, Data, Numero o Stringa |
   | CONCAT | Unisci due o più stringhe tra loro end-to-end per creare una nuova stringa. | Stringa |
   | CONTAINS | Valutare se un campo argomento stringa (testo Trova) è contenuto all&#39;interno di un altro campo argomento stringa (all&#39;interno di testo). | Vero/Falso |
   | TRA | Valuta se il valore di un campo argomento (Find) corrisponde al valore di almeno un altro campo argomento (Within) | Vero/Falso |
   | ISBLANK | Valutare se un campo argomento è vuoto. | Vero/Falso |
   | LEN | Misura la lunghezza (in numero di caratteri) di un campo argomento. | Numero |
   | ROUND | Restituisce un numero arrotondato in base alla precisione selezionata. | Numero |
   | FLOOR | Restituisce il numero intero più vicino, arrotondato verso il basso. | Numero |
   | NUMBER | Restituisce l&#39;intervallo più grande minore del valore di un argomento numerico (identico a una funzione Floor). | Numero |
   | STRING | Converte il contenuto di un campo argomento in una stringa | Stringa |
   | SUBSTR | Crea una nuova stringa da una stringa più grande, contenente i caratteri compresi tra un numero di indice (Start) e un altro (End). | Stringa |
   | SINISTRA | Crea una nuova stringa da una stringa più grande, che contiene caratteri che iniziano con il più a sinistra e contano a destra un numero di caratteri (Length). | Stringa |
   | DESTRA | Crea una nuova stringa da una stringa più grande, che contiene caratteri che iniziano con il più a destra e contano a sinistra un numero di caratteri (Length). | Stringa |
   | SOMMA  | Aggiungere insieme i valori di due o più campi argomento. | Numero |
   | SUB | Sottrae i valori di due o più campi argomento (in ordine da sinistra a destra). | Numero |
   | PROD | Moltiplica i valori di due o più campi di argomento insieme. | Numero |
   | DIV | Dividi il valore di due o più campi argomento (in ordine da sinistra a destra). | Numero |
   | MESE | Restituisce un numero uguale al valore del mese di una data. | Numero |
   | ANNO | Restituisce un numero uguale al valore dell&#39;anno per una data. | Numero |
   | DATEDIFF | Calcola il numero totale di giorni tra due date, arrotondato a una posizione decimale. | Numero |
   | WEEKDAYDIFF | Calcola il numero di giorni feriali tra due date, arrotondato a una posizione decimale. | Numero |

   {style="table-layout:auto"}

1. Fai clic sul pulsante **Torna indietro** nell’angolo in alto a sinistra dello schermo per tornare alla tabella.
