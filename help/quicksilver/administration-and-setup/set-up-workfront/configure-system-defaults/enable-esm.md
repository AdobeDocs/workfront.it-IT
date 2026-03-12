---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Abilitare lo storage aziendale Adobe per la tua organizzazione
description: È possibile abilitare lo storage aziendale Adobe per la propria organizzazione per utilizzare una soluzione di storage unificato per tutti i prodotti Adobe.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 97c351ca38a8b6075634b2f755f2330562bc8b52
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 13%

---

# Abilitare lo storage aziendale Adobe per la tua organizzazione

Lo storage aziendale Adobe è una soluzione di storage unificato per tutti i prodotti Adobe. Si tratta di una soluzione di archiviazione basata su cloud che funge da archivio centrale per le risorse tra i prodotti aziendali Adobe.

Lo storage aziendale Adobe è abilitato per impostazione predefinita per i nuovi clienti e può essere abilitato per i clienti esistenti al rinnovo del contratto.

Per ulteriori informazioni sull&#39;archiviazione aziendale Adobe, vedere [Panoramica sull&#39;archiviazione aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Standard</p> <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Abilitare lo storage aziendale Adobe per la tua organizzazione

Per abilitare lo storage aziendale Adobe per la tua organizzazione:

{{step-1-to-setup}}

1. Seleziona **Sistema** nel menu di navigazione a sinistra, quindi seleziona **Preferenze**.
1. Scorri verso il basso fino alla sezione **Preferenze di archiviazione**.
1. Nel menu a discesa Default, selezionare **Adobe enterprise storage**.
1. (Facoltativo) Se si desidera utilizzare una combinazione di storage aziendale Adobe e storage Workfront legacy, selezionare la casella di controllo **Consenti all&#39;utente di selezionare il provider di archiviazione**.

   >[!NOTE]
   >
   >L’attivazione di questa opzione consente agli utenti di selezionare il provider di archiviazione al momento della creazione di un nuovo progetto. lo storage aziendale è etichettato come &quot;Nuovo progetto&quot; in quanto è il provider di storage predefinito. Lo storage Workfront legacy è etichettato come &quot;Progetto legacy&quot;.
   >
   >![nuove opzioni progetto e progetto legacy](assets/new-esm-project.png)

1. Fai clic su **Salva**.