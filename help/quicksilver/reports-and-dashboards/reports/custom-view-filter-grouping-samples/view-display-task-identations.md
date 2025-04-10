---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visualizzazione: visualizzazione dei rientri di attività in un elenco attività'
description: In questa visualizzazione delle attività è possibile aggiungere codice alla colonna Nome attività per visualizzare le attività rientrate in base alla struttura funzionale del progetto.
author: Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Visualizza: visualizza rientri attività in un elenco attività

<!--Audited: 11/2024-->

In questa visualizzazione delle attività è possibile aggiungere codice alla colonna Nome attività per visualizzare le attività rientrate in base alla struttura funzionale del progetto.

![Visualizza rientro attività](assets/view-text-mode-indentation-task-list-350x171.png)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
    <p>Nuovo:</p>
   <ul><li><p>Collaboratore per modificare un filtro </p></li>
   <li><p>Standard per modificare un rapporto</p></li> </ul>

<p>Corrente:</p>
   <ul><li><p>Richiesta di modifica di un filtro </p></li>
   <li><p>Pianificare la modifica di un rapporto</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare i rientri delle attività in una colonna di un elenco di attività

1. Consente di passare a un elenco di attività.
1. Dal menu a discesa **Visualizza**, fare clic su **Nuova visualizzazione**.

1. Fai clic su **Aggiungi colonna** e inizia a digitare &quot;Nome attività&quot; nel campo **Mostra in questa colonna**, quindi selezionalo quando viene visualizzato nell&#39;elenco.

1. Nella nuova colonna fare clic su **Passa alla modalità testo** > **Modifica modalità testo**.
1. Rimuovere il testo trovato nella riga `valuefield=` e sostituirlo con il seguente codice:

   ```
   displayname=Task hierarchy
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Fai clic su **Fine**, quindi su **Salva visualizzazione**.
1. (Facoltativo) Aggiorna il nome della visualizzazione, quindi fai clic su **Salva visualizzazione**.
