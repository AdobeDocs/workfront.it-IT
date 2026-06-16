---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Aggiungere progetti a un Portfolio
description: È consigliabile aggiungere progetti ai portfolio quando vengono avviati. Tuttavia, puoi aggiungerli a un portfolio in qualsiasi momento della loro durata.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 97f36c18-3ac8-45ac-b5bc-dfe8b1363faf
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UkUQdW12tLqRjh5zmbwtjNfRxFwc-Uhj2gGwjmDyKb8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 397e5e36632872bb7be3f4e219b36e33b44136e9
workflow-type: tm+mt
source-wordcount: 674
ht-degree: 3%

---

# Aggiungere progetti a un portfolio

<!--Audited: 08/2025-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

È consigliabile aggiungere progetti ai portfolio quando vengono avviati. Tuttavia, puoi aggiungerli a un portfolio in qualsiasi momento della loro durata.

Quando aggiungi progetti ai portfolio, tieni presente quanto segue:

* È possibile associare un solo portfolio a un progetto.
* Un progetto rimane in un portfolio fino a quando non viene rimosso o associato a un altro portfolio.
* Un portfolio può contenere un numero illimitato di progetti.

>[!CAUTION]
>
>Le autorizzazioni ereditate potrebbero non essere applicate correttamente se utilizzate in un numero elevato di oggetti figlio.
>   
>Per evitare problemi di autorizzazioni ereditati, consigliamo quanto segue:
>
>* Limita il numero di oggetti figlio (progetti) sotto un singolo elemento padre (portfolio o programma). È consigliabile non più di 10.000 progetti per portfolio o programma.
>
>* Riduci la profondità dell’ereditarietà applicando le autorizzazioni a un oggetto di livello inferiore.
>
>  Ad esempio, applica le autorizzazioni direttamente a livello di progetto, anziché fare affidamento sulle autorizzazioni ereditate dal portfolio al programma e quindi al progetto.
>
>* Dividere i programmi in modo che contengano meno progetti, riducendo la complessità delle autorizzazioni.
>


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] pacchetto</td> 
   <td> <p>Qualsiasi</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td><p>Standard</p> 
   <p>[!UICONTROL Piano] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Portafogli di accesso a [!UICONTROL Edit]</p> <p>Accesso [!UICONTROL Edit] ai progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Autorizzazioni di [!UICONTROL Manage] per il portfolio</p> <p>Autorizzazioni [!UICONTROL Manage] per i progetti</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>[!UICONTROL Edit] access Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>[!UICONTROL Manage] permissions to the projects</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Aggiungere un progetto a un portfolio

1. Vai a un portfolio, quindi fai clic su **[!UICONTROL Progetti]** nel pannello a sinistra.

   ![Portfolio con progetti](assets/qs-portfolio-with-projects-350x90.png)

1. Fare clic su **[!UICONTROL Nuovo progetto]** e selezionare un metodo per aggiungere un progetto.

   >[!TIP]
   >
   >Impossibile aggiungere un progetto quando si visualizza l&#39;elenco dei progetti nella visualizzazione [!UICONTROL Milestone].

   Selezionare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody>

   <tr> 
      <td role="rowheader">[!UICONTROL Nuovo Progetto]</td> 
      <td> <p>Aggiungi un nuovo progetto. </p> <p>Per ulteriori informazioni sulla creazione di un progetto, vedere <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Creare un progetto</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nuovo progetto (archiviazione legacy)]</td> 
      <td> <p>Aggiungi un nuovo progetto di archiviazione Workfront. </p>
      <p>L’opzione è visibile solo se l’organizzazione utilizza sia l’archiviazione cloud dei documenti Workfront che Adobe. È possibile che l'istanza Workfront non disponga di entrambi i tipi di archiviazione.</p>
       <p>Per ulteriori informazioni sulla creazione di un progetto, vedere <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Creare un progetto</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nuovo progetto da modello]</td> 
      <td> <p>Aggiungi un nuovo progetto utilizzando un modello esistente. </p> <p>Per ulteriori informazioni sulla creazione di un progetto da un modello, vedere <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Creare un progetto utilizzando un modello</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Importa [!DNL MS Project]] </td> 
      <td> <p>Aggiungere un progetto esportato in precedenza da [!DNL MS Project] e salvato nel computer. </p> <p>Per ulteriori informazioni sulla creazione di un nuovo progetto importandolo da [!DNL Microsoft Project], vedere <a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">Importare un progetto da [!DNL Microsoft Project]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Project]</td> 
      <td> <p>Richiesta di approvazione di un progetto.</p> <p>Per informazioni sulla richiesta di progetti, vedere <a href="../../../manage-work/projects/create-projects/request-project.md">Richiesta di un progetto</a>. </p> </td> 
     </tr> 
          <tr> 
      <td role="rowheader">[!UICONTROL Progetto Esistente]</td> 
      <td> <p>Aggiungi un progetto già creato.</p> </td> 
     </tr>
    </tbody> 
   </table>

   <!-- update screen shot for both kinds of storages??-->

   ![Menu a discesa Nuovo progetto](assets/new-project-dropdown-expanded-from-portfolio-nwe-350x376.png)

1. (Condizionale) Se hai selezionato di aggiungere un progetto esistente, viene visualizzata la casella **Aggiungi progetti**. <!--check this after UI changes-->

   ![Aggiungi progetto esistente](assets/add-existing-projects-to-portfolios-box.png) <!--check this after UI changes-->

1. Inizia a digitare il nome di un progetto nel campo **[!UICONTROL Aggiungi progetti a questo portfolio]**, quindi fai clic su di essi quando compaiono nell&#39;elenco.  <!--check this after UI changes-->

   È possibile aggiungere più progetti.

   >[!NOTE]
   >
   >Quando l’organizzazione utilizza sia l’archiviazione cloud legacy di Workfront che Adobe per i documenti, esistono i seguenti scenari:
   >
   >
   >* Non puoi aggiungere un progetto di archiviazione legacy a un portfolio di archiviazione cloud Adobe o un progetto di archiviazione cloud Adobe a un portfolio di archiviazione legacy.
   >* Non puoi creare un progetto da un modello di archiviazione cloud Adobe in un portfolio di archiviazione legacy.
   >* Puoi creare un progetto da un modello di archiviazione legacy in un portfolio di archiviazione cloud Adobe, ma i documenti e le cartelle presenti nel modello non vengono aggiunti al nuovo progetto. Il progetto riceve l’archiviazione cloud di Adobe.
   >
   >Per ulteriori informazioni, vedere [Panoramica sulla gestione dei documenti per progetti e oggetti correlati](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).
   >
   >Non tutte le istanze di Workfront dispongono di entrambi i tipi di archiviazione dei documenti.


1. (Facoltativo) Se decidi di non aggiungerlo al portfolio, fai clic sull&#39;icona **X** a destra del nome del progetto per rimuoverlo dall&#39;elenco.

   <!--replace last step with this, for unshim: 1. (Optional) Click the **Delete** icon ![Delete icon](assets/delete-icon.png) next to the name of a project if you decide not to add it to the portfolio.-->

1. Fai clic su **[!UICONTROL Aggiungi progetti]**. <!--check this after UI changes-->

   Il progetto o i progetti selezionati sono ora associati al portfolio.
