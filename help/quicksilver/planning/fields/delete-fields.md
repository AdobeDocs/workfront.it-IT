---
title: Elimina campi
description: In Adobe Workfront Planning è possibile eliminare i campi personalizzati che non sono più rilevanti.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EusoK7-jmYJHg9nqyvvQamsfVeUy802p36EyDmLGwik
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 733
ht-degree: 1%

---

# Elimina campi

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo il rilascio in anteprima, le stesse funzioni sono disponibili mensilmente nell’ambiente di produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

In Adobe Workfront Planning è possibile creare campi personalizzati per memorizzare informazioni sui record.

Per informazioni sulla creazione di campi personalizzati in Workfront Planning, vedere [Creare campi](/help/quicksilver/planning/fields/create-fields.md).

È possibile eliminare i campi di Workfront Planning che non sono più rilevanti.

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
<ul> 
<li><p>Qualsiasi pacchetto Workfront e Planning</p></li>
Oppure
<li><p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p></li></ul>

<p>Per eliminare campi dai tipi di record globali:</p>
<ul><li><p>Qualsiasi pacchetto Workfront e un pacchetto Planning Plus</p></li>
Oppure
<li><p>Tutti i pacchetti Workflow e Planning Prime e Ultimate</p></li></ul>

<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Gestire le autorizzazioni per un’area di lavoro</p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--
Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table>
-->

## Considerazioni sull&#39;eliminazione dei campi di Workfront Planning:

* È possibile eliminare un campo solo nella vista tabella del tipo di record.
* Impossibile eliminare il campo principale di un record.
* Tutte le informazioni memorizzate nel campo vengono eliminate e non possono essere recuperate.
* Quando si elimina un campo record connesso, vengono eliminati anche tutti i campi di ricerca connessi dal tipo di record da cui ci si connette. I campi dei record connessi dei tipi di record a cui ci si connette vengono eliminati anche dal record a cui ci si connette.

  Ad esempio, quando si connettono Campagne a un altro tipo di record denominato Prodotto e si eliminano dalla campagna il campo Collegato al prodotto e il campo di ricerca Stato del prodotto, vengono eliminati i seguenti elementi:

   * Il campo Prodotto connesso dalla campagna
   * Il campo di ricerca Stato prodotto dalla campagna
   * Il campo Campaign connesso dal prodotto

  Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

* Non è possibile eliminare i campi dai record globali aggiunti a un&#39;area di lavoro secondaria dalle aree di lavoro secondarie.

## Elimina campi

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera eliminare i campi record.

   Viene aperto il workspace e vengono visualizzati i tipi di record.

1. Fare clic sulla scheda di un tipo di record.

1. (Condizionale) Se non è già selezionata, fare clic sulla scheda di una **visualizzazione tabella** nella pagina del tipo di record.

   Tutti i record esistenti associati al tipo di record vengono visualizzati nelle righe della vista tabella.

1. Individuare il campo da eliminare nelle intestazioni di colonna, posizionare il puntatore del mouse sull&#39;intestazione di colonna e fare clic sulla freccia rivolta verso il basso dopo il nome del campo.

   ![Menu freccia dopo il nome del campo nell&#39;intestazione della tabella evidenziato](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Fai clic su **Elimina**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. <span class="preview">(Condizionale) Se il campo che si sta eliminando fa parte di un modulo di richiesta, viene visualizzata la casella **Elimina campo** per indicare i moduli che saranno interessati dalle modifiche. Eseguire una delle operazioni seguenti:</span>

   <div class="preview">

   * Fare clic sulla freccia rivolta a destra per visualizzare le maschere interessate dalla modifica, quindi fare clic sul nome della maschera per aprire la maschera in una nuova scheda e decidere se si desidera mantenere il campo nella maschera o apportare ulteriori modifiche alla maschera.
   * Fai clic su **Elimina** per eliminare il campo da tutte le aree in cui viene visualizzato.

   </div>

   Non è possibile recuperare i campi eliminati.

   A seconda del tipo di campo eliminato, si verifica quanto segue:

   * Se si elimina un campo che appartiene al record selezionato, il campo viene eliminato e non può più essere associato ad alcun record. Se questo campo viene aggiunto come campo di ricerca in altri record, anche tali campi vengono eliminati.
   * Se si elimina un campo di connessione, il campo viene eliminato dal record selezionato. Viene eliminato anche il campo di connessione corrispondente dal record originale.
   * Se si elimina un campo di ricerca aggiunto da un record connesso, il campo viene eliminato dal tipo di record selezionato, ma rimane nel tipo di record originale.
   * Se si elimina un campo da un tipo di record globale nell&#39;area di lavoro principale, il campo viene eliminato da tutte le aree di lavoro in cui è stato aggiunto il tipo di record. Non è possibile eliminare i campi dai tipi di record globali dalle aree di lavoro secondarie.
