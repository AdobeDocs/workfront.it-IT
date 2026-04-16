---
content-type: overview
product-area: projects
navigation-topic: financials
title: Definire una proporzione di lavoro straordinario
description: È possibile definire un rapporto di lavoro straordinario per un task per adeguare il calcolo della Retribuzione pianificata per le assegnazioni del task.
author: Lisa
feature: Work Management
exl-id: 832d3aab-3e09-4d83-91a6-be0145ce3554
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 11%

---

# Definire una proporzione di lavoro straordinario

Quando si aggiunge una proporzione di lavoro straordinario a un&#39;attività, questa viene applicata a tutte le assegnazioni dell&#39;attività. Moltiplica tutte le ore pianificate per tale attività e influisce sui calcoli delle retribuzioni pianificate.

Il rapporto di lavoro straordinario non può variare per le assegnazioni all&#39;interno della stessa attività. Se sono necessari moltiplicatori di lavoro straordinario diversi, è necessario creare sottoattività separate in un&#39;attività padre.

>[!NOTE]
>
>Nessuna convalida impedisce l&#39;aggiunta della proporzione di lavoro straordinario a un&#39;attività non straordinaria.

## Calcolo del lavoro straordinario sulla retribuzione pianificata

Il sistema determina innanzitutto la tariffa di fatturazione utilizzando la gerarchia di tariffe di fatturazione standard. Per ulteriori informazioni, vedere [Panoramica sulla gerarchia dei ricavi e dei costi](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Se per l&#39;attività esiste il rapporto di lavoro straordinario, il calcolo è il seguente:
Reddito Pianificato = Tariffa Di Fatturazione × Rapporto Lavoro Straordinario × Ore Pianificate

Se il rapporto di lavoro straordinario è vuoto, il calcolo è:
Reddito Pianificato = Tariffa Di Fatturazione × Ore Pianificate

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td>Flusso di lavoro Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Modifica accesso ad attività, progetti e dati finanziari</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td><p>Gestire le autorizzazioni per un'attività che include Modifica tariffe di fatturazione</p>
     <p>Autorizzazioni Contribute (Contribute) o superiori per il progetto</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Il tipo di retribuzione dell&#39;attività deve essere Ore Utente e Ruolo. Per ulteriori informazioni, vedere [Panoramica sulla gerarchia dei ricavi e dei costi](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

Il campo **Rapporto lavoro straordinario** deve essere abilitato nel modello di layout.

1. Nel modello di layout, fai clic sulla freccia giù sotto **Personalizza gli elementi visualizzati dagli utenti**, quindi fai clic su **Attività**.
1. Nella sezione **Dettagli**, selezionare il campo **Rapporto straordinario** nell&#39;area **Finanza**.

   Per ulteriori informazioni, vedere [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

## Definire la proporzione di lavoro straordinario per un&#39;attività

1. Passare all&#39;attività da modificare.

   Per ulteriori informazioni, vedere [Gestire i dati finanziari delle attività nella sezione Dettagli attività](/help/quicksilver/manage-work/tasks/manage-tasks/task-finances-in-details.md).

1. Fai clic su **Dettagli attività** nel pannello a sinistra.
1. Nell&#39;area **Finanza** immettere il moltiplicatore del lavoro straordinario nel campo **Rapporto lavoro straordinario**.
1. Fai clic su **Salva modifiche**.
