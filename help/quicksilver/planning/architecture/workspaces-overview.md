---
title: Panoramica delle aree di lavoro
description: Un'area di lavoro è una raccolta di tipi di record utilizzati da un team e rappresenta il ciclo di vita del lavoro del team. In Adobe Workfront Planning è possibile personalizzare completamente le aree di lavoro in modo che corrispondano ai flussi di lavoro delle unità organizzative.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
TQID: https://experienceleague.adobe.com/Hh1Gh4ex1dLrPhsmqiLv3x5NAU0yKzIwcsV4hEogXTo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: 4ac828444e49213cdc4e00a5f92e404899e2225d
workflow-type: tm+mt
source-wordcount: 608
ht-degree: 3%

---

# Panoramica delle aree di lavoro

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo il rilascio in anteprima, le stesse funzioni sono disponibili mensilmente nell’ambiente di produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Un’area di lavoro è una raccolta di tipi di record utilizzati da un’unità organizzativa che rappresenta il ciclo di vita lavorativa e i processi dell’unità. È possibile personalizzare completamente le aree di lavoro in Adobe Workfront Planning.

<!--update screenshot with production, it was broken at Preview-->

![Account amministratore pagina di destinazione aree di lavoro](assets/workspaces-landing-page-admin-account.png)

## Considerazioni sulle aree di lavoro

* Puoi creare aree di lavoro per specifiche unità organizzative all’interno dell’organizzazione, in base al funzionamento univoco di ciascuna unità.
* Workfront Planning non include aree di lavoro preconfigurate. Devi crearli in base alle esigenze della tua organizzazione.
* È possibile creare aree di lavoro nei modi seguenti:

   * Da zero
   * Utilizzo di un modello. I modelli contengono un numero preconfigurato di tipi di record e i relativi campi.
   * Utilizzo di Planning Designer basato sull’intelligenza artificiale. Questa funzione è attualmente in Beta.
   * Utilizzo di un bundle di modelli per più aree di lavoro.

  Per informazioni, consulta [Creare le aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

* Le aree di lavoro sono strutture all’interno delle quali lavorano le unità organizzative (un team, un gruppo, un reparto o una divisione). Non possono essere associati a campi. Solo i tipi di record all&#39;interno di un&#39;area di lavoro possono essere associati ai campi.

  Per informazioni, vedere [Panoramica sui tipi di record](/help/quicksilver/planning/architecture/overview-of-record-types.md).
* Le aree di lavoro vengono visualizzate nelle seguenti schede nell&#39;area Pianificazione:

   * **Aree di lavoro in cui si trova**: visualizza le aree di lavoro create dall&#39;utente o condivise con l&#39;utente.
   * **Altre aree di lavoro**: mostra tutte le altre aree di lavoro nel sistema. Questa opzione è disponibile solo per gli amministratori di sistema.
   * <span class="preview">**Aree di lavoro di esempio**: visualizza esempi incorporati di aree di lavoro basate su best practice. Non è possibile modificare le aree di lavoro, i tipi di record o aggiungere record o campi, ma è possibile aggiungere, modificare e condividere visualizzazioni con altri utenti.</span>

  >[!NOTE]
  >
  ><span class="preview">È consigliabile non modificare le aree di lavoro di esempio, ma utilizzarle come riferimento per crearne di personalizzate. Utilizza il bundle di modelli per più aree di lavoro per creare aree di lavoro identiche a quelle elencate nella scheda Aree di lavoro di esempio. Per informazioni, vedere la sezione &quot;Creare più aree di lavoro utilizzando un bundle di modelli multisfera basato sulle best practice&quot; nell&#39;articolo [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md). </span>

<!--
No longer the case - they match now: 

* For all other users:

* **Workspaces I'm on**: Workspaces they created (for Standard-license users) and workspaces others shared with them display in the Workspaces area.

<div class="preview"> 

* **Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.

</div>
-->



* I tipi di record contenuti in un&#39;area di lavoro devono riflettere il ciclo di vita lavorativa e i concetti di un&#39;unità organizzativa.

  Ad esempio, se gli oggetti di lavoro di un’unità sono campagne, prodotti e aree geografiche, il workspace di tale unità deve contenere i tipi di record Campaign, Product e Region.
* Quando crei un’area di lavoro, solo tu disponi dell’autorizzazione per accedere a essa e gestirla. È necessario condividerlo con altri utenti affinché possano collaborare con te nello stesso spazio.

  Per informazioni, vedere [Condividere un&#39;area di lavoro](/help/quicksilver/planning/access/share-workspaces.md).

  Gli amministratori di sistema possono gestire tutte le aree di lavoro, anche quelle che non hanno creato.

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* Il numero di oggetti del workspace che è possibile creare nell&#39;istanza di Workfront Planning è limitato. Per informazioni, vedere [Panoramica delle limitazioni degli oggetti di Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).

## Panoramica sulla ricerca globale

Nella pagina di destinazione di Planning è possibile utilizzare la casella di ricerca globale per cercare i seguenti oggetti di Planning:

* Aree di lavoro
* Tipi di record
* Viste

![Casella di ricerca globale](assets/global-search-box.png)

Considera quanto segue sull’utilizzo della ricerca globale:

* È possibile accedere alla ricerca dalla pagina di destinazione di Planning o da qualsiasi pagina di Planning premendo la seguente combinazione di tastiera:

   * CTRL+K per Windows
   * ⌘+K per Mac
* Gli ultimi 7 risultati di ogni oggetto vengono visualizzati nella casella di ricerca.
* È possibile eseguire una ricerca generale oppure selezionare un oggetto e cercare singoli elenchi.


