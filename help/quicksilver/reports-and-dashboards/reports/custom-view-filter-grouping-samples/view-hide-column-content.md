---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: nascondere il contenuto di una colonna"'
description: È possibile nascondere le informazioni nella colonna di una visualizzazione. Per farlo, modifica la modalità testo della colonna.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Visualizza: nascondere il contenuto di una colonna

È possibile nascondere le informazioni nella colonna di una visualizzazione. Per farlo, modifica la modalità testo della colonna.

>[!TIP]
>
>* È possibile utilizzare colonne nascoste per ordinare in base a un determinato oggetto che non si desidera visualizzare nella visualizzazione.\
   >  Ad esempio, è possibile ordinare in base al numero di attività in una visualizzazione attività e nascondere le informazioni relative al numero di attività dalla visualizzazione. In questo caso, l’oggetto a cui si fa riferimento nella colonna consente di ordinare la visualizzazione, ma le informazioni relative a tale oggetto non vengono visualizzate nella visualizzazione.
>* Quando nascondi una colonna, tieni presente che le informazioni contenute nella colonna sono nascoste, ma che la colonna esiste ancora nella visualizzazione.
>


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

## Esempio: Ordinare e nascondere la colonna Numero task in una visualizzazione task:

1. Passare a un elenco di attività.
1. Da **Visualizza** menu a discesa, fai clic su **Nuova vista**.

1. Fai clic su **Aggiungi colonna** e inizia a digitare &quot;Task Number&quot; nel **Mostra in questa colonna** quindi selezionalo quando viene visualizzato nell’elenco.

1. Fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>Le modifiche importanti di questo codice che rendono la colonna nascosta sono le seguenti:

   ```
   displayname
   ```

   questa riga deve essere vuota.

   ```
   valuefield
   ```

   È stato sostituito da *value* e deve essere vuoto.

   ```
   width
   ```

   : A seconda del campo, deve essere presente un valore di *0* o *1*.

1. Fai clic su **Salva**, quindi **Salva visualizzazione**.
