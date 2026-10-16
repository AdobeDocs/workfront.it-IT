---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Conversione di oggetti legacy in Adobe Cloud Storage
description: Scopri i tre casi in cui puoi convertire un oggetto di archiviazione Workfront legacy in archiviazione cloud Adobe e cosa rimane durante ogni conversione.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---
# Conversione di oggetti legacy in Adobe Cloud Storage

Nella maggior parte degli scenari, è possibile spostare, copiare e convertire oggetti Workfront solo tra modelli di memorizzazione simili. Ad esempio, puoi spostare un’attività da un progetto di archiviazione cloud Adobe a un altro progetto di archiviazione cloud Adobe. In tre casi specifici, puoi convertire un oggetto di archiviazione Workfront legacy in archiviazione cloud Adobe:

* Convertire un’attività di archiviazione Workfront legacy in un progetto di archiviazione cloud Adobe
* Conversione di un portfolio di storage Workfront legacy in un portfolio di storage cloud Adobe
* Creare un progetto di archiviazione cloud Adobe da un modello di archiviazione Workfront legacy

Per informazioni sull&#39;orientamento per lo spostamento e sulle differenze nell&#39;archiviazione cloud Adobe, consulta [Sposta in Workfront nell&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

<!-- 
need to validate with PM
>[!NOTE]
>
>In all three conversion scenarios, documents and document folders don't move from legacy Workfront storage to Adobe cloud storage. Documents that exist on the legacy object before the conversion remain on legacy storage.
-->

## Convertire un’attività legacy in un progetto di archiviazione cloud Adobe

Per convertire un’attività di archiviazione Workfront legacy in un progetto di archiviazione cloud Adobe, utilizza il flusso di conversione in progetto esistente per l’attività. Durante la conversione:

* Le sottoattività e i problemi vengono spostati nel nuovo progetto.
* I documenti allegati all&#39;attività e i relativi flussi di lavoro di approvazione rimangono sul progetto originale.
* Le approvazioni del lavoro e i collegamenti agli oggetti di risoluzione vengono rimossi.
* L&#39;attività originale viene eliminata.

## Convertire un portfolio legacy in un portfolio di archiviazione cloud Adobe

Un amministratore Workfront può convertire un portfolio di archiviazione Workfront legacy in un portfolio di archiviazione cloud Adobe dall’area di configurazione. Dopo la conversione:

* Non è più possibile spostare i progetti di storage Workfront legacy nel portfolio.
* Tutti i nuovi progetti creati nel portfolio utilizzano l’archiviazione cloud Adobe.
* Frame.io è il visualizzatore di documenti nei progetti di archiviazione cloud Adobe del portfolio.
* I progetti secondari che utilizzano lo storage legacy Workfront rimangono sullo storage legacy.
* I programmi secondari rimangono nell&#39;archiviazione legacy.

>[!NOTE]
>
>Un programma legacy secondario viene convertito automaticamente in Adobe Cloud Storage solo quando qualcuno vi aggiunge manualmente un progetto Adobe Cloud Storage.

Per ulteriori informazioni, consulta [Convertire i portfolio legacy in Adobe Cloud Storage](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md).

## Creare un progetto di archiviazione cloud Adobe da un modello legacy

Quando crei un progetto da un modello di archiviazione Workfront legacy, la casella di controllo **Crea il progetto nell&#39;archiviazione cloud Adobe** nella finestra di dialogo di creazione del progetto determina il tipo di archiviazione del nuovo progetto. Il comportamento della casella di controllo dipende dalla posizione in cui viene creato il progetto:

* **Esterno a un portfolio**: la casella di controllo è disponibile e deselezionata per impostazione predefinita. Selezionala per creare il nuovo progetto sull’archiviazione cloud Adobe.
* **All&#39;interno di un portfolio di archiviazione cloud Adobe**: la casella di controllo è selezionata e bloccata. Il nuovo progetto deve corrispondere al tipo di archiviazione del portfolio.
* **In un portfolio di archiviazione legacy di Workfront**: la casella di controllo non è disponibile. Il nuovo progetto utilizza lo storage legacy Workfront.

Per ulteriori informazioni, vedere [Creare progetti](/help/quicksilver/manage-work/projects/create-projects/create-project.md).
