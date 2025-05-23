---
title: Creare un campo formula nell’area di lavoro Reporting
description: Creare un campo formula nell’area di lavoro Reporting
hidefromtoc: true
hide: true
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 7%

---

# Creare un campo formula nell’area di lavoro Reporting

Il generatore di campi nell’area di lavoro Reporting consente di creare campi che eseguono calcoli personalizzati.

## Prerequisiti

Prima di iniziare, devi iscriverti alla versione beta di Reporting Canvas. Per ulteriori informazioni, vedere [Reporting Canvas beta: overview](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Creare un campo formula

1. Creare o passare a un blocco di tabella, come descritto in [Aggiungere o modificare un blocco di tabella nell&#39;area di lavoro Reporting](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md).
1. Nell&#39;intestazione della tabella del report fare clic sull&#39;icona **Modifica** ![Modifica](assets/edit-icon.png).

   ![Icona Modifica nell&#39;intestazione della tabella](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Se la tabella è stata appena creata e non sono ancora stati aggiunti campi, fare clic sul pulsante Modifica al centro della tabella.

1. Fai clic su **Nuovo +** nella parte superiore dell&#39;elenco **Campi** nel pannello di destra.
1. Nella nuova pagina visualizzata, fai clic sull&#39;icona **Modifica** ![Icona Modifica](assets/edit-icon.png) accanto al nome del campo nell&#39;angolo in alto a sinistra per modificare il nome del campo formula.
1. Trascina **Funzioni** o **Campi** dal pannello di sinistra al generatore di campi al centro per aggiungerli al campo formula.


   >[!TIP]
   >
   >Durante la creazione del campo formula, l&#39;**Anteprima campo** a destra visualizza esempi del campo risultante.

   Ogni funzione contiene un numero di rettangoli punteggiati vuoti che verranno utilizzati come argomenti nel calcolo di un risultato. Questi possono essere compilati immettendo testo statico o numeri, trascinando un campo dal pannello di sinistra (utilizzando il valore del campo nel calcolo) o trascinando un’altra funzione (creando una funzione nidificata). Le funzioni possibili includono:

   | Funzione | Descrizione | Output |
   |---|---|---|
   | IF | Confronta due argomenti in base a un modificatore selezionato, quindi esegui un’azione specificata in base al valore risultante True (Is True:) o False (Is False:). Nota: attualmente, il secondo argomento non può essere un valore statico True o False. È invece possibile utilizzare una funzione nidificata come ISBLANK(Project Name) che restituisce sempre False come soluzione alternativa. | True/False, Date, Number o String |
   | CONCAT | Unisci due o più stringhe in modo da creare una nuova stringa. | Stringa |
   | CONTAINS | Valuta se un campo argomento stringa (testo Trova) è contenuto in un altro campo argomento stringa (testo Interno). | Vero/Falso |
   | TRA | Valuta se il valore di un campo argomento (Find) corrisponde al valore di almeno un altro campo argomento (Within) | Vero/Falso |
   | ISBLANK | Valuta se un campo argomento è vuoto. | Vero/Falso |
   | LEN | Misura la lunghezza (in numero di caratteri) di un campo argomento. | Numero |
   | ROUND | Restituisce un numero arrotondato in base alla precisione selezionata. | Numero |
   | FLOOR | Restituisce il numero intero più vicino, arrotondato per difetto. | Numero |
   | NUMBER | Restituisce l&#39;interger più grande minore del valore di un argomento numerico, identico a una funzione Floor. | Numero |
   | STRING | Converte il contenuto di un campo argomento in una stringa | Stringa |
   | SUBSTR | Creare una nuova stringa da una stringa più grande contenente i caratteri compresi tra un numero di indice (Inizio) e un altro (Fine). | Stringa |
   | SINISTRA | Crea una nuova stringa da una stringa più grande, che contiene i caratteri che iniziano con l’estrema sinistra e contano a destra un numero di caratteri (Lunghezza). | Stringa |
   | DESTRA | Crea una nuova stringa da una stringa più grande, che contiene caratteri che iniziano con l’estrema destra e contano a sinistra di un numero di caratteri (Lunghezza). | Stringa |
   | SOMMA | Aggiungi i valori di due o più campi argomento insieme. | Numero |
   | SUB | Sottrarre i valori di due o più campi argomento (in ordine da sinistra a destra). | Numero |
   | PROD | Moltiplica i valori di due o più campi argomento. | Numero |
   | DIV | Dividi il valore di due o più campi argomento (in ordine da sinistra a destra). | Numero |
   | MESE | Restituisce un numero uguale al valore del mese per una data. | Numero |
   | ANNO | Restituisce un numero uguale al valore anno di una data. | Numero |
   | DATEDIFF | Calcola il numero totale di giorni tra due date, arrotondato a una cifra decimale. | Numero |
   | WEEKDAYDIFF | Calcola il numero di giorni feriali tra due date, arrotondato a una cifra decimale. | Numero |

   {style="table-layout:auto"}

1. Fai clic sulla freccia **Indietro** nell&#39;angolo in alto a sinistra dello schermo per tornare alla tabella.
