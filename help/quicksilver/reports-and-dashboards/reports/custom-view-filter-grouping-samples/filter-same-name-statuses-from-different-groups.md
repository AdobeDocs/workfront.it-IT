---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filtro: visualizza gli elementi in base allo stato dello stesso nome quando gli stati sono associati a gruppi diversi'
description: È possibile assegnare uno stato attività al gruppo A denominato Nuovo stato con la chiave NST a 3 lettere. È possibile che al gruppo B sia stato assegnato un altro stato di attività denominato Nuovo stato con la chiave NES a 3 lettere. Anche se i nomi dei 2 stati possono essere identici, il codice a 3 lettere è sempre univoco. Per ulteriori informazioni sugli stati del gruppo, vedere Creare o modificare uno stato del gruppo.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Filtro: visualizza gli elementi in base allo stato dello stesso nome quando gli stati sono associati a gruppi diversi

È possibile assegnare uno stato attività al gruppo A denominato *Nuovo stato* con la chiave a 3 lettere *NST*. È possibile assegnare un altro stato attività al Gruppo B anche denominato *Nuovo stato* con la chiave a 3 lettere *NES.* Anche se i nomi dei 2 stati possono essere identici, il codice a 3 lettere è sempre univoco.\
Per ulteriori informazioni sugli stati del gruppo, consulta [Creare o modificare uno stato di gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Con il generatore di filtri non è possibile identificare tra i 2 stati con lo stesso nome. È necessario utilizzare la modalità Testo per distinguere i due stati.

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

## Visualizza gli elementi in base allo stato dello stesso nome quando gli stati sono associati a gruppi diversi

1. Passa al filtro che desideri personalizzare per un elenco di attività, ad esempio.\
   Questo funziona allo stesso modo anche per i progetti e i problemi.
1. Fai clic su **Aggiungere una regola filtro** per **Stato** campo dell&#39;oggetto dell&#39;elenco.\
   Ad esempio, in un rapporto attività, aggiungi **Stato uguale a nuovo stato**, se si desidera visualizzare solo le attività che si trovano in uno stato di **Nuovo stato**.

   >[!TIP]
   >
   >Si noti che si dispone di una sola opzione per uno stato denominato Nuovo stato.

1. Fai clic su **Passa alla modalità testo**.\
   Dovrebbe essere visualizzato il seguente codice:

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Viene visualizzato un solo stato. Nella riga di stato viene visualizzata una delle chiavi a 3 lettere per uno degli stati.

1. Aggiungi le 2 seguenti righe di codice per aggiungere lo stato mancante dal filtro:

   <pre>O:1:status=NES<br>O:1:status_Mod=in</pre>

1. Fai clic su **Fine**, quindi **Salva filtro**.

   Nell&#39;elenco sono visualizzate entrambe le attività con lo stato &quot;Nuovo stato&quot; dal gruppo A e con lo stato &quot;Nuovo stato&quot; dal gruppo B.
