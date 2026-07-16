---
product-area: documents
navigation-topic: manage-documents
title: Verificare i limiti di archiviazione dei documenti
description: In qualità di amministratore di Adobe Workfront, puoi visualizzare l’utilizzo e la quota di archiviazione dei documenti nella pagina Informazioni cliente. La modalità di visualizzazione dell’archiviazione dipende dal fatto che l’organizzazione utilizzi l’archiviazione Workfront legacy o l’archiviazione cloud Adobe.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/vOjgBLxX5rFIGHBCHB2a6Q3Bs3KE5x-opXUMvANjI1E
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 09dff59503604894e61f2a62af7ae1c2e8a39068
workflow-type: tm+mt
source-wordcount: 491
ht-degree: 9%

---

# Verificare i limiti di archiviazione dei documenti

Anche se non esistono restrizioni sui tipi e sulle dimensioni dei singoli file che gli utenti possono caricare nell’istanza di Workfront, il piano Workfront include una quota di archiviazione totale. In qualità di amministratore di Workfront, puoi monitorare l’utilizzo e la quota dall’area Configurazione della pagina Informazioni cliente.

La modalità di visualizzazione dell’archiviazione dipende dal fatto che l’organizzazione utilizzi l’archiviazione legacy Workfront o l’archiviazione cloud Adobe:

* Se utilizzi l&#39;archiviazione legacy di Workfront, vedi [Archiviazione legacy di Workfront](#legacy-workfront-storage) in questo articolo.
* Se utilizzi l&#39;archiviazione cloud Adobe, vedi [Archiviazione cloud Adobe](#adobe-cloud-storage) in questo articolo.

  Per ulteriori informazioni sull&#39;archiviazione cloud Adobe, consulta [Panoramica sull&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">piano Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workfront per gestire i documenti utilizzando lo storage legacy</p>
      <p>Qualsiasi pacchetto di flusso di lavoro per gestire i documenti utilizzando l’archiviazione cloud Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Archiviazione legacy di Workfront

Se l&#39;organizzazione utilizza un sistema di storage Workfront legacy, nella pagina Informazioni cliente viene visualizzata una quota singola per i documenti caricati direttamente in Workfront.

Per controllare l&#39;archiviazione dei documenti Workfront legacy:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Sistema** > **Informazioni cliente**.
1. Nella sezione **Informazioni di base**, trovare **Quota di archiviazione**. Qui è possibile visualizzare la quantità di storage attualmente utilizzata e la quantità totale di storage inclusa nel piano Workfront.

La quota di archiviazione viene aggiornata quotidianamente per mostrare il conteggio più aggiornato.

>[!NOTE]
>
>Questo limite non si applica ai documenti collegati a Workfront da altri provider di servizi di terze parti (SharePoint, Google Drive, Webdam, Box, Dropbox o qualsiasi altro provider di gestione di risorse di documenti).

## Archiviazione cloud Adobe


Se la tua organizzazione utilizza l’archiviazione cloud Adobe, la quota di archiviazione viene segnalata come un’unica allocazione in pool che combina l’archiviazione fornita tramite la licenza Workfront e qualsiasi archiviazione fornita tramite un componente aggiuntivo Frame.io Enterprise. Non esiste un limite massimo per l&#39;utilizzo dello storage; gli utenti possono continuare a caricare i documenti anche quando l&#39;utilizzo supera la quota.

### Visualizzazione dell&#39;utilizzo dello storage nelle informazioni del cliente

Per verificare la presenza di documenti nell’archiviazione cloud di Adobe:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Sistema** > **Informazioni cliente**.
1. Passare alla sezione **Panoramica archiviazione**.
1. Controlla l’utilizzo. La panoramica dello storage mostra la quota di storage in pool e suddivide l&#39;utilizzo in:

   * I progetti legacy di Workfront e i progetti di Adobe cloud storage vengono visualizzati nella barra blu.
   * I progetti autonomi con frame vengono visualizzati nella barra verde. Questi progetti sono separati da Workfront e sono disponibili solo se si dispone di una licenza Frame.io Enterprise.


![Utilizzo dell&#39;archiviazione cloud Adobe nelle informazioni sul cliente](assets/storage-usage.png)

I dati di utilizzo vengono aggiornati regolarmente in modo da visualizzare un conteggio aggiornato.

### Notifiche e-mail per gli amministratori

Quando l&#39;utilizzo supera il 75%, 90% o 100% della quota di storage, Workfront invia una notifica e-mail agli amministratori di sistema.
