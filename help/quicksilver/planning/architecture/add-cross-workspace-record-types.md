---
title: Aggiungi tipi di record esistenti
description: I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile aggiungere un tipo di record esistente creato in un'altra area di lavoro.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 38c397594449856a0f1404848a527b86083654b8
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

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

In qualità di responsabile dell&#39;area di lavoro, è possibile aggiungere un tipo di record esistente in un&#39;area di lavoro a un&#39;area di lavoro gestita in Adobe Workfront Planning.

È necessario innanzitutto designare un tipo di record come centralizzato prima che i responsabili dell&#39;area di lavoro possano aggiungerlo ad altre aree di lavoro come tipo di record esistente.

È possibile impostare un tipo di record come centralizzato quando lo si crea o lo si modifica, mentre si definiscono le relative impostazioni per più aree di lavoro.

Per informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Prima di aggiungere record a un&#39;area di lavoro da un tipo di record centralizzato, vedere l&#39;articolo [Panoramica sui tipi di record centralizzati](/help/quicksilver/planning/architecture/centralized-record-types-overview.md).

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
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
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

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Creare un tipo di record da un tipo di record esistente

1. Inizia a creare un tipo di record come descritto nell&#39;articolo [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md), quindi fai clic su **Aggiungi esistente**. <!--check this - the option might have been renamed in the UI-->

   ![Modale per aggiungere il tipo di record con opzione da aggiungere da un&#39;altra area di lavoro](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Fai clic su **Continua**.
1. Nella casella **Scegli tipo di record**, fai clic sulla scheda del tipo di record che desideri aggiungere da un&#39;area di lavoro esistente, quindi fai clic su **Aggiungi**.

   Il tipo di record viene aggiunto all&#39;area di lavoro selezionata.

   >[!TIP]
   >
   >Quando non sono presenti tipi di record configurati per l&#39;aggiunta a un&#39;altra area di lavoro, l&#39;opzione per aggiungerli da un&#39;altra area di lavoro non viene visualizzata durante la creazione di un tipo di record.

   Si verificano le seguenti situazioni:

   * Vengono aggiunte anche le seguenti informazioni dal tipo di record centralizzato esistente:

      * Tutti i campi originali
      * Tutte le connessioni record
   * È possibile visualizzare i record aggiunti da altre aree di lavoro solo se si dispone almeno delle autorizzazioni di visualizzazione per tali aree di lavoro.
   * Alla scheda del nuovo tipo di record viene aggiunta l&#39;icona **tipo di record centralizzato** ![icona tipo di record centralizzato](assets/global-icon.png).
   * Il campo **Workspace** di sola lettura è stato aggiunto alla nuova visualizzazione della tabella del tipo di record. Nel campo viene visualizzata l’area di lavoro in cui è stato creato ogni record.

     >[!NOTE]
     >
     >* Non è possibile modificare l&#39;aspetto del nuovo tipo di record, le impostazioni avanzate o i campi originali. È possibile modificare il tipo di record e tutti i campi e le impostazioni originali solo dall&#39;area di lavoro originale.

1. (Facoltativo) Fai clic su, quindi trascina e rilascia il nuovo tipo di record aggiunto in una sezione all’interno dell’area di lavoro.

1. (Facoltativo) Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nella scheda del nuovo tipo di record o a destra del nome del tipo di record nella relativa pagina, quindi fai clic su **Condividi** per condividerlo con altri utenti nella stessa area di lavoro.

1. (Facoltativo) Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nella scheda del nuovo tipo di record o a destra del nome del tipo di record nella relativa pagina, quindi fai clic su **Elimina**.
1. (Condizionale) Digita **delete** nel campo fornito, quindi fai clic su **Delete** definitivamente.

   Si verificano le seguenti situazioni:

   * Il tipo di record creato da un tipo di record centralizzato viene rimosso dall&#39;area di lavoro selezionata.
   * Il tipo di record originale e i relativi campi rimangono nell&#39;area di lavoro originale.
   * Tutti gli altri tipi di record aggiunti dallo stesso tipo di record centralizzato rimangono nelle aree di lavoro.
   * I record aggiunti al tipo di record dall&#39;area di lavoro corrente vengono eliminati. Tutti gli altri record aggiunti da aree di lavoro aggiuntive in cui è stato aggiunto il tipo di record centralizzato vengono conservati.





