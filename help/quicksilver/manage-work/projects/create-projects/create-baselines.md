---
product-area: projects
navigation-topic: create-projects
title: Crea linee di base progetto
description: Una previsione è un'istantanea del progetto che rappresenta le informazioni chiave incluse nel piano di progetto iniziale o in un dato momento durante il ciclo di vita del progetto.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Crea linee di base progetto

<!-- Audited: 12/2023 -->

Una previsione è un&#39;istantanea del progetto che rappresenta le informazioni chiave incluse nel piano di progetto iniziale o in un dato momento durante il ciclo di vita del progetto.

È possibile utilizzare la previsione per confrontare tali informazioni dal piano corrente al piano originale o a qualsiasi altro point-in-time, per identificare le attività problematiche, lo slittamento dell&#39;ambito e altre tendenze nel tempo.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<!--
drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
    <td><p>Nuovo: Standard</p>
        <p>oppure</p>
        <p>Corrente: Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per il progetto o versione successiva per visualizzare le linee di base</p> <p>Gestire le autorizzazioni per il progetto per creare linee di base</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sull&#39;utilizzo delle linee di base

* È possibile acquisire un&#39;istantanea dello stato di avanzamento di un progetto più volte durante la durata del progetto, creando più linee di base.
* È possibile visualizzare le informazioni incluse nelle previsioni di un progetto creando una previsione o creando un rapporto di previsione.
* Quando si crea una previsione, le informazioni sulle attività vengono acquisite anche sulle attività previste della previsione.
* È possibile visualizzare le informazioni sulle attività previste creando un rapporto Attività previste.

>[!IMPORTANT]
>
>Una previsione crea un&#39;istantanea del nome, delle date e delle informazioni finanziarie del progetto. La previsione non include i valori dei campi personalizzati nel progetto. Per informazioni sulle informazioni finanziarie incluse nella previsione, vedere [Dati finanziari del progetto inclusi nelle previsioni del progetto](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Creare una baseline

È possibile creare una baseline nei modi seguenti:

* **Automaticamente**: l&#39;amministratore di Workfront o di un gruppo imposta la preferenza di Workfront per la creazione automatica di una previsione quando un progetto diventa Attuale. Quando questa impostazione è attivata, viene creata una baseline quando lo stato del progetto diventa Attuale. Se questa impostazione non è abilitata, è necessario creare manualmente le baseline.

  Per ulteriori informazioni sulla configurazione delle preferenze di progetto e sulla creazione automatica della linea di base, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  >[!CAUTION]
  >
  >Se si attiva questa impostazione, viene creata automaticamente una previsione per un progetto ogni volta che lo stato di un progetto cambia in Corrente. La prima baseline creata è quella predefinita. È necessario creare manualmente tutte le altre linee di base durante il ciclo di vita del progetto.

* **Manualmente**: è possibile creare nuove linee di base per il progetto in base alle esigenze man mano che il progetto procede. Puoi quindi confrontare le linee di base per vedere come il progetto è progredito nel tempo.

Per creare una baseline:

1. Vai a un progetto.
1. Nel pannello a sinistra, fai clic su **Baseline**.

   ![Sezione previsioni sul progetto](assets/baselines-section-on-project-with-header.png)

1. Fare clic su **Nuova previsione.**
1. Specificare il nome della baseline.
1. (Facoltativo) Se si tratta della prima previsione, è possibile sceglierla come predefinita.
1. Fai clic su **Salva**.

   Per impostazione predefinita, vengono visualizzate le seguenti informazioni sulla baseline creata:

   * Nome linea di base
   * Data voce linea di base
   * Data inizio pianificata del progetto al momento della creazione della previsione
   * Data di inizio prevista del progetto al momento della creazione della previsione
   * Durata effettiva del progetto al momento della creazione della previsione
   * % completamento del progetto al momento della creazione della baseline
   * Indicatore Previsione predefinita che indica se una Previsione è la Predefinita del progetto

     >[!TIP]
     >
     >Non è possibile visualizzare contemporaneamente le informazioni di due baseline nella stessa visualizzazione o nello stesso report. Nello stesso rapporto è possibile visualizzare solo le informazioni di una determinata baseline e della baseline predefinita. È possibile modificare la baseline che si considera essere la baseline predefinita in qualsiasi momento durante la durata del progetto.

1. (Facoltativo) Fai clic sul pulsante **Visualizza**, quindi crea una nuova visualizzazione o modifica la visualizzazione corrente per aggiungere campi alla visualizzazione e confrontare informazioni aggiuntive tra le linee di base. Per informazioni, vedere [Creare o modificare le visualizzazioni in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Creare un report di attività previsto o previsto

Per visualizzare le informazioni sulle previsioni, è inoltre possibile creare un report delle attività previste o previste. In questo modo è possibile visualizzare un numero qualsiasi di campi relativi alle previsioni o alle attività previste per confrontarle in un&#39;unica visualizzazione.

>[!TIP]
>
>È necessario creare una baseline prima di creare un report di attività baseline o baseline.

Per informazioni sulla creazione di un report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

È consigliabile aggiungere un raggruppamento Nome progetto al report Attività linea di base o Previsione per semplificarne la lettura.

Per informazioni sulla creazione di un raggruppamento, vedere [Creare raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).
