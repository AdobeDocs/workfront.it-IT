---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: visualizza solo gli elementi in stato di approvazione"
description: È possibile visualizzare solo gli elementi con un determinato stato attualmente in In attesa di approvazione. Funziona allo stesso modo per qualsiasi altro oggetto con uno stato di approvazione.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 1%

---

# Filtro: consente di visualizzare solo gli elementi con stato di approvazione

È possibile visualizzare solo gli elementi con un determinato stato attualmente in In attesa di approvazione. Funziona allo stesso modo per qualsiasi altro oggetto con uno stato di approvazione.

È possibile inserire i seguenti oggetti in uno stato di approvazione:

* Attività
* Problemi
* Progetti

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

## Visualizza solo gli elementi nello stato di approvazione

1. Vai al filtro che desideri personalizzare per un elenco di progetti, ad esempio.
1. Clic **Aggiungere una regola di filtro** per **Stato** dell&#39;oggetto dell&#39;elenco.\
   Ad esempio, in un report di progetto, aggiungi **Pianificazione uguale stato**, se desideri visualizzare solo i progetti con stato **Pianificazione - In attesa di approvazione**.

1. Clic **Passa alla modalità testo**.
1. Modifica il

   ```
   status
   ```

   riga mediante aggiunta **:A** alla chiave di 3 lettere dello stato:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Clic **Fine**, quindi **Salva filtro**.

   Nell&#39;elenco vengono visualizzati solo i progetti con stato Pianificazione - In attesa di approvazione.
