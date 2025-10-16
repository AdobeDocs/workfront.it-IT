---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vista: visualizza gli oggetti non inclusi nell''interfaccia standard'
description: È possibile visualizzare in una vista oggetti non inclusi nell'interfaccia in modalità standard. Puoi eseguire questa operazione solo facendo riferimento a essi tramite la modalità testo.
author: Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Visualizza: oggetti di visualizzazione non inclusi nell&#39;interfaccia standard

È possibile visualizzare in una vista oggetti non inclusi nell&#39;interfaccia in modalità standard. Puoi eseguire questa operazione solo facendo riferimento a essi tramite la modalità testo.\
È possibile determinare quali campi possono essere inclusi in una visualizzazione in uno dei seguenti modi:

* Utilizza [API Explorer](../../../wf-api/general/api-explorer.md) per individuare altri oggetti a cui è possibile fare riferimento tramite la modalità testo.\
  Non tutti i campi documentati in API Explorer sono campi validi per la modalità testo. Alcuni campi sono segnalabili solo tramite l’API.

* Trova il campo ID dell&#39;oggetto in una colonna. La maggior parte degli oggetti che hanno un ID campo hanno anche un nome di colonna o di campo corrispondente che potrebbe non essere accessibile tramite l&#39;interfaccia in modalità standard.

  È possibile utilizzare la modalità testo per includere in una visualizzazione il nome della colonna o del campo anziché l&#39;ID sostituendo `fieldnameID` con `fieldname:name`.

  Nell&#39;interfaccia in modalità standard, ad esempio, il campo **ID proprietario Portfolio** è disponibile per la visualizzazione di un progetto, ma il campo **Nome proprietario Portfolio** non lo è. È possibile utilizzare la modalità testo per visualizzare il **Nome proprietario Portfolio** nella colonna di una visualizzazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un rapporto</p>
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

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Esempio: aggiungere la colonna Nome proprietario Portfolio a una vista del progetto

1. Consente di passare a un elenco di progetti.
1. Dal menu a discesa **Visualizza**, fare clic su **Nuova visualizzazione**.

1. Fai clic su **Aggiungi colonna**, quindi inizia a digitare &quot;ID proprietario Portfolio&quot; nel campo **Mostra in questa colonna**, quindi selezionalo quando viene visualizzato nell&#39;elenco.

1. Fare clic su **Passa alla modalità testo**, quindi su **Modifica modalità testo**.
1. Sostituire la riga `valuefield` (`valuefield=portfolio:ownerID`) con la seguente riga:

   `valuefield=portfolio:owner:name`

   Oppure

   Rimuovere il testo trovato nella casella **Modifica modalità testo** e sostituirlo con il seguente codice:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   In questo esempio particolare, il report verrà ordinato in base all&#39;ID proprietario Portfolio, come indicato dalla riga `querysort`.

   >[!TIP]
   >
   >Per sostituire qualsiasi campo `ID` con il campo `name` utilizzando la modalità testo, sostituire sempre `ID` con `:name` nella riga `valuefield`.

1. Fai clic su **Fine**, quindi su **Salva visualizzazione**.
