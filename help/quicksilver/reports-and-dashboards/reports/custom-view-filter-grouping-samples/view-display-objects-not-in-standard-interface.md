---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: oggetti di visualizzazione non inclusi nell’interfaccia standard"
description: È possibile visualizzare in una vista oggetti non inclusi nell'interfaccia in modalità standard. Puoi eseguire questa operazione solo facendo riferimento a essi tramite la modalità testo.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '492'
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
   <td> <p>Richiesta di modifica di una vista </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Esempio: aggiungere la colonna Nome proprietario Portfolio a una vista del progetto

1. Consente di passare a un elenco di progetti.
1. Dal menu a discesa **Visualizza**, fare clic su **Nuova visualizzazione**.

1. Fai clic su **Aggiungi colonna**, quindi inizia a digitare &quot;ID proprietario Portfolio&quot; nel campo **Mostra in questa colonna**, quindi selezionalo quando viene visualizzato nell&#39;elenco.

1. Fare clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull&#39;area della modalità testo e fai clic su **Fai clic per modificare il testo**.
1. Sostituire la riga `valuefield` (`valuefield=portfolio:ownerID`) con la seguente riga:

   ```
   valuefield=portfolio:owner:name
   ```

   Oppure

   Rimuovere il testo trovato nella casella **Modalità testo** e sostituirlo con il seguente codice:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   In questo esempio particolare, il report verrà ordinato in base all&#39;ID proprietario del Portfolio, come indicato dalla riga `querysort`.

   >[!TIP]
   >
   >Per sostituire qualsiasi campo `ID` con il campo `name` utilizzando la modalità testo, sostituire sempre `ID` con `:name` nella riga `valuefield`.

1. Fai clic su **Salva**, quindi su **Salva visualizzazione**.
