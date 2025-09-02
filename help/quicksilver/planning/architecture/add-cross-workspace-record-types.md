---
title: Aggiungi tipi di record esistenti
description: I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile importare un tipo di record esistente da un'altra area di lavoro.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 976810c8cedc5d3c5afd8333fdbace4fe8d0ccda
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Aggiungi tipi di record esistenti

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

In qualità di responsabile dell&#39;area di lavoro, è possibile importare o aggiungere un tipo di record esistente a un&#39;altra area di lavoro.

È necessario innanzitutto designare un tipo di record come centralizzato prima che i responsabili dell&#39;area di lavoro possano importarlo in altre aree di lavoro.

È possibile impostare un tipo di record come centralizzato quando lo si crea o lo si modifica, mentre si definiscono le relative impostazioni per più aree di lavoro.

Per informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr>

</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront*</p></td> 
   <td> 
<ul><li><p>Qualsiasi pacchetto Workfront</p></li>
E
<li><p>Pacchetto Planning Plus</p></li></ul>
Oppure:
<ul><li><p>Qualsiasi pacchetto flusso di lavoro</p> </li>
E
<li><p>Pacchetto Planning Prime o Ultimate</p></li></ul>
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestione delle autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Panoramica dei tipi di record centralizzati

Considerazioni durante l&#39;aggiunta di tipi di record esistenti da un&#39;altra area di lavoro

* Quando non sono presenti tipi di record configurati per l&#39;aggiunta a un&#39;altra area di lavoro, l&#39;opzione per importarli da un&#39;altra area di lavoro non viene visualizzata durante la creazione di un tipo di record. <!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* Dopo l&#39;aggiunta del tipo di record da un&#39;altra area di lavoro, vengono aggiunte anche le seguenti informazioni dal tipo di record esistente:

   * Campi
   * Registra connessioni

* È possibile visualizzare i record aggiunti da altre aree di lavoro solo se si dispone delle autorizzazioni per tali aree.

* È possibile modificare il tipo di record, inclusi i relativi campi, solo nell&#39;area di lavoro originale. Non è possibile modificarlo dalle aree di lavoro in cui è stato aggiunto.
* I record aggiunti da tutte le aree di lavoro saranno visibili a tutti gli utenti che vi accedono da tutte le aree di lavoro, anche se vengono creati in un&#39;area di lavoro in cui non dispongono di autorizzazioni.

## Creare un tipo di record da un tipo di record esistente

1. Inizia a creare un tipo di record come descritto nell&#39;articolo [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md), quindi fai clic su **Aggiungi esistente**. <!--check this - the option might have been renamed in the UI-->

   ![Modale per aggiungere il tipo di record con opzione da importare da un&#39;altra area di lavoro](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Fai clic su **Continua**.
1. Nella casella **Scegli tipo di record**, fai clic sulla scheda del tipo di record che desideri aggiungere da un&#39;area di lavoro esistente, quindi fai clic su **Aggiungi**.

   Il tipo di record viene aggiunto all&#39;area di lavoro selezionata e si verificano gli eventi seguenti:

   * Alla scheda del tipo di record importato è stata aggiunta l&#39;icona **cross-workspace record type** ![Cross-Workspace connection icon](assets/global-icon.png).
   * Il campo **Workspace** di sola lettura è stato aggiunto al tipo di record importato. Nel campo viene visualizzata l’area di lavoro in cui è stato creato ogni record.

     >[!NOTE]
     >
     >* Impossibile modificare il tipo di record importato o i relativi campi. È possibile modificare il tipo di record e i relativi campi dall&#39;area di lavoro originale.

1. (Facoltativo) Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nella scheda del tipo di record importato o a destra del nome del tipo di record nella relativa pagina, quindi fai clic su **Elimina**.
1. (Condizionale) Digita **delete** nel campo fornito, quindi fai clic su **Delete** definitivamente.

   Il tipo di record importato verrà rimosso dall&#39;area di lavoro selezionata. Il tipo di record originale e i relativi campi rimangono nell&#39;area di lavoro originale.

   <!--**************************ASK LILIT ON THIS ONE, NOT SURE IF THIS IS TRUE: Any records added in the current workspace are saved in the original workspace.**********-->



