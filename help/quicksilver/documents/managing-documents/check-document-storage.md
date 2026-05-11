---
product-area: documents
navigation-topic: manage-documents
title: Verificare i limiti di archiviazione dei documenti
description: In qualità di amministratore di Adobe Workfront, puoi visualizzare l’utilizzo e la quota di archiviazione dei documenti nella pagina Informazioni cliente. La visualizzazione dello storage dipende dal fatto che l'organizzazione utilizzi lo storage legacy Workfront o lo storage aziendale Adobe.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7b6d24d6a5b7fd052a3e7c97034e920e771022a6
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 8%

---

# Verificare i limiti di archiviazione dei documenti

{{highlighted-preview}}

Anche se non esistono restrizioni sui tipi e sulle dimensioni dei singoli file che gli utenti possono caricare nell’istanza di Workfront, il piano Workfront include una quota di archiviazione totale. In qualità di amministratore di Workfront, puoi monitorare l’utilizzo e la quota dall’area Configurazione della pagina Informazioni cliente.

La visualizzazione dello storage dipende dal fatto che l’organizzazione utilizzi lo storage legacy Workfront o lo storage aziendale Adobe:

* Se utilizzi l&#39;archiviazione legacy di Workfront, vedi [Archiviazione legacy di Workfront](#legacy-workfront-storage) in questo articolo.
* Se utilizzi l&#39;archiviazione aziendale Adobe, vedi [Archiviazione aziendale Adobe](#adobe-enterprise-storage) in questo articolo.

  Per ulteriori informazioni sull&#39;archiviazione aziendale, vedere [Panoramica sull&#39;archiviazione aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">piano Workfront</td> 
   <td> <p>Qualsiasi pacchetto Workfront per gestire i documenti utilizzando lo storage legacy</p>
      <p>Qualsiasi pacchetto di flusso di lavoro per gestire i documenti utilizzando lo storage aziendale Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Storage Workfront legacy

Se l&#39;organizzazione utilizza un sistema di storage Workfront legacy, nella pagina Informazioni cliente viene visualizzata una quota singola per i documenti caricati direttamente in Workfront.

Per controllare l&#39;archiviazione dei documenti Workfront legacy:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Sistema** > **Informazioni cliente**.
1. Nella sezione **Informazioni di base**, trovare **Quota di archiviazione**. Qui è possibile visualizzare la quantità di storage attualmente utilizzata e la quantità totale di storage inclusa nel piano Workfront.

La quota di archiviazione viene aggiornata quotidianamente per mostrare il conteggio più aggiornato.

>[!NOTE]
>
>Questo limite non si applica ai documenti collegati a Workfront da altri provider di servizi di terze parti (SharePoint, Google Drive, Webdam, Box, Dropbox o qualsiasi altro provider di gestione di risorse di documenti).

<div class="preview">

## Storage aziendale Adobe

<!--
If your organization uses Adobe enterprise storage, your storage quota is reported as a single pooled allocation that combines storage provisioned through your V2 Workfront SKU and any storage provisioned through a Frame.io Enterprise SKU or add-on. There's no hard cap on storage usage; users can continue uploading documents even when usage exceeds your quota.

Beginning with the May 2026 release, you can view your pooled storage quota and a usage breakdown on the Customer Info page.

-->

### Visualizzazione dell&#39;utilizzo dello storage nelle informazioni del cliente

Per controllare l&#39;archiviazione di documenti aziendali Adobe:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Sistema** > **Informazioni cliente**.
1. Passare alla sezione **Panoramica archiviazione**.
1. Controlla l’utilizzo. La panoramica dello storage mostra la quota di storage in pool e suddivide l&#39;utilizzo in:

   * I progetti legacy di Workfront e i progetti di storage aziendale Adobe vengono visualizzati nella barra blu.
   * I progetti autonomi con frame vengono visualizzati nella barra verde. Questi progetti sono separati da Workfront e sono disponibili solo se si dispone di una licenza Frame.io Enterprise.


![Utilizzo dello storage aziendale Adobe nelle informazioni sul cliente](assets/storage-usage.png)

I dati di utilizzo vengono aggiornati regolarmente in modo da visualizzare un conteggio aggiornato.

### Notifiche e-mail per gli amministratori

Quando l&#39;utilizzo supera il 75%, 90% o 100% della quota di storage, Workfront invia una notifica e-mail agli amministratori di sistema.

</div>