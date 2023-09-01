---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Caricare bozze da Illustrator
description: Puoi caricare le tue bacheche grafiche come documenti per una revisione e approvazione rapida o semplicemente per archiviarle in Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: e98f27d4-7c07-44cc-8df5-e04472ec946e
source-git-commit: 66186bb8af14e7ce86b3fb5e8bb1b07fe32dca7a
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Carica bozze da [!DNL Illustrator]

Puoi caricare le tue bacheche artistiche come bozze direttamente in [!DNL Adobe Workfront] per una revisione e approvazione completa.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Piano corrente: [!UICONTROL Pro] o versione successiva</p> <p>oppure</p> <p>Piano legacy: [!UICONTROL Premium]</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>Piano corrente: [!UICONTROL Lavoro] o [!UICONTROL Bozza]</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>Devi avere un [!DNL Adobe Creative Cloud] licenza in aggiunta a una [!DNL Workfront] licenza.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>[!UICONTROL Manager] o versione successiva</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Modifica accesso a [!UICONTROL Documents]</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, la mansione o il profilo di autorizzazione della bozza, contattare [!DNL Workfront] o [!DNL Workfront Proof] amministratore.

## Prerequisiti

* Installazione obbligatoria [!DNL Adobe Workfront for design and video] prima di caricare le bozze da [!DNL Illustrator].

  Per istruzioni, consulta [Installa [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md).

## Caricare una bozza di base

1. Fai clic su **[!UICONTROL Menu]** nell’angolo in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti padre.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vai all’elemento di lavoro in cui desideri caricare una bozza.
1. Fai clic su **[!UICONTROL Documento]** icona ![](assets/documents.png) nella barra di navigazione.
1. Clic **[!UICONTROL Nuovo file]** nella parte inferiore del plug-in.
1. Abilita **[!UICONTROL Creare una bozza]** attivare/disattivare.
1. (Facoltativo) Immetti un nome per la bozza nella **[!UICONTROL Nome bozza]** casella di testo.
1. In **[!UICONTROL Approvazioni bozza]** sezione, seleziona **[!UICONTROL Base]**.
1. (Facoltativo) Aggiungi approvatori.
1. (Facoltativo) Immetti un commento nella **[!UICONTROL Aggiornamenti]** area.

   ![](assets/add-comment.png)

1. Scegli la **[!UICONTROL Tipo risorsa]** dal menu a discesa.

1. (Facoltativo) Seleziona **[!UICONTROL Aggiungi file esterno]** per aggiungere un file dal computer.
1. Clic **[!UICONTROL Carica]**, quindi configura le opzioni di esportazione desiderate in base al tipo di risorsa scelto in precedenza.

   ![](assets/plugin-files-350x307.png)\
   Il documento viene visualizzato nel [!UICONTROL Documenti] nel plug-in e nell’app desktop.


## Caricare una bozza automatica

1. Fai clic su **[!UICONTROL Menu]** nell’angolo in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti padre.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vai all’elemento di lavoro in cui desideri caricare una bozza.
1. Fai clic su **[!UICONTROL Documento]** icona ![](assets/documents.png) nella barra di navigazione.

1. Clic **[!UICONTROL Nuovo file]** nella parte inferiore del plug-in.
1. Abilita **[!UICONTROL Creare una bozza]** attivare/disattivare.
1. (Facoltativo) Immetti un nome per la bozza nella **[!UICONTROL Nome bozza]** casella di testo.
1. In **[!UICONTROL Approvazioni bozza]** sezione, seleziona **[!UICONTROL Automatizzato]**.
1. (Facoltativo) In **[!UICONTROL Modello flusso di lavoro]** digita il nome di un modello di flusso di lavoro bozza.

{{adjust-proof-settings}}

>[!NOTE]
>
> Se nel modello di flusso di lavoro sono presenti campi obbligatori vuoti, le impostazioni di bozza automatizzata vengono aperte automaticamente e ti viene richiesto di compilare tali campi per caricare la bozza.


1. (Facoltativo) Immetti un commento nella **[!UICONTROL Aggiornamenti]** area.

   ![](assets/add-comment-automated-approval.png)

1. Scegli la **[!UICONTROL Tipo risorsa]** dal menu a discesa.
1. (Facoltativo) Seleziona **[!UICONTROL Aggiungi file esterno]** per aggiungere un file dal computer.
1. Clic **[!UICONTROL Carica]**, quindi configura le opzioni di esportazione desiderate in base al tipo di risorsa scelto in precedenza.
Il documento viene visualizzato nel [!UICONTROL Documenti] nel plug-in e nell’app desktop.

## Carica una nuova versione di bozza

Puoi caricare una nuova versione di una bozza. Il plug-in ricorda il flusso di lavoro di verifica impostato nella versione precedente, ma puoi modificarlo se lo desideri.

1. Fai clic su **[!UICONTROL Menu]** nell’angolo in alto a destra, quindi seleziona **[!UICONTROL Elenco lavori]**. È inoltre possibile utilizzare il menu per passare agli oggetti padre.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vai all’elemento di lavoro necessario per caricare un documento in.
1. Fai clic su **[!UICONTROL Documento]** icona ![](assets/documents.png)nella barra di navigazione.

1. Clic **[!UICONTROL Nuova versione]** nella parte inferiore del plug-in.
1. Abilita **[!UICONTROL Creare una bozza]** attivare/disattivare.

1. In *[!UICONTROL *Approvazioni bozza]** sezione, scegliere **[!UICONTROL Base]** o **[!UICONTROL Automatizzato]**.

1. Aggiungi **[!UICONTROL Revisori]** o un **[!UICONTROL Modello flusso di lavoro]** in base al tipo di approvazione selezionato al punto 7.

1. (Facoltativo) Immetti un commento nella **[!UICONTROL Aggiornamenti]** area.
1. Scegli la **[!UICONTROL Tipo risorsa]** dal menu a discesa.
1. Clic **[!UICONTROL Carica]**, quindi configura le opzioni di esportazione desiderate in base al tipo di risorsa scelto in precedenza.
Il documento viene visualizzato nel [!UICONTROL Documenti] nel plug-in e nell’app desktop.
