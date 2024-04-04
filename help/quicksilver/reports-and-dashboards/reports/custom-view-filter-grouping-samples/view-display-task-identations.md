---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualizzazione: visualizzazione dei rientri delle attività in un elenco attività"
description: In questa visualizzazione delle attività è possibile aggiungere codice alla colonna Nome attività per visualizzare le attività rientrate in base alla struttura funzionale del progetto.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Visualizza: visualizza rientri attività in un elenco attività

In questa visualizzazione delle attività è possibile aggiungere codice alla colonna Nome attività per visualizzare le attività rientrate in base alla struttura funzionale del progetto.

![](assets/view-text-mode-indentation-task-list-350x171.png)

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

## Visualizzare i rientri delle attività in una colonna di un elenco di attività

1. Consente di passare a un elenco di attività.
1. Dalla sezione **Visualizza** menu a discesa, fai clic su **Nuova visualizzazione**.

1. Clic **Aggiungi colonna** e inizia a digitare &quot;Task Name&quot; (Nome attività) nel **Mostra in questa colonna** quindi selezionarlo quando viene visualizzato nell&#39;elenco.

1. Dalla nuova colonna, fai clic su **Passa alla modalità testo**.
1. Passa il puntatore del mouse sull’area della modalità testo e fai clic su **Fare clic per modificare il testo**.
1. Rimuove il testo trovato in `valuefield=` e sostituirla con il seguente codice:

   ```
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Clic **Salva**, quindi **Salva visualizzazione**.
