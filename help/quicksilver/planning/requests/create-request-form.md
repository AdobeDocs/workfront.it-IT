---
title: Creazione di un modulo di richiesta in Adobe Workfront Planning
description: Dopo aver selezionato un tipo di record nell'area Adobe Workfront Planning, è possibile creare un modulo di richiesta associato a tale tipo di record e condividere un collegamento ad esso con altri utenti interni o esterni.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 2%

---

# Creazione di un modulo di richiesta in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Dopo aver selezionato un tipo di record nell&#39;area Adobe Workfront Planning, è possibile creare un modulo di richiesta e associarlo a tale tipo di record. Puoi quindi condividere un collegamento con altri utenti interni o esterni. <!--double-check on the external part of it-->

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per accedere a Workfront Planning, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotti</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td>
   <td>
<p>Uno dei seguenti piani di Workfront:</p>
<ul><li>Seleziona</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p>
   </td>

<tr>
   <td role="rowheader"><p>Piano di pianificazione Adobe Workfront*</p></td>
   <td>
<p>Qualsiasi </p>   </td>

<tr>
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td>
   <td>
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p>
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata di Adobe per Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td>
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td>
   <td>
   <ul>
   <li><p>Gestire le autorizzazioni per un’area di lavoro</p></li>
    <li><p>Gli amministratori di sistema possono gestire le aree di lavoro che non hanno creato. </p></li>
    </ul>
   <p>Per informazioni sulle autorizzazioni di condivisione per gli oggetti di Workfront Planning, vedere  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Panoramica delle autorizzazioni di condivisione in Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p>  
</td>
  </tr>
 </tbody>
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un modulo di richiesta per un tipo di record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera aggiungere i record.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

   La pagina del tipo di record viene visualizzata nella visualizzazione a cui si è effettuato l&#39;ultimo accesso. Per impostazione predefinita, nella vista tabella viene visualizzata una pagina del tipo di record.

1. Fai clic sul menu **Altro** ![](assets/more-menu.png) a destra del nome del tipo di record nell&#39;intestazione della pagina, quindi fai clic su **Crea modulo di richiesta**.
1. Aggiorna il nome del modulo di richiesta. Per impostazione predefinita, il nome del modulo è **Modulo di richiesta senza titolo**. <!--check this; you logged a bug to rename it to this but was it fixed?-->
1. (Facoltativo) Aggiungi una **Descrizione** per il modulo di richiesta.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Fai clic su **Crea**. Viene aperto il modulo di richiesta per il tipo di record selezionato.

   Per impostazione predefinita, il modulo di richiesta contiene le seguenti informazioni:

   * **Sezione predefinita**: questa è l&#39;interruzione di sezione predefinita che Workfront applica al modulo di richiesta. Impossibile rinominare o rimuovere la sezione predefinita.
   * Campo **Oggetto**: campo che identificherà la richiesta in Workfront. Questa funzionalità non è ancora disponibile.
   * Tutti i campi associati al tipo di record.

   I campi contenuti nel modulo di richiesta saranno visibili a tutti coloro che inviano una richiesta a questo tipo di record.

1. (Facoltativo) Rimuovere il campo **Oggetto**, in quanto non è visibile in Workfront Planning. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Passare il puntatore del mouse su tutti i campi del modulo che si desidera rimuovere. Vengono aggiunti alla scheda **Campi** sul lato sinistro del modulo.
1. Fare clic su un campo qualsiasi, quindi utilizzare i controlli sul lato destro del modulo per definire una delle seguenti informazioni sui campi:

   * **Etichetta**: questo è il nome del campo che verrà visualizzato nel modulo di richiesta. Questo non modifica il nome del campo record.
   * **Istruzioni**: aggiungere ulteriori informazioni sul campo.
   * **Imposta un campo obbligatorio**: se selezionata, il campo deve avere un valore. In caso contrario, il modulo non può essere inviato.
   * **Aggiungi logica**: definisci quali condizioni devono essere soddisfatte affinché il campo venga visualizzato o nascosto.

1. Fare clic sulla scheda Elementi contenuto a destra del modulo e aggiungere uno dei seguenti elementi:

   * Testo descrittivo
   * Interruzione di sezione

   Per ulteriori informazioni sulla creazione di un modulo personalizzato, vedere [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).





