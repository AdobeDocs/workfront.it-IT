---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Caricare bozze da InDesign
description: Puoi caricare le tue bacheche grafiche come documenti per una revisione e approvazione rapida o semplicemente per archiviarle in Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: ee3dc446-6886-4285-a942-4f44f5c0ac31
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Carica bozze da [!DNL InDesign]

Puoi caricare le tue bacheche grafiche come bozze direttamente in [!DNL Adobe Workfront] per una revisione e approvazione completa.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] pacchetto</td> 
   <td>Qualsiasi </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>Standard</p> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotti aggiuntivi</td> 
   <td>È necessario disporre di una licenza [!DNL Adobe Creative Cloud] oltre a una licenza [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>[!UICONTROL Manager] o versione successiva</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Modifica accesso a [!UICONTROL Documents]</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Prerequisiti

* È necessario installare il plug-in [!DNL Adobe Workfront for design and video] prima di caricare le bozze da [!DNL InDesign].

  Per istruzioni, vedere [Installa [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md).

## Caricare una bozza di base

1. Fai clic sull&#39;icona **[!UICONTROL Menu]** in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti padre.

   ![Torna all&#39;elenco di lavoro](assets/go-back-to-work-list-350x314.png)

1. Vai all’elemento di lavoro in cui desideri caricare una bozza.
1. Fai clic sull&#39;icona **[!UICONTROL Documento]** ![Icona documento](assets/documents.png) nella barra di navigazione.
1. Fai clic su **[!UICONTROL Nuovo file]** nella parte inferiore del plug-in.
1. Attiva l&#39;interruttore **[!UICONTROL Crea una bozza]**.
1. (Facoltativo) Digitare un nome per la bozza nella casella di testo **[!UICONTROL Nome bozza]**.
1. Nella sezione **[!UICONTROL Proof Approvals]** (Approvazioni bozza), selezionare **[!UICONTROL Basic]**.
1. (Facoltativo) Aggiungi approvatori.
1. (Facoltativo) Digita un commento nell&#39;area **[!UICONTROL Aggiornamenti]**.

   ![Aggiungi un commento](assets/add-comment.png)

1. Scegli il **[!UICONTROL Tipo risorsa]** dal menu a discesa.

1. (Facoltativo) Seleziona **[!UICONTROL Aggiungi file esterno]** per aggiungere un file dal computer.
1. Fai clic su **[!UICONTROL Carica]**, quindi configura le opzioni di esportazione desiderate in base al tipo di risorsa scelto in precedenza.

   ![File nel plug-in](assets/plugin-files-350x307.png)\
   Il documento verrà visualizzato nell&#39;area [!UICONTROL Documenti] del plug-in e dell&#39;app desktop.


## Caricare una bozza automatica

1. Fai clic sull&#39;icona **[!UICONTROL Menu]** in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti padre.

   ![Torna all&#39;elenco di lavoro](assets/go-back-to-work-list-350x314.png)

1. Vai all’elemento di lavoro in cui desideri caricare una bozza.
1. Fai clic sull&#39;icona **[!UICONTROL Documento]** ![Icona documento](assets/documents.png) nella barra di navigazione.

1. Fai clic su **[!UICONTROL Nuovo file]** nella parte inferiore del plug-in.
1. Attiva l&#39;interruttore **[!UICONTROL Crea una bozza]**.
1. (Facoltativo) Digitare un nome per la bozza nella casella di testo **[!UICONTROL Nome bozza]**.
1. Nella sezione **[!UICONTROL Proof Approvals]** (Approvazioni bozza), selezionare **[!UICONTROL Automated]**.
1. (Facoltativo) Nella casella **[!UICONTROL Modello flusso di lavoro]** digitare il nome di un modello di flusso di lavoro bozza.

{{adjust-proof-settings}}

>[!NOTE]
>
> Se nel modello di flusso di lavoro sono presenti campi obbligatori vuoti, le impostazioni di bozza automatizzata vengono aperte automaticamente e ti viene richiesto di compilare tali campi per caricare la bozza.


1. (Facoltativo) Digita un commento nell&#39;area **[!UICONTROL Aggiornamenti]**.

   ![Aggiungi commento approvazione automatica](assets/add-comment-automated-approval.png)

1. Scegli il **[!UICONTROL Tipo risorsa]** dal menu a discesa.
1. (Facoltativo) Seleziona **[!UICONTROL Aggiungi file esterno]** per aggiungere un file dal computer.
1. Fai clic su **[!UICONTROL Carica]**, quindi configura le opzioni di esportazione desiderate in base al tipo di risorsa scelto in precedenza.
Il documento verrà visualizzato nell&#39;area [!UICONTROL Documenti] del plug-in e dell&#39;app desktop.

## Carica una nuova versione di bozza

Puoi caricare una nuova versione di una bozza. Il plug-in ricorda il flusso di lavoro di verifica impostato nella versione precedente, ma puoi modificarlo se lo desideri.

1. Fai clic sull&#39;icona **[!UICONTROL Menu]** in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti padre.

   ![Torna all&#39;elenco di lavoro](assets/go-back-to-work-list-350x314.png)

1. Vai all’elemento di lavoro necessario per caricare un documento in.
1. Fai clic sull&#39;icona **[!UICONTROL Documento]** ![Icona documento](assets/documents.png)nella barra di navigazione.

1. Fai clic su **[!UICONTROL Nuova versione]** nella parte inferiore del plug-in.
1. Attiva l&#39;interruttore **[!UICONTROL Crea una bozza]**.

1. Nella sezione *[!UICONTROL *Proof approvals]**, scegli **[!UICONTROL Basic]** o **[!UICONTROL Automated]**.

1. Aggiungi **[!UICONTROL Revisori]** o un **[!UICONTROL modello di flusso di lavoro]** in base al tipo di approvazione selezionato al passaggio 7.

1. (Facoltativo) Digita un commento nell&#39;area **[!UICONTROL Aggiornamenti]**.
1. Scegli il **[!UICONTROL Tipo risorsa]** dal menu a discesa.
1. Fai clic su **[!UICONTROL Carica]**, quindi configura le opzioni di esportazione desiderate in base al tipo di risorsa scelto in precedenza.
Il documento verrà visualizzato nell&#39;area [!UICONTROL Documenti] del plug-in e dell&#39;app desktop.
