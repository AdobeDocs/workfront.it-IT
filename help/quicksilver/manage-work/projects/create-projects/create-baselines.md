---
product-area: projects
navigation-topic: create-projects
title: Creare le linee di base dei progetti
description: Una linea di base è un’istantanea del progetto che rappresenta le informazioni chiave incluse nel piano di progetto iniziale o in un dato momento durante la durata del progetto.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Creare le linee di base dei progetti

Una linea di base è un’istantanea del progetto che rappresenta le informazioni chiave incluse nel piano di progetto iniziale o in un dato momento durante la durata del progetto.

È possibile utilizzare la linea di base per confrontare le informazioni del piano corrente con il piano originale o qualsiasi altro momento nel tempo, per identificare le attività che presentano problemi, il margine di scorrimento e altre tendenze nel tempo.

## Requisiti di accesso

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

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p><b>NOTA</b>
   Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull'accesso ai progetti, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concedere l’accesso ai progetti</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza le autorizzazioni per il progetto o versioni successive per visualizzare le linee di base</p> <p>Gestisci le autorizzazioni per il progetto per creare linee di base</p> <p> Per informazioni sulle autorizzazioni del progetto, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Condivisione di un progetto in Adobe Workfront</a>.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sull’utilizzo delle linee di base

* È possibile acquisire un’istantanea dell’avanzamento di un progetto più volte durante la sua durata, creando più linee di base.
* È possibile visualizzare le informazioni incluse nelle linee di base di un progetto creando una baseline o creando un report di baseline.
* Quando si crea una baseline, le informazioni sull&#39;attività vengono acquisite anche sulle attività della baseline della baseline.
* È possibile visualizzare le informazioni sulle attività della linea di base creando un rapporto sulle attività della linea di base.

>[!IMPORTANT]
>
>Una baseline acquisisce un&#39;istantanea del nome, delle date e delle informazioni finanziarie del progetto. La baseline non include i valori dei campi personalizzati nel progetto. Per informazioni sulle informazioni finanziarie incluse nella linea di base, vedi [Finanze del progetto incluse nelle linee di base del progetto](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Creare una baseline

Puoi creare una baseline nei seguenti modi:

* **Automaticamente**: L’amministratore di Workfront o un amministratore di gruppo imposta le preferenze di progetto affinché Workfront crei automaticamente una linea di base quando un progetto diventa corrente. Quando questa impostazione è abilitata, viene creata una baseline quando lo stato del progetto diventa Corrente. Se questa impostazione non è abilitata, devi creare manualmente le linee di base.

   Per ulteriori informazioni sulla configurazione delle preferenze di progetto e sulla configurazione della creazione automatica della linea di base, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   >[!CAUTION]
   >
   >Attivando questa impostazione si crea automaticamente una baseline per un progetto ogni volta che lo stato di un progetto diventa Corrente. La prima baseline creata è quella predefinita. È necessario creare manualmente tutte le altre linee di base durante la durata del progetto .

* **Manualmente**: Puoi creare nuove linee di base per il progetto, in base alle esigenze, mentre il progetto progredisce. Puoi quindi confrontare le linee di base per vedere come si è evoluto il progetto nel tempo.

Per creare una baseline:

1. Passa a un progetto.
1. Nel pannello a sinistra, fai clic su **Linee di base**.

   Oppure

   Fai clic su **Mostra altro**, quindi fai clic su **Linee di base**.

   ![](assets/nwe-baselines-section-on-project-with-header-350x78.png)

1. Fai clic su **Nuova linea di base.**
1. Specifica il nome della baseline.
1. (Facoltativo) Se si tratta della prima linea di base, è possibile sceglierla come predefinita.
1. Fai clic su **Salva**.

   Per impostazione predefinita, vengono visualizzate le seguenti informazioni sulla baseline creata:

   * Nome della linea di base
   * Data di ingresso linea di base
   * Data di inizio pianificata del progetto quando è stata creata la baseline
   * Data di inizio prevista del progetto quando è stata creata la baseline
   * Durata effettiva del progetto quando è stata creata la baseline
   * % Completato del progetto quando è stata creata la baseline
   * Indicatore Linea di base predefinita che mostra se una linea di base è la linea di base predefinita del progetto

      >[!TIP]
      >
      >Non è possibile visualizzare le informazioni di due linee di base contemporaneamente nella stessa visualizzazione o nello stesso rapporto. È possibile visualizzare le informazioni solo da una data linea di base e dalla linea di base predefinita nello stesso rapporto. È possibile modificare la baseline che si considera predefinita in qualsiasi momento durante la durata del progetto.

1. (Facoltativo) Fai clic sulla freccia a discesa accanto alla vista, quindi **Personalizza visualizzazione** per aggiungere campi alla visualizzazione e confrontare informazioni aggiuntive tra le linee di base.

## Creare un rapporto Previsione o Attività prevista

Per visualizzare le informazioni della linea di base, è inoltre possibile creare un rapporto Previsione o Attività linea di base. Ciò consente di visualizzare un numero qualsiasi di campi relativi alle linee di base o alle attività della linea di base per confrontarli in un’unica vista.

>[!TIP]
>
>È necessario creare una baseline prima di poter creare un report Previsione o Attività linea di base.

Per informazioni sulla creazione di un rapporto, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

È consigliabile aggiungere un raggruppamento Nome progetto al rapporto Linea di base o Linea di base per facilitarne la lettura.

Per informazioni sulla creazione di un raggruppamento, consulta [Creare raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).
