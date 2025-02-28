---
product-area: projects;templates
navigation-topic: create-projects
title: Creare un progetto utilizzando un modello
description: Puoi utilizzare i modelli come framework per creare progetti in Adobe Workfront. Se i progetti si ripetono spesso, l’utilizzo dei modelli per il nuovo progetto evita di dover creare ripetutamente gli stessi progetti.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Creare un progetto utilizzando un modello

<!-- Audited: 01/2024 -->

Puoi utilizzare i modelli come framework per creare progetti in Adobe Workfront. Se i progetti si ripetono spesso, l’utilizzo dei modelli per la timeline generale del nuovo progetto evita di dover creare ripetutamente gli stessi progetti.

I modelli consentono di acquisire processi, informazioni e impostazioni ripetibili associati ai progetti. Le informazioni associate a un modello vengono trasferite al progetto. Ciò include attività, assegnazioni, durate, documenti, dettagli finanziari, rischi e moduli personalizzati.

>[!TIP]
>
>Workfront definisce il gruppo e lo stato del nuovo progetto come segue:
>
>* Lo stato predefinito di un nuovo progetto creato da un modello corrisponde a quello definito dall&#39;amministratore di Workfront nell&#39;area Preferenze progetto principale o da un amministratore di gruppo (o amministratore Workfront) nell&#39;area Preferenze progetto per un gruppo. Per informazioni sulla configurazione delle preferenze di progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* Il Gruppo del nuovo progetto è il Gruppo del modello. Se il modello non è associato a un gruppo, il gruppo del progetto è il gruppo predefinito dell’utente che crea il progetto.
>
>* Gli stati disponibili per un nuovo progetto corrispondono agli stati del Gruppo del progetto, che è il Gruppo del modello o il Gruppo Predefinito dell’utente che crea il progetto.

Per creare un progetto da un modello, puoi utilizzare le seguenti opzioni:

* Creare un progetto da un modello nell’area Progetti
* Creare un progetto da un modello a livello di modello
* Allega un modello a un progetto esistente

  Per informazioni, vedere [Allegare un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Creare un progetto da un modello nell’area Gruppi

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Workfront*</td> 
   <td> <p>Nuovo: Standard</p>
        <p>oppure</p>
        <p>Corrente: Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> <p>Modificare l’accesso a progetti e modelli</p>

<p>modificare l'accesso a portafogli e programmi, se il modello utilizzato contiene un Portfolio e un programma</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni per un modello</p> 
  <p>Se il modello utilizzato contiene un Portfolio e un programma, è necessario disporre delle autorizzazioni di gestione per il portfolio e il programma per creare il progetto </p> 
   <p>Quando crei un progetto, ricevi automaticamente le autorizzazioni di gestione per il progetto.</p></td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un progetto da un modello nell’area Progetti

Puoi creare un progetto dall’area Progetti nel Menu principale oppure dall’area Progetti di un portfolio o di un programma.

>[!NOTE]
>
>L&#39;amministratore di sistema o di gruppo potrebbe modificare l&#39;interfaccia utilizzando un modello di layout. In questo caso, alcuni dei nomi delle sezioni e delle aree a cui si fa riferimento nei passaggi seguenti potrebbero essere diversi nell’istanza di Workfront.

1. Esegui una delle operazioni seguenti:

   * Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro. Fai clic su **Progetti**, quindi espandi **Nuovo progetto**.
   * Vai a un portfolio, quindi espandi **Nuovo progetto**.

     >[!TIP]
     >
     >Quando crei un progetto utilizzando un modello di un portfolio, il campo Portfolio del nuovo progetto viene aggiornato in modo da visualizzare il portfolio da cui hai scelto di creare il progetto. In questo modo viene sovrascritto il campo Portfolio del modello, se specificato.

   * Vai a un programma, quindi espandi **Nuovo progetto**.

     >[!TIP]
     >
     >Quando si crea un progetto utilizzando un modello di un programma, il campo Programma dei nuovi progetti viene aggiornato in modo da visualizzare il programma dal quale si è scelto di creare il progetto. Il campo Portfolio del modello viene aggiornato per visualizzare il portfolio del programma da cui hai scelto di creare il progetto. In questo modo vengono sovrascritti i campi Programma e Portfolio del modello, se specificati.

   * Se sei un amministratore gruppo, puoi anche creare un progetto nella sezione Progetti di un gruppo che gestisci. Per ulteriori informazioni, vedere [Creare e modificare i progetti di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >Quando si crea un progetto utilizzando un modello di un gruppo, il gruppo da cui si crea il progetto viene visualizzato nel campo Gruppo del nuovo progetto solo se non è specificato il campo Gruppo del modello. Se si specifica il campo Gruppo del modello, il campo Gruppo del nuovo progetto è quello del modello.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![Nuove opzioni progetto](assets/new-project-dropdown.png)

1. Fare clic sul nome di un modello nell&#39;elenco **Modelli preferiti**.

   ![Seleziona un modello preferito](assets/new-project-from-template-dropdown-with-template-favorites.png)

   Oppure

   Effettua le seguenti operazioni:

   1. Seleziona **Nuovo progetto dal modello**.
   1. Nel campo **Cerca modelli**, inizia a digitare il nome di un modello e fai clic su di esso quando viene visualizzato nell&#39;elenco.
   1. Rivedi i dettagli del modello a destra.

      I dettagli del modello includono quanto segue:

      * Durata modello
      * Proprietario del modello
      * Numero di attività di primo livello, inclusi i nomi delle tre attività principali
      * Numero di tutte le attività nel modello
      * Nomi dei moduli personalizzati del modello

   1. (Facoltativo) Passa il puntatore del mouse sul nome di un modello nel riquadro di sinistra e fai clic sull&#39;icona **Preferiti** **icona** ![Preferiti](assets/favorites-icon-small.png) per contrassegnarlo come preferito per un utilizzo futuro.

      Oppure

      Espandere l&#39;elenco **Modelli preferiti** e selezionare un modello dall&#39;elenco a discesa.

      >[!TIP]
      >
      >Puoi avere fino a 40 elementi Workfront contrassegnati come preferiti. Ciò include modelli e altri elementi.

   1. Fare clic su **Usa modello** dopo aver selezionato un modello.

      ![Dettagli modello](assets/new-project-from-template-small-box-with-template-details-panel.png)

      >[!NOTE]
      >
      >Se all&#39;elenco dei progetti è applicata la visualizzazione Milestone, fare clic sul nome di un modello nella sezione **Nuovo da modello**.
      >
      >
      >![Vista milestone della creazione di un progetto da un modello](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >

   Viene visualizzata la casella **Nuovo progetto**.

   ![Casella Nuovo progetto](assets/new-project-from-template-box.png)

1. Se un campo è già popolato nel modello, il campo viene prepopolato nella casella **Nuovo progetto**. Puoi modificare i valori precompilati in modo che corrispondano meglio al tuo progetto. Per ulteriori informazioni, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Fare clic su **Crea progetto**.

   Tutti i dettagli definiti nel modello vengono associati automaticamente al nuovo progetto creato se non sono stati modificati nel passaggio precedente.

## Creare un progetto da un modello nell’area Modelli

Invece di iniziare dall’area Progetti, puoi creare un progetto da un modello iniziando dal modello.

{{step1-to-templates}}

1. Fare clic sul nome del modello che si desidera utilizzare.
1. Fai clic sul menu **Altro** ![Icona Altro](assets/more-icon.png), quindi fai clic su **Crea progetto**.

   ![Crea progetto da modello](assets/project-sharing-on-template.png)

   Viene visualizzata la casella **Nuovo progetto**.

1. Immetti un nome per il progetto, quindi controlla ogni sezione e apporta le modifiche necessarie.

   ![Casella Nuovo progetto](assets/new-project-from-template-box.png)

   Se un campo è già popolato nel modello, il campo viene prepopolato nella casella **Nuovo progetto**. Puoi modificare i valori precompilati in modo che corrispondano meglio al tuo progetto. Per ulteriori informazioni, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Fare clic su **Crea progetto**.

   Tutti i dettagli definiti nel modello vengono associati automaticamente al nuovo progetto creato se non sono stati modificati nel passaggio precedente.
