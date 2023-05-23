---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizza: nascondere il contenuto di una colonna"
description: È possibile nascondere le informazioni nella colonna di una visualizzazione. A tale scopo, è possibile modificare la modalità testo della colonna.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Visualizza: nasconde il contenuto di una colonna

È possibile nascondere le informazioni nella colonna di una visualizzazione. A tale scopo, è possibile modificare la modalità testo della colonna.

>[!TIP]
>
>* È possibile utilizzare le colonne nascoste per ordinare in base a un determinato oggetto che non si desidera visualizzare nella visualizzazione.\
   >  È ad esempio possibile ordinare in base al numero di task in una visualizzazione delle attività e nascondere le informazioni sul numero di task dalla visualizzazione. In questo caso, l&#39;oggetto a cui si fa riferimento nella colonna consente di ordinare la visualizzazione, ma le informazioni dell&#39;oggetto non vengono visualizzate nella visualizzazione.
>* Quando si nasconde una colonna, si noti che le informazioni contenute nella colonna sono nascoste, ma la colonna esiste ancora nella visualizzazione.
>


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
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Esempio: ordinare e nascondere la colonna Numero attività in una visualizzazione delle attività:

1. Consente di passare a un elenco di attività.
1. Dalla sezione **Visualizza** menu a discesa, fai clic su **Nuova visualizzazione**.

1. Clic **Aggiungi colonna** e inizia a digitare &quot;Task Number&quot; (Numero attività) nel **Mostra in questa colonna** quindi selezionarlo quando viene visualizzato nell&#39;elenco.

1. Clic **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuove il testo trovato in **Modalità testo** e sostituirlo con il seguente codice:

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value= valore</strong>valueformat=int<br><strong>width=0</strong></pre>Le modifiche importanti di questo codice che rendono la colonna nascosta sono:

   ```
   displayname
   ```

   questa riga deve essere vuota.

   ```
   valuefield
   ```

   Questo è stato sostituito da *valore*, e deve essere vuoto.

   ```
   width
   ```

   : a seconda del campo, questo deve avere un valore *0* o *1*.

1. Clic **Salva**, quindi **Salva visualizzazione**.
