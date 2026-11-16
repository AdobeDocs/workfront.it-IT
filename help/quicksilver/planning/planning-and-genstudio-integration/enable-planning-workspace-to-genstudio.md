---
title: Abilitare un Workspace di Workfront Planning in GenStudio for Performance Marketing
description: È possibile rendere disponibile un'area di lavoro di Adobe Workfront Planning in GenStudio for Performance Marketing quando si ha accesso a entrambe le applicazioni.
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 9dc53e749a61247529d67ce077856ea6bea8e494
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 4%
---
# Abilitare un&#39;area di lavoro di Workfront Planning in GenStudio for Performance Marketing

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--Iskuhi said "ACPC projects" will be renamed when this will be released but not sure if it has been. Follow up with Syuzanna, Gurgen Mosesyan and possibly Himanshi Kumar - see slack threads -->

Quando la tua azienda acquista anche Adobe GenStudio for Performance Marketing e sei un cliente Adobe Workfront Planning, l’area di lavoro GenStudio è disponibile anche in Workfront Planning.

Se si dispone già di un&#39;area di lavoro Planning in Workfront Planning, è possibile abilitarla per GenStudio for Performance Marketing anziché ricrearne gli stessi dati in GenStudio.

L’abilitazione di un’area di lavoro la collega a un progetto Adobe Could Storage e ne mappa i tipi di record e i campi nell’area di lavoro GenStudio. Dopo aver completato la configurazione, puoi aprire i record dell’area di lavoro in GenStudio.

Devi avere i seguenti:

* Accesso a Workfront Planning e GenStudio for Performance Marketing.
* Un progetto Adobe Cloud Storage per il collegamento all’area di lavoro. L’amministratore dell’organizzazione può crearne una in Adobe Admin Console.

  Per informazioni, consulta [Gestire l&#39;archiviazione Adobe](https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html). <!--ensure this site still works-->

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
<p>Qualsiasi Workfront o flusso di lavoro e qualsiasi pacchetto Planning</p> 
Oppure
<p>Qualsiasi pacchetto Planning acquistato come prodotto standalone</p>

</td> 
   <tr> 
<td> 
   <p> Prodotti aggiuntivi</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>

<tr> 
<td> 
   <p> Impostazioni Adobe Admin Console</p> </td> 
   <td> 
   <p> Devi creare progetti Adobe Storage Cloud in Adobe Admin Console </p>

<p>Per informazioni, vedere <a href="https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/projects-in-business-storage.html#project-policies">Gestione progetti</a>

</td> 
  </tr>
  <tr>

<tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Standard flusso di lavoro</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Planning</p></td> 
   <td><p>Standard di pianificazione</p>
   </td> 
  </tr>
<tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso di Adobe Workfront</p></td> 
   <td> <p>È necessario aggiungere sia un flusso di lavoro che un tipo di licenza Planning al livello di accesso a Workfront quando si dispone sia di un flusso di lavoro che di un pacchetto Planning</p>   
</td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Ruoli utente di Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Qualsiasi ruolo utente di GenStudio se devi accedere a Campagne, Prodotti e Utenti tipo</li>
   <li>GenSudio System Manager se è necessario accedere ad Activations <!--and Events--></li></ul>
   Per informazioni, vedere <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Ruoli utente e autorizzazioni</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Gestire le autorizzazioni per l’area di lavoro <!--to add new fields or record types to the GenStudio workspace--></p></li>
   <!--
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   -->
   </ul>
   <!--
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   -->
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <!--
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   -->
   <li><p> Creare le autorizzazioni in Adobe GenStudio for Performance Marketing per creare elementi</p></li></ul>
   </td>  
</tbody> 
</table>

Per informazioni sull&#39;accesso ad Adobe Workfront Planning, vedere [Panoramica dell&#39;accesso ad Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Per ulteriori informazioni su Adobe GenStudio for Performance Marketing, consulta [Guida utente di Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/it/docs/genstudio-for-performance-marketing/user-guide/home).

+++ 

## Abilitare un&#39;area di lavoro di Workfront Planning in GenStudio

1. In Workfront Planning aprire l&#39;area di lavoro che si desidera abilitare.
1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome dell&#39;area di lavoro, quindi fai clic su **Abilita GenStudio**.

   La casella **Imposta come area di lavoro GenStudio** abilitata si apre con i seguenti passaggi:

   1. **Progetto ACPC**: seleziona il **Progetto ACPC** (progetto Adobe Cloud Storage) che desideri sincronizzare con questa area di lavoro, quindi fai clic su **Avanti**. Gli utenti accedono all’area di lavoro in GenStudio tramite questo progetto.

      ![Abilita il GenStudio dell&#39;area di lavoro - Passaggio del progetto ACPC](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **Tipi di record**: associare i tipi di record dell&#39;area di lavoro ai sei tipi di record richiesti da GenStudio:

      * Campagne
      * Prodotti
      * Persone
      * Canali
      * Aree geografiche
      * Attivazioni

      Per ognuno, aprire l&#39;elenco e selezionare il tipo di record Planning corrispondente oppure selezionare **Aggiungi nuovo** per crearlo, quindi fare clic su **Avanti**.

      ![Abilita GenStudio area di lavoro - Tipi di record, passaggio](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **Campi**: mappa i campi per ogni tipo di record. Utilizzare le schede nella parte superiore della finestra di dialogo per spostarsi tra i tipi di record. Per ogni campo, selezionare il campo Planning corrispondente oppure selezionare **Aggiungi nuovo** per creare un campo.

      Ripetere l&#39;impostazione del campo per tutti i tipi di record.

      ![Abilita GenStudio area di lavoro - Passaggio campi](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. Rivedi e risolvi eventuali avvisi.

      Ad esempio, un nuovo campo può diventare il campo principale per il tipo di record oppure un alias di campo già in uso viene rinominato (se disponi già di un campo denominato &quot;Aree&quot;, quello importato potrebbe diventare &quot;Aree 2&quot;).

      La mappatura di un campo **Stato** aggiunge le opzioni richieste.

   1. Fai clic su **Pubblica**.

      Quando l’area di lavoro è abilitata, viene visualizzato un messaggio di conferma. I tipi di record mappati vengono contrassegnati nell&#39;area di lavoro.

      I tipi di record mappati per essere accessibili da GenStudio hanno una nuova icona **Adobe** sulle loro schede.

      ![Tipo di record Campagne con icona Adobe](assets/campaigns-record-type-card-with-adobe-icon.png)

1. Apri GenStudio e seleziona **Campagne**, quindi fai clic sul **progetto ACPC** originariamente configurato per questa installazione nell&#39;angolo inferiore sinistro della schermata. Esaminare i tipi di record e i campi importati.

   >[!TIP]
   >
   >Puoi visualizzare solo i record consentiti dall’iscrizione al progetto Adobe Cloud Storage.
