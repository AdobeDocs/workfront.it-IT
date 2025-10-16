---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizzazione: rimozione del collegamento a un oggetto in una colonna'
description: Per impostazione predefinita, alcuni oggetti visualizzati in una visualizzazione vengono collegati alla pagina Dettagli dell'oggetto. Ad esempio, la colonna in cui viene visualizzato il Nome di un progetto è un collegamento al progetto; la colonna in cui viene visualizzato il Nome di un utente è un collegamento alla pagina del profilo dell’utente.
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Visualizzazione: rimozione di un collegamento a un oggetto in una colonna

<!--Audited: 11/2024-->

Per impostazione predefinita, alcuni oggetti visualizzati in una visualizzazione vengono collegati alla pagina Dettagli dell&#39;oggetto. Ad esempio, la colonna in cui viene visualizzato il Nome di un progetto è un collegamento al progetto; la colonna in cui viene visualizzato il Nome di un utente è un collegamento alla pagina del profilo dell’utente.

È possibile rimuovere questo collegamento utilizzando la modalità testo nelle colonne visualizzate in tutte le visualizzazioni.

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
   <p>Collaboratore o richiesta di modifica di una visualizzazione </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++


## Esempio: rimuovere il collegamento a un&#39;attività dalla colonna Nome attività in una visualizzazione attività:

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Visualizza**, fare clic su **Nuova visualizzazione** per creare una nuova visualizzazione.

   Oppure

   Fai clic sull&#39;icona **Modifica** ![Modifica](assets/edit-icon.png) per modificare una visualizzazione esistente, quindi seleziona la visualizzazione.

1. Fare clic su **Aggiungi colonna** per aggiungere una nuova colonna.

   Oppure

   Fare clic su una colonna esistente con un collegamento a un oggetto.

1. Fare clic su **Passa a modalità testo** > **Modifica modalità testo**.
1. Rimuovere il testo trovato nella casella **Modifica modalità testo** e sostituirlo con il seguente codice:

   ```
   displayname=Task Name
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression={name}
   valueformat=Compound
   ```

   >[!TIP]
   >
   >È possibile utilizzare codice simile per altri oggetti regolando i seguenti elementi:
   >
   >* Sostituisci la riga `valuefield` del codice con `valueexpression` e mantieni lo stesso nome incluso tra parentesi graffe dopo il segno di uguale.
   >* Elimina tutte le righe che iniziano con `link.` dal testo originale della colonna. Ad esempio, eliminare tutte le righe seguenti:
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Fai clic su **Fine**, quindi su **Salva visualizzazione**.

