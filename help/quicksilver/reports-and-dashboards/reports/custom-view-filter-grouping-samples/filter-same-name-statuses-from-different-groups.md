---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: visualizza gli elementi in base agli stati con lo stesso nome quando gli stati sono associati a gruppi diversi"
description: È possibile assegnare uno stato attività al gruppo A denominato Nuovo stato con la chiave di 3 lettere NST. È possibile che al gruppo B venga assegnato un altro stato di attività denominato anche Nuovo stato con la chiave di 3 lettere NES. Anche se i nomi per i 2 stati possono essere identici, il codice di 3 lettere è sempre univoco. Per ulteriori informazioni sugli stati dei gruppi, vedere Creare o modificare uno stato dei gruppi.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Filtro: consente di visualizzare gli elementi in base agli stati con lo stesso nome quando gli stati sono associati a gruppi diversi

È possibile assegnare uno stato attività al Gruppo A denominato *Nuovo stato* con la chiave di 3 lettere *NST*. È possibile che al gruppo B venga assegnato un altro stato di attività denominato *Nuovo stato* con la chiave di 3 lettere *NO.* Anche se i nomi per i 2 stati possono essere identici, il codice di 3 lettere è sempre univoco.\
Per ulteriori informazioni sugli stati dei gruppi, consulta [Creare o modificare lo stato di un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Utilizzando il generatore di filtri, non è possibile identificare tra i 2 stati che hanno lo stesso nome. È necessario utilizzare la modalità testo per distinguere i due stati.

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
   <td> <p>Richiesta di modifica di un filtro </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Visualizza gli elementi in base agli stati con lo stesso nome quando gli stati sono associati a gruppi diversi

1. Vai al filtro che desideri personalizzare per un elenco di attività, ad esempio.\
   Funziona allo stesso modo anche per progetti e problemi.
1. Clic **Aggiungere una regola di filtro** per **Stato** dell&#39;oggetto dell&#39;elenco.\
   Ad esempio, in un report attività, aggiungere **Stato uguale al nuovo stato**, se si desidera visualizzare solo le attività con stato **Nuovo stato**.

   >[!TIP]
   >
   >Si noti che è disponibile una sola opzione per uno stato denominato Nuovo stato.

1. Clic **Passa alla modalità testo**.\
   Dovrebbe essere visualizzato il seguente codice:

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Qui viene visualizzato un solo stato. Nella riga di stato viene visualizzata una delle chiavi a 3 lettere per uno degli stati.

1. Aggiungi le seguenti 2 righe di codice per aggiungere lo stato mancante dal filtro:

   <pre>OPPURE:1:status=NES<br>OPPURE:1:status_Mod=in</pre>

1. Clic **Fine**, quindi **Salva filtro**.

   Nell&#39;elenco vengono visualizzate entrambe le attività con lo stato &quot;Nuovo stato&quot; dal gruppo A e con lo stato &quot;Nuovo stato&quot; dal gruppo B.
