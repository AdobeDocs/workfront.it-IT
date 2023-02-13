---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Visualizza: rimuovi il collegamento a un oggetto in una colonna"'
description: Per impostazione predefinita, alcuni oggetti visualizzati in una visualizzazione collegano alla pagina Dettagli dell’oggetto. Ad esempio, la colonna che visualizza il Nome di un progetto è un collegamento al progetto; la colonna che visualizza il nome di un utente è un collegamento alla pagina del profilo dell’utente.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Visualizza: rimuovere un collegamento a un oggetto in una colonna

Per impostazione predefinita, alcuni oggetti visualizzati in una visualizzazione collegano alla pagina Dettagli dell’oggetto. Ad esempio, la colonna che visualizza il Nome di un progetto è un collegamento al progetto; la colonna che visualizza il nome di un utente è un collegamento alla pagina del profilo dell’utente.

Puoi rimuovere questo collegamento utilizzando la modalità testo nelle colonne visualizzate in tutte le viste.

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

## Esempio: Rimuovere il collegamento a un&#39;attività dalla colonna Nome attività in una visualizzazione attività:

1. Passare a un elenco di attività.
1. Da **Visualizza** menu a discesa, fai clic su **Nuova vista** per creare una nuova visualizzazione.

   Oppure

   Fai clic sul pulsante **Icona Modifica** ![](assets/edit-icon.png)

   per modificare una visualizzazione esistente, selezionarla.

1. Fai clic su **Aggiungi colonna** per aggiungere una nuova colonna.

   Oppure

   Fare clic su una colonna esistente con un collegamento a un oggetto.

1. Fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuovi il testo che trovi nella **Modalità testo** e sostituirlo con il seguente codice:

   <pre>displayname=Nome attività<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >È possibile utilizzare un codice simile per altri oggetti regolando quanto segue:
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



1. Fai clic su **Salva**, quindi **Salva visualizzazione**.
