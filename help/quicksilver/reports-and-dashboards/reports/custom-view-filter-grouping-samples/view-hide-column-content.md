---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizza: nasconde il contenuto di una colonna'
description: È possibile nascondere le informazioni nella colonna di una visualizzazione. A tale scopo, è possibile modificare la modalità testo della colonna.
author: Courtney
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 13%

---

# Visualizzazione: nascondere il contenuto di una colonna

<!--Audited: 11/2024-->

È possibile nascondere le informazioni nella colonna di una visualizzazione. A tale scopo, è possibile modificare la modalità testo della colonna.

>[!NOTE]
>
>* È possibile utilizzare le colonne nascoste per ordinare in base a un determinato oggetto che non si desidera visualizzare nella visualizzazione.\
>  È ad esempio possibile ordinare in base al numero di task in una visualizzazione delle attività e nascondere le informazioni sul numero di task dalla visualizzazione. In questo caso, l&#39;oggetto a cui si fa riferimento nella colonna consente di ordinare la visualizzazione, ma le informazioni dell&#39;oggetto non vengono visualizzate nella visualizzazione.
>* Quando si nasconde una colonna, si noti che le informazioni contenute nella colonna sono nascoste, ma la colonna esiste ancora nella visualizzazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di una visualizzazione </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l'accesso a Filtri, Viste, Raggruppamenti per modificare una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Esempio: ordinare e nascondere la colonna Numero attività in una visualizzazione delle attività:

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Visualizza**, fare clic su **Nuova visualizzazione**.

1. Fai clic su **Aggiungi colonna** e inizia a digitare &quot;Numero attività&quot; nel campo **Mostra in questa colonna**, quindi selezionalo quando viene visualizzato nell&#39;elenco.

1. Fare clic su **Passa alla modalità testo**, quindi su **Modifica modalità testo**.
1. Rimuovere il testo trovato nella casella **Modifica modalità testo** e sostituirlo con il seguente codice:

   ```
   displayname=
   linkedname=direct
   querysort=taskNumber
   sortOrder=1
   sortType=asc
   textmode=true
   value=
   valueformat=int
   width=0
   ```

   Le modifiche importanti di questo codice che rendono la colonna nascosta sono:

   * `displayname=`: la riga deve essere vuota.
   * `valuefield=`: questa riga deve essere sostituita da `value=`, che deve essere vuoto.
   * `width=`: a seconda del campo, il valore deve essere **0** o **1**.

1. Fai clic su **Fine**, quindi su **Salva visualizzazione**.
