---
title: Abilitare un Workspace di Workfront Planning in GenStudio for Performance Marketing
description: Se in Adobe Workfront Planning è già disponibile un'area di lavoro, è possibile abilitarla per GenStudio for Performance Marketing anziché ricreare i dati.
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 0bcb6ef2abbf3789339af27119422ef413cd6eef
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 2%
---
# Abilitare un&#39;area di lavoro di Workfront Planning in GenStudio for Performance Marketing

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--
Better metadata, at publishing:
---
title: Promote a Workfront Planning workspace to GenStudio
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can promote a Workfront Planning workspace to GenStudio and have its information visible and updated from both systems.
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->
Oltre a Workfront Planning, se la tua azienda ha acquistato anche Adobe GenStudio for Performance Marketing, l’area di lavoro GenStudio è disponibile in Adobe Workfront Planning quando l’istanza di Workfront viene integrata con l’istanza di GenStudio della tua azienda.

Se si dispone già di un&#39;area di lavoro in Workfront Planning, è possibile abilitarla per GenStudio anziché ricreare i dati.

L’abilitazione di un’area di lavoro la collega a un progetto di archiviazione Adobe e ne mappa i tipi di record e i campi sullo schema dell’area di lavoro GenStudio. Dopo aver completato la configurazione, puoi aprire i record dell’area di lavoro in GenStudio.

Considera i seguenti aspetti:

* È necessario avere accesso sia a Workfront Planning che a GenStudio for Performance Marketing.
* Per collegarti all’area di lavoro, devi disporre di un progetto di archiviazione cloud Adobe. L’amministratore dell’organizzazione può crearne una in Adobe Admin Console.

  Per informazioni, consulta [Gestire l&#39;archiviazione Adobe](https://helpx.adobe.com/it/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html). <!--ensure this site still works-->


## Abilitare un&#39;area di lavoro di Workfront Planning in GenStudio

1. In Workfront Planning aprire l&#39;area di lavoro che si desidera abilitare.
1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome dell&#39;area di lavoro, quindi fai clic su **Abilita GenStudio**.

   La casella **Imposta come area di lavoro GenStudio** abilitata si apre con i seguenti passaggi:

   1. **Progetto ACPC**: seleziona il **Progetto ACPC** (progetto di archiviazione cloud Adobe) da sincronizzare con questa area di lavoro, quindi fai clic su **Avanti**. Gli utenti accedono all’area di lavoro in GenStudio tramite questo progetto.

      ![Abilita il GenStudio dell&#39;area di lavoro - Passaggio del progetto ACPC](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **Tipi di record**: associare i tipi di record dell&#39;area di lavoro ai sei tipi di record richiesti da GenStudio:

      * Campagne
      * Prodotti
      * Persone
      * Canali
      * Aree geografiche
      * Attivazioni

      Per ognuno, aprire l&#39;elenco e selezionare il tipo di record Planning corrispondente oppure selezionare **Aggiungi nuovo** per crearlo, quindi fare clic su **Avanti**.

      ![Abilita GenStudio area di lavoro - Tipi di record, passaggio](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **Campi**: mappa i campi per ogni tipo di record. Utilizzare le schede nella parte superiore della finestra di dialogo per spostarsi tra i tipi di record. Per ogni campo, selezionare il campo Planning corrispondente oppure selezionare **Aggiungi nuovo** per crearlo.

      Ripetere l&#39;impostazione del campo per tutti i tipi di record.

      ![Abilita GenStudio area di lavoro - Passaggio campi](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. Rivedi e risolvi eventuali avvisi.

      Ad esempio, un nuovo campo può diventare il campo principale per il tipo di record oppure un alias di campo già in uso viene rinominato (se disponi già di un campo denominato &quot;Aree&quot;, quello importato potrebbe diventare &quot;Aree 2&quot;).

      La mappatura di un campo **Stato** aggiunge le opzioni richieste.

   1. Fai clic su **Pubblica**.

      Quando l’area di lavoro è abilitata, viene visualizzato un messaggio di conferma. I tipi di record mappati vengono contrassegnati nell&#39;area di lavoro.

      I tipi di record mappati per essere accessibili da GenStudio hanno una nuova icona **Adobe** sulle loro schede.

      ![Tipo di record Campagne con icona Adobe](assets/campaigns-record-type-card-with-adobe-icon.png)

1. Apri GenStudio e seleziona **Campagne**, quindi fai clic sul **progetto ACPC** originariamente configurato per questa installazione nell&#39;angolo inferiore sinistro della schermata. Esaminare i tipi di record e i campi importati.

   >[!TIP]
   >
   >Puoi visualizzare solo i record consentiti dall’iscrizione al progetto ACPC.
