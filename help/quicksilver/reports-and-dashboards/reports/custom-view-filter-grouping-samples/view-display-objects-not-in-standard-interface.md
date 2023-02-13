---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: oggetti di visualizzazione non inclusi nell''interfaccia standard"'
description: 'È possibile visualizzare in una visualizzazione oggetti non inclusi nell’interfaccia in modalità standard. Puoi farlo solo facendo riferimento a essi tramite la modalità testo. È possibile determinare quali campi possono essere inclusi in una visualizzazione in uno dei seguenti modi: MODIFICA ME.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Visualizzazione: oggetti di visualizzazione non inclusi nell’interfaccia standard

È possibile visualizzare in una visualizzazione oggetti non inclusi nell’interfaccia in modalità standard. Puoi farlo solo facendo riferimento a essi tramite la modalità testo.\
È possibile determinare quali campi possono essere inclusi in una visualizzazione in uno dei seguenti modi:

* Utilizza la [Esplora API](https://one.workfront.com/s/api-explorer) per individuare altri oggetti a cui è possibile fare riferimento tramite la modalità testo.\
   Non tutti i campi documentati in API Explorer sono campi validi per la modalità testo. Alcuni campi sono riportati solo tramite l’API .

* Trova il campo ID dell’oggetto in una colonna. La maggior parte degli oggetti con ID campo dispone anche di una colonna o di un nome di campo corrispondente che potrebbe non essere accessibile tramite l’interfaccia in modalità standard.

   È possibile utilizzare la modalità testo per includere in una visualizzazione il nome della colonna o del campo invece dell’ID sostituendo l’ `fieldnameID` con `fieldname:name`.

   Ad esempio, nell’interfaccia in modalità standard, la **ID proprietario Portfolio** è disponibile per una visualizzazione del progetto, ma la **Nome proprietario Portfolio** Il campo non è valido. È possibile utilizzare la modalità testo per visualizzare la **Nome proprietario Portfolio** nella colonna di una visualizzazione.

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

## Esempio: aggiungi la colonna Nome proprietario Portfolio a una visualizzazione del progetto

1. Vai a un elenco di progetti.
1. Da **Visualizza** menu a discesa, fai clic su **Nuova vista**.

1. Fai clic su **Aggiungi colonna** quindi inizia a digitare &quot;ID proprietario Portfolio&quot; nel **Mostra in questa colonna** , quindi selezionalo quando viene visualizzato nell’elenco.

1. Fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Sostituisci il `valuefield` line (`valuefield=portfolio:ownerID`) con la seguente riga:

   ```
   valuefield=portfolio:owner:name
   ```

   Oppure

   Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   In questo particolare esempio, il report ordinerà il report in base all&#39;ID proprietario del Portfolio, come indicato dalla `querysort` linea.

   >[!TIP]
   >
   >Per sostituire qualsiasi campo `ID` con il campo `name` utilizzando la modalità testo, sostituisci sempre `ID` con `:name` in `valuefield` linea.

1. Fai clic su **Salva**, quindi **Salva visualizzazione**.
