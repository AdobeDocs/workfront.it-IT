---
product-area: projects;templates
navigation-topic: create-projects
title: Creare un progetto utilizzando un modello
description: Puoi utilizzare i modelli come framework per creare progetti. Se i progetti vengono ripetuti spesso, l’utilizzo di modelli per la timeline generale del nuovo progetto evita di dover creare ripetutamente gli stessi progetti.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: e38411056b3f9be6d0241ee18e71984ef2a678a0
workflow-type: tm+mt
source-wordcount: '1104'
ht-degree: 0%

---

# Creare un progetto utilizzando un modello

Puoi utilizzare i modelli come framework per creare progetti. Se i progetti vengono ripetuti spesso, l’utilizzo di modelli per la timeline generale del nuovo progetto evita di dover creare ripetutamente gli stessi progetti.

I modelli consentono di acquisire processi, informazioni e impostazioni ripetibili associati ai progetti. Le informazioni associate a un modello vengono trasferite al progetto. Ciò include attività, assegnazioni, durate, documenti, dettagli finanziari, rischi e moduli personalizzati.

>[!TIP]
>
>Workfront definisce il gruppo e lo stato del nuovo progetto come segue:
>
>* Lo stato predefinito di un nuovo progetto creato da un modello corrisponde allo stato definito dall’amministratore Workfront nell’area Preferenze progetto principale o da un amministratore di gruppo (o amministratore Workfront) nell’area Preferenze progetto di un gruppo. Per informazioni sulla configurazione delle preferenze del progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* Il gruppo del nuovo progetto è il gruppo del modello. Se il modello non è associato a un gruppo, il gruppo del progetto è il gruppo principale dell’utente che crea il progetto.
>
>* Gli stati disponibili per un nuovo progetto corrispondono agli stati del gruppo del progetto, ovvero il gruppo del modello o il gruppo home dell’utente che crea il progetto.


Per creare un progetto da un modello sono disponibili le seguenti opzioni:

* Creare un progetto da un modello nell’area Progetti
* Crea un progetto da un modello a livello di modello
* Allega un modello a un progetto esistente

   Per informazioni, consulta [Allegare un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Creare un progetto da un modello nell’area Gruppi

## Requisiti di accesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Panoramica delle licenze Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica l’accesso a Progetti e Modelli</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull&#39;accesso ai progetti, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concedere l’accesso ai progetti</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per un modello</p> <p>Quando crei un progetto, riceverai automaticamente le autorizzazioni di gestione per il progetto </p> <p> Per informazioni sulle autorizzazioni del progetto, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Condivisione di un progetto in Adobe Workfront</a>.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare un progetto da un modello nell’area Progetti

Puoi creare un progetto dall’area Progetti nel menu principale o dall’area Progetti di un portfolio o di un programma.

1. Esegui una delle operazioni seguenti:

   * Fai clic sul pulsante **Menu principale** ![](assets/main-menu-icon.png), fai clic su **Progetti**, quindi espandi **Nuovo progetto**.
   * Passa a un portfolio, quindi espandi **Nuovo progetto**.

      >[!TIP]
      >
      >Quando crei un progetto utilizzando un modello di un portfolio, il campo Portfolio del nuovo progetto viene aggiornato per visualizzare il portfolio da cui hai scelto di creare il progetto. Questo sovrascrive il campo Portfolio sul modello, se specificato.

   * Vai a un programma, quindi espandi **Nuovo progetto**.

      >[!TIP]
      >
      >Quando crei un progetto utilizzando un modello di un programma, il campo Programma dei nuovi progetti viene aggiornato per visualizzare il programma da cui hai scelto di creare il progetto. Il campo Portfolio del modello viene aggiornato per visualizzare il portfolio del programma da cui hai scelto di creare il progetto. Questo sovrascrive i campi Programma e Portfolio nel modello, se specificati.

   * Gli amministratori di gruppo possono creare un progetto anche nella sezione Progetti di un gruppo gestito. Per ulteriori informazioni, consulta [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

      >[!TIP]
      >
      >Quando crei un progetto utilizzando un modello di un gruppo, il gruppo da cui crei il progetto viene visualizzato nel campo Gruppo del nuovo progetto solo quando il campo Gruppo del modello non è specificato. Se il campo Gruppo modello è specificato, il campo Gruppo del nuovo progetto è quello del modello.
   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Fai clic sul nome di un modello nel **Modelli preferiti** elenco

   ![](assets/new-project-from-template-dropdown-with-template-favorites-nwe-350x235.png)

   Oppure

   Effettua le seguenti operazioni:

   1. Seleziona **Nuovo progetto da modello**.
   1. In **Modelli di ricerca** inizia a digitare il nome di un modello e fai clic su di esso quando viene visualizzato nell’elenco.
   1. Rivedi i dettagli del modello a destra.

      I dettagli del modello includono quanto segue:

      * Durata del modello
      * Proprietario del modello
      * Numero di attività di primo livello che include i nomi delle tre attività principali
      * Numero di tutte le attività nel modello
      * Nomi dei moduli personalizzati del modello
   1. (Facoltativo) Passa il puntatore del mouse sul nome di un modello e fai clic sul pulsante **Preferiti** **icona** ![](assets/favorites-icon-small.png) contrassegnarlo come preferito per uso futuro.

      Oppure

      Espandi la **Modelli preferiti** e seleziona un modello dall’elenco a discesa.

      >[!TIP]
      >
      >Puoi avere fino a 40 elementi Workfront contrassegnati come preferiti. Ciò include modelli e altri elementi.

   1. Fai clic su **Utilizza modello** quando hai selezionato un modello.

   ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!NOTE]
   >
   >Se la vista Milestone è stata applicata all’elenco dei progetti, fare clic sul nome di un modello nel **Nuovo dalla sezione Modello**.
   >
   >
   >![](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)   >

1. La **Nuovo progetto** si apre la casella.

   ![](assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x282.png)

1. Se un campo è già compilato nel modello, viene precompilato nel **Nuovo progetto** scatola. Puoi modificare i valori precompilati per adattarli al meglio al tuo progetto. Per ulteriori informazioni, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Fai clic su **Crea progetto**.

   Tutti i dettagli definiti nel modello si associano automaticamente al progetto appena creato, se non li hai modificati nel passaggio precedente.

## Creare un progetto da un modello nell’area Modelli

Invece di iniziare dall’area Progetti , puoi creare un progetto da un modello partendo dal modello stesso.

 

1. Da **Menu principale**, fai clic su **Modelli**.

1. Fare clic sul nome di un modello da utilizzare.
1. Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Crea progetto.**

   ![Crea progetto da modello](assets/project-sharing-on-template-nwe-2022-350x172.png)

   La **Nuovo progetto** si apre la casella.

1. Specifica un nome per il progetto, quindi esamina ogni sezione e apporta le modifiche necessarie.

   ![](assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x282.png)

   Se un campo è già compilato nel modello, viene precompilato nel **Nuovo progetto** scatola. Puoi modificare i valori precompilati per adattarli al meglio al tuo progetto. Per ulteriori informazioni, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Fai clic su **Crea progetto.**

   Tutti i dettagli definiti nel modello si associano automaticamente al progetto appena creato, se non li hai modificati nel passaggio precedente.
