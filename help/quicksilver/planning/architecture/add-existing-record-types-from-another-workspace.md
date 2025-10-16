---
title: Aggiungi tipi di record esistenti da un altro Workspace
description: I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile aggiungere un tipo di record esistente creato in un'altra area di lavoro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 0%

---


# Aggiungere tipi di record esistenti da un&#39;altra area di lavoro

{{planning-important-intro}}

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

In qualità di responsabile dell&#39;area di lavoro, è possibile aggiungere un tipo di record esistente in un&#39;altra area di lavoro a un&#39;area di lavoro gestita in Adobe Workfront Planning.

Prima di poter aggiungere un tipo di record globale alle aree di lavoro gestite come tipo di record esistente, è necessario che il manager dell&#39;area di lavoro indichi un tipo di record. I responsabili di Workspace possono definire un tipo di record globale quando li creano o li modificano, definendo le impostazioni per più aree di lavoro del tipo di record.

Per informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Questo articolo descrive come aggiungere un tipo di record da uno esistente.

Prima di aggiungere record a un&#39;area di lavoro da un tipo di record globale, vedere anche l&#39;articolo [Panoramica sui tipi di record tra aree di lavoro](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


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
<ul><li><p>Qualsiasi pacchetto Workfront e un pacchetto Planning Plus</p></li>
<p>Oppure</p>
<li><p>Qualsiasi flusso di lavoro e un pacchetto Planning Prime o Ultimate</p></p></li></ul>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestire le autorizzazioni per un’area di lavoro</p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
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
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Prime or Ultimate Workflow package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 

  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table>-->

## Creare un tipo di record aggiungendo un record esistente da un&#39;altra area di lavoro

>[!NOTE]
>
>Verificare che almeno un tipo di record sia designato come globale in almeno un&#39;altra area di lavoro.
>
>Per informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

1. Inizia a creare un tipo di record come descritto nell&#39;articolo [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md), quindi fai clic su **Aggiungi esistente**. <!--check this - the option might have been renamed in the UI-->

   ![Modale per aggiungere il tipo di record con opzione da aggiungere da un&#39;altra area di lavoro](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >Se non sono presenti tipi di record configurati per l&#39;aggiunta ad altre aree di lavoro nel sistema, l&#39;opzione **Aggiungi esistente** non viene visualizzata.

1. Fai clic su **Continua**.
1. Nella casella **Scegli il tipo di record**, fai clic sulla scheda del tipo di record che desideri aggiungere da un&#39;area di lavoro esistente, quindi fai clic su **Aggiungi**.

   Il tipo di record viene aggiunto all&#39;area di lavoro selezionata e l&#39;icona **del tipo di record globale**![](assets/global-icon.png) viene visualizzata nella scheda del tipo di record.

   Si verificano le seguenti situazioni:

   * Vengono aggiunte anche le seguenti informazioni dal tipo di record globale esistente:

      * Tutti i campi originali
      * Tutte le connessioni record
   * È possibile visualizzare i record aggiunti da altre aree di lavoro che utilizzano lo stesso tipo di record globale solo se si dispone almeno delle autorizzazioni di visualizzazione per tali aree di lavoro.
   * Il campo **Workspace** di sola lettura è stato aggiunto alla nuova visualizzazione della tabella del tipo di record. Nel campo viene visualizzata l&#39;area di lavoro in cui è stato creato ogni record.

     >[!NOTE]
     >
     >Non è possibile modificare l&#39;aspetto del nuovo tipo di record, le impostazioni aggiuntive o i campi originali. È possibile modificare il tipo di record e tutti i campi e le impostazioni originali solo dall&#39;area di lavoro originale.

1. (Facoltativo) Fai clic su, quindi trascina e rilascia il nuovo tipo di record aggiunto in una sezione all’interno dell’area di lavoro.
1. (Facoltativo) Fai clic sul menu **Altro** sulla scheda del nuovo tipo di record o a destra del nome del tipo di record nella relativa pagina, quindi fai clic su **Elimina**.

   Per ulteriori informazioni, vedere la sezione &quot;Eliminare tipi di record globali&quot; nell&#39;articolo [Eliminare tipi di record](/help/quicksilver/planning/architecture/delete-record-types.md).

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;!—verificare con Lilit se è possibile aggiungere automazioni o moduli di richiesta a RT globali secondari??—aggiungere un passaggio con collegamenti a tali articoli se/quando sì—>







