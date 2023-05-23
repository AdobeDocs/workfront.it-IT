---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizzazione: rimozione del collegamento a un oggetto in una colonna"
description: Per impostazione predefinita, alcuni oggetti visualizzati in una visualizzazione vengono collegati alla pagina Dettagli dell'oggetto. Ad esempio, la colonna in cui viene visualizzato il Nome di un progetto è un collegamento al progetto; la colonna in cui viene visualizzato il Nome di un utente è un collegamento alla pagina del profilo dell’utente.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Visualizzazione: rimozione di un collegamento a un oggetto in una colonna

Per impostazione predefinita, alcuni oggetti visualizzati in una visualizzazione vengono collegati alla pagina Dettagli dell&#39;oggetto. Ad esempio, la colonna in cui viene visualizzato il Nome di un progetto è un collegamento al progetto; la colonna in cui viene visualizzato il Nome di un utente è un collegamento alla pagina del profilo dell’utente.

È possibile rimuovere questo collegamento utilizzando la modalità testo nelle colonne visualizzate in tutte le visualizzazioni.

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

## Esempio: rimuovere il collegamento a un&#39;attività dalla colonna Nome attività in una visualizzazione attività:

1. Consente di passare a un elenco di attività.
1. Dalla sezione **Visualizza** menu a discesa, fai clic su **Nuova visualizzazione** per creare una nuova vista.

   Oppure

   Fai clic su **Icona Modifica** ![](assets/edit-icon.png)

   per modificare una vista esistente, selezionare la vista.

1. Clic **Aggiungi colonna** per aggiungere una nuova colonna.

   Oppure

   Fare clic su una colonna esistente con un collegamento a un oggetto.

1. Clic **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuove il testo trovato in **Modalità testo** e sostituirlo con il seguente codice:

   <pre>displayname=Nome attività<br>linkedname=direct<br>namekey=name<br>querysort=nome<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Composto</pre>

   >[!TIP]
   >
   >È possibile utilizzare codice simile per altri oggetti regolando i seguenti elementi:
   >
   >   
   >   
   >   * Sostituisci il **valuefield** riga del codice con **valueexpression** e mantenere lo stesso nome incluso tra parentesi graffe dopo il segno di uguale.
   >   
   >   
   >
   >   
   >   
   >   * Elimina tutte le righe che iniziano con >

      >   
      >     ```>   
      >     link.
      >     ```   >   
      >   
      >     
      from the original text of the column. For example, eliminate all the following lines:
      >     <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>
      >   
      >   
      >



1. Clic **Salva**, quindi **Salva visualizzazione**.
